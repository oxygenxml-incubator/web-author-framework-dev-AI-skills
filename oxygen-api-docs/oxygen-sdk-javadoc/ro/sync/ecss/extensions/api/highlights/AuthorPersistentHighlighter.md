Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Interface AuthorPersistentHighlighter
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorPersistentHighlighter
Manage the user custom persistent highlights which get serialized in the XML as processing instructions with the form:  <?oxy_custom_start prop1="val1"....?> xml content <?oxy_custom_end?> The Highlighter is accessible from [WSAuthorEditorPageBase.getPersistentHighlighter()](../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getPersistentHighlighter()).
  Since: 12
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorPersistentHighlight](AuthorPersistentHighlight.md) [addHighlight](#addHighlight(int,int,java.util.LinkedHashMap))(int startOffset, int endOffset, [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties)
Add a custom persistent highlight.
  boolean [canAddHighlight](#canAddHighlight(int,int))(int startOffset, int endOffset)
Check if a custom [AuthorPersistentHighlight](AuthorPersistentHighlight.md) can be added for the given start and end offsets.
  [AuthorPersistentHighlight](AuthorPersistentHighlight.md)[] [getHighlights](#getHighlights())()
Fetches the list of custom persistent highlights.
  [AuthorPersistentHighlight](AuthorPersistentHighlight.md)[] [getHighlights](#getHighlights(int,int))(int startOffset, int endOffset)
Fetches the list of custom persistent highlights that intersect the interval between the given start offset and end offset.
  void [removeAllHighlights](#removeAllHighlights())()
Removes all custom persistent highlights.
  void [removeHighlight](#removeHighlight(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)
Removes a highlight from the view.
  void [setHighlightRenderer](#setHighlightRenderer(ro.sync.ecss.extensions.api.highlights.PersistentHighlightRenderer))([PersistentHighlightRenderer](PersistentHighlightRenderer.md) renderer)
Set a renderer for customizing the way that the custom persistent highlights are displayed.
  void [setHighlightsActionsProvider](#setHighlightsActionsProvider(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightActionsProvider))([AuthorPersistentHighlightActionsProvider](AuthorPersistentHighlightActionsProvider.md) provider)
Set the provider for the actions that are available for a specific highlight.
  void [setProperties](#setProperties(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight,java.util.LinkedHashMap))([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight, [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> newProperties)
Set new properties of a specific highlight. A copy of the initial properties can be obtained from [AuthorPersistentHighlight.getClonedProperties()](AuthorPersistentHighlight.md#getClonedProperties())

## Method Details

### addHighlight

[AuthorPersistentHighlight](AuthorPersistentHighlight.md) addHighlight(int startOffset, int endOffset, [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties)throws [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html)

Add a custom persistent highlight. The name of the processing instruction markers corresponding to this type of highlight are oxy_custom_start and oxy_custom_end. The type of the added persistent highlight is [AuthorPersistentHighlight.PersistentHighlightType.CUSTOM_HIGHLIGHT](AuthorPersistentHighlight.PersistentHighlightType.md#CUSTOM_HIGHLIGHT).
  Parameters: startOffset - Start offset (inclusive). endOffset - End offset (inclusive). The highlight end offset must be equal or greater than the start offset. properties - name/value pairs which will get serialized to disk.
Notes:1. Each property name must be a valid XML attribute name.2. Each property value will be escaped to be a valid XML attribute value.3. In order to change the properties for a highlight you have to use the method: [setProperties(AuthorPersistentHighlight, LinkedHashMap)](#setProperties(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight,java.util.LinkedHashMap)).
 Returns: The added highlight or null if the highlight cannot be added if for example the offsets are in read-only content or there is a marker with the same properties over the same interval. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - Thrown when a property name is not a valid XML attribute name or when the given end offset is less than start offset.
### canAddHighlight

boolean canAddHighlight(int startOffset, int endOffset)

Check if a custom [AuthorPersistentHighlight](AuthorPersistentHighlight.md) can be added for the given start and end offsets. If one of these offsets correspond to a read-only context (they are inside a content deleted with track changes, an element set as read-only from CSS or a content generated from expanding a reference) the highlight cannot be inserted and this method returns false.  A custom persistent highlight can be added by using the [addHighlight(int, int, LinkedHashMap)](#addHighlight(int,int,java.util.LinkedHashMap)) method. The name of the processing instruction markers corresponding to the custom persistent highlight are oxy_custom_start and oxy_custom_end.
  Parameters: startOffset - Start offset (inclusive). endOffset - End offset (inclusive). The highlight end offset must be equal or greater than the start offset. Returns: true if a custom persistent highlight can be inserted Since: 14.1
### removeHighlight

void removeHighlight([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)

Removes a highlight from the view.
  Parameters: highlight - the highlight to remove
### removeAllHighlights

void removeAllHighlights()

Removes all custom persistent highlights.

### getHighlights

[AuthorPersistentHighlight](AuthorPersistentHighlight.md)[] getHighlights()

Fetches the list of custom persistent highlights.
  Returns: the highlight array.
### getHighlights

[AuthorPersistentHighlight](AuthorPersistentHighlight.md)[] getHighlights(int startOffset, int endOffset)

Fetches the list of custom persistent highlights that intersect the interval between the given start offset and end offset.
  Parameters: startOffset - The start offset(inclusive). endOffset - The end offset (inclusive). Returns: The custom persistent highlights array. Can be null if no custom persistent highlight intersects the given offsets interval. Since: 14.1
### setProperties

void setProperties([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight, [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> newProperties)throws [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html)

Set new properties of a specific highlight. A copy of the initial properties can be obtained from [AuthorPersistentHighlight.getClonedProperties()](AuthorPersistentHighlight.md#getClonedProperties())
  Parameters: highlight - The highlight for which the properties will be set. newProperties - The new highlight properties.
Notes:1. Each property name must be a valid XML attribute name. 2. Each property value will be escaped to be a valid XML attribute value.
 Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - Thrown when a property name is not a valid XML attribute name. The properties may not be set of the marker is in read-only content or if there is already a marker with the same properties added over the same interval.
### setHighlightRenderer

void setHighlightRenderer([PersistentHighlightRenderer](PersistentHighlightRenderer.md) renderer)

Set a renderer for customizing the way that the custom persistent highlights are displayed.
  Parameters: renderer - The renderer defining the way in which the highlights are painted.
### setHighlightsActionsProvider

void setHighlightsActionsProvider([AuthorPersistentHighlightActionsProvider](AuthorPersistentHighlightActionsProvider.md) provider)

Set the provider for the actions that are available for a specific highlight. The actions are currently displayed in the persistent highlights associated callouts popup menu, but in future could be also used as actions presented for a highlight in the contextual menu of the main editing area. The callouts are representations of Track Changes insert and delete highlights, review comment highlights and custom review highlights in Author mode. To associate callout information to a custom highlight the [AuthorCalloutsController.setCalloutsRenderingInformationProvider(CalloutsRenderingInformationProvider)](../callouts/AuthorCalloutsController.md#setCalloutsRenderingInformationProvider(ro.sync.ecss.extensions.api.callouts.CalloutsRenderingInformationProvider))method must be used.
  Parameters: provider - The highlights callout rendering information provider. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - Thrown when a property name is not a valid XML attribute name. Since: 14
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
