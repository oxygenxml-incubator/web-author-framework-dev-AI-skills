Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorSelectionAndCaretModel
    All Superinterfaces: [AuthorSelectionModel](AuthorSelectionModel.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorSelectionAndCaretModelextends [AuthorSelectionModel](AuthorSelectionModel.md)
Interface to the author selection and caret model providing methods to query and modify the selection intervals and caret position.
  Since: 15.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 int [getCaretOffset](#getCaretOffset())()
Returns the offset of the caret in the document.
  void [moveTo](#moveTo(int))(int offset)
Moves the caret to the specified position.
  void [moveTo](#moveTo(int,boolean))(int offset, boolean select)
Moves the caret to the new offset, possibly changing the selection.

### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorSelectionModel](AuthorSelectionModel.md)
 [addSelection](AuthorSelectionModel.md#addSelection(int,int)), [addSelectionIntervals](AuthorSelectionModel.md#addSelectionIntervals(java.util.List,boolean)), [clearSelection](AuthorSelectionModel.md#clearSelection()), [getSelectionInterpretationMode](AuthorSelectionModel.md#getSelectionInterpretationMode()), [getSelectionInterval](AuthorSelectionModel.md#getSelectionInterval()), [getSelectionIntervals](AuthorSelectionModel.md#getSelectionIntervals()), [hasMultipleSelection](AuthorSelectionModel.md#hasMultipleSelection()), [hasSelection](AuthorSelectionModel.md#hasSelection()), [setSelection](AuthorSelectionModel.md#setSelection(int,int)), [setSelection](AuthorSelectionModel.md#setSelection(int,int,boolean)), [setSelectionInterpretationMode](AuthorSelectionModel.md#setSelectionInterpretationMode(ro.sync.ecss.extensions.api.SelectionInterpretationMode)), [setSelectionIntervals](AuthorSelectionModel.md#setSelectionIntervals(java.util.List,boolean))
## Method Details

### getCaretOffset

int getCaretOffset()

Returns the offset of the caret in the document.
  Returns: The offset of the caret in the document.
### moveTo

void moveTo(int offset)

Moves the caret to the specified position.
  Parameters: offset - The new position of the caret.
### moveTo

void moveTo(int offset, boolean select)

Moves the caret to the new offset, possibly changing the selection.
  Parameters: offset - new offset for the caret. The offset must be >= 1 and less than the document size; if not, it is silently ignored. select - if true, the current selection is extended to match the new caret offset.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
