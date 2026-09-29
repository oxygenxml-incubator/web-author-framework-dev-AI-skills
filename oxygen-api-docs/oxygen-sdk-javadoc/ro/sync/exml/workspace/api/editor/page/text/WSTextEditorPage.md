Package [ro.sync.exml.workspace.api.editor.page.text](package-summary.md)

# Interface WSTextEditorPage
    All Superinterfaces: [WSEditorPage](../WSEditorPage.md), [WSTextBasedEditorPage](../WSTextBasedEditorPage.md)   All Known Subinterfaces: [WSXMLTextEditorPage](xml/WSXMLTextEditorPage.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WSTextEditorPageextends [WSTextBasedEditorPage](../WSTextBasedEditorPage.md)
Text editor page access.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addExternalContentCompletionProvider](#addExternalContentCompletionProvider(ro.sync.exml.workspace.api.editor.page.text.ExternalContentCompletionProvider))([ExternalContentCompletionProvider](ExternalContentCompletionProvider.md) ccProvider)
Add a content completion provider, that can be used to display additional content completion proposals.
  void [addPopUpMenuCustomizer](#addPopUpMenuCustomizer(ro.sync.exml.workspace.api.editor.page.text.TextPopupMenuCustomizer))([TextPopupMenuCustomizer](TextPopupMenuCustomizer.md) popUpCustomizer)
Add the pop-up menu customizer which can be used to customize the pop-up menu (add/remove actions) before showing it in the Text page.
  void [addQuickAssistProcessor](#addQuickAssistProcessor(ro.sync.exml.editor.quickassist.SimpleQuickAssistProcessor))([SimpleQuickAssistProcessor](../../../../../editor/quickassist/SimpleQuickAssistProcessor.md) processor)
Register a quick assist processor.
  void [beginCompoundUndoableEdit](#beginCompoundUndoableEdit())()
Begin a compound undoable edit operation.
  void [endCompoundUndoableEdit](#endCompoundUndoableEdit())()
End a compound undoable edit operation.
  [TextActionsProvider](actions/TextActionsProvider.md) [getActionsProvider](#getActionsProvider())()
Provides access to actions already defined in the Text page like: Undo, Redo, etc.
  int [getColumnOfOffset](#getColumnOfOffset(int))(int offset)
Retrieve for an offset position in the content the corresponding column number in the line that contains the offset.
  [Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html) [getDocument](#getDocument())()
Get the edited document.
  int [getLineOfOffset](#getLineOfOffset(int))(int offset)
Retrieve for an offset position in the content the line number that contains the offset.
  int [getOffsetOfLineEnd](#getOffsetOfLineEnd(int))(int lineNumber)
Gets the offset of the end of the specified line (return >=0).
  int [getOffsetOfLineStart](#getOffsetOfLineStart(int))(int lineNumber)
Gets the offset of the start of the specified line (return >=0).
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getTextComponent](#getTextComponent())()
Get the internal text component which is currently used for editing.
  [WSTextXMLSchemaManager](WSTextXMLSchemaManager.md) [getXMLSchemaManager](#getXMLSchemaManager())()
Get the schema manager used to ask useful information about allowed elements and the context of the current offset.
  void [removeExternalContentCompletionProvider](#removeExternalContentCompletionProvider(ro.sync.exml.workspace.api.editor.page.text.ExternalContentCompletionProvider))([ExternalContentCompletionProvider](ExternalContentCompletionProvider.md) ccProvider)
Remove a content completion provider that was added to the current editor.
  void [removePopUpMenuCustomizer](#removePopUpMenuCustomizer(ro.sync.exml.workspace.api.editor.page.text.TextPopupMenuCustomizer))([TextPopupMenuCustomizer](TextPopupMenuCustomizer.md) popUpCustomizer)
Remove the pop-up menu customizer which is used to customize the pop-up menu (add/remove actions) before showing it in the Text page.
  void [removeQuickAssistProcessor](#removeQuickAssistProcessor(ro.sync.exml.editor.quickassist.SimpleQuickAssistProcessor))([SimpleQuickAssistProcessor](../../../../../editor/quickassist/SimpleQuickAssistProcessor.md) processor)
The processor to be unregistered.

### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSEditorPage](../WSEditorPage.md)
 [getParentEditor](../WSEditorPage.md#getParentEditor()), [hasFocus](../WSEditorPage.md#hasFocus()), [isEditable](../WSEditorPage.md#isEditable()), [requestFocus](../WSEditorPage.md#requestFocus()), [setEditable](../WSEditorPage.md#setEditable(boolean)), [setReadOnly](../WSEditorPage.md#setReadOnly(java.lang.String)), [setReadOnly](../WSEditorPage.md#setReadOnly(ro.sync.exml.workspace.api.editor.ReadOnlyReason))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSTextBasedEditorPage](../WSTextBasedEditorPage.md)
 [copy](../WSTextBasedEditorPage.md#copy()), [createAnchor](../WSTextBasedEditorPage.md#createAnchor(int)), [deleteSelection](../WSTextBasedEditorPage.md#deleteSelection()), [getCaretOffset](../WSTextBasedEditorPage.md#getCaretOffset()), [getLocationOnScreenAsPoint](../WSTextBasedEditorPage.md#getLocationOnScreenAsPoint(int,int)), [getLocationRelativeToEditorFromScreen](../WSTextBasedEditorPage.md#getLocationRelativeToEditorFromScreen(int,int)), [getOffsetForAnchor](../WSTextBasedEditorPage.md#getOffsetForAnchor(ro.sync.exml.workspace.api.editor.page.Anchor)), [getSelectedText](../WSTextBasedEditorPage.md#getSelectedText()), [getSelectionEnd](../WSTextBasedEditorPage.md#getSelectionEnd()), [getSelectionStart](../WSTextBasedEditorPage.md#getSelectionStart()), [getStartEndOffsets](../WSTextBasedEditorPage.md#getStartEndOffsets(ro.sync.document.DocumentPositionedInfo)), [getWordAtCaret](../WSTextBasedEditorPage.md#getWordAtCaret()), [hasSelection](../WSTextBasedEditorPage.md#hasSelection()), [modelToViewRectangle](../WSTextBasedEditorPage.md#modelToViewRectangle(int)), [scrollCaretToVisible](../WSTextBasedEditorPage.md#scrollCaretToVisible()), [select](../WSTextBasedEditorPage.md#select(int,int)), [selectWord](../WSTextBasedEditorPage.md#selectWord()), [setCaretPosition](../WSTextBasedEditorPage.md#setCaretPosition(int)), [viewToModelOffset](../WSTextBasedEditorPage.md#viewToModelOffset(int,int))
## Method Details

### getDocument

[Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html) getDocument()

Get the edited document. For eclipse, the returned instance is an javax.swing.text.Document adapter over the Eclipse native document.
  Returns: The edited document.
### getTextComponent

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getTextComponent()

Get the internal text component which is currently used for editing.
  Returns: for the stand alone version, a javax.swing.JTextArea and for the eclipse implementation a org.eclipse.swt.custom.StyledText. Since: 12
### getXMLSchemaManager

[WSTextXMLSchemaManager](WSTextXMLSchemaManager.md) getXMLSchemaManager()

Get the schema manager used to ask useful information about allowed elements and the context of the current offset.
  Returns: the XML Schema Manager used to ask useful information about allowed elements and the context of the current offset. Only available for opened XML files. Since: 12.1
### beginCompoundUndoableEdit

void beginCompoundUndoableEdit()

Begin a compound undoable edit operation. This is useful if you make modifications through the API and want Oxygen to undo in a single step. This should be used like:
```
try{
  beginCompoundUndoableEdit();
  //YOUR CODE HERE
 } finally{
  endCompoundUndoableEdit();
 }

```

  Since: 12.2
### endCompoundUndoableEdit

void endCompoundUndoableEdit()

End a compound undoable edit operation. This is useful if you make modifications through the API and want Oxygen to undo in a single step. This should be used like:
```
try{
  beginCompoundUndoableEdit();
  //YOUR CODE HERE
 } finally{
  endCompoundUndoableEdit();
 }

```

  Since: 12.2
### getLineOfOffset

int getLineOfOffset(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Retrieve for an offset position in the content the line number that contains the offset. The line number returned is indexed in 1.
  Specified by: [getLineOfOffset](../WSTextBasedEditorPage.md#getLineOfOffset(int)) in interface [WSTextBasedEditorPage](../WSTextBasedEditorPage.md) Parameters: offset - Offset in document. Returns: The line which contains the specified offset. 1 based. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offset is not valid. Since: 14
### getColumnOfOffset

int getColumnOfOffset(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Retrieve for an offset position in the content the corresponding column number in the line that contains the offset.
  Specified by: [getColumnOfOffset](../WSTextBasedEditorPage.md#getColumnOfOffset(int)) in interface [WSTextBasedEditorPage](../WSTextBasedEditorPage.md) Parameters: offset - The offset that is to be checked. Returns: The column in the line that contains the offset, 1 based. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - Bad Location Exception. Since: 14
### getOffsetOfLineStart

int getOffsetOfLineStart(int lineNumber)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Gets the offset of the start of the specified line (return >=0). The line number is indexed in 1.
  Parameters: lineNumber - The number of the line. Indexed in 1. Returns: The offset of the start of the specified line. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When line does not exist. [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - If the line number is out of range. Since: 14
### getOffsetOfLineEnd

int getOffsetOfLineEnd(int lineNumber)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Gets the offset of the end of the specified line (return >=0). This will be equal to the start offset of the next line, if there is one. The line number is indexed in 1.
  Parameters: lineNumber - The number of the line. Indexed in 1. Returns: The offset of the end of the specified line. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If the line number is out of range. Since: 14
### addPopUpMenuCustomizer

void addPopUpMenuCustomizer([TextPopupMenuCustomizer](TextPopupMenuCustomizer.md) popUpCustomizer)

Add the pop-up menu customizer which can be used to customize the pop-up menu (add/remove actions) before showing it in the Text page. If the customizer is already added, it will not be added again.
  Parameters: popUpCustomizer - the pop-up menu customizer. Since: 14.1
### removePopUpMenuCustomizer

void removePopUpMenuCustomizer([TextPopupMenuCustomizer](TextPopupMenuCustomizer.md) popUpCustomizer)

Remove the pop-up menu customizer which is used to customize the pop-up menu (add/remove actions) before showing it in the Text page.
  Parameters: popUpCustomizer - the pop-up menu customizer. Since: 14.1
### getActionsProvider

[TextActionsProvider](actions/TextActionsProvider.md) getActionsProvider()

Provides access to actions already defined in the Text page like: Undo, Redo, etc.
  Returns: access to actions already defined in the Text page. Since: 14.2
### addExternalContentCompletionProvider

void addExternalContentCompletionProvider([ExternalContentCompletionProvider](ExternalContentCompletionProvider.md) ccProvider)

Add a content completion provider, that can be used to display additional content completion proposals. Not implemented in the Oxygen Eclipse Plug-in.
  Parameters: ccProvider - The content completion provider. Since: 22.1
### removeExternalContentCompletionProvider

void removeExternalContentCompletionProvider([ExternalContentCompletionProvider](ExternalContentCompletionProvider.md) ccProvider)

Remove a content completion provider that was added to the current editor. Not implemented in the Oxygen Eclipse Plug-in.
  Parameters: ccProvider - The content completion provider to be removed. Since: 22.1
### addQuickAssistProcessor

void addQuickAssistProcessor([SimpleQuickAssistProcessor](../../../../../editor/quickassist/SimpleQuickAssistProcessor.md) processor)

Register a quick assist processor. This allow you to provide quick custom quick assist proposals in the current editor page quick assist menu.
  Parameters: processor - The processor to be registered. Since: 26.1
### removeQuickAssistProcessor

void removeQuickAssistProcessor([SimpleQuickAssistProcessor](../../../../../editor/quickassist/SimpleQuickAssistProcessor.md) processor)

The processor to be unregistered.
  Parameters: processor - The processor to be unregistered. Since: 26.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
