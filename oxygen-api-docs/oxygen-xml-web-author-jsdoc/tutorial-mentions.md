## Implementing a Custom Mentions (User @mention) Provider

When users add or edit a review comment, they can mention other users by typing the "@" symbol. The editor shows a list of suggested users to mention. By default, this list is built from authors that appear in the document (comments and change tracking). You can replace it with your own list by implementing the mentions API: provide a custom sync.api.author.UserMentionProposalsProvider and set it on the sync.api.author.ReviewCommentsManager.

## Setting a custom provider

Obtain the review comments manager from the current editor's editing support and call sync.api.author.ReviewCommentsManager#setUserMentionProposalsProvider. This should be done when the editor is loaded so that the provider is in place when the user opens the Add Comment dialog:

```
workspace.listen(sync.api.Workspace.EventType.EDITOR_LOADED, function(e) {
  var editor = e.editor;
  var reviewCommentsManager = editor.getEditingSupport().getReviewCommentsManager();
  if (reviewCommentsManager) {
    reviewCommentsManager.setUserMentionProposalsProvider(new MyUserMentionProposalsProvider());
  }
});

```

## Implementing the provider

Your provider must implement sync.api.author.UserMentionProposalsProvider: it has a single method, `getUserMentionsProposals()`, which returns a **Promise** that resolves to either a flat array of sync.api.author.UserMentionProposal objects or an array of sync.api.author.UserMentionProposalsGroup objects (groups with a category name and a list of users).

Each user proposal has:

* **username** (required): the name that identifies the user and is inserted into the document when the mention is confirmed. For example, selecting "John Doe" from the dropdown inserts `@"John Doe"` into the comment text.
* **email** (optional): used purely as an identifier for the user — it is not inserted into the document. It is displayed in the suggestions list alongside the username to help distinguish users who share the same display name.

If multiple proposals share the same **username**, they are merged into a single entry in the dropdown, with all their emails shown together separated by commas (e.g. `john.doe@example.com, j.doe@corp.com`). Since mentions are always inserted by username, it is not possible to mention only one of them — selecting that entry mentions everyone who shares that username. To allow them to be mentioned independently, ensure each person has a unique username.

### Flat list of users

```
/**
 * Provides a simple flat list of users that can be mentioned in comments.
 */
class MyUserMentionProposalsProvider extends sync.api.author.UserMentionProposalsProvider {
  /** @override */
  getUserMentionsProposals() {
    return Promise.resolve([
      { username: 'Alice Smith', email: 'alice@example.com' },
      { username: 'Bob Jones', email: 'bob@example.com' },
      { username: 'Carol White' }
    ]);
  }
}

```

### Grouped users (categories)

You can return groups so that the "@" menu shows categories (e.g. "Recent Collaborators", "Team"):

```
/**
 * Provides users grouped by category in the mentions dropdown.
 */
class GroupedUserMentionProposalsProvider extends sync.api.author.UserMentionProposalsProvider {
  /** @override */
  getUserMentionsProposals() {
    return Promise.resolve([
      {
        categoryName: 'Recent Collaborators',
        users: [
          { username: 'Alice Smith', email: 'alice@example.com' },
          { username: 'Bob Jones' }
        ]
      },
      {
        categoryName: 'Others',
        users: [
          { username: 'Carol White', email: 'carol@example.com' },
          { username: 'Dave Brown' }
        ]
      }
    ]);
  }
}

```

Categories appear as section headers in the dropdown; users are listed under each category.

### Loading users asynchronously

The method returns a Promise, so you can load users from a server or other async source:

```
/**
 * Fetches mentionable users from a REST API.
 */
class ApiUserMentionProposalsProvider extends sync.api.author.UserMentionProposalsProvider {
  /** @override */
  getUserMentionsProposals() {
    return fetch('/api/collaborators')
      .then(function(response) { return response.json(); })
      .then(function(data) {
        return data.users.map(function(u) {
          return { username: u.displayName, email: u.email };
        });
      });
  }
}

```

## Default behavior

If you do not set a custom provider, the editor uses a default implementation that collects authors from the current document (review comments and change tracking) and the current reviewer name. Setting your own provider replaces this behavior entirely.

## Notifying mentioned users

Once you have the right users appearing in the dropdown, you may also want to send them a notification when they are actually mentioned in a comment. This is handled separately via the sync.api.author.ReviewCommentHook API, which lets you react after a comment is inserted in the document and read the list of mentioned user names from it.

See the [Intercepting and Reacting to Review Comments](tutorial-reviewcommenthook.md) tutorial for details and a complete example.

## Related APIs

* sync.api.author.ReviewCommentsManager – manager for review comments; use `setUserMentionProposalsProvider` to install your provider.
* sync.api.author.ReviewCommentHook – hook into comment add/edit events.

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
