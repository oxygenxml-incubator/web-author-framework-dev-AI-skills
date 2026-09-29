## Intercepting and Reacting to Review Comments

When a user adds or edits a review comment through the Add/Edit Comment dialog, the editor fires two interception points: one **before** the comment is written to the document and one **after**. You can register a sync.api.author.ReviewCommentHook on the sync.api.author.ReviewCommentsManager to tap into either or both of these points.

**Note:** The hook is only called when a comment is added or edited through the Add/Edit Comment dialog. Other ways to introduce comments into the document (copy-paste, XML Source view, etc.) do not trigger it.

## Registering the hook

Obtain the review comments manager from the editor's editing support and call sync.api.author.ReviewCommentsManager#registerReviewCommentHook. Register in the `EDITOR_LOADED` event so that the hook is in place before the user opens the comment dialog:

```
workspace.listen(sync.api.Workspace.EventType.EDITOR_LOADED, function(e) {
  var reviewCommentsManager = e.editor.getEditingSupport().getReviewCommentsManager();
  if (reviewCommentsManager) {
    reviewCommentsManager.registerReviewCommentHook(new MyReviewCommentHook());
  }
});

```

You only need to implement the methods relevant to your use case. The rest can be omitted.

## Validating a comment before it is inserted

`beforeCommentAdded` and `beforeCommentEdited` are called after the user presses **Add/Save** in the dialog but **before** the comment is written to the document. Returning a resolved Promise allows the insertion to proceed; returning a rejected Promise with an `Error` cancels the insertion and displays the error message to the user.

```
class ValidatingCommentHook extends sync.api.author.ReviewCommentHook {
  /** @override */
  async beforeCommentAdded(comment) {
    return this.validate_(comment);
  }

  /** @override */
  async beforeCommentEdited(newComment, oldComment) {
    return this.validate_(newComment);
  }

  async validate_(comment) {
    var mentioned = comment.getMentionedUserNames();
    for (var i = 0; i &lt; mentioned.length; i++) {
      var exists = await checkUserExists(mentioned[i]);
      if (!exists) {
        return Promise.reject(new Error(
          'User "' + mentioned[i] + '" does not exist. Please remove the mention before saving.'
        ));
      }
    }
  }
}

```

## Reacting after a comment is inserted

`commentAdded` and `commentEdited` are called **after** the comment is already written to the document. This is the right place to trigger side effects such as notifying mentioned users or updating their roles on the document.

If the returned Promise is rejected, the error message is shown to the user, but the comment remains in the document.

### Notifying mentioned users

`getMentionedUserNames()` returns only the **usernames** as they appear in the document (e.g. `['Alice Johnson', 'Bob Smith']`). Email addresses are not included — they are used solely for display in the suggestions dropdown and are never stored in the document. If you need to send an email notification, your server side must resolve the username to an email address.

```
class NotifyingCommentHook extends sync.api.author.ReviewCommentHook {
  /** @override */
  async commentAdded(comment) {
    return this.notifyMentioned_(comment);
  }

  /** @override */
  async commentEdited(newComment, oldComment) {
    return this.notifyMentioned_(newComment);
  }

  async notifyMentioned_(comment) {
    var mentioned = comment.getMentionedUserNames();
    if (mentioned.length === 0) {
      return;
    }
    // Only usernames are available here. The server is responsible for
    // resolving them to email addresses or other contact details.
    var response = await fetch('/api/notify-mentions', {
      method: 'POST',
      headers: { 'Content-Type': 'application/json' },
      body: JSON.stringify({
        mentionedUsers: mentioned,
        commentText: comment.getCommentText(),
        author: comment.getAuthorName()
      })
    });
    if (!response.ok) {
      return Promise.reject(new Error('Failed to notify mentioned users.'));
    }
  }
}

```

### Updating reviewer roles

```
class RoleUpdateCommentHook extends sync.api.author.ReviewCommentHook {
  /** @override */
  async commentAdded(comment) {
    var mentioned = comment.getMentionedUserNames();
    if (mentioned.length &gt; 0) {
      await fetch('/api/grant-reviewer-role', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({ users: mentioned })
      });
    }
  }
}

```

## The comment object

All hook methods receive a sync.api.author.ReviewComment object. The available information is:

* `getCommentText()` — the full comment text as typed by the user, including raw mention syntax (e.g. `Hello @"Alice Smith", please review this.`).
* `getMentionedUserNames()` — array of user names extracted from the mentions in the comment (e.g. `['Alice Smith']`).
* `getAuthorName()` — the name of the user who wrote the comment.
* `getTimestamp()` — the raw timestamp value as stored in the document (e.g. `20260202T164200+0200`). This can be used to identify the comment on the server side.

For `beforeCommentEdited` and `commentEdited`, both the new and the old comment are provided, so you can compare what changed.

## Related APIs

* sync.api.author.ReviewCommentsManager – use `registerReviewCommentHook` to install your hook.
* For controlling which users appear in the "@" mention dropdown, see the [Implementing a Custom Mentions (User @mention) Provider](tutorial-mentions.md) tutorial.

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
