Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Interface Highlight
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface Highlight
The highlight interface.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [HOVER_ACTIONS_PROVIDER_ADDITIONAL_DATA](#HOVER_ACTIONS_PROVIDER_ADDITIONAL_DATA)
Key for the menu creator getting the actions that can be performed over the highlight, as well as information about rendering.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getAdditionalData](#getAdditionalData())()

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getAdditionalData](#getAdditionalData(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
Gets the additional data for the given key.
  int [getEndOffset](#getEndOffset())()
Gets the ending model offset for the highlight.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getId](#getId())()
Gets the highlight id.
  [HighlightPainter](HighlightPainter.md) [getPainter](#getPainter())()
Gets the painter for the highlighter.
  int [getStartOffset](#getStartOffset())()
Gets the starting model offset for the highlight.
  boolean [isEmpty](#isEmpty())()

 void [setAdditionalData](#setAdditionalData(java.lang.String,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) additionalData)
Sets the additional data for the given key.

## Field Details

### HOVER_ACTIONS_PROVIDER_ADDITIONAL_DATA

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) HOVER_ACTIONS_PROVIDER_ADDITIONAL_DATA

Key for the menu creator getting the actions that can be performed over the highlight, as well as information about rendering. The value should be a [HighlightActionsProvider](HighlightActionsProvider.md)
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.Highlight.HOVER_ACTIONS_PROVIDER_ADDITIONAL_DATA)

## Method Details

### getStartOffset

int getStartOffset()

Gets the starting model offset for the highlight.
  Returns: the starting offset >= 0
### getEndOffset

int getEndOffset()

Gets the ending model offset for the highlight.
**Note:** empty highlights have startOffset == endOffset + 1

  Returns: the ending offset (inclusive).
### isEmpty

boolean isEmpty()
  Returns: true if the highlight is empty. Since: 22
### getAdditionalData

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getAdditionalData()
  Returns: Additional data for the highlight.
### getAdditionalData

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getAdditionalData([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

Gets the additional data for the given key.
  Parameters: key - the key for which the additional data is to be retrieved. The key [HOVER_ACTIONS_PROVIDER_ADDITIONAL_DATA](#HOVER_ACTIONS_PROVIDER_ADDITIONAL_DATA) can be used in order to get the [HighlightActionsProvider](HighlightActionsProvider.md) object, providing a set of actions and some rendering information. This can be used to display a widget when hovering over the highlight, from which the provided actions can be performed. Returns: The additional data for the given key. Since: 17.1
### setAdditionalData

void setAdditionalData([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) additionalData)

Sets the additional data for the given key.
  Parameters: key - The key for which the additional data is set.The key [HOVER_ACTIONS_PROVIDER_ADDITIONAL_DATA](#HOVER_ACTIONS_PROVIDER_ADDITIONAL_DATA) can be used in order to set an actions provider for the highlight, containing a set of actions, as well as some information about their rendering. The goal is to display a widget when hovering over the highlight, from which the provided actions can be performed. additionalData - The additional data to set.For the [HOVER_ACTIONS_PROVIDER_ADDITIONAL_DATA](#HOVER_ACTIONS_PROVIDER_ADDITIONAL_DATA) key, the value must be a [HighlightActionsProvider](HighlightActionsProvider.md). Since: 17.1
### getPainter

[HighlightPainter](HighlightPainter.md) getPainter()

Gets the painter for the highlighter.
  Returns: the painter
### getId

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getId()

Gets the highlight id.
  Returns: The id of the highlight.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
