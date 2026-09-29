Package [ro.sync.exml.workspace.api.editor.page](package-summary.md)

# Interface WSTextBasedEditorPage
    All Superinterfaces: [WSEditorPage](WSEditorPage.md)   All Known Subinterfaces: [AuthorEditorAccess](../../../../../ecss/extensions/api/access/AuthorEditorAccess.md), [IWebappAuthorEditorAccess](../../../../../ecss/extensions/api/webapp/access/IWebappAuthorEditorAccess.md), [WSAuthorComponentEditorPage](author/WSAuthorComponentEditorPage.md), [WSAuthorEditorPage](author/WSAuthorEditorPage.md), [WSAuthorEditorPageBase](author/WSAuthorEditorPageBase.md), [WSTextEditorPage](text/WSTextEditorPage.md), [WSXMLTextEditorPage](text/xml/WSXMLTextEditorPage.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WSTextBasedEditorPageextends [WSEditorPage](WSEditorPage.md)
Provides access to methods related to the editor actions and information for the Text and Author pages.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [copy](#copy())()
Copy the selected content to clipboard.
  [Anchor](Anchor.md) [createAnchor](#createAnchor(int))(int offset)
Create an anchor at a certain offset in the content of this Text or Author editing mode.
  void [deleteSelection](#deleteSelection())()
Delete the selected text, if any.
  int [getCaretOffset](#getCaretOffset())()
The current caret offset.
  int [getColumnOfOffset](#getColumnOfOffset(int))(int offset)
Returns the column number corresponding to the given offset within the content.
  int [getLineOfOffset](#getLineOfOffset(int))(int offset)
Retrieves the line number that contains the specified offset within the content.
  [Point](../../../../view/graphics/Point.md) [getLocationOnScreenAsPoint](#getLocationOnScreenAsPoint(int,int))(int x, int y)
Take relative mouse coordinates and translate then to absolute on-screen coordinates.
  [Point](../../../../view/graphics/Point.md) [getLocationRelativeToEditorFromScreen](#getLocationRelativeToEditorFromScreen(int,int))(int x, int y)
Take mouse coordinates relative to the main application frame/display and translate then to coordinates relative to the editing area.
  int [getOffsetForAnchor](#getOffsetForAnchor(ro.sync.exml.workspace.api.editor.page.Anchor))([Anchor](Anchor.md) anchor)
Get the offset corresponding to an Anchor which was created either in this editing mode or in another editing mode/page.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSelectedText](#getSelectedText())()
Get the selected text.
  int [getSelectionEnd](#getSelectionEnd())()
Get selection end offset.
  int [getSelectionStart](#getSelectionStart())()
Get selection start offset.
  int[] [getStartEndOffsets](#getStartEndOffsets(ro.sync.document.DocumentPositionedInfo))([DocumentPositionedInfo](../../../../../document/DocumentPositionedInfo.md) dpInfo)
Find the start and end offsets that correspond to the given [DocumentPositionedInfo](../../../../../document/DocumentPositionedInfo.md) (DPI) object.
  int[] [getWordAtCaret](#getWordAtCaret())()
Compute the offsets of the word that contains the caret position.
  boolean [hasSelection](#hasSelection())()
Check if the editor page has a selection
  [Rectangle](../../../../view/graphics/Rectangle.md) [modelToViewRectangle](#modelToViewRectangle(int))(int offset)
Returns a representation of the caret shape for the specified document offset.
  void [scrollCaretToVisible](#scrollCaretToVisible())()
Smart scroll so that the current caret position and some content around it becomes visible.
  void [select](#select(int,int))(int startOffset, int endOffset)
Select the interval between start and end offset.
  void [selectWord](#selectWord())()
Select the word at caret, if any.
  void [setCaretPosition](#setCaretPosition(int))(int offset)
Move the caret to the specified offset.
  int [viewToModelOffset](#viewToModelOffset(int,int))(int x, int y)
Get the position in the document corresponding to the point in the editing component.

### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSEditorPage](WSEditorPage.md)
 [getParentEditor](WSEditorPage.md#getParentEditor()), [hasFocus](WSEditorPage.md#hasFocus()), [isEditable](WSEditorPage.md#isEditable()), [requestFocus](WSEditorPage.md#requestFocus()), [setEditable](WSEditorPage.md#setEditable(boolean)), [setReadOnly](WSEditorPage.md#setReadOnly(java.lang.String)), [setReadOnly](WSEditorPage.md#setReadOnly(ro.sync.exml.workspace.api.editor.ReadOnlyReason))
## Method Details

### getSelectionStart

int getSelectionStart()

Get selection start offset. It is inclusive.
  Returns: The selection start offset, 0 based.
### getSelectionEnd

int getSelectionEnd()

Get selection end offset. It is exclusive.
  Returns: The selection end offset, 0 based.
### getSelectedText

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSelectedText()

Get the selected text. The text does not contain XML tags for the Author page.
  Returns: The selected text or an empty string if no selection is present.
### getCaretOffset

int getCaretOffset()

The current caret offset.
  Returns: The caret offset, 0 based.
### deleteSelection

void deleteSelection()

Delete the selected text, if any.

### hasSelection

boolean hasSelection()

Check if the editor page has a selection
  Returns: true if there is a selection, false otherwise.
### selectWord

void selectWord()

Select the word at caret, if any.

### setCaretPosition

void setCaretPosition(int offset)

Move the caret to the specified offset.
  Parameters: offset - The offset where the caret should be positioned, 0 based.
### select

void select(int startOffset, int endOffset)

Select the interval between start and end offset.
  Parameters: startOffset - Inclusive start offset endOffset - Exclusive end offset
### getWordAtCaret

int[] getWordAtCaret()

Compute the offsets of the word that contains the caret position.
  Returns: An array with the start and end offsets of the word at caret or null if the values couldn't be obtained. The start offset is inclusive and greater or equal than 1. The end offset is also inclusive and less or equal than the content length.
### getLocationOnScreenAsPoint

[Point](../../../../view/graphics/Point.md) getLocationOnScreenAsPoint(int x, int y)

Take relative mouse coordinates and translate then to absolute on-screen coordinates.
  Parameters: x - The "x" coordinate relative to the viewport origin. y - The "y" coordinate relative to the viewport origin. Returns: A point with the "x" and "y" coordinates relative to the screen. It does not return a null Point.
### getLocationRelativeToEditorFromScreen

[Point](../../../../view/graphics/Point.md) getLocationRelativeToEditorFromScreen(int x, int y)

Take mouse coordinates relative to the main application frame/display and translate then to coordinates relative to the editing area.
  Parameters: x - The "x" coordinate which is relative to the main application frame/display. y - The "y" coordinate which is relative to the main application frame/display. Returns: A point with the "x" and "y" coordinates relative to the editing component area. It does not return a null Point. For example an Eclipse org.eclipse.swt.dnd.DropTargetEvent has the x and y coordinates relative to the Display. In order to use API like viewToModelOffset(), the coordinates need to be translated relative to the editing area. Since: 14.2
### modelToViewRectangle

[Rectangle](../../../../view/graphics/Rectangle.md) modelToViewRectangle(int offset)

Returns a representation of the caret shape for the specified document offset.
  Parameters: offset - The document offset to get the corresponding caret shape for. Returns: The caret rectangle shape. It does not return a null Rectangle.
### viewToModelOffset

int viewToModelOffset(int x, int y)

Get the position in the document corresponding to the point in the editing component.
  Parameters: x - The "x" coordinate relative to the editing component origin. y - The "y" coordinate relative to the editing component origin. Returns: The offset corresponding to the given point. The method does not return null, instead an undefined view to model info object is returned if a valid one could not be determined.
### getStartEndOffsets

int[] getStartEndOffsets([DocumentPositionedInfo](../../../../../document/DocumentPositionedInfo.md) dpInfo)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Find the start and end offsets that correspond to the given [DocumentPositionedInfo](../../../../../document/DocumentPositionedInfo.md) (DPI) object.
  Parameters: dpInfo - The document position information. Returns: an array of length two containing the start offset at index 0 and the end offset at index 1, or null if the offset cannot be computed for the given DPI. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If the document position info does not correspond to a valid position in document. Since: 14.1
### createAnchor

[Anchor](Anchor.md) createAnchor(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create an anchor at a certain offset in the content of this Text or Author editing mode. The anchor can later be used in the current or in another editing mode to identify an offset particular to it. For example you can create an anchor in the Author editing mode based on an Author-specific offset and then use it in the Text editing mode to identify a specific offset in the Text editing page. A previous created anchor will not be updated dynamically when changes are made in the document so using it later on will not guarantee that it will point exactly at the offset for which it was originally computed.
  Parameters: offset - The offset in the edited content. Returns: An implementation independent anchor which indicates to this offset. The anchor is not automatically updated when the content in the document changes. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offset is not valid. Since: 21
### getOffsetForAnchor

int getOffsetForAnchor([Anchor](Anchor.md) anchor)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Get the offset corresponding to an Anchor which was created either in this editing mode or in another editing mode/page.
  Parameters: anchor - The anchor. Returns: The offset in this page's contents corresponding to the Anchor object. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When there are problems identifying the offset. Since: 21
### scrollCaretToVisible

void scrollCaretToVisible()

Smart scroll so that the current caret position and some content around it becomes visible.
  Since: 18
### copy

void copy()

Copy the selected content to clipboard. If there is no selection, this method does nothing.
  Since: 27
### getLineOfOffset

int getLineOfOffset(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Retrieves the line number that contains the specified offset within the content.
  Parameters: offset - Offset in document. Returns: The line which contains the specified offset. 1 based. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offset is not valid. Since: 28.1  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

### getColumnOfOffset

int getColumnOfOffset(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Returns the column number corresponding to the given offset within the content. The column is determined within the line that contains the offset.
  Parameters: offset - The offset to check. Returns: The column in the line that contains the offset. 1 based. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If the offset is not a valid position in the content Since: 28.1  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
