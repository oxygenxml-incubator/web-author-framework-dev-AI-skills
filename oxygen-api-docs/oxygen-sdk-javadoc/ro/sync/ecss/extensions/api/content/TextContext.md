Package [ro.sync.ecss.extensions.api.content](package-summary.md)

# Interface TextContext
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface TextContext
Current Text Context where the text content iterator is positioned.
  Since: 13
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [EDITABLE](#EDITABLE)
The returned text is in editable context.
  static final int [EDITABLE_IN_FILTERED_CONDITIONAL_PROFILING](#EDITABLE_IN_FILTERED_CONDITIONAL_PROFILING)
The returned text is in editable context but a profiling condition is applied and filters the node when the output will be published..
  static final int [NOT_EDITABLE_IN_DELETE_CHANGE_TRACKING](#NOT_EDITABLE_IN_DELETE_CHANGE_TRACKING)
The returned text is in delete change tracking context.
  static final int [NOT_EDITABLE_IN_READ_ONLY](#NOT_EDITABLE_IN_READ_ONLY)
The returned text is in an entity or content reference.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 int [getEditableState](#getEditableState())()
Check if we can edit at the current iterator offset.
  [AuthorNode](../node/AuthorNode.md) [getNode](#getNode())()
Get the parent node surrounding this text.
  [CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html) [getText](#getText())()
Gets the current text from the context.
  int [getTextEndOffset](#getTextEndOffset())()
Gets the end offset of the returned text.
  int [getTextStartOffset](#getTextStartOffset())()
Gets the start offset of the returned text.
  boolean [inSpacePreserve](#inSpacePreserve())()
Check if the range is in a CSS white-space preserve context.
  boolean [inVisibleContent](#inVisibleContent())()
Check if the range is in visible content.
  void [replaceText](#replaceText(java.lang.CharSequence))([CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html) newTextContent)
Replaces the current context text with the new text content.

## Field Details

### EDITABLE

static final int EDITABLE

The returned text is in editable context.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.content.TextContext.EDITABLE)

### EDITABLE_IN_FILTERED_CONDITIONAL_PROFILING

static final int EDITABLE_IN_FILTERED_CONDITIONAL_PROFILING

The returned text is in editable context but a profiling condition is applied and filters the node when the output will be published..
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.content.TextContext.EDITABLE_IN_FILTERED_CONDITIONAL_PROFILING)

### NOT_EDITABLE_IN_DELETE_CHANGE_TRACKING

static final int NOT_EDITABLE_IN_DELETE_CHANGE_TRACKING

The returned text is in delete change tracking context.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.content.TextContext.NOT_EDITABLE_IN_DELETE_CHANGE_TRACKING)

### NOT_EDITABLE_IN_READ_ONLY

static final int NOT_EDITABLE_IN_READ_ONLY

The returned text is in an entity or content reference.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.content.TextContext.NOT_EDITABLE_IN_READ_ONLY)

## Method Details

### getNode

[AuthorNode](../node/AuthorNode.md) getNode()

Get the parent node surrounding this text.
  Returns: The node in which the text is located, never null Since: 23
### getText

[CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html) getText()

Gets the current text from the context.
  Returns: The current text from the context.
### getTextStartOffset

int getTextStartOffset()

Gets the start offset of the returned text. The start offset is absolute in the Author Document's content.
  Returns: The start offset of the returned text.
### getTextEndOffset

int getTextEndOffset()

Gets the end offset of the returned text. The end offset is absolute in the Author Document's content.
  Returns: The end offset of the returned text. It is exclusive.
### getEditableState

int getEditableState()

Check if we can edit at the current iterator offset.
  Returns: The returned value is one of the following constants:
        * [EDITABLE](#EDITABLE) - text is in editable context.
        * [EDITABLE_IN_FILTERED_CONDITIONAL_PROFILING](#EDITABLE_IN_FILTERED_CONDITIONAL_PROFILING) - text is in editable context but a profiling condition is applied and filters the node when the output will be published
        * [NOT_EDITABLE_IN_READ_ONLY](#NOT_EDITABLE_IN_READ_ONLY) - text is in an entity or content reference
        * [NOT_EDITABLE_IN_DELETE_CHANGE_TRACKING](#NOT_EDITABLE_IN_DELETE_CHANGE_TRACKING) - text is in delete change tracking context

### inVisibleContent

boolean inVisibleContent()

Check if the range is in visible content.
  Returns: true if the range is in visible content.
### inSpacePreserve

boolean inSpacePreserve()

Check if the range is in a CSS white-space preserve context.
  Returns: true if the range is in space preserve context. Since: 23
### replaceText

void replaceText([CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html) newTextContent)

Replaces the current context text with the new text content.
  Parameters: newTextContent - The new text content.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
