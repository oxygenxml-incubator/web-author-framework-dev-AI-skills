Package [ro.sync.exml.workspace.api.editor.page.text.xml](package-summary.md)

# Interface WSXMLTextEditorPage
    All Superinterfaces: [WSEditorPage](../../WSEditorPage.md), [WSTextBasedEditorPage](../../WSTextBasedEditorPage.md), [WSTextEditorPage](../WSTextEditorPage.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WSXMLTextEditorPageextends [WSTextEditorPage](../WSTextEditorPage.md)
Contains methods specific to XML editors.
  Since: 14
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] [evaluateXPath](#evaluateXPath(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression)
Evaluates an XPath expression.
  [WSXMLTextNodeRange](WSXMLTextNodeRange.md)[] [findElementsByXPath](#findElementsByXPath(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression)
Finds the nodes selected by the given XPath expression.
  [TextDocumentController](TextDocumentController.md) [getDocumentController](#getDocumentController())()
Get a controller which has utility methods to manipulate XML content in the Text editing mode.
  [WSTextXMLSchemaManager](../WSTextXMLSchemaManager.md) [getXMLSchemaManager](#getXMLSchemaManager())()
Get the schema manager used to ask useful information about allowed elements and the context of the current offset.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXPath](#getXPath(int,boolean))(int offset, boolean includeIndexInParent)
Get the XPath corresponding to the XML element containing the given offset.

### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSEditorPage](../../WSEditorPage.md)
 [getParentEditor](../../WSEditorPage.md#getParentEditor()), [hasFocus](../../WSEditorPage.md#hasFocus()), [isEditable](../../WSEditorPage.md#isEditable()), [requestFocus](../../WSEditorPage.md#requestFocus()), [setEditable](../../WSEditorPage.md#setEditable(boolean)), [setReadOnly](../../WSEditorPage.md#setReadOnly(java.lang.String)), [setReadOnly](../../WSEditorPage.md#setReadOnly(ro.sync.exml.workspace.api.editor.ReadOnlyReason))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSTextBasedEditorPage](../../WSTextBasedEditorPage.md)
 [copy](../../WSTextBasedEditorPage.md#copy()), [createAnchor](../../WSTextBasedEditorPage.md#createAnchor(int)), [deleteSelection](../../WSTextBasedEditorPage.md#deleteSelection()), [getCaretOffset](../../WSTextBasedEditorPage.md#getCaretOffset()), [getLocationOnScreenAsPoint](../../WSTextBasedEditorPage.md#getLocationOnScreenAsPoint(int,int)), [getLocationRelativeToEditorFromScreen](../../WSTextBasedEditorPage.md#getLocationRelativeToEditorFromScreen(int,int)), [getOffsetForAnchor](../../WSTextBasedEditorPage.md#getOffsetForAnchor(ro.sync.exml.workspace.api.editor.page.Anchor)), [getSelectedText](../../WSTextBasedEditorPage.md#getSelectedText()), [getSelectionEnd](../../WSTextBasedEditorPage.md#getSelectionEnd()), [getSelectionStart](../../WSTextBasedEditorPage.md#getSelectionStart()), [getStartEndOffsets](../../WSTextBasedEditorPage.md#getStartEndOffsets(ro.sync.document.DocumentPositionedInfo)), [getWordAtCaret](../../WSTextBasedEditorPage.md#getWordAtCaret()), [hasSelection](../../WSTextBasedEditorPage.md#hasSelection()), [modelToViewRectangle](../../WSTextBasedEditorPage.md#modelToViewRectangle(int)), [scrollCaretToVisible](../../WSTextBasedEditorPage.md#scrollCaretToVisible()), [select](../../WSTextBasedEditorPage.md#select(int,int)), [selectWord](../../WSTextBasedEditorPage.md#selectWord()), [setCaretPosition](../../WSTextBasedEditorPage.md#setCaretPosition(int)), [viewToModelOffset](../../WSTextBasedEditorPage.md#viewToModelOffset(int,int))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.text.[WSTextEditorPage](../WSTextEditorPage.md)
 [addExternalContentCompletionProvider](../WSTextEditorPage.md#addExternalContentCompletionProvider(ro.sync.exml.workspace.api.editor.page.text.ExternalContentCompletionProvider)), [addPopUpMenuCustomizer](../WSTextEditorPage.md#addPopUpMenuCustomizer(ro.sync.exml.workspace.api.editor.page.text.TextPopupMenuCustomizer)), [addQuickAssistProcessor](../WSTextEditorPage.md#addQuickAssistProcessor(ro.sync.exml.editor.quickassist.SimpleQuickAssistProcessor)), [beginCompoundUndoableEdit](../WSTextEditorPage.md#beginCompoundUndoableEdit()), [endCompoundUndoableEdit](../WSTextEditorPage.md#endCompoundUndoableEdit()), [getActionsProvider](../WSTextEditorPage.md#getActionsProvider()), [getColumnOfOffset](../WSTextEditorPage.md#getColumnOfOffset(int)), [getDocument](../WSTextEditorPage.md#getDocument()), [getLineOfOffset](../WSTextEditorPage.md#getLineOfOffset(int)), [getOffsetOfLineEnd](../WSTextEditorPage.md#getOffsetOfLineEnd(int)), [getOffsetOfLineStart](../WSTextEditorPage.md#getOffsetOfLineStart(int)), [getTextComponent](../WSTextEditorPage.md#getTextComponent()), [removeExternalContentCompletionProvider](../WSTextEditorPage.md#removeExternalContentCompletionProvider(ro.sync.exml.workspace.api.editor.page.text.ExternalContentCompletionProvider)), [removePopUpMenuCustomizer](../WSTextEditorPage.md#removePopUpMenuCustomizer(ro.sync.exml.workspace.api.editor.page.text.TextPopupMenuCustomizer)), [removeQuickAssistProcessor](../WSTextEditorPage.md#removeQuickAssistProcessor(ro.sync.exml.editor.quickassist.SimpleQuickAssistProcessor))
## Method Details

### findElementsByXPath

[WSXMLTextNodeRange](WSXMLTextNodeRange.md)[] findElementsByXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression)throws [XPathException](XPathException.md)

Finds the nodes selected by the given XPath expression. The result of this function is an array of [WSXMLTextNodeRange](WSXMLTextNodeRange.md) selected by the given XPath expression. For example executing the expression:  //node() will return an array with all the node ranges in the document. But the result of calling the function with the expression:  count(//node()) will return an empty array.
  Parameters: xpathExpression - The XPath expression. If the XPath expression is relative, it will be computed in the context of the current caret position. Returns: The node ranges selected by the XPath expression. It does not return a null array of nodes. If the evaluation of the XPath expression fails it will return an empty array. Throws: [XPathException](XPathException.md) - If the XPath expression failed to be evaluated.
### evaluateXPath

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] evaluateXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression)throws [XPathException](XPathException.md)

Evaluates an XPath expression. This function returns the result of the given XPath expression as an array of [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html). For example, executing the expression:  //node() will return an array with all the DOM Nodes created over the XML structure. while evaluating the expression:  count(//node()) will return an array having a single component representing the number of nodes in the document. Evaluating the expression:  //node(), count(//node()) will return an array containing all DOM Nodes and having as last component the total number of nodes.
  Parameters: xpathExpression - The XPath expression. If the XPath expression is relative, it will be computed in the context of the current caret position. Returns: An array of objects representing the XPath result. It does not return a null array. If the XPath evaluation fails it will return an empty array. Throws: [XPathException](XPathException.md) - If the XPath expression failed to be evaluated.
### getXMLSchemaManager

[WSTextXMLSchemaManager](../WSTextXMLSchemaManager.md) getXMLSchemaManager()

Get the schema manager used to ask useful information about allowed elements and the context of the current offset.
  Specified by: [getXMLSchemaManager](../WSTextEditorPage.md#getXMLSchemaManager()) in interface [WSTextEditorPage](../WSTextEditorPage.md) Returns: the XML Schema Manager used to ask useful information about allowed elements and the context of the current offset.
### getDocumentController

[TextDocumentController](TextDocumentController.md) getDocumentController()

Get a controller which has utility methods to manipulate XML content in the Text editing mode.
  Returns: The text document controller. Since: 16.1
### getXPath

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXPath(int offset, boolean includeIndexInParent)

Get the XPath corresponding to the XML element containing the given offset.
  Parameters: offset - The current offset. includeIndexInParent - If true the child index in parent is included. Example (without index): /personnel/person/name/family Example (with index): /personnel/person[2]/name[1]/family[1] Returns: The XPath or null if cannot be computed. Since: 27
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
