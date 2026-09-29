# Global

##

### Members

#### workspace

 The workspace that corresponds to the currently opened tab.

### Methods

#### &lt;async&gt; beforeCommentAdded(comment)

 Method called right before a commment is added in the document from the Add Comment dialog, when user presses Add.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `comment` |   ReviewComment   | The comment to add. |
    Since:
* 28.1

##### Returns:

 Promise that if resolved the comment is added in the document, or rejected with an error with message.
     Type     Promise.&lt;Void&gt;
#### &lt;async&gt; beforeCommentEdited(newComment, oldComment)

 Method called right before a commment is edited in the document from the Edit Comment dialog, when user presses Add.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `newComment` |   ReviewComment   | The new comment. |
| `oldComment` |   ReviewComment   | The old comment. |
    Since:
* 28.1

##### Returns:

 Promise that if resolved the comment is added in the document, or rejected with an error with message.
     Type     Promise.&lt;Void&gt;
#### &lt;async&gt; commentAdded(comment)

 Method called right after a comment is added in the document.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `comment` |   ReviewComment   | The comment to add. |
    Since:
* 28.1

##### Returns:

 A promise.
     Type     Promise.&lt;Void&gt;
#### &lt;async&gt; commentEdited(newComment, oldComment)

 Method called right after a comment is edited in the document.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `newComment` |   ReviewComment   | The new comment. |
| `oldComment` |   ReviewComment   | The old comment. |
    Since:
* 28.1

##### Returns:

 A promise.
     Type     Promise.&lt;Void&gt;
#### createSelectionAroundOffsets(startOffset, opt_endOffset, opt_anchorOffset, opt_focusOffset)

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `startOffset` |   number   | The start offset. |
| `opt_endOffset` |   number   | The end offset. Exclusive offset. |
| `opt_anchorOffset` |   number   | The anchor offset. |
| `opt_focusOffset` |   number   | The focus offset. |

##### Returns:

 The selection on text.
     Type     SelectionCore
#### editorChanged()

#### getAuthorName()

 Get the comment author name.

##### Returns:

 The author name.
     Type     string
#### getCommentText()

 Get the comment text.

##### Returns:

 The comment.
     Type     string
#### getIcon()

#### getMentionedUserNames()

 Get the mentioned user names within the comment.

##### Returns:

 The mentioned user names within the comment.
     Type     Array.&lt;string&gt;
#### getTimestamp()

 Get the raw timestamp value as it can be found in document (see the "timestamp" attribute of the "oxy_comment_start" PI). This can be use to find the corresponding Java object via ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.MODIFICATION_TIME.

##### Returns:

 The raw timestamp value. For example: "20260202T164200+0200".
     Type     string
#### getTitle()

#### getToolbarActionsMap()

#### getToolbarDescriptor()

#### getUserMentionsProposals()

 Returns a promise that resolves to an array of user mention proposals groups. For example: [ { categoryName: 'Recent Collaborators', users: [ { username: 'John Doe 1', email: 'john.doe@example.com' }, { username: 'Jane Doe 2' }, ] }, { categoryName: 'Others', users: [ { username: 'John Doe 3', email: 'john.doe3@example.com' }, { username: 'Jane Doe 4' }, ] }, ] OR it can be: [ { username: 'John Doe 1', email: 'john.doe@example.com' }, { username: 'Jane Doe 2' }, { username: 'John Doe 3', email: 'john.doe3@example.com' }, { username: 'Jane Doe 4' }, ]
    Since:
* 28.1

##### Returns:

 User mention proposals or groups of users.
     Type     Promise.&lt;(Array.&lt;[UserMentionProposalsGroup](global.md#UserMentionProposalsGroup)&gt;|Array.&lt;[UserMentionProposal](global.md#UserMentionProposal)&gt;)&gt;
#### install()

#### opened()

#### refreshNodes(href)

 Refresh all nodes that have the given href.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `href` |   string   | Href to find the nodes to refresh. If null all nodes will be refreshed. |
    Since:
* 27.0

#### registerReviewCommentHook(reviewCommentHook)

 Registers a hook that is called when a review comment is explicitly added or edited in the document by the user Note that this hook is called when the user explicitly adds a comment in the document using the Add Comment dialog, but there are also other ways to add a comment in the document, for example when the user adds a fragment with copy-paste, from XML Source (text page), etc.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `reviewCommentHook` |   sync.api.author.ReviewCommentHook   | Hook that intercepts review comments added or edited in the document. |
    Since:
* 28.1

#### setUserMentionProposalsProvider(userMentionProposalsProvider)

 Sets a provider that returns user names that will be presented as proposals when user types "@" in the Add Comment dialog.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `userMentionProposalsProvider` |   sync.api.author.UserMentionProposalsProvider   | Provider that returns user names that can be mentioned in a comment. |
    Since:
* 28.1

#### supportsEditor()

### Type Definitions

#### LoadedDocument

##### Properties:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `contentType` |   string   |    | The MIME type of the document. |
| `document` |   string   |  &lt;optional&gt;   | The content of the document, for documents with a text/\* MIME type. |

#### UserMentionProposal

##### Type:

*   Object

##### Properties:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `username` |   String   |    | The user name. |
| `email` |   String   |  &lt;optional&gt;   | The user email. |

#### UserMentionProposalsGroup

##### Type:

*   Object

##### Properties:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `users` |   Array.&lt;[UserMentionProposal](global.md#UserMentionProposal)&gt;   |    | The users in this category. |
| `categoryName` |   String   |  &lt;optional&gt;   | The category to which this user, proposed to be mentioned, belongs. The categories are displayed visually in the UI in the menu shown when the ‘@’ symbol is pressed. Each category is a group of users. |

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
