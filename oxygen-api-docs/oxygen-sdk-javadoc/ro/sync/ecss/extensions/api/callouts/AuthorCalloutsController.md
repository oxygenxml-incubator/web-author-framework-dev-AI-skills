Package [ro.sync.ecss.extensions.api.callouts](package-summary.md)

# Interface AuthorCalloutsController
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorCalloutsController
The callouts are representations of Track Changes insert and delete highlights, review comment highlights and custom review highlights in the Author mode on a side bar. This controller can be used to decide what types of callouts must be presented in Author mode. It must be provided through [AuthorReviewController.getAuthorCalloutsController()](../AuthorReviewController.md#getAuthorCalloutsController())method.  To render a custom highlight as a callout in Author mode, a callout information provider must be set from [setCalloutsRenderingInformationProvider(CalloutsRenderingInformationProvider)](#setCalloutsRenderingInformationProvider(ro.sync.ecss.extensions.api.callouts.CalloutsRenderingInformationProvider)) method.  By default, the callouts visibility in Author mode is controlled from Oxygen Preferences but it can be changed by using the methods in this class. The Preferences will not be affected by the API.
  Since: 14
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addCalloutActionsProvider](#addCalloutActionsProvider(ro.sync.ecss.extensions.api.callouts.CalloutActionsProvider))([CalloutActionsProvider](CalloutActionsProvider.md) actionsProvider)
Add a callout actions provider.
  [Rectangle](../../../../exml/view/graphics/Rectangle.md) [getCalloutRectangle](#getCalloutRectangle(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) persistentHighlight)
Retrieves the bounds of the callout box associated with an Author persistent highlight.
  [AuthorCalloutRenderingInformation](AuthorCalloutRenderingInformation.md) [getDefaultAuthorCalloutRenderingInformation](#getDefaultAuthorCalloutRenderingInformation(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) highlight)
Return the default rendering information for built-in persistent highlights (comment, insertion or deletion change).
  boolean [isShowingCommentsCallouts](#isShowingCommentsCallouts())()
Check if the callouts corresponding to review comments and Change Tracking deletions and insertions with comments are visible in Author mode.
  boolean [isShowingDeletionsCallouts](#isShowingDeletionsCallouts())()
Check if the callouts corresponding to Change Tracking deletions are visible in Author mode.
  boolean [isShowingInsertionsCallouts](#isShowingInsertionsCallouts())()
Check if the callouts corresponding to Change Tracking insertions are visible in Author mode.
  void [removeCalloutActionsProvider](#removeCalloutActionsProvider(ro.sync.ecss.extensions.api.callouts.CalloutActionsProvider))([CalloutActionsProvider](CalloutActionsProvider.md) actionsProvider)
Remove a callout actions provider.
  void [setCalloutsRenderingInformationProvider](#setCalloutsRenderingInformationProvider(ro.sync.ecss.extensions.api.callouts.CalloutsRenderingInformationProvider))([CalloutsRenderingInformationProvider](CalloutsRenderingInformationProvider.md) provider)
Set the provider for data that will be rendered as a callout, in Author mode, for a specific highlight.
  void [setShowCommentsCallouts](#setShowCommentsCallouts(java.lang.Boolean))([Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) showCommentsCallouts)
The Track Changes insert and delete markers, the review comment markers and the custom review markers can be presented in Author mode as callouts.
  void [setShowDeletionsCallouts](#setShowDeletionsCallouts(java.lang.Boolean))([Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) showDeletionsCallouts)
The Track Changes insert and delete markers, the review comment markers and the custom review markers can be presented in Author mode as callouts.
  void [setShowInsertionsCallouts](#setShowInsertionsCallouts(java.lang.Boolean))([Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) showInsertionsCallouts)
The Track Changes insert and delete markers, the review comment markers and the custom review markers can be presented in Author mode as callouts.

## Method Details

### isShowingCommentsCallouts

boolean isShowingCommentsCallouts()

Check if the callouts corresponding to review comments and Change Tracking deletions and insertions with comments are visible in Author mode. By default, the comments callouts visibility in Author mode is controlled from Oxygen Preferences but it can be changed by using the [setShowCommentsCallouts(Boolean)](#setShowCommentsCallouts(java.lang.Boolean)) method. Note that when there are no review callouts, the callouts side bar is collapsed.
  Returns: true if the callouts with comments are visible.
### setShowCommentsCallouts

void setShowCommentsCallouts([Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) showCommentsCallouts)

The Track Changes insert and delete markers, the review comment markers and the custom review markers can be presented in Author mode as callouts. This method can be used to override the default option from Oxygen Preferences that controls if the callouts corresponding to review comments and Change Tracking deletions and insertions with comments are displayed in Author mode. Note that when there are no review callouts, the callouts side bar is collapsed.
  Parameters: showCommentsCallouts - If true, the review callouts with comments are displayed in Author mode. The callouts with comments are hidden when the provided value is false.  When the value is set to null, the option from Oxygen Preferences is taken into consideration.
### isShowingDeletionsCallouts

boolean isShowingDeletionsCallouts()

Check if the callouts corresponding to Change Tracking deletions are visible in Author mode. By default, the Change Tracking deletions callouts visibility in Author mode is controlled from Oxygen Preferences but it can be changed by using the [setShowDeletionsCallouts(Boolean)](#setShowDeletionsCallouts(java.lang.Boolean)) method. Note that when there are no review callouts, the callouts side bar is collapsed.
  Returns: true if the Track Changes deletions callouts are displayed in Author mode.
### setShowDeletionsCallouts

void setShowDeletionsCallouts([Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) showDeletionsCallouts)

The Track Changes insert and delete markers, the review comment markers and the custom review markers can be presented in Author mode as callouts. This method can be used to override the default option from Oxygen Preferences that controls if the callouts corresponding to Change Tracking deletions are displayed in Author mode. Note that when there are no review callouts, the callouts side bar is collapsed.
  Parameters: showDeletionsCallouts - If true, the Track Changes deletions callouts are displayed in Author mode. The deletions callouts are hidden when the provided value is false.  When the value is set to null, the option from Oxygen Preferences is taken into consideration.
### isShowingInsertionsCallouts

boolean isShowingInsertionsCallouts()

Check if the callouts corresponding to Change Tracking insertions are visible in Author mode. By default, the Change Tracking insertions callouts visibility in Author mode is controlled from Oxygen Preferences but it can be changed by using the [setShowInsertionsCallouts(Boolean)](#setShowInsertionsCallouts(java.lang.Boolean)) method. Note that when there are no review callouts, the callouts side bar is collapsed.
  Returns: true if the Track Changes insertions callouts are visible.
### setShowInsertionsCallouts

void setShowInsertionsCallouts([Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) showInsertionsCallouts)

The Track Changes insert and delete markers, the review comment markers and the custom review markers can be presented in Author mode as callouts. This method can be used to override the default option from Oxygen Preferences that controls if the callouts corresponding to Change Tracking insertions are displayed in Author mode. Note that when there are no review callouts, the callouts side bar is collapsed.
  Parameters: showInsertionsCallouts - If true, the Track Changes insertions callouts are displayed in Author mode. The insertions callouts are hidden when the provided value is false.  When the value is set to null, the option from Oxygen Preferences is taken into consideration.
### setCalloutsRenderingInformationProvider

void setCalloutsRenderingInformationProvider([CalloutsRenderingInformationProvider](CalloutsRenderingInformationProvider.md) provider)

Set the provider for data that will be rendered as a callout, in Author mode, for a specific highlight. The callouts are representations of Track Changes insert and delete highlights, review comment highlights and custom review highlights in Author mode. By default, the callouts visibility in Author mode is controlled from Oxygen Preferences but it can be changed by using the [AuthorCalloutsController](AuthorCalloutsController.md) methods.
  Parameters: provider - The highlights callout rendering information provider. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - Thrown when a property name is not a valid XML attribute name. Since: 14
### getCalloutRectangle

[Rectangle](../../../../exml/view/graphics/Rectangle.md) getCalloutRectangle([AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) persistentHighlight)

Retrieves the bounds of the callout box associated with an Author persistent highlight.
  Parameters: persistentHighlight - The Author persistent highlight. Returns: The bounds of the callout box associated with the given Author persistent highlight, relative to the editor area's origins, or null if there is no corresponding callout box. Since: 14.2
### addCalloutActionsProvider

void addCalloutActionsProvider([CalloutActionsProvider](CalloutActionsProvider.md) actionsProvider)

Add a callout actions provider.
  Parameters: actionsProvider - The callout actions provider. Since: 17
### removeCalloutActionsProvider

void removeCalloutActionsProvider([CalloutActionsProvider](CalloutActionsProvider.md) actionsProvider)

Remove a callout actions provider.
  Parameters: actionsProvider - The callout actions provider. Since: 17
### getDefaultAuthorCalloutRenderingInformation

[AuthorCalloutRenderingInformation](AuthorCalloutRenderingInformation.md) getDefaultAuthorCalloutRenderingInformation([AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) highlight)

Return the default rendering information for built-in persistent highlights (comment, insertion or deletion change). You can change the rendering information for such highlights by setting a [CalloutsRenderingInformationProvider](CalloutsRenderingInformationProvider.md) and overriding its method [CalloutsRenderingInformationProvider.handlesAlsoDefaultHighlights()](CalloutsRenderingInformationProvider.md#handlesAlsoDefaultHighlights()) to return true. The callouts are representations of Track Changes insert and delete highlights, review comment highlights and custom review highlights in Author mode.
  Parameters: highlight - The Author persistent highlight. The type of the highlight can be obtained by using the [AuthorPersistentHighlight.getType()](../highlights/AuthorPersistentHighlight.md#getType()) Returns: the default rendering information for built-in persistent highlights (comment, insertion or deletion change). Since: 17.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
