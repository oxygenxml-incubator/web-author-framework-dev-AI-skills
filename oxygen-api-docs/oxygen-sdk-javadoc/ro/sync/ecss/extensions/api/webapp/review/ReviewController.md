Package [ro.sync.ecss.extensions.api.webapp.review](package-summary.md)

# Interface ReviewController
    All Superinterfaces: [AuthorChangeTrackingController](../../AuthorChangeTrackingController.md), [AuthorReviewerNameController](../../AuthorReviewerNameController.md), [ChangeTrackingController](../../ChangeTrackingController.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ReviewControllerextends [AuthorChangeTrackingController](../../AuthorChangeTrackingController.md), [AuthorReviewerNameController](../../AuthorReviewerNameController.md)
Provides support for marker related actions (accept/reject tracked changes, add/edit comments, edit author name etc.).

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addComment](#addComment(int,int,java.lang.String))(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) comment)
Adds a comment marker at given offsets.
  boolean [addCommentOnSelection](#addCommentOnSelection(int,int,java.lang.String))(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) comment)
Add comment on a selection.
  [AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md) [addPersistentMarker](#addPersistentMarker(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight.PersistentHighlightType,int,int,java.util.Map))([AuthorPersistentHighlight.PersistentHighlightType](../../highlights/AuthorPersistentHighlight.PersistentHighlightType.md) type, int startOffset, int endOffset, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties)
Add comment on a selection.
  void [addReply](#addReply(java.lang.String,ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) replyComment, [AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md) parentHighlight)
Adds a reply to the specified highlight.
  void [addReply](#addReply(java.util.Map,ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties, [AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md) parentHighlight)
Adds a reply to the specified highlight.
  void [editComment](#editComment(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight,java.lang.String))([AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md) highlight, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newComment)
Edits the comment of a marker (comment and tracked change).
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md)> [getAllHighlights](#getAllHighlights())()

 [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) [getAuthorNumber](#getAuthorNumber(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) author)
Returns a number representing the author number.
  void [removeComment](#removeComment(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md) highlight)
Removes a comment marker.
  void [toggleMarkAsDone](#toggleMarkAsDone(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md) highlight)
Toggle the "done" state of the specified highlight.

### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorReviewerNameController](../../AuthorReviewerNameController.md)
 [getReviewerAuthorName](../../AuthorReviewerNameController.md#getReviewerAuthorName()), [setReviewerAuthorName](../../AuthorReviewerNameController.md#setReviewerAuthorName(java.lang.String))
### Methods inherited from interface ro.sync.ecss.extensions.api.[ChangeTrackingController](../../ChangeTrackingController.md)
 [accept](../../ChangeTrackingController.md#accept(int,int)), [accept](../../ChangeTrackingController.md#accept(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight)), [acceptSelection](../../ChangeTrackingController.md#acceptSelection(int,int)), [getAttributeChangeHighlights](../../ChangeTrackingController.md#getAttributeChangeHighlights()), [getChangeHighlights](../../ChangeTrackingController.md#getChangeHighlights()), [getChangeHighlights](../../ChangeTrackingController.md#getChangeHighlights(int,int)), [isTrackingChanges](../../ChangeTrackingController.md#isTrackingChanges()), [reject](../../ChangeTrackingController.md#reject(int,int)), [reject](../../ChangeTrackingController.md#reject(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight)), [rejectSelection](../../ChangeTrackingController.md#rejectSelection(int,int)), [toggleTrackChanges](../../ChangeTrackingController.md#toggleTrackChanges())
## Method Details

### toggleMarkAsDone

void toggleMarkAsDone([AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md) highlight)

Toggle the "done" state of the specified highlight. This state is also applied to all its replies. The highlight can one of the following types:
        1. [AuthorPersistentHighlight.PersistentHighlightType.CHANGE_INSERT](../../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#CHANGE_INSERT)
        2. [AuthorPersistentHighlight.PersistentHighlightType.CHANGE_DELETE](../../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#CHANGE_DELETE)
        3. [AuthorPersistentHighlight.PersistentHighlightType.COMMENT](../../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#COMMENT)
For other types, this method does nothing.
  Parameters: highlight - The highlight to toggle the done state for. Since: 18
### addReply

void addReply([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) replyComment, [AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md) parentHighlight)

Adds a reply to the specified highlight. If the highlight is the last child of its parent, the reply is added to the parent highlight instead. The parent highlight can one of the following types:
        1. [AuthorPersistentHighlight.PersistentHighlightType.CHANGE_INSERT](../../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#CHANGE_INSERT)
        2. [AuthorPersistentHighlight.PersistentHighlightType.CHANGE_DELETE](../../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#CHANGE_DELETE)
        3. [AuthorPersistentHighlight.PersistentHighlightType.COMMENT](../../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#COMMENT)
For other types, this method does not insert any reply or comment. When the first reply is added to a highlight, a new property is set to this highlight: [AuthorPersistentHighlightConstants.COMMENT_ID](../../highlights/AuthorPersistentHighlightConstants.md#COMMENT_ID). All its replies will have the [AuthorPersistentHighlightConstants.COMMENT_PARENT_ID](../../highlights/AuthorPersistentHighlightConstants.md#COMMENT_PARENT_ID)property set, with the same value as the id of the parent.
  Parameters: replyComment - The reply comment. parentHighlight - The parent highlight. Since: 18
### addReply

void addReply([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties, [AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md) parentHighlight)

Adds a reply to the specified highlight. The parent highlight can one of the following types:
        1. [AuthorPersistentHighlight.PersistentHighlightType.CHANGE_INSERT](../../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#CHANGE_INSERT)
        2. [AuthorPersistentHighlight.PersistentHighlightType.CHANGE_DELETE](../../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#CHANGE_DELETE)
        3. [AuthorPersistentHighlight.PersistentHighlightType.COMMENT](../../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#COMMENT)
For other types, this method does not insert any reply or comment. When the first reply is added to a highlight, a new property is set to this highlight: [AuthorPersistentHighlightConstants.COMMENT_ID](../../highlights/AuthorPersistentHighlightConstants.md#COMMENT_ID). All its replies will have the [AuthorPersistentHighlightConstants.COMMENT_PARENT_ID](../../highlights/AuthorPersistentHighlightConstants.md#COMMENT_PARENT_ID)property set, with the same value as the id of the parent. The [AuthorPersistentHighlightConstants.COMMENT_PARENT_ID](../../highlights/AuthorPersistentHighlightConstants.md#COMMENT_PARENT_ID) property in the given map is ignored. The ID of the parent highlight is used instead.
  Parameters: properties - The reply properties. See [AuthorPersistentHighlightConstants](../../highlights/AuthorPersistentHighlightConstants.md) for properties that are meaningful in Oxygen. parentHighlight - The parent highlight. Since: 23
### addComment

void addComment(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) comment)

Adds a comment marker at given offsets. An error message is reported if the comment cannot be added.
  Parameters: startOffset - The start offset of the marker (inclusive). endOffset - The end offset of the marker (exclusive). comment - The comment of the marker.
### addCommentOnSelection

boolean addCommentOnSelection(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) comment)

Add comment on a selection. It returns false if the comment cannot be added.
  Parameters: startOffset - The selection start offset. endOffset - Interval end offset. Inclusive comment - The comment. Returns: true if the comment is added. Since: 21.1.1
### addPersistentMarker

[AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md) addPersistentMarker([AuthorPersistentHighlight.PersistentHighlightType](../../highlights/AuthorPersistentHighlight.PersistentHighlightType.md) type, int startOffset, int endOffset, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties)

Add comment on a selection. It returns false if the comment cannot be added.
  Parameters: type - The persistent highlight type (custom or comment) startOffset - The selection start offset. endOffset - Interval end offset. Inclusive properties - The comment properties. See [AuthorPersistentHighlightConstants](../../highlights/AuthorPersistentHighlightConstants.md) for properties that are meaningful in Oxygen. Returns: The added comment highlight if the comment was added or null. Since: 23
### removeComment

void removeComment([AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md) highlight)

Removes a comment marker.
  Parameters: highlight - The comment marker.
### editComment

void editComment([AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md) highlight, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newComment)

Edits the comment of a marker (comment and tracked change).
  Parameters: highlight - The marker. newComment - The new comment.
### getAllHighlights

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../../highlights/AuthorPersistentHighlight.md)> getAllHighlights()
  Returns: An array with all highlights.
### getAuthorNumber

[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) getAuthorNumber([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) author)

Returns a number representing the author number.
  Parameters: author - The name of the author. Returns: A number representing the author number.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
