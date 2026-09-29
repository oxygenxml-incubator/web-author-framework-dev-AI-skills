Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorAccessDeprecated
    All Known Subinterfaces: [AuthorAccess](AuthorAccess.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorAccessDeprecated
Contains methods that are deprecated in the [AuthorAccess](AuthorAccess.md) and should no longer be used.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 void [addAuthorListener](#addAuthorListener(ro.sync.ecss.extensions.api.AuthorListener))([AuthorListener](AuthorListener.md) listener)  Deprecated.
Use [AuthorDocumentController.addAuthorListener(AuthorListener)](AuthorDocumentController.md#addAuthorListener(ro.sync.ecss.extensions.api.AuthorListener)) intead.
   [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [chooseFile](#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr)  Deprecated.
Use [WorkspaceUtilities.chooseURL(String, String[], String)](../../../exml/workspace/api/WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String)) instead.
   [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [chooseFile](#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr, boolean openForSave)  Deprecated.
Use [WorkspaceUtilities.chooseFile(String, String[], String, boolean)](../../../exml/workspace/api/WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)) instead.
   [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [chooseURL](#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr)  Deprecated.
Use [WorkspaceUtilities.chooseURL(String, String[], String)](../../../exml/workspace/api/WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String)) instead.
   [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [correctURL](#correctURL(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)  Deprecated.
Use [UtilAccess.correctURL(String)](../../../exml/workspace/api/util/UtilAccess.md#correctURL(java.lang.String)) instead.
   void [deleteSelection](#deleteSelection())()  Deprecated.
Use [WSAuthorEditorPageBase.deleteSelection()](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#deleteSelection()) instead.
   [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [escapeAttributeValue](#escapeAttributeValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)  Deprecated.
Use [AuthorUtilAccess.escapeAttributeValue(String)](access/AuthorUtilAccess.md#escapeAttributeValue(java.lang.String)) instead.
   [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] [evaluateXPath](#evaluateXPath(java.lang.String,boolean,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments)  Deprecated.
Use [AuthorDocumentController.evaluateXPath(String, boolean, boolean, boolean)](AuthorDocumentController.md#evaluateXPath(java.lang.String,boolean,boolean,boolean)) instead.
   [AuthorNode](node/AuthorNode.md)[] [findNodesByXPath](#findNodesByXPath(java.lang.String,boolean,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments)  Deprecated.
Use [AuthorDocumentController.findNodesByXPath(String, boolean, boolean, boolean)](AuthorDocumentController.md#findNodesByXPath(java.lang.String,boolean,boolean,boolean)) instead.
   int [getCaretOffset](#getCaretOffset())()  Deprecated.
Use [WSTextBasedEditorPage.getCaretOffset()](../../../exml/workspace/api/editor/page/WSTextBasedEditorPage.md#getCaretOffset()) instead.
   [AuthorChangeTrackingController](AuthorChangeTrackingController.md) [getChangeTrackingController](#getChangeTrackingController())()  Deprecated.
Use [AuthorAccess.getReviewController()](AuthorAccess.md#getReviewController()) instead.
   [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getEditorLocation](#getEditorLocation())()  Deprecated.
Use [WSEditorBase.getEditorLocation()](../../../exml/workspace/api/editor/WSEditorBase.md#getEditorLocation()) instead.
   [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getParentFrame](#getParentFrame())()  Deprecated.
Use [WorkspaceUtilities.getParentFrame()](../../../exml/workspace/api/WorkspaceUtilities.md#getParentFrame()) instead.
   [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSelectedText](#getSelectedText())()  Deprecated.
Use [WSAuthorEditorPageBase.getSelectedText()](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getSelectedText()) instead.
   int [getSelectionEnd](#getSelectionEnd())()  Deprecated.
Use [WSAuthorEditorPageBase.getSelectionEnd()](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getSelectionEnd()) instead.
   int [getSelectionStart](#getSelectionStart())()  Deprecated.
Use [WSAuthorEditorPageBase.getSelectionStart()](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getSelectionStart()) instead.
   [AuthorElement](node/AuthorElement.md) [getTableCellAbove](#getTableCellAbove(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) cellElement)  Deprecated.
Use [AuthorTableAccess.getTableCellAbove(AuthorElement)](access/AuthorTableAccess.md#getTableCellAbove(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
   [AuthorElement](node/AuthorElement.md) [getTableCellAt](#getTableCellAt(int,int,ro.sync.ecss.extensions.api.node.AuthorElement))(int row, int column, [AuthorElement](node/AuthorElement.md) tableElement)  Deprecated.
Use [AuthorTableAccess.getTableCellAt(int, int, AuthorElement)](access/AuthorTableAccess.md#getTableCellAt(int,int,ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
   [AuthorElement](node/AuthorElement.md) [getTableCellBelow](#getTableCellBelow(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) cellElement)  Deprecated.
Use [AuthorTableAccess.getTableCellBelow(AuthorElement)](access/AuthorTableAccess.md#getTableCellBelow(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
   int[] [getTableCellIndex](#getTableCellIndex(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) authorElement)  Deprecated.
Use [AuthorTableAccess.getTableCellIndex(AuthorElement)](access/AuthorTableAccess.md#getTableCellIndex(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
   int[] [getTableColSpanIndices](#getTableColSpanIndices(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) cellElement)  Deprecated.
Use [AuthorTableAccess.getTableColSpanIndices(AuthorElement)](access/AuthorTableAccess.md#getTableColSpanIndices(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
   int [getTableNumberOfColumns](#getTableNumberOfColumns(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) tableElement)  Deprecated.
Use [AuthorTableAccess.getTableNumberOfColumns(AuthorElement)](access/AuthorTableAccess.md#getTableNumberOfColumns(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
   [AuthorElement](node/AuthorElement.md) [getTableRow](#getTableRow(int,ro.sync.ecss.extensions.api.node.AuthorElement))(int index, [AuthorElement](node/AuthorElement.md) tableElement)  Deprecated.
Use [AuthorTableAccess.getTableRow(int, AuthorElement)](access/AuthorTableAccess.md#getTableRow(int,ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
   int [getTableRowCount](#getTableRowCount(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) tableElement)  Deprecated.
Use [AuthorTableAccess.getTableRowCount(AuthorElement)](access/AuthorTableAccess.md#getTableRowCount(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
   int[] [getWordAtCaret](#getWordAtCaret())()  Deprecated.
Use [WSTextBasedEditorPage.getWordAtCaret()](../../../exml/workspace/api/editor/page/WSTextBasedEditorPage.md#getWordAtCaret()) instead.
   boolean [hasSelection](#hasSelection())()  Deprecated.
Use [WSAuthorEditorPageBase.hasSelection()](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#hasSelection()) instead.
   boolean [inInlineContext](#inInlineContext(int))(int offset)  Deprecated.
Use [AuthorDocumentController.inInlineContext(int)](AuthorDocumentController.md#inInlineContext(int)) instead.
   void [insertMultipleElements](#insertMultipleElements(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,int%5B%5D,java.lang.String))([AuthorElement](node/AuthorElement.md) parentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementNames, int[] offsets, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)  Deprecated.
Use [AuthorDocumentController.insertMultipleElements(AuthorElement, String[], int[], String)](AuthorDocumentController.md#insertMultipleElements(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,int%5B%5D,java.lang.String)) instead.
   void [insertText](#insertText(java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, int offset)  Deprecated.
Use [AuthorDocumentController.insertText(int, String)](AuthorDocumentController.md#insertText(int,java.lang.String)) instead.
   void [insertXMLFragment](#insertXMLFragment(java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int offset)  Deprecated.
Use [AuthorDocumentController.insertXMLFragment(String, int)](AuthorDocumentController.md#insertXMLFragment(java.lang.String,int)) instead.
   void [insertXMLFragment](#insertXMLFragment(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)  Deprecated.
Use [AuthorDocumentController.insertXMLFragment(String, String, String)](AuthorDocumentController.md#insertXMLFragment(java.lang.String,java.lang.String,java.lang.String)) instead.
   boolean [isStandalone](#isStandalone())()  Deprecated.
Use [Workspace.isStandalone()](../../../exml/workspace/api/Workspace.md#isStandalone()) instead.
   boolean [isTrackingChanges](#isTrackingChanges())()  Deprecated.
Use [ChangeTrackingController.isTrackingChanges()](ChangeTrackingController.md#isTrackingChanges()) instead.
   [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [locateFile](#locateFile(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)  Deprecated.
Use [UtilAccess.locateFile(URL)](../../../exml/workspace/api/util/UtilAccess.md#locateFile(java.net.URL)) instead.
   [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [makeRelative](#makeRelative(java.net.URL,java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) childURL)  Deprecated.
Use [UtilAccess.makeRelative(URL, URL)](../../../exml/workspace/api/util/UtilAccess.md#makeRelative(java.net.URL,java.net.URL)) instead.
   void [multipleDelete](#multipleDelete(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D,int%5B%5D))([AuthorElement](node/AuthorElement.md) parentElement, int[] startOffsets, int[] endOffsets)  Deprecated.
Use [AuthorDocumentController.multipleDelete(AuthorElement, int[], int[])](AuthorDocumentController.md#multipleDelete(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D,int%5B%5D)) instead.
   [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newNonValidatingXMLReader](#newNonValidatingXMLReader())()  Deprecated.
Use [AuthorUtilAccess.newNonValidatingXMLReader()](access/AuthorUtilAccess.md#newNonValidatingXMLReader()) instead.
   void [removeAuthorListener](#removeAuthorListener(ro.sync.ecss.extensions.api.AuthorListener))([AuthorListener](AuthorListener.md) listener)  Deprecated.
Use [AuthorDocumentController.removeAuthorListener(AuthorListener)](AuthorDocumentController.md#removeAuthorListener(ro.sync.ecss.extensions.api.AuthorListener)) intead.
   void [removeClonedElementAttribute](#removeClonedElementAttribute(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String))([AuthorElement](node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName)  Deprecated.
Use [AuthorElement.removeAttribute(String)](node/AuthorElement.md#removeAttribute(java.lang.String)) instead.
   [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolvePath](#resolvePath(java.net.URL,java.lang.String,boolean,boolean))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativeLocation, boolean entityResolve, boolean uriResolve)  Deprecated.
Use [AuthorUtilAccess.resolvePath(URL, String, boolean, boolean)](access/AuthorUtilAccess.md#resolvePath(java.net.URL,java.lang.String,boolean,boolean)) instead.
   void [select](#select(int,int))(int startOffset, int endOffset)  Deprecated.
Use [WSAuthorEditorPageBase.select(int, int)](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#select(int,int)) instead.
   void [selectWord](#selectWord())()  Deprecated.
Use [WSTextBasedEditorPage.selectWord()](../../../exml/workspace/api/editor/page/WSTextBasedEditorPage.md#selectWord()) instead.
   void [setCaretPosition](#setCaretPosition(int))(int offset)  Deprecated.
Use [WSTextBasedEditorPage.setCaretPosition(int)](../../../exml/workspace/api/editor/page/WSTextBasedEditorPage.md#setCaretPosition(int)) instead.
   void [setClonedElementAttribute](#setClonedElementAttribute(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue))([AuthorElement](node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [AttrValue](node/AttrValue.md) attributeValue)  Deprecated.
Use [AuthorElement.setAttribute(String, AttrValue)](node/AuthorElement.md#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue)) instead.
   int [showConfirmDialog](#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] buttonNames, int[] buttonIds)  Deprecated.
Use [WorkspaceUtilities.showConfirmDialog(String, String, String[], int[])](../../../exml/workspace/api/WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)) instead.
   void [showErrorMessage](#showErrorMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)  Deprecated.
Use [WorkspaceUtilities.showErrorMessage(String)](../../../exml/workspace/api/WorkspaceUtilities.md#showErrorMessage(java.lang.String)) instead.
   void [surroundInFragment](#surroundInFragment(java.lang.String,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int startOffset, int endOffset)  Deprecated.
Use [AuthorDocumentController.surroundInFragment(String, int, int)](AuthorDocumentController.md#surroundInFragment(java.lang.String,int,int)) instead.
   void [surroundInText](#surroundInText(java.lang.String,java.lang.String,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) header, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) footer, int startOffset, int endOffset)  Deprecated.
Use [AuthorDocumentController.surroundInText(String, String, int, int)](AuthorDocumentController.md#surroundInText(java.lang.String,java.lang.String,int,int)) instead.
   void [toggleTrackChanges](#toggleTrackChanges())()  Deprecated.
Use [ChangeTrackingController.toggleTrackChanges()](ChangeTrackingController.md#toggleTrackChanges()) instead.
   [AuthorViewToModelInfo](AuthorViewToModelInfo.md) [viewToModel](#viewToModel(int,int))(int x, int y)  Deprecated.
Use [WSAuthorEditorPageBase.viewToModel(int, int)](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#viewToModel(int,int)) instead.

## Method Details

### getSelectionStart

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) int getSelectionStart()
 Deprecated.
Use [WSAuthorEditorPageBase.getSelectionStart()](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getSelectionStart()) instead.

Get the offset of the selection start. It is inclusive.
  Returns: The offset of the selection start, 0 based.
### getSelectionEnd

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) int getSelectionEnd()
 Deprecated.
Use [WSAuthorEditorPageBase.getSelectionEnd()](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getSelectionEnd()) instead.

Get the offset of the selection end. It is exclusive.
  Returns: The offset of the selection end, zero based.
### getSelectedText

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSelectedText()
 Deprecated.
Use [WSAuthorEditorPageBase.getSelectedText()](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getSelectedText()) instead.

Get the selected text. The text does not contains XML tags.
  Returns: The selected text or the empty string if no selection is present.
### getCaretOffset

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) int getCaretOffset()
 Deprecated.
Use [WSTextBasedEditorPage.getCaretOffset()](../../../exml/workspace/api/editor/page/WSTextBasedEditorPage.md#getCaretOffset()) instead. For example if you have an AuthorAccess object then use authorAccess.getEditorAccess().getCaretOffset().

The current caret offset.
  Returns: The caret offset, 0 based.
### insertText

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void insertText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, int offset)
 Deprecated.
Use [AuthorDocumentController.insertText(int, String)](AuthorDocumentController.md#insertText(int,java.lang.String)) instead.

Inserts a text at the offset. After the operation is performed the caret will be positioned at the end of the inserted text.
  Parameters: text - The text to insert. offset - The offset of the insertion point, 0 based.
### insertXMLFragment

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void insertXMLFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int offset)throws [AuthorOperationException](AuthorOperationException.md)
 Deprecated.
Use [AuthorDocumentController.insertXMLFragment(String, int)](AuthorDocumentController.md#insertXMLFragment(java.lang.String,int)) instead.

Insert an XML fragment at the given offset. After the operation is performed the caret will be positioned at the end of the inserted XML fragment.
  Parameters: xmlFragment - The XML fragment. offset - The offset of the insertion point, 0 based. Throws: [AuthorOperationException](AuthorOperationException.md) - If it could not be inserted.
### insertXMLFragment

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void insertXMLFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)throws [AuthorOperationException](AuthorOperationException.md)
 Deprecated.
Use [AuthorDocumentController.insertXMLFragment(String, String, String)](AuthorDocumentController.md#insertXMLFragment(java.lang.String,java.lang.String,java.lang.String)) instead.

Insert an XML fragment at the node specified by the xpathLocation and relativePosition. Note: if the xpathLocation is not specified then the XML fragment will be inserted at the caret position(relativePosition is ignored). After the operation is performed the caret will be positioned at the end of the inserted XML fragment.
  Parameters: xmlFragment - The XML fragment. xpathLocation - The xpath location. relativePosition - The position relative to the node identified by the xpath location. Can be one of the constants: AuthorConstants.POSITION_BEFORE, AuthorConstants.POSITION_AFTER, AuthorConstants.POSITION_INSIDE. Throws: [AuthorOperationException](AuthorOperationException.md) - If it could not be inserted.
### deleteSelection

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void deleteSelection()
 Deprecated.
Use [WSAuthorEditorPageBase.deleteSelection()](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#deleteSelection()) instead.

Delete the selected text, if any.

### hasSelection

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) boolean hasSelection()
 Deprecated.
Use [WSAuthorEditorPageBase.hasSelection()](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#hasSelection()) instead.
   Returns: true If there is a selection, false otherwise.
### selectWord

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void selectWord()
 Deprecated.
Use [WSTextBasedEditorPage.selectWord()](../../../exml/workspace/api/editor/page/WSTextBasedEditorPage.md#selectWord()) instead.

Select the word at caret.

### surroundInFragment

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void surroundInFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int startOffset, int endOffset)throws [AuthorOperationException](AuthorOperationException.md)
 Deprecated.
Use [AuthorDocumentController.surroundInFragment(String, int, int)](AuthorDocumentController.md#surroundInFragment(java.lang.String,int,int)) instead.

Surround the given offsets in xmlFragment. If endOffset < startOffset the xmlFragment will be inserted at startOffset.
  Parameters: xmlFragment - The XML fragment which will surround the given offsets. The first XML fragment leaf(deepest on the first branch) will be the surround point. startOffset - The start offset of the fragment to be surrounded, 0 based and inclusive. endOffset - The end offset of the fragment to be surrounded, 0 based and inclusive. Throws: [AuthorOperationException](AuthorOperationException.md) - If the fragment between the offsets could not be surrounded.
### surroundInText

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void surroundInText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) header, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) footer, int startOffset, int endOffset)
 Deprecated.
Use [AuthorDocumentController.surroundInText(String, String, int, int)](AuthorDocumentController.md#surroundInText(java.lang.String,java.lang.String,int,int)) instead.

Surround the given offsets in plain text(without XML parsing) by inserting the header at the start offset and the footer at the endOffset.
  Parameters: header - The header to be inserted before the surrounded text. footer - The footer to be inserted after the surrounded text. startOffset - The start offset of the text to be surrounded, 0 based. endOffset - The end offset of the text to be surrounded, zero based.
### setCaretPosition

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void setCaretPosition(int offset)
 Deprecated.
Use [WSTextBasedEditorPage.setCaretPosition(int)](../../../exml/workspace/api/editor/page/WSTextBasedEditorPage.md#setCaretPosition(int)) instead.

Move the caret to the specified offset.
  Parameters: offset - The offset where the caret should be positioned, 0 based.
### select

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void select(int startOffset, int endOffset)
 Deprecated.
Use [WSAuthorEditorPageBase.select(int, int)](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#select(int,int)) instead.

Select the interval between start and end offset.
  Parameters: startOffset - Inclusive start offset endOffset - Exclusive end offset
### getWordAtCaret

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) int[] getWordAtCaret()
 Deprecated.
Use [WSTextBasedEditorPage.getWordAtCaret()](../../../exml/workspace/api/editor/page/WSTextBasedEditorPage.md#getWordAtCaret()) instead.

Compute the offsets of the word that contains the caret position.
  Returns: An array with the start and end offsets of the word at caret. null if the offsets couldn't be obtained.
### getParentFrame

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getParentFrame()
 Deprecated.
Use [WorkspaceUtilities.getParentFrame()](../../../exml/workspace/api/WorkspaceUtilities.md#getParentFrame()) instead.

Returns the parent frame.
  Returns: The parent frame ([or @link java.awt.Frame (when running as a JApplet)](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JFrame.html)) of the Oxygen application or the parent shell(Shell) if this is the Eclipse implementation.
### makeRelative

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) makeRelative([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) childURL)
 Deprecated.
Use [UtilAccess.makeRelative(URL, URL)](../../../exml/workspace/api/util/UtilAccess.md#makeRelative(java.net.URL,java.net.URL)) instead.

Make the child path relative to the parent.
The child path is relatively expressed to the base file. If is not possible, the child URL is returned.

Ex: Base: "file://c:/projects/exml/base.prx", Child "file://c:/projects/exml/test/someTest.xml"

Result: "test/someTest.xml"

  Parameters: baseURL - The base URL. childURL - The child URL. Returns: The relative path or the childURL if a relative path cannot be computed.
### escapeAttributeValue

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) escapeAttributeValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)
 Deprecated.
Use [AuthorUtilAccess.escapeAttributeValue(String)](access/AuthorUtilAccess.md#escapeAttributeValue(java.lang.String)) instead.

Escape an attribute value so that the XML remains wellformed.
  Parameters: attributeValue - The attribute value. Returns: The escaped value.
### getEditorLocation

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getEditorLocation()
 Deprecated.
Use [WSEditorBase.getEditorLocation()](../../../exml/workspace/api/editor/WSEditorBase.md#getEditorLocation()) instead.

Get the editor location.
  Returns: The editor location.
### locateFile

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) locateFile([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
 Deprecated.
Use [UtilAccess.locateFile(URL)](../../../exml/workspace/api/util/UtilAccess.md#locateFile(java.net.URL)) instead.

Locate the file on disk corresponding to the URL.
  Parameters: url - The URL to be checked. Returns: The corresponding file or null if URL is remote.
### chooseFile

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) chooseFile([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr, boolean openForSave)
 Deprecated.
Use [WorkspaceUtilities.chooseFile(String, String[], String, boolean)](../../../exml/workspace/api/WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)) instead.

Choose a file.
  Parameters: title - The file chooser title. allowedExtensions - Allowed file extensions. filterDescr - Description for this file filter. openForSave - True to show the file chooser for saving, false to use it for opening Returns: The chosen file or null if user canceled the dialog...
### chooseFile

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) chooseFile([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr)
 Deprecated.
Use [WorkspaceUtilities.chooseURL(String, String[], String)](../../../exml/workspace/api/WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String)) instead.

Choose a file.
  Parameters: title - The file chooser title. allowedExtensions - Allowed file extensions. filterDescr - Description for this file filter. Returns: The chosen file or null if user canceled the dialog...
### chooseURL

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) chooseURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr)
 Deprecated.
Use [WorkspaceUtilities.chooseURL(String, String[], String)](../../../exml/workspace/api/WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String)) instead.

Choose an url.
  Parameters: title - The file chooser title. allowedExtensions - Allowed extensions. filterDescr - Description for this file filter. Returns: The chosen url or null if user canceled the dialog...
### getTableCellAbove

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [AuthorElement](node/AuthorElement.md) getTableCellAbove([AuthorElement](node/AuthorElement.md) cellElement)
 Deprecated.
Use [AuthorTableAccess.getTableCellAbove(AuthorElement)](access/AuthorTableAccess.md#getTableCellAbove(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.

Find the cell included into the previous row that has the same column index.
  Parameters: cellElement - The table cell element. Returns: The cell above. Can be null.
### getTableCellBelow

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [AuthorElement](node/AuthorElement.md) getTableCellBelow([AuthorElement](node/AuthorElement.md) cellElement)
 Deprecated.
Use [AuthorTableAccess.getTableCellBelow(AuthorElement)](access/AuthorTableAccess.md#getTableCellBelow(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.

Find the cell included into the next row that has the same column index.
  Parameters: cellElement - The table cell element. Returns: The cell bellow. Can be null.
### getTableCellIndex

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) int[] getTableCellIndex([AuthorElement](node/AuthorElement.md) authorElement)
 Deprecated.
Use [AuthorTableAccess.getTableCellIndex(AuthorElement)](access/AuthorTableAccess.md#getTableCellIndex(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.

Obtain the table row and column index for the given element.
  Parameters: authorElement - The element. Returns: an array with row index on the first position and column index on the second one. 0 based. Can be null.
### getTableCellAt

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [AuthorElement](node/AuthorElement.md) getTableCellAt(int row, int column, [AuthorElement](node/AuthorElement.md) tableElement)
 Deprecated.
Use [AuthorTableAccess.getTableCellAt(int, int, AuthorElement)](access/AuthorTableAccess.md#getTableCellAt(int,int,ro.sync.ecss.extensions.api.node.AuthorElement)) instead.

Obtain the element at the given row and column in the table.
  Parameters: row - The row, 0 based. column - The column, 0 based. tableElement - The table element. Returns: The element at the specified location. Can be null if it could not be found.
### getTableRow

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [AuthorElement](node/AuthorElement.md) getTableRow(int index, [AuthorElement](node/AuthorElement.md) tableElement)
 Deprecated.
Use [AuthorTableAccess.getTableRow(int, AuthorElement)](access/AuthorTableAccess.md#getTableRow(int,ro.sync.ecss.extensions.api.node.AuthorElement)) instead.

Find the table row element for the given index.
  Parameters: index - The index of the row to find, 0 based. tableElement - The table element. Returns: The table row. Can be null.
### getTableRowCount

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) int getTableRowCount([AuthorElement](node/AuthorElement.md) tableElement)
 Deprecated.
Use [AuthorTableAccess.getTableRowCount(AuthorElement)](access/AuthorTableAccess.md#getTableRowCount(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.

Get the row count for the table.
  Parameters: tableElement - The table element. Returns: The row count.
### getTableNumberOfColumns

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) int getTableNumberOfColumns([AuthorElement](node/AuthorElement.md) tableElement)
 Deprecated.
Use [AuthorTableAccess.getTableNumberOfColumns(AuthorElement)](access/AuthorTableAccess.md#getTableNumberOfColumns(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.

Returns the number of columns for the given table element.
  Parameters: tableElement - The table element. Returns: The number of columns.
### getTableColSpanIndices

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) int[] getTableColSpanIndices([AuthorElement](node/AuthorElement.md) cellElement)
 Deprecated.
Use [AuthorTableAccess.getTableColSpanIndices(AuthorElement)](access/AuthorTableAccess.md#getTableColSpanIndices(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.

For the given cell find the start column and the end column defining the column span. The indices are 0 based.
  Parameters: cellElement - The table cell element. Returns: The column span indices. Can be null.
### isStandalone

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) boolean isStandalone()
 Deprecated.
Use [Workspace.isStandalone()](../../../exml/workspace/api/Workspace.md#isStandalone()) instead.

Returns information about the Oxygen underlying implementation.
  Returns: true if this is the standalone Oxygen version, false if this is the Oxygen Eclipse plugin version.
### inInlineContext

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) boolean inInlineContext(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
 Deprecated.
Use [AuthorDocumentController.inInlineContext(int)](AuthorDocumentController.md#inInlineContext(int)) instead.

Test if the context at the given offset is inline or not. For example a text paragraph determines an inline context, and for an offset inside this paragraph the method will return true. For an offset between two paragraphs(block boxes) the method will returns false.
  Parameters: offset - The offset in the document, zero based. Returns: Returns true if the given offset is inside an inline context. false otherwise. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offset does not exists in document model.
### insertMultipleElements

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void insertMultipleElements([AuthorElement](node/AuthorElement.md) parentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementNames, int[] offsets, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
 Deprecated.
Use [AuthorDocumentController.insertMultipleElements(AuthorElement, String[], int[], String)](AuthorDocumentController.md#insertMultipleElements(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,int%5B%5D,java.lang.String)) instead.

Insert multiple empty elements at the given offsets. The offsets and elements must be in the document order.
  Parameters: parentElement - The element that will be the parent of the inserted elements. elementNames - The element names to be inserted. offsets - The absolute offsets where the elements will be inserted. namespace - The namespace of the new inserted elements. null for default namespace.
### multipleDelete

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void multipleDelete([AuthorElement](node/AuthorElement.md) parentElement, int[] startOffsets, int[] endOffsets)
 Deprecated.
Use [AuthorDocumentController.multipleDelete(AuthorElement, int[], int[])](AuthorDocumentController.md#multipleDelete(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D,int%5B%5D)) instead.

Deletes the given intervals. The offsets must be in document order and the intervals must not intersect with one another.
  Parameters: parentElement - The element that contains all the deleted intervals. startOffsets - The start offset for each interval. Must be in document order. endOffsets - The end offset for each interval. Must be in document order.
### removeClonedElementAttribute

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void removeClonedElementAttribute([AuthorElement](node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName)
 Deprecated.
Use [AuthorElement.removeAttribute(String)](node/AuthorElement.md#removeAttribute(java.lang.String)) instead.

Remove the attribute from a cloned element. Warning: Use this only when the element is not from the existing content. All operations on nodes from the document model must be done through the AuthorDocumentController.
  Parameters: element - Element node. attrName - The attribute name to remove.
### setClonedElementAttribute

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void setClonedElementAttribute([AuthorElement](node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [AttrValue](node/AttrValue.md) attributeValue)
 Deprecated.
Use [AuthorElement.setAttribute(String, AttrValue)](node/AuthorElement.md#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue)) instead.

Set the attribute value for a cloned element. Warning: Use this only when the element is not from the existing content. All operations on nodes from the document model must be done through the AuthorDocumentController.
  Parameters: element - Element node. name - Name of the attribute to be set. attributeValue - The attribute value to set. Must not be null.
### showConfirmDialog

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) int showConfirmDialog([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] buttonNames, int[] buttonIds)
 Deprecated.
Use [WorkspaceUtilities.showConfirmDialog(String, String, String[], int[])](../../../exml/workspace/api/WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)) instead.

Shows a question message.
  Parameters: title - The dialog title. message - The message to be presented to the user. buttonNames - The names of the buttons representing the choices. buttonIds - The id for each button. Used to identify which button was pressed. All ids must be greater or equal to 0. Returns: the id of the pressed button or -1 if the dialog was closed by other means.
### newNonValidatingXMLReader

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newNonValidatingXMLReader()
 Deprecated.
Use [AuthorUtilAccess.newNonValidatingXMLReader()](access/AuthorUtilAccess.md#newNonValidatingXMLReader()) instead.

Creates an XML Reader without validation.
  Returns: A new XML Reader.
### correctURL

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) correctURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)
 Deprecated.
Use [UtilAccess.correctURL(String)](../../../exml/workspace/api/util/UtilAccess.md#correctURL(java.lang.String)) instead.

Corrects the given URL.
  Parameters: url - The URL to be corrected. Returns: The corrected URL.
### showErrorMessage

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void showErrorMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)
 Deprecated.
Use [WorkspaceUtilities.showErrorMessage(String)](../../../exml/workspace/api/WorkspaceUtilities.md#showErrorMessage(java.lang.String)) instead.

Presents the error message.
  Parameters: message - The error message to be presented.
### resolvePath

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolvePath([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativeLocation, boolean entityResolve, boolean uriResolve)
 Deprecated.
Use [AuthorUtilAccess.resolvePath(URL, String, boolean, boolean)](access/AuthorUtilAccess.md#resolvePath(java.net.URL,java.lang.String,boolean,boolean)) instead.

Try to resolve a relative href to an absolute path by passing through catalog.
  Parameters: baseURL - The URL of the current opened XML file. relativeLocation - The relative href. entityResolve - True to pass through catalog entity resolver uriResolve - True to pass through catalog URI resolver. Returns: The absolute URL.
### findNodesByXPath

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [AuthorNode](node/AuthorNode.md)[] findNodesByXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments)throws [AuthorOperationException](AuthorOperationException.md)
 Deprecated.
Use [AuthorDocumentController.findNodesByXPath(String, boolean, boolean, boolean)](AuthorDocumentController.md#findNodesByXPath(java.lang.String,boolean,boolean,boolean)) instead.

Finds the author nodes selected by the given XPath expression. The result of this function is an array of AuthorNode's selected by the given XPath expression. Author text nodes, Author CDATA section nodes and Author comment nodes can be ignored for performance reasons. For example executing the expression:  //node() will return an array with all the AuthorNode's in the document. But the result of calling the function with the expression:  count(//node()) will return an empty array.
  Parameters: xpathExpression - The XPath expression. ignoreTexts - If true Author text nodes will not be returned. ignoreCData - If true Author CDATA sections will not be returned. ignoreComments - If true Author comments will not be returned. Returns: The Author nodes selected by the XPath expression. Throws: [AuthorOperationException](AuthorOperationException.md) - If the XPath expression failed to be evaluated.
### evaluateXPath

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] evaluateXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments)throws [AuthorOperationException](AuthorOperationException.md)
 Deprecated.
Use [AuthorDocumentController.evaluateXPath(String, boolean, boolean, boolean)](AuthorDocumentController.md#evaluateXPath(java.lang.String,boolean,boolean,boolean)) instead.

Evaluates an XPath expression. This functions returns the result of the given XPath expression as an array of Object's. Author DOM text nodes, DOM CDATA sections and DOM comments wrappers can be ignored for performance reasons. For example, executing the expression:  //node() will return an array with all the Author DOM Node wrappers in the document. while evaluating the expression:  count(//node()) will return an array having a single component representing the number of nodes in the document. Evaluating the expression:  //node(), count(//node()) will return an array containing all the Author DOM Node wrappers in the document and having as last component the total number of nodes.
  Parameters: xpathExpression - The XPath expression. ignoreTexts - If true DOM text nodes will not be returned. ignoreCData - If true DOM CDATA sections will not be returned. ignoreComments - If true DOM comments will not be returned. Returns: An array of objects representing the XPath result. Throws: [AuthorOperationException](AuthorOperationException.md) - If the XPath expression failed to be evaluated.
### addAuthorListener

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void addAuthorListener([AuthorListener](AuthorListener.md) listener)
 Deprecated.
Use [AuthorDocumentController.addAuthorListener(AuthorListener)](AuthorDocumentController.md#addAuthorListener(ro.sync.ecss.extensions.api.AuthorListener)) intead.

Add an Author listener to be notified about changes regarding document and document structure.
  Parameters: listener - The listener to be added.
### removeAuthorListener

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void removeAuthorListener([AuthorListener](AuthorListener.md) listener)
 Deprecated.
Use [AuthorDocumentController.removeAuthorListener(AuthorListener)](AuthorDocumentController.md#removeAuthorListener(ro.sync.ecss.extensions.api.AuthorListener)) intead.

Remove an Author listener.
  Parameters: listener - The listener to be removed.
### viewToModel

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [AuthorViewToModelInfo](AuthorViewToModelInfo.md) viewToModel(int x, int y)
 Deprecated.
Use [WSAuthorEditorPageBase.viewToModel(int, int)](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#viewToModel(int,int)) instead.

Get the position in the document corresponding to the point in the viewport.
  Parameters: x - The "x" coordinate relative to the viewport origin. y - The "y" coordinate relative to the viewport origin. Returns: The information about the view-at-position.
### isTrackingChanges

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) boolean isTrackingChanges()
 Deprecated.
Use [ChangeTrackingController.isTrackingChanges()](ChangeTrackingController.md#isTrackingChanges()) instead.

Return true if the current editor is in change tracking mode
  Returns: true if the current editor is in change tracking mode
### toggleTrackChanges

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void toggleTrackChanges()
 Deprecated.
Use [ChangeTrackingController.toggleTrackChanges()](ChangeTrackingController.md#toggleTrackChanges()) instead.

Toggle the track changes mode.

### getChangeTrackingController

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [AuthorChangeTrackingController](AuthorChangeTrackingController.md) getChangeTrackingController()
 Deprecated.
Use [AuthorAccess.getReviewController()](AuthorAccess.md#getReviewController()) instead.

The change tracking controller used to toggle change tracking on and off and check its state.
  Returns: The change tracking controller. Cannot be null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
