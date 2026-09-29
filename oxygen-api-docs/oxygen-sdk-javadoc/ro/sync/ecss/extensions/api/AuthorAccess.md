Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorAccess
    All Superinterfaces: [AuthorAccessDeprecated](AuthorAccessDeprecated.md), [AuthorClipboardAccess](AuthorClipboardAccess.md), [AuthorConstants](AuthorConstants.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorAccessextends [AuthorConstants](AuthorConstants.md), [AuthorAccessDeprecated](AuthorAccessDeprecated.md), [AuthorClipboardAccess](AuthorClipboardAccess.md)
Access class to the author functions. Provides access to specific components corresponding to editor, document, workspace, tables, change tracking and utility informations and actions.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorConstants](AuthorConstants.md)
 [ARG_VALUE_FALSE](AuthorConstants.md#ARG_VALUE_FALSE), [ARG_VALUE_TRUE](AuthorConstants.md#ARG_VALUE_TRUE), [MOVE_DOWN](AuthorConstants.md#MOVE_DOWN), [MOVE_UP](AuthorConstants.md#MOVE_UP), [POSITION_AFTER](AuthorConstants.md#POSITION_AFTER), [POSITION_BEFORE](AuthorConstants.md#POSITION_BEFORE), [POSITION_INSIDE](AuthorConstants.md#POSITION_INSIDE), [POSITION_INSIDE_AT_THE_BEGINNING](AuthorConstants.md#POSITION_INSIDE_AT_THE_BEGINNING), [POSITION_INSIDE_AT_THE_END](AuthorConstants.md#POSITION_INSIDE_AT_THE_END), [POSITION_INSIDE_FIRST](AuthorConstants.md#POSITION_INSIDE_FIRST), [POSITION_INSIDE_LAST](AuthorConstants.md#POSITION_INSIDE_LAST), [SELECT_CONTENT](AuthorConstants.md#SELECT_CONTENT), [SELECT_ELEMENT](AuthorConstants.md#SELECT_ELEMENT), [SELECT_NONE](AuthorConstants.md#SELECT_NONE)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorResourceBundle](AuthorResourceBundle.md) [getAuthorResourceBundle](#getAuthorResourceBundle())()
A message bundle that holds all the internationalized messages displayed in Oxygen frameworks for a language set in Preferences.
  int [getCaretOffsetByAnchor](#getCaretOffsetByAnchor(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) anchor)
Get the caret offset identified by the given URL anchor.
  [ClassPathResourcesAccess](ClassPathResourcesAccess.md) [getClassPathResourcesAccess](#getClassPathResourcesAccess())()
Get access to the list of resources the user has added to the classpath of the corresponding framework.
  [AuthorDocumentController](AuthorDocumentController.md) [getDocumentController](#getDocumentController())()
Returns the Author document controller.
  [AuthorEditorAccess](access/AuthorEditorAccess.md) [getEditorAccess](#getEditorAccess())()
Get the author editor access providing editor related information.
  [AuthorElement](node/AuthorElement.md) [getElementByAnchor](#getElementByAnchor(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) anchor)
Get the author element identified by the given URL anchor.
  [OptionsStorage](OptionsStorage.md) [getOptionsStorage](#getOptionsStorage())()
The object that manages the options stored for author extensions.
  [AuthorOutlineAccess](access/AuthorOutlineAccess.md) [getOutlineAccess](#getOutlineAccess())()
Get the author Outline access providing Outline related information.
  [AuthorReviewController](AuthorReviewController.md) [getReviewController](#getReviewController())()
Controller that can be used to toggle the change tracking state, modify the review highlight author name, the highlight painting or to obtain information about the properties used in the serialization and representation of the review highlight (author name, reviewer auto color or the current time stamp in a format identical to the one used by Oxygen for insert, delete and comment markers).
  [AuthorTableAccess](access/AuthorTableAccess.md) [getTableAccess](#getTableAccess())()
Returns the author table access provider responsible for obtaining table related information and executing table actions.
  [AuthorUtilAccess](access/AuthorUtilAccess.md) [getUtilAccess](#getUtilAccess())()
Get the author access utility methods provider.
  [AuthorWorkspaceAccess](access/AuthorWorkspaceAccess.md) [getWorkspaceAccess](#getWorkspaceAccess())()
Get the workspace access.
  [AuthorXMLUtilAccess](access/AuthorXMLUtilAccess.md) [getXMLUtilAccess](#getXMLUtilAccess())()
Get the author access utility methods provider.

### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorAccessDeprecated](AuthorAccessDeprecated.md)
 [addAuthorListener](AuthorAccessDeprecated.md#addAuthorListener(ro.sync.ecss.extensions.api.AuthorListener)), [chooseFile](AuthorAccessDeprecated.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseFile](AuthorAccessDeprecated.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)), [chooseURL](AuthorAccessDeprecated.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [correctURL](AuthorAccessDeprecated.md#correctURL(java.lang.String)), [deleteSelection](AuthorAccessDeprecated.md#deleteSelection()), [escapeAttributeValue](AuthorAccessDeprecated.md#escapeAttributeValue(java.lang.String)), [evaluateXPath](AuthorAccessDeprecated.md#evaluateXPath(java.lang.String,boolean,boolean,boolean)), [findNodesByXPath](AuthorAccessDeprecated.md#findNodesByXPath(java.lang.String,boolean,boolean,boolean)), [getCaretOffset](AuthorAccessDeprecated.md#getCaretOffset()), [getChangeTrackingController](AuthorAccessDeprecated.md#getChangeTrackingController()), [getEditorLocation](AuthorAccessDeprecated.md#getEditorLocation()), [getParentFrame](AuthorAccessDeprecated.md#getParentFrame()), [getSelectedText](AuthorAccessDeprecated.md#getSelectedText()), [getSelectionEnd](AuthorAccessDeprecated.md#getSelectionEnd()), [getSelectionStart](AuthorAccessDeprecated.md#getSelectionStart()), [getTableCellAbove](AuthorAccessDeprecated.md#getTableCellAbove(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTableCellAt](AuthorAccessDeprecated.md#getTableCellAt(int,int,ro.sync.ecss.extensions.api.node.AuthorElement)), [getTableCellBelow](AuthorAccessDeprecated.md#getTableCellBelow(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTableCellIndex](AuthorAccessDeprecated.md#getTableCellIndex(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTableColSpanIndices](AuthorAccessDeprecated.md#getTableColSpanIndices(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTableNumberOfColumns](AuthorAccessDeprecated.md#getTableNumberOfColumns(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTableRow](AuthorAccessDeprecated.md#getTableRow(int,ro.sync.ecss.extensions.api.node.AuthorElement)), [getTableRowCount](AuthorAccessDeprecated.md#getTableRowCount(ro.sync.ecss.extensions.api.node.AuthorElement)), [getWordAtCaret](AuthorAccessDeprecated.md#getWordAtCaret()), [hasSelection](AuthorAccessDeprecated.md#hasSelection()), [inInlineContext](AuthorAccessDeprecated.md#inInlineContext(int)), [insertMultipleElements](AuthorAccessDeprecated.md#insertMultipleElements(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,int%5B%5D,java.lang.String)), [insertText](AuthorAccessDeprecated.md#insertText(java.lang.String,int)), [insertXMLFragment](AuthorAccessDeprecated.md#insertXMLFragment(java.lang.String,int)), [insertXMLFragment](AuthorAccessDeprecated.md#insertXMLFragment(java.lang.String,java.lang.String,java.lang.String)), [isStandalone](AuthorAccessDeprecated.md#isStandalone()), [isTrackingChanges](AuthorAccessDeprecated.md#isTrackingChanges()), [locateFile](AuthorAccessDeprecated.md#locateFile(java.net.URL)), [makeRelative](AuthorAccessDeprecated.md#makeRelative(java.net.URL,java.net.URL)), [multipleDelete](AuthorAccessDeprecated.md#multipleDelete(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D,int%5B%5D)), [newNonValidatingXMLReader](AuthorAccessDeprecated.md#newNonValidatingXMLReader()), [removeAuthorListener](AuthorAccessDeprecated.md#removeAuthorListener(ro.sync.ecss.extensions.api.AuthorListener)), [removeClonedElementAttribute](AuthorAccessDeprecated.md#removeClonedElementAttribute(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String)), [resolvePath](AuthorAccessDeprecated.md#resolvePath(java.net.URL,java.lang.String,boolean,boolean)), [select](AuthorAccessDeprecated.md#select(int,int)), [selectWord](AuthorAccessDeprecated.md#selectWord()), [setCaretPosition](AuthorAccessDeprecated.md#setCaretPosition(int)), [setClonedElementAttribute](AuthorAccessDeprecated.md#setClonedElementAttribute(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue)), [showConfirmDialog](AuthorAccessDeprecated.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)), [showErrorMessage](AuthorAccessDeprecated.md#showErrorMessage(java.lang.String)), [surroundInFragment](AuthorAccessDeprecated.md#surroundInFragment(java.lang.String,int,int)), [surroundInText](AuthorAccessDeprecated.md#surroundInText(java.lang.String,java.lang.String,int,int)), [toggleTrackChanges](AuthorAccessDeprecated.md#toggleTrackChanges()), [viewToModel](AuthorAccessDeprecated.md#viewToModel(int,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorClipboardAccess](AuthorClipboardAccess.md)
 [getAuthorObjectFromClipboard](AuthorClipboardAccess.md#getAuthorObjectFromClipboard()), [getTextFromClipboard](AuthorClipboardAccess.md#getTextFromClipboard())
## Method Details

### getEditorAccess

[AuthorEditorAccess](access/AuthorEditorAccess.md) getEditorAccess()

Get the author editor access providing editor related information.
  Returns: The editor related informations and actions provider. Cannot be null.
### getDocumentController

[AuthorDocumentController](AuthorDocumentController.md) getDocumentController()

Returns the Author document controller. It has methods for changing the document model.
  Returns: The controller for Author document. Cannot be null.
### getWorkspaceAccess

[AuthorWorkspaceAccess](access/AuthorWorkspaceAccess.md) getWorkspaceAccess()

Get the workspace access. Provides methods for obtaining workspace related informations and performing workspace specific actions.
  Returns: The workspace access provider. Cannot be null.
### getUtilAccess

[AuthorUtilAccess](access/AuthorUtilAccess.md) getUtilAccess()

Get the author access utility methods provider.
  Returns: The provider for utility methods. Cannot be null.
### getXMLUtilAccess

[AuthorXMLUtilAccess](access/AuthorXMLUtilAccess.md) getXMLUtilAccess()

Get the author access utility methods provider.
  Returns: The provider for XML utility methods. Cannot be null.
### getTableAccess

[AuthorTableAccess](access/AuthorTableAccess.md) getTableAccess()

Returns the author table access provider responsible for obtaining table related information and executing table actions.
  Returns: The table related information and actions provider. Cannot be null.
### getReviewController

[AuthorReviewController](AuthorReviewController.md) getReviewController()

Controller that can be used to toggle the change tracking state, modify the review highlight author name, the highlight painting or to obtain information about the properties used in the serialization and representation of the review highlight (author name, reviewer auto color or the current time stamp in a format identical to the one used by Oxygen for insert, delete and comment markers).
  Returns: The review controller. Cannot be null. Since: 12
### getOptionsStorage

[OptionsStorage](OptionsStorage.md) getOptionsStorage()

The object that manages the options stored for author extensions. This is also responsible for adding and removing listeners that are notified about the option changes.
  Returns: The object that manages the options stored for author extensions.
### getOutlineAccess

[AuthorOutlineAccess](access/AuthorOutlineAccess.md) getOutlineAccess()

Get the author Outline access providing Outline related information.
  Returns: The Outline related informations and actions provider. Cannot be null.
### getClassPathResourcesAccess

[ClassPathResourcesAccess](ClassPathResourcesAccess.md) getClassPathResourcesAccess()

Get access to the list of resources the user has added to the classpath of the corresponding framework.
  Returns: access to the list of resources the user has added to the classpath of the corresponding framework. Since: 12.1
### getAuthorResourceBundle

[AuthorResourceBundle](AuthorResourceBundle.md) getAuthorResourceBundle()

A message bundle that holds all the internationalized messages displayed in Oxygen frameworks for a language set in Preferences. It works as a map in which any message is accessed by a key defined in the [ExtensionTags](../commons/ExtensionTags.md) interface.
  Returns: The message bundle. Since: 14
### getElementByAnchor

[AuthorElement](node/AuthorElement.md) getElementByAnchor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) anchor)

Get the author element identified by the given URL anchor. The syntax of the anchor is interpreted by the [ElementLocatorProvider](link/ElementLocatorProvider.md) provided by the framework.
  Parameters: anchor - The anchor. Returns: The element identified by the anchor. Since: 18.0
### getCaretOffsetByAnchor

int getCaretOffsetByAnchor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) anchor)

Get the caret offset identified by the given URL anchor. The syntax of the anchor is interpreted by the [ElementLocatorProvider](link/ElementLocatorProvider.md) provided by the framework or: "short;locationInfo\0pathItems\0isWhitespaceBefore\0tokenPosition\0chCount\0anchorsOnChangeTrackingPI" example: "short;chrysanthemum/section_anp_qrw_p1b /section[1]/p[3]/b[1] false 0 16 false"
  Parameters: anchor - The anchor. Returns: The caret offset identified by the anchor. Since: 19.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
