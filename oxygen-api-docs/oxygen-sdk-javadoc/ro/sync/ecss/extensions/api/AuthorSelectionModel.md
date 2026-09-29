Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorSelectionModel
    All Known Subinterfaces: [AuthorSelectionAndCaretModel](AuthorSelectionAndCaretModel.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorSelectionModel
Get the Author selection model containing access to all Author selection intervals and methods for adding simple and multiple selections.
  Since: 14
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addSelection](#addSelection(int,int))(int startOffset, int endOffset)
Select the interval between start and end offset.
  void [addSelectionIntervals](#addSelectionIntervals(java.util.List,boolean))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](ContentInterval.md)> intervals, boolean scrollToVisible)
Add Author editor page selection intervals.
  void [clearSelection](#clearSelection())()
Clears all selections from Author editor page and resets the selection interpretation mode (see [getSelectionInterpretationMode()](#getSelectionInterpretationMode())).
  [SelectionInterpretationMode](SelectionInterpretationMode.md) [getSelectionInterpretationMode](#getSelectionInterpretationMode())()
Get the interpretation mode of the actual selection from the Author editor page.
  [ContentInterval](ContentInterval.md) [getSelectionInterval](#getSelectionInterval())()
Get the current selection interval.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](ContentInterval.md)> [getSelectionIntervals](#getSelectionIntervals())()
Get all Author editor page selection intervals.
  boolean [hasMultipleSelection](#hasMultipleSelection())()
Check if the Author editor page has multiple selections.
  boolean [hasSelection](#hasSelection())()
Check if the Author editor page has selection.
  void [setSelection](#setSelection(int,int))(int startOffset, int endOffset)
Select the interval between start and end offset.
  void [setSelection](#setSelection(int,int,boolean))(int startOffset, int endOffset, boolean scrollToBVisible)
Select the interval between start and end offset.
  void [setSelectionInterpretationMode](#setSelectionInterpretationMode(ro.sync.ecss.extensions.api.SelectionInterpretationMode))([SelectionInterpretationMode](SelectionInterpretationMode.md) interpretationMode)
Impose the interpretation mode of the actual selection from the Author editor page.
  void [setSelectionIntervals](#setSelectionIntervals(java.util.List,boolean))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](ContentInterval.md)> intervals, boolean scrollToVisible)
Sets the Author editor page selection intervals.

## Method Details

### setSelectionInterpretationMode

void setSelectionInterpretationMode([SelectionInterpretationMode](SelectionInterpretationMode.md) interpretationMode)

Impose the interpretation mode of the actual selection from the Author editor page. See [SelectionInterpretationMode](SelectionInterpretationMode.md) for more details about the interpretation of selection in Author mode.  This interpretation mode is reseted when the next caret moved is performed or another interpretation mode is imposed.
  Parameters: interpretationMode - The selection interpretation mode.
### getSelectionInterpretationMode

[SelectionInterpretationMode](SelectionInterpretationMode.md) getSelectionInterpretationMode()

Get the interpretation mode of the actual selection from the Author editor page. See [SelectionInterpretationMode](SelectionInterpretationMode.md) for more details about the interpretation of selection in Author mode.  This interpretation mode is reseted when the next caret moved is performed or another interpretation mode is imposed.
  Returns: The selection interpretation mode.
### getSelectionIntervals

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](ContentInterval.md)> getSelectionIntervals()

Get all Author editor page selection intervals. Each [ContentInterval](ContentInterval.md) contains the **inclusive** start selection offset and the **exclusive** end selection offset.  The selection intervals are added to the list in the same order in which the selections are made in the Author editor page. If the caret is not inside a selection the last selection interval points to the caret offset (both [ContentInterval.getStartOffset()](ContentInterval.md#getStartOffset()) and [ContentInterval.getEndOffset()](ContentInterval.md#getEndOffset())will return the caret position). Otherwise, the last [ContentInterval](ContentInterval.md) from the list corresponds with the last selection made in the editor.  This method never returns null. If there is no selection, the list contains a single [ContentInterval](ContentInterval.md) that points to the caret offset.
  Returns: the list containing all the Author editor page selection intervals.
### getSelectionInterval

[ContentInterval](ContentInterval.md) getSelectionInterval()

Get the current selection interval. This is the last selection made in the Author editor page (the last selection from the [getSelectionIntervals()](#getSelectionIntervals())selections list). If the caret offset is not included in a selection range, the selection interval points to the caret offset (both [ContentInterval.getStartOffset()](ContentInterval.md#getStartOffset())and [ContentInterval.getEndOffset()](ContentInterval.md#getEndOffset()) will return the caret position). The [ContentInterval](ContentInterval.md) contains the **inclusive** start selection offset and the **exclusive** end selection offset.  This method never returns null. If there is no selection, both the start and end offset of the interval will be the caret position.
  Returns: The interval of the current selection.
### hasSelection

boolean hasSelection()

Check if the Author editor page has selection.
  Returns: true if there is a selection in Author editor page.
### hasMultipleSelection

boolean hasMultipleSelection()

Check if the Author editor page has multiple selections.
  Returns: true if there are at least two selections in Author editor page.
### setSelection

void setSelection(int startOffset, int endOffset)

Select the interval between start and end offset. This selection interval is considered to be the current one (the one that will be returned by the [getSelectionInterval()](#getSelectionInterval()) method).   The previous Author selections are discarded.
  Parameters: startOffset - **Inclusive** start offset endOffset - **Exclusive** end offset
### setSelection

void setSelection(int startOffset, int endOffset, boolean scrollToBVisible)

Select the interval between start and end offset. This selection interval is considered to be the current one (the one that will be returned by the [getSelectionInterval()](#getSelectionInterval()) method).   The previous Author selections are discarded.
  Parameters: startOffset - **Inclusive** start offset endOffset - **Exclusive** end offset scrollToBVisible - true to scroll to visible
### addSelection

void addSelection(int startOffset, int endOffset)

Select the interval between start and end offset.  This selection interval is considered to be the current one (the one that will be returned by the [getSelectionInterval()](#getSelectionInterval()) method).   The previous Author selections are kept. Call [getSelectionIntervals()](#getSelectionIntervals()) method to get all the selection intervals from Author editor page.
  Parameters: startOffset - **Inclusive** start offset endOffset - **Exclusive** end offset
### clearSelection

void clearSelection()

Clears all selections from Author editor page and resets the selection interpretation mode (see [getSelectionInterpretationMode()](#getSelectionInterpretationMode())). The caret will remain in the same position.  After this method is executed, [getSelectionIntervals()](#getSelectionIntervals()) will return a single selection interval that points to the caret offset (both [ContentInterval.getStartOffset()](ContentInterval.md#getStartOffset())and [ContentInterval.getEndOffset()](ContentInterval.md#getEndOffset()) will return the caret position).

### setSelectionIntervals

void setSelectionIntervals([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](ContentInterval.md)> intervals, boolean scrollToVisible)

Sets the Author editor page selection intervals. Each [ContentInterval](ContentInterval.md) contains the **inclusive** start selection offset and the **exclusive** end selection offset.  The selection intervals are added to the Author editor page order in which they are in the list. The last selection interval end offset will set the caret position.
  Parameters: intervals - the list containing all the Author editor page selection intervals. scrollToVisible - If true the start offset of the last interval will be scrolled to visible. Since: 17.1
### addSelectionIntervals

void addSelectionIntervals([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](ContentInterval.md)> intervals, boolean scrollToVisible)

Add Author editor page selection intervals. Each [ContentInterval](ContentInterval.md) contains the **inclusive** start selection offset and the **exclusive** end selection offset.  The selection intervals are added to the Author editor page order in which they are in the list. The last selection interval end offset will set the caret position.
  Parameters: intervals - the list containing all the Author editor page selection intervals. scrollToVisible - If true the start offset of the last interval will be scrolled to visible. Since: 18
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
