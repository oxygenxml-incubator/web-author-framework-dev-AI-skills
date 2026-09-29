Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorReviewController
    All Superinterfaces: [AuthorChangeTrackingController](AuthorChangeTrackingController.md), [AuthorReviewerNameController](AuthorReviewerNameController.md), [ChangeTrackingController](ChangeTrackingController.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorReviewControllerextends [AuthorChangeTrackingController](AuthorChangeTrackingController.md), [AuthorReviewerNameController](AuthorReviewerNameController.md)
Controller that can be used to toggle the change tracking state, modify the review highlight author name, the highlight painting or to obtain information about the properties used in the serialization and representation of the review highlight (author name, reviewer auto color or the current time stamp in a format identical to the one used by Oxygen for insert, delete and comment review highlights).
  Since: 12
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addAuthorPersistentHighlightListener](#addAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener))([AuthorPersistentHighlightsListener](highlights/AuthorPersistentHighlightsListener.md) listener)
Adds a listener to be notified about changes regarding the persistent highlights.
  void [addPersistentHighlightsFilter](#addPersistentHighlightsFilter(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsFilter))([AuthorPersistentHighlightsFilter](highlights/AuthorPersistentHighlightsFilter.md) persistentHighlightsFilter)
Add a persistent highlights filter.
  [AuthorCalloutsController](callouts/AuthorCalloutsController.md) [getAuthorCalloutsController](#getAuthorCalloutsController())()
The callouts are representations of Track Changes insert and delete highlights, review comment highlights and the custom review highlights in Author mode.
  [AuthorReviewViewController](review/AuthorReviewViewController.md) [getAuthorReviewViewController](#getAuthorReviewViewController())()
The entries in the Review View are representations of Track Changes insert and delete highlights, review comment highlights in Author mode.
  [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md)[] [getCommentHighlights](#getCommentHighlights())()
Fetches the list of comment highlights.
  [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md)[] [getCommentHighlights](#getCommentHighlights(int,int))(int startOffset, int endOffset)
Fetches the list of comment highlights that intersect the interval between the given start offset and end offset.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCurrentTimestamp](#getCurrentTimestamp())()
Get the current time stamp in a format identical to the one used by Oxygen for insert and delete review highlights.
  [Color](../../../exml/view/graphics/Color.md) [getReviewerAutoColor](#getReviewerAutoColor(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reviewerAuthorName)
Get a color assigned automatically to the reviewer author name.
  void [removeAuthorPersistentHighlightListener](#removeAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener))([AuthorPersistentHighlightsListener](highlights/AuthorPersistentHighlightsListener.md) listener)
Removes a persistent highlights listener.
  void [removePersistentHighlightProperties](#removePersistentHighlightProperties(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight,java.util.List))([AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) highlight, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties)
Remove properties from a persistent highlight.
  void [setPersistentHighlightProperties](#setPersistentHighlightProperties(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight,java.util.LinkedHashMap))([AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) highlight, [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties)
Set some properties to a persistent highlight.
  void [setReviewRenderer](#setReviewRenderer(ro.sync.ecss.extensions.api.highlights.PersistentHighlightRenderer))([PersistentHighlightRenderer](highlights/PersistentHighlightRenderer.md) renderer)
Set a renderer for customizing the way that the review highlights (Insert, Delete or Comment) are displayed.

### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorReviewerNameController](AuthorReviewerNameController.md)
 [getReviewerAuthorName](AuthorReviewerNameController.md#getReviewerAuthorName()), [setReviewerAuthorName](AuthorReviewerNameController.md#setReviewerAuthorName(java.lang.String))
### Methods inherited from interface ro.sync.ecss.extensions.api.[ChangeTrackingController](ChangeTrackingController.md)
 [accept](ChangeTrackingController.md#accept(int,int)), [accept](ChangeTrackingController.md#accept(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight)), [acceptSelection](ChangeTrackingController.md#acceptSelection(int,int)), [getAttributeChangeHighlights](ChangeTrackingController.md#getAttributeChangeHighlights()), [getChangeHighlights](ChangeTrackingController.md#getChangeHighlights()), [getChangeHighlights](ChangeTrackingController.md#getChangeHighlights(int,int)), [isTrackingChanges](ChangeTrackingController.md#isTrackingChanges()), [reject](ChangeTrackingController.md#reject(int,int)), [reject](ChangeTrackingController.md#reject(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight)), [rejectSelection](ChangeTrackingController.md#rejectSelection(int,int)), [toggleTrackChanges](ChangeTrackingController.md#toggleTrackChanges())
## Method Details

### getAuthorCalloutsController

[AuthorCalloutsController](callouts/AuthorCalloutsController.md) getAuthorCalloutsController()

The callouts are representations of Track Changes insert and delete highlights, review comment highlights and the custom review highlights in Author mode. This controller can be used to check what types of callouts are presented in Author mode. It also can be used to override the callouts display options from Oxygen Preferences.
  Returns: The Author review callouts controller. Since: 14
### getAuthorReviewViewController

[AuthorReviewViewController](review/AuthorReviewViewController.md) getAuthorReviewViewController()

The entries in the Review View are representations of Track Changes insert and delete highlights, review comment highlights in Author mode. This controller can override review entries display options and contextual menu actions.
  Returns: The Author Review View controller. Since: 17.1
### getCurrentTimestamp

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCurrentTimestamp()

Get the current time stamp in a format identical to the one used by Oxygen for insert and delete review highlights. Form: yyyyMMdd'T'HHmmssZ
  Returns: the current time stamp.
### getReviewerAutoColor

[Color](../../../exml/view/graphics/Color.md) getReviewerAutoColor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reviewerAuthorName)

Get a color assigned automatically to the reviewer author name. It is used when in the Oxygen Preferences **Auto** coloring is set for the Insert, Delete or Comment reviews.
  Parameters: reviewerAuthorName - The reviewer author name. Returns: The color automatically assigned to the specified author. Never null.
### setReviewRenderer

void setReviewRenderer([PersistentHighlightRenderer](highlights/PersistentHighlightRenderer.md) renderer)

Set a renderer for customizing the way that the review highlights (Insert, Delete or Comment) are displayed.
  Parameters: renderer - the renderer used to customize painting for the review highlights.
### getCommentHighlights

[AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md)[] getCommentHighlights()

Fetches the list of comment highlights.
  Returns: The comment highlights array. Since: 12
### getCommentHighlights

[AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md)[] getCommentHighlights(int startOffset, int endOffset)

Fetches the list of comment highlights that intersect the interval between the given start offset and end offset.
  Parameters: startOffset - The start offset(inclusive). endOffset - The end offset (inclusive). Returns: The comment highlights array. Can be null if no comment highlight intersects the given offsets interval. Since: 14.1
### setPersistentHighlightProperties

void setPersistentHighlightProperties([AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) highlight, [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties)throws [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html)

Set some properties to a persistent highlight. A copy of the initial properties can be obtained from [AuthorPersistentHighlight.getClonedProperties()](highlights/AuthorPersistentHighlight.md#getClonedProperties())Please note that this method allows setting the properties of all persistent highlights, whether the current author is the author of the highlight or not. The existing properties will be overwritten, excepting the ones that are specific to Oxygen XML comments or track changes processing instructions, that cannot be changed. You can see the name of these specific properties in [AuthorPersistentHighlightConstants](highlights/AuthorPersistentHighlightConstants.md).
  Parameters: highlight - The highlight. properties - name/value pairs which will get serialized to disk.
Notes:1. Each property name must be a valid XML attribute name.2. Each property value will be escaped to be a valid XML attribute value. 3. A null value means that the property will be removed.
 Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - Thrown when a property name is not a valid XML attribute name or when the given properties map contains a property specific to Oxygen XML comments or track changes processing instructions Since: 23.1
### removePersistentHighlightProperties

void removePersistentHighlightProperties([AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) highlight, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties)throws [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html)

Remove properties from a persistent highlight. A copy of the initial properties can be obtained from [AuthorPersistentHighlight.getClonedProperties()](highlights/AuthorPersistentHighlight.md#getClonedProperties())Please note that the properties that are specific to Oxygen XML comments or track changes processing instructions cannot be removed. You can see the name of these specific properties in [AuthorPersistentHighlightConstants](highlights/AuthorPersistentHighlightConstants.md)
  Parameters: highlight - The highlight. properties - The names of the properties to be removed. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - Thrown when trying to remove a property specific to Oxygen XML comments or track changes processing instructions Since: 23.1
### addAuthorPersistentHighlightListener

void addAuthorPersistentHighlightListener([AuthorPersistentHighlightsListener](highlights/AuthorPersistentHighlightsListener.md) listener)

Adds a listener to be notified about changes regarding the persistent highlights. In the persistent highlights are included:
        *  Change tracking markers and comments
        *  Additional persistent highlights added using [AuthorPersistentHighlighter.addHighlight(int, int, java.util.LinkedHashMap)](highlights/AuthorPersistentHighlighter.md#addHighlight(int,int,java.util.LinkedHashMap))

  Parameters: listener - The listener Since: 23.1 See Also:
        * [AuthorPersistentHighlight.PersistentHighlightType](highlights/AuthorPersistentHighlight.PersistentHighlightType.md)
        * [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md)

### removeAuthorPersistentHighlightListener

void removeAuthorPersistentHighlightListener([AuthorPersistentHighlightsListener](highlights/AuthorPersistentHighlightsListener.md) listener)

Removes a persistent highlights listener.
  Parameters: listener - The listener to remove. Since: 23.1
### addPersistentHighlightsFilter

void addPersistentHighlightsFilter([AuthorPersistentHighlightsFilter](highlights/AuthorPersistentHighlightsFilter.md) persistentHighlightsFilter)

Add a persistent highlights filter. A filter capable of filtering the highlights by author is present by default.
  Parameters: persistentHighlightsFilter - The filter to be added. Since: 23.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
