Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorReviewerNameController
    All Known Subinterfaces: [AuthorReviewController](AuthorReviewController.md), [ReviewController](webapp/review/ReviewController.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorReviewerNameController
Provides access to reviewer author name, used in the processing instruction that results when a tracked change or a comment is serialized.
  Since: 15.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReviewerAuthorName](#getReviewerAuthorName())()
Get the current reviewer author name.
  void [setReviewerAuthorName](#setReviewerAuthorName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) authorName)
Set the current reviewer author name, used in the processing instruction that results when a  Tracked Change   (<?oxy_insert_start author="reviewer_name"...?>xml content<?oxy_insert_end?>)   or  Comment  (<?oxy_comment_start author="reviewer_name"...?>xml content<?oxy_comment_end?>)   is serialized, as value of the "author" attribute.

## Method Details

### setReviewerAuthorName

void setReviewerAuthorName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) authorName)

Set the current reviewer author name, used in the processing instruction that results when a  Tracked Change   (<?oxy_insert_start author="reviewer_name"...?>xml content<?oxy_insert_end?>)   or  Comment  (<?oxy_comment_start author="reviewer_name"...?>xml content<?oxy_comment_end?>)   is serialized, as value of the "author" attribute. By default the author name specified in the Oxygen Preferences is used for serialization.
  Parameters: authorName - The reviewer author name. If set to null, the default author name (as set in the Oxygen Preferences) will be used in Change Tracking and Comments serialization.
### getReviewerAuthorName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReviewerAuthorName()

Get the current reviewer author name. By default, the reviewer author name is the author name specified in the Oxygen Preferences but it can be changed by using [setReviewerAuthorName(String)](#setReviewerAuthorName(java.lang.String)).
  Returns: The current reviewer author name.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
