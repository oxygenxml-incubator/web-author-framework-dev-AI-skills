# Deprecated API

## Contents

* [Interfaces](#interface)
* [Classes](#class)
* [Exceptions](#exception)
* [Fields](#field)
* [Methods](#method)
* [Constructors](#constructor)
* [Enum Constants](#enum-constant)

*   Deprecated Interfaces
Interface

Description
 [ro.sync.ecss.extensions.api.AttributesValueEditor](ro/sync/ecss/extensions/api/AttributesValueEditor.md)
Starting with version 15 the [CustomAttributeValueEditor](ro/sync/ecss/extensions/api/CustomAttributeValueEditor.md) can be used instead to edit only specific attributes using a custom editor.
  [ro.sync.ecss.extensions.api.webapp.SafeAuthorOperation](ro/sync/ecss/extensions/api/webapp/SafeAuthorOperation.md)
This interface is not used anymore as marker interface for operations that can be invoked via REST API with user supplied arguments. These AuthorOperations must be instead annotated with [WebappRestSafe](ro/sync/ecss/extensions/api/webapp/WebappRestSafe.md) annotation.
  [ro.sync.exml.plugin.urlstreamhandler.URLChooserPluginExtension](ro/sync/exml/plugin/urlstreamhandler/URLChooserPluginExtension.md)
This approach will continue to work but it is recommanded to use the **ro.sync.exml.plugin.urlstreamhandler.URLChooserPluginExtension2** interface which also receives access to the Oxygen workspace.

*   Deprecated Classes
Class

Description
 [ro.sync.ecss.extensions.api.webapp.plugin.PluginConfigExtension](ro/sync/ecss/extensions/api/webapp/plugin/PluginConfigExtension.md)
This API is deprecated because it's based on javax package that's no more supported starting with Servlet 5.0 specification and because this extension type isn't protected against CSRF attacks. Use [ServletPluginConfigExtension](ro/sync/ecss/extensions/api/webapp/plugin/ServletPluginConfigExtension.md) instead.
  [ro.sync.ecss.extensions.api.webapp.plugin.WebappServletPluginExtension](ro/sync/ecss/extensions/api/webapp/plugin/WebappServletPluginExtension.md)
This API is deprecated because it's based on javax package that's no more supported starting with Servlet 5.0 specification and because this extension type isn't protected against CSRF attacks. Use [ServletPluginExtension](ro/sync/ecss/extensions/api/webapp/plugin/ServletPluginExtension.md) instead.

*   Deprecated Exceptions
Exceptions

Description
 [ro.sync.ecss.extensions.commons.CannotEditException](ro/sync/ecss/extensions/commons/CannotEditException.md)

*   Deprecated Fields
Field

Description
 [ro.sync.ecss.css.Styles.KEY_LINK_URL](ro/sync/ecss/css/Styles.md#KEY_LINK_URL)
since 17
  [ro.sync.ecss.css.Styles.KEY_TEXT_DECORATION](ro/sync/ecss/css/Styles.md#KEY_TEXT_DECORATION)
It is a shorthand now, use [Styles.KEY_TEXT_DECORATION_LINE](ro/sync/ecss/css/Styles.md#KEY_TEXT_DECORATION_LINE), [Styles.KEY_TEXT_DECORATION_COLOR](ro/sync/ecss/css/Styles.md#KEY_TEXT_DECORATION_COLOR), [Styles.KEY_TEXT_DECORATION_STYLE](ro/sync/ecss/css/Styles.md#KEY_TEXT_DECORATION_STYLE) instead.
  [ro.sync.ecss.css.Styles.KEY_VISIBITY](ro/sync/ecss/css/Styles.md#KEY_VISIBITY)
This is a typo of the [Styles.KEY_VISIBILITY](ro/sync/ecss/css/Styles.md#KEY_VISIBILITY).
  [ro.sync.ecss.dita.DITAAccess.ID_ANY](ro/sync/ecss/dita/DITAAccess.md#ID_ANY)
Use [DITAAccess.ID_FIRST_TOPIC_ID](ro/sync/ecss/dita/DITAAccess.md#ID_FIRST_TOPIC_ID) instead which has a clearer meaning. Identifier used in references path, representing that the topic id can be excluded from the reference.
  [ro.sync.ecss.extensions.api.AuthorConstants.POSITION_INSIDE](ro/sync/ecss/extensions/api/AuthorConstants.md#POSITION_INSIDE)
Use the constant POSITION_INSIDE_FIRST instead.
  [ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_EDIT](ro/sync/ecss/extensions/api/editor/InplaceEditorCSSConstants.md#PROPERTY_EDIT)
Use [InplaceEditorArgumentKeys.PROPERTY_EDIT_QUALIFIED](ro/sync/ecss/extensions/api/editor/InplaceEditorArgumentKeys.md#PROPERTY_EDIT_QUALIFIED) instead. In case of an attribute it will offer a clark name instead of the QName used in the CSS.
  [ro.sync.exml.MainFrameComponentsConstants.CUSTOM](ro/sync/exml/MainFrameComponentsConstants.md#CUSTOM)
Since Oxygen 12.2 the preferred way is to define view IDs at plugin.xml level.
  [ro.sync.exml.MainFrameComponentsConstants.DATASOURCE_VIEW](ro/sync/exml/MainFrameComponentsConstants.md#DATASOURCE_VIEW)
Datasource (relational or native XML) View
  [ro.sync.exml.MainFrameComponentsConstants.DITA_MAPS](ro/sync/exml/MainFrameComponentsConstants.md#DITA_MAPS)
The DITA maps organizer. WARN: Adding a new View Frame also means changing the version in MainFrameLayoutManager.VIEWS_LAYOUT_VERSION.
  [ro.sync.exml.MainFrameComponentsConstants.HIERARCHY_DEPENDENCE](ro/sync/exml/MainFrameComponentsConstants.md#HIERARCHY_DEPENDENCE)
Resource dependencies or hierarchy view. WARN: Adding a new View Frame also means changing the version in MainFrameLayoutManager.VIEWS_LAYOUT_VERSION.
  [ro.sync.exml.MainFrameComponentsConstants.PREVIEW](ro/sync/exml/MainFrameComponentsConstants.md#PREVIEW)
Preview view. WARN: Adding a new View Frame also means changing the version in MainFrameLayoutManager.VIEWS_LAYOUT_VERSION.
  [ro.sync.exml.MainFrameComponentsConstants.TABLE_VIEW](ro/sync/exml/MainFrameComponentsConstants.md#TABLE_VIEW)
Database table (relational) View
  [ro.sync.exml.MainFrameComponentsConstants.TOOLBAR_CUSTOM](ro/sync/exml/MainFrameComponentsConstants.md#TOOLBAR_CUSTOM)
Since Oxygen 12.2 toolbar IDs are defined in the "plugin.xml".
  [ro.sync.exml.plugin.PluginDescriptor.URL_STREAM_HANDLER](ro/sync/exml/plugin/PluginDescriptor.md#URL_STREAM_HANDLER)

 [ro.sync.exml.workspace.api.standalone.ToolbarComponentsCustomizer.CUSTOM](ro/sync/exml/workspace/api/standalone/ToolbarComponentsCustomizer.md#CUSTOM)
Since Oxygen 12.2 toolbar IDs are defined in the "plugin.xml".
  [ro.sync.exml.workspace.api.standalone.ViewComponentCustomizer.CUSTOM](ro/sync/exml/workspace/api/standalone/ViewComponentCustomizer.md#CUSTOM)
since Oxygen 12.2. Please define a view id for the extension in the "plugin.xml".
  [ro.sync.exml.workspace.api.util.XMLUtilAccess.TRANSFORMER_SAXON_ENTERPRISE_EDITION](ro/sync/exml/workspace/api/util/XMLUtilAccess.md#TRANSFORMER_SAXON_ENTERPRISE_EDITION)
Since Oxygen 23 you can no longer create Saxon 9 PE transformers using this constant. The created transformer will be a Saxon HE transformer instead.
  [ro.sync.exml.workspace.api.util.XMLUtilAccess.TRANSFORMER_SAXON_PROFESSIONAL_EDITION](ro/sync/exml/workspace/api/util/XMLUtilAccess.md#TRANSFORMER_SAXON_PROFESSIONAL_EDITION)
Since Oxygen 23 you can no longer create Saxon 9 PE transformers using this constant. The created transformer will be a Saxon HE transformer instead.

*   Deprecated Methods
Method

Description
 [ro.sync.ecss.css.Styles.getTextDecoration()](ro/sync/ecss/css/Styles.md#getTextDecoration())
This was used to return only the text-decoration-line part from the text-decoration shorthand, as defined here https://drafts.csswg.org/css-text-decor-3/#text-decoration-property.
  [ro.sync.ecss.dita.DITAAccess.annotateAttributes(List<CIAttribute>)](ro/sync/ecss/dita/DITAAccess.md#annotateAttributes(java.util.List))
This method does not do anything anynmore, the attribute annotations are gathered from the framework folder.
  [ro.sync.ecss.dita.DITAAccess.attachKeyScopeInformation(URL, String, String)](ro/sync/ecss/dita/DITAAccess.md#attachKeyScopeInformation(java.net.URL,java.lang.String,java.lang.String))  [ro.sync.ecss.dita.DITAAccess.computeLinkText(String, String)](ro/sync/ecss/dita/DITAAccess.md#computeLinkText(java.lang.String,java.lang.String))
Use [DITAAccess.computeLinkText(AuthorNode, String, String, String, KeysManagerBase)](ro/sync/ecss/dita/DITAAccess.md#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.dita.KeysManagerBase)) instead.
  [ro.sync.ecss.dita.DITAAccess.computeLinkText(AuthorNode, String, String)](ro/sync/ecss/dita/DITAAccess.md#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String))
Use [DITAAccess.computeLinkText(AuthorNode, String, String, String, KeysManagerBase)](ro/sync/ecss/dita/DITAAccess.md#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.dita.KeysManagerBase)) instead.
  [ro.sync.ecss.dita.DITAAccess.computeLinkText(AuthorNode, String, String, String)](ro/sync/ecss/dita/DITAAccess.md#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String))
Use [DITAAccess.computeLinkText(AuthorNode, String, String, String, KeysManagerBase)](ro/sync/ecss/dita/DITAAccess.md#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.dita.KeysManagerBase)) instead.
  [ro.sync.ecss.dita.DITAAccess.filterAttributeValues(List<CIValue>, WhatPossibleValuesHasAttributeContext, String)](ro/sync/ecss/dita/DITAAccess.md#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext,java.lang.String))
Please use the equivalent method which also receives the URL of the requestor.
  [ro.sync.ecss.dita.DITAAccess.getFormat(String, String, boolean)](ro/sync/ecss/dita/DITAAccess.md#getFormat(java.lang.String,java.lang.String,boolean))
Use [DITAAccess.getFormatForLinkCreatedFromGUI(String, String, boolean)](ro/sync/ecss/dita/DITAAccess.md#getFormatForLinkCreatedFromGUI(java.lang.String,java.lang.String,boolean))
  [ro.sync.ecss.dita.DITAAccess.getKeys()](ro/sync/ecss/dita/DITAAccess.md#getKeys())
Please use the equivalent method which also receives the URL of the requestor.
  [ro.sync.ecss.dita.DITAAccess.getTopicRefInfo(URL, Object, AuthorCCManager, AuthorDocumentControllerImpl, int, TopicrefInfo, TopicRefInserter)](ro/sync/ecss/dita/DITAAccess.md#getTopicRefInfo(java.net.URL,java.lang.Object,ro.sync.ecss.contentcompletion.AuthorCCManager,ro.sync.ecss.ue.AuthorDocumentControllerImpl,int,ro.sync.ecss.dita.topic.ref.TopicrefInfo,ro.sync.ecss.dita.topic.ref.TopicRefInserter))
This method is not used anymore from oXygen to insert topic reference elements and it will be removed in a future release. All topic reference elements are inserted using the same method: [DITAAccess.editProperties(URL, AuthorCCManager, AuthorDocumentControllerImpl, AuthorElement[], TopicRefInserter, Object, boolean)](ro/sync/ecss/dita/DITAAccess.md#editProperties(java.net.URL,ro.sync.ecss.contentcompletion.AuthorCCManager,ro.sync.ecss.ue.AuthorDocumentControllerImpl,ro.sync.ecss.extensions.api.node.AuthorElement%5B%5D,ro.sync.ecss.dita.topic.ref.TopicRefInserter,java.lang.Object,boolean))
  [ro.sync.ecss.dita.DITAAccess.isGeneralizationOf(String, String)](ro/sync/ecss/dita/DITAAccess.md#isGeneralizationOf(java.lang.String,java.lang.String))
use getInheritanceType instead.
  [ro.sync.ecss.dita.DITAAccess.parseDITAKeyRef(String)](ro/sync/ecss/dita/DITAAccess.md#parseDITAKeyRef(java.lang.String))
Please use the equivalent method which also receives the URL of the requestor.
  [ro.sync.ecss.dita.DITAAccess.resolveKeyRef(String)](ro/sync/ecss/dita/DITAAccess.md#resolveKeyRef(java.lang.String))
Please use the equivalent method which also receives the URL of the requestor.
  [ro.sync.ecss.dita.DITAAccess.resolveKeyRef(String, boolean)](ro/sync/ecss/dita/DITAAccess.md#resolveKeyRef(java.lang.String,boolean))
Please use the equivalent method which also receives the URL of the requestor.
  [ro.sync.ecss.dita.DITATextAccess.getPreferredKeyRefElementName(WSXMLTextEditorPage, KeyInfo, boolean)](ro/sync/ecss/dita/DITATextAccess.md#getPreferredKeyRefElementName(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,ro.sync.ecss.dita.reference.keyref.KeyInfo,boolean))

 [ro.sync.ecss.extensions.api.access.AuthorEditorAccess.getLocationOnScreen(int, int)](ro/sync/ecss/extensions/api/access/AuthorEditorAccess.md#getLocationOnScreen(int,int))
Use the getLocationOnScreenAsPoint(int x, int y) method instead.
  [ro.sync.ecss.extensions.api.access.AuthorEditorAccess.modelToView(int)](ro/sync/ecss/extensions/api/access/AuthorEditorAccess.md#modelToView(int))
use modelToViewRectangle(int offset) instead
  [ro.sync.ecss.extensions.api.access.AuthorUtilAccess.escapeAttributeValue(String)](ro/sync/ecss/extensions/api/access/AuthorUtilAccess.md#escapeAttributeValue(java.lang.String))
Use the method from the AuthorXMLUtilAccess class.
  [ro.sync.ecss.extensions.api.access.AuthorUtilAccess.newNonValidatingXMLReader()](ro/sync/ecss/extensions/api/access/AuthorUtilAccess.md#newNonValidatingXMLReader())
Use the method from the AuthorXMLUtilAccess class.
  [ro.sync.ecss.extensions.api.access.AuthorUtilAccess.resetXMLCatalogs()](ro/sync/ecss/extensions/api/access/AuthorUtilAccess.md#resetXMLCatalogs())
Use the method from the AuthorXMLUtilAccess class.
  [ro.sync.ecss.extensions.api.access.AuthorUtilAccess.resolvePath(URL, String, boolean, boolean)](ro/sync/ecss/extensions/api/access/AuthorUtilAccess.md#resolvePath(java.net.URL,java.lang.String,boolean,boolean))
Use the method from the AuthorXMLUtilAccess class.
  [ro.sync.ecss.extensions.api.access.AuthorWorkspaceAccess.open(File)](ro/sync/ecss/extensions/api/access/AuthorWorkspaceAccess.md#open(java.io.File))
Use [Workspace.open(URL)](ro/sync/exml/workspace/api/Workspace.md#open(java.net.URL)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.addAuthorListener(AuthorListener)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#addAuthorListener(ro.sync.ecss.extensions.api.AuthorListener))
Use [AuthorDocumentController.addAuthorListener(AuthorListener)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#addAuthorListener(ro.sync.ecss.extensions.api.AuthorListener)) intead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.chooseFile(String, String[], String)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String))
Use [WorkspaceUtilities.chooseURL(String, String[], String)](ro/sync/exml/workspace/api/WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.chooseFile(String, String[], String, boolean)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean))
Use [WorkspaceUtilities.chooseFile(String, String[], String, boolean)](ro/sync/exml/workspace/api/WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.chooseURL(String, String[], String)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String))
Use [WorkspaceUtilities.chooseURL(String, String[], String)](ro/sync/exml/workspace/api/WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.correctURL(String)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#correctURL(java.lang.String))
Use [UtilAccess.correctURL(String)](ro/sync/exml/workspace/api/util/UtilAccess.md#correctURL(java.lang.String)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.deleteSelection()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#deleteSelection())
Use [WSAuthorEditorPageBase.deleteSelection()](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#deleteSelection()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.escapeAttributeValue(String)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#escapeAttributeValue(java.lang.String))
Use [AuthorUtilAccess.escapeAttributeValue(String)](ro/sync/ecss/extensions/api/access/AuthorUtilAccess.md#escapeAttributeValue(java.lang.String)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.evaluateXPath(String, boolean, boolean, boolean)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#evaluateXPath(java.lang.String,boolean,boolean,boolean))
Use [AuthorDocumentController.evaluateXPath(String, boolean, boolean, boolean)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#evaluateXPath(java.lang.String,boolean,boolean,boolean)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.findNodesByXPath(String, boolean, boolean, boolean)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#findNodesByXPath(java.lang.String,boolean,boolean,boolean))
Use [AuthorDocumentController.findNodesByXPath(String, boolean, boolean, boolean)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#findNodesByXPath(java.lang.String,boolean,boolean,boolean)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getCaretOffset()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getCaretOffset())
Use [WSTextBasedEditorPage.getCaretOffset()](ro/sync/exml/workspace/api/editor/page/WSTextBasedEditorPage.md#getCaretOffset()) instead. For example if you have an AuthorAccess object then use authorAccess.getEditorAccess().getCaretOffset().
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getChangeTrackingController()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getChangeTrackingController())
Use [AuthorAccess.getReviewController()](ro/sync/ecss/extensions/api/AuthorAccess.md#getReviewController()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getEditorLocation()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getEditorLocation())
Use [WSEditorBase.getEditorLocation()](ro/sync/exml/workspace/api/editor/WSEditorBase.md#getEditorLocation()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getParentFrame()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getParentFrame())
Use [WorkspaceUtilities.getParentFrame()](ro/sync/exml/workspace/api/WorkspaceUtilities.md#getParentFrame()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getSelectedText()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getSelectedText())
Use [WSAuthorEditorPageBase.getSelectedText()](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getSelectedText()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getSelectionEnd()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getSelectionEnd())
Use [WSAuthorEditorPageBase.getSelectionEnd()](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getSelectionEnd()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getSelectionStart()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getSelectionStart())
Use [WSAuthorEditorPageBase.getSelectionStart()](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getSelectionStart()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getTableCellAbove(AuthorElement)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getTableCellAbove(ro.sync.ecss.extensions.api.node.AuthorElement))
Use [AuthorTableAccess.getTableCellAbove(AuthorElement)](ro/sync/ecss/extensions/api/access/AuthorTableAccess.md#getTableCellAbove(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getTableCellAt(int, int, AuthorElement)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getTableCellAt(int,int,ro.sync.ecss.extensions.api.node.AuthorElement))
Use [AuthorTableAccess.getTableCellAt(int, int, AuthorElement)](ro/sync/ecss/extensions/api/access/AuthorTableAccess.md#getTableCellAt(int,int,ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getTableCellBelow(AuthorElement)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getTableCellBelow(ro.sync.ecss.extensions.api.node.AuthorElement))
Use [AuthorTableAccess.getTableCellBelow(AuthorElement)](ro/sync/ecss/extensions/api/access/AuthorTableAccess.md#getTableCellBelow(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getTableCellIndex(AuthorElement)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getTableCellIndex(ro.sync.ecss.extensions.api.node.AuthorElement))
Use [AuthorTableAccess.getTableCellIndex(AuthorElement)](ro/sync/ecss/extensions/api/access/AuthorTableAccess.md#getTableCellIndex(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getTableColSpanIndices(AuthorElement)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getTableColSpanIndices(ro.sync.ecss.extensions.api.node.AuthorElement))
Use [AuthorTableAccess.getTableColSpanIndices(AuthorElement)](ro/sync/ecss/extensions/api/access/AuthorTableAccess.md#getTableColSpanIndices(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getTableNumberOfColumns(AuthorElement)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getTableNumberOfColumns(ro.sync.ecss.extensions.api.node.AuthorElement))
Use [AuthorTableAccess.getTableNumberOfColumns(AuthorElement)](ro/sync/ecss/extensions/api/access/AuthorTableAccess.md#getTableNumberOfColumns(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getTableRow(int, AuthorElement)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getTableRow(int,ro.sync.ecss.extensions.api.node.AuthorElement))
Use [AuthorTableAccess.getTableRow(int, AuthorElement)](ro/sync/ecss/extensions/api/access/AuthorTableAccess.md#getTableRow(int,ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getTableRowCount(AuthorElement)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getTableRowCount(ro.sync.ecss.extensions.api.node.AuthorElement))
Use [AuthorTableAccess.getTableRowCount(AuthorElement)](ro/sync/ecss/extensions/api/access/AuthorTableAccess.md#getTableRowCount(ro.sync.ecss.extensions.api.node.AuthorElement)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.getWordAtCaret()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#getWordAtCaret())
Use [WSTextBasedEditorPage.getWordAtCaret()](ro/sync/exml/workspace/api/editor/page/WSTextBasedEditorPage.md#getWordAtCaret()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.hasSelection()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#hasSelection())
Use [WSAuthorEditorPageBase.hasSelection()](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#hasSelection()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.inInlineContext(int)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#inInlineContext(int))
Use [AuthorDocumentController.inInlineContext(int)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#inInlineContext(int)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.insertMultipleElements(AuthorElement, String[], int[], String)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#insertMultipleElements(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,int%5B%5D,java.lang.String))
Use [AuthorDocumentController.insertMultipleElements(AuthorElement, String[], int[], String)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#insertMultipleElements(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,int%5B%5D,java.lang.String)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.insertText(String, int)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#insertText(java.lang.String,int))
Use [AuthorDocumentController.insertText(int, String)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#insertText(int,java.lang.String)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.insertXMLFragment(String, int)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#insertXMLFragment(java.lang.String,int))
Use [AuthorDocumentController.insertXMLFragment(String, int)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#insertXMLFragment(java.lang.String,int)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.insertXMLFragment(String, String, String)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#insertXMLFragment(java.lang.String,java.lang.String,java.lang.String))
Use [AuthorDocumentController.insertXMLFragment(String, String, String)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#insertXMLFragment(java.lang.String,java.lang.String,java.lang.String)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.isStandalone()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#isStandalone())
Use [Workspace.isStandalone()](ro/sync/exml/workspace/api/Workspace.md#isStandalone()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.isTrackingChanges()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#isTrackingChanges())
Use [ChangeTrackingController.isTrackingChanges()](ro/sync/ecss/extensions/api/ChangeTrackingController.md#isTrackingChanges()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.locateFile(URL)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#locateFile(java.net.URL))
Use [UtilAccess.locateFile(URL)](ro/sync/exml/workspace/api/util/UtilAccess.md#locateFile(java.net.URL)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.makeRelative(URL, URL)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#makeRelative(java.net.URL,java.net.URL))
Use [UtilAccess.makeRelative(URL, URL)](ro/sync/exml/workspace/api/util/UtilAccess.md#makeRelative(java.net.URL,java.net.URL)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.multipleDelete(AuthorElement, int[], int[])](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#multipleDelete(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D,int%5B%5D))
Use [AuthorDocumentController.multipleDelete(AuthorElement, int[], int[])](ro/sync/ecss/extensions/api/AuthorDocumentController.md#multipleDelete(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D,int%5B%5D)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.newNonValidatingXMLReader()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#newNonValidatingXMLReader())
Use [AuthorUtilAccess.newNonValidatingXMLReader()](ro/sync/ecss/extensions/api/access/AuthorUtilAccess.md#newNonValidatingXMLReader()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.removeAuthorListener(AuthorListener)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#removeAuthorListener(ro.sync.ecss.extensions.api.AuthorListener))
Use [AuthorDocumentController.removeAuthorListener(AuthorListener)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#removeAuthorListener(ro.sync.ecss.extensions.api.AuthorListener)) intead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.removeClonedElementAttribute(AuthorElement, String)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#removeClonedElementAttribute(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String))
Use [AuthorElement.removeAttribute(String)](ro/sync/ecss/extensions/api/node/AuthorElement.md#removeAttribute(java.lang.String)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.resolvePath(URL, String, boolean, boolean)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#resolvePath(java.net.URL,java.lang.String,boolean,boolean))
Use [AuthorUtilAccess.resolvePath(URL, String, boolean, boolean)](ro/sync/ecss/extensions/api/access/AuthorUtilAccess.md#resolvePath(java.net.URL,java.lang.String,boolean,boolean)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.select(int, int)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#select(int,int))
Use [WSAuthorEditorPageBase.select(int, int)](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#select(int,int)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.selectWord()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#selectWord())
Use [WSTextBasedEditorPage.selectWord()](ro/sync/exml/workspace/api/editor/page/WSTextBasedEditorPage.md#selectWord()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.setCaretPosition(int)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#setCaretPosition(int))
Use [WSTextBasedEditorPage.setCaretPosition(int)](ro/sync/exml/workspace/api/editor/page/WSTextBasedEditorPage.md#setCaretPosition(int)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.setClonedElementAttribute(AuthorElement, String, AttrValue)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#setClonedElementAttribute(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue))
Use [AuthorElement.setAttribute(String, AttrValue)](ro/sync/ecss/extensions/api/node/AuthorElement.md#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.showConfirmDialog(String, String, String[], int[])](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D))
Use [WorkspaceUtilities.showConfirmDialog(String, String, String[], int[])](ro/sync/exml/workspace/api/WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.showErrorMessage(String)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#showErrorMessage(java.lang.String))
Use [WorkspaceUtilities.showErrorMessage(String)](ro/sync/exml/workspace/api/WorkspaceUtilities.md#showErrorMessage(java.lang.String)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.surroundInFragment(String, int, int)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#surroundInFragment(java.lang.String,int,int))
Use [AuthorDocumentController.surroundInFragment(String, int, int)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#surroundInFragment(java.lang.String,int,int)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.surroundInText(String, String, int, int)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#surroundInText(java.lang.String,java.lang.String,int,int))
Use [AuthorDocumentController.surroundInText(String, String, int, int)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#surroundInText(java.lang.String,java.lang.String,int,int)) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.toggleTrackChanges()](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#toggleTrackChanges())
Use [ChangeTrackingController.toggleTrackChanges()](ro/sync/ecss/extensions/api/ChangeTrackingController.md#toggleTrackChanges()) instead.
  [ro.sync.ecss.extensions.api.AuthorAccessDeprecated.viewToModel(int, int)](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md#viewToModel(int,int))
Use [WSAuthorEditorPageBase.viewToModel(int, int)](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#viewToModel(int,int)) instead.
  [ro.sync.ecss.extensions.api.AuthorDocumentController.addAuthorPersistentHighlightListener(AuthorPersistentHighlightsListener)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#addAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener))
Use [AuthorReviewController.addAuthorPersistentHighlightListener(AuthorPersistentHighlightsListener)](ro/sync/ecss/extensions/api/AuthorReviewController.md#addAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener)) instead
  [ro.sync.ecss.extensions.api.AuthorDocumentController.addPersistentHighlightsFilter(AuthorPersistentHighlightsFilter)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#addPersistentHighlightsFilter(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsFilter))
Use [AuthorReviewController.addPersistentHighlightsFilter(AuthorPersistentHighlightsFilter)](ro/sync/ecss/extensions/api/AuthorReviewController.md#addPersistentHighlightsFilter(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsFilter)) instead
  [ro.sync.ecss.extensions.api.AuthorDocumentController.getText(int, int)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#getText(int,int))
Please use the API [AuthorDocumentController.getContentCharSequence()](ro/sync/ecss/extensions/api/AuthorDocumentController.md#getContentCharSequence()).
  [ro.sync.ecss.extensions.api.AuthorDocumentController.getTextContentLength()](ro/sync/ecss/extensions/api/AuthorDocumentController.md#getTextContentLength())
Use the API based on the [AuthorNode](ro/sync/ecss/extensions/api/node/AuthorNode.md) to get the length of the displayed text only, without mark-up markers.
  [ro.sync.ecss.extensions.api.AuthorDocumentController.removeAuthorPersistentHighlightListener(AuthorPersistentHighlightsListener)](ro/sync/ecss/extensions/api/AuthorDocumentController.md#removeAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener))
Use [AuthorReviewController.removeAuthorPersistentHighlightListener(AuthorPersistentHighlightsListener)](ro/sync/ecss/extensions/api/AuthorReviewController.md#removeAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener)) instead
  [ro.sync.ecss.extensions.api.AuthorElementBaseInterface.getBeforeElement()](ro/sync/ecss/extensions/api/AuthorElementBaseInterface.md#getBeforeElement())
This functionality is needed from the CSS style matcher, so it will eventually move there. Will be removed in 17.0 or later.
  [ro.sync.ecss.extensions.api.AuthorElementBaseInterface.isFirstChildElement()](ro/sync/ecss/extensions/api/AuthorElementBaseInterface.md#isFirstChildElement())  [ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandlerAdapter.getLastResult()](ro/sync/ecss/extensions/api/AuthorSchemaAwareEditingHandlerAdapter.md#getLastResult())
Will be removed in a future version
  [ro.sync.ecss.extensions.api.ChangeTrackingController.accept(int, int)](ro/sync/ecss/extensions/api/ChangeTrackingController.md#accept(int,int))
Replaced by "ro.sync.ecss.extensions.api.ChangeTrackingController.acceptSelection(int, int)"
  [ro.sync.ecss.extensions.api.ChangeTrackingController.reject(int, int)](ro/sync/ecss/extensions/api/ChangeTrackingController.md#reject(int,int))
Replaced by "ro.sync.ecss.extensions.api.ChangeTrackingController.rejectSelection(int, int)"
  [ro.sync.ecss.extensions.api.component.AuthorComponentProvider.createExtensionActionsToolbars()](ro/sync/ecss/extensions/api/component/AuthorComponentProvider.md#createExtensionActionsToolbars())
Please use instead the method ((WSAuthorComponentEditorPage)getWSEditorAccess().getCurrentPage()).createExtensionActionsToolbars();
  [ro.sync.ecss.extensions.api.component.AuthorComponentProvider.getAuthorAccess()](ro/sync/ecss/extensions/api/component/AuthorComponentProvider.md#getAuthorAccess())
Please use instead the method ((WSAuthorEditorPage)getWSEditorAccess().getCurrentPage()).getAuthorAccess().
  [ro.sync.ecss.extensions.api.component.AuthorComponentProvider.getAuthorCommonActions()](ro/sync/ecss/extensions/api/component/AuthorComponentProvider.md#getAuthorCommonActions())
Please use instead the method ((WSAuthorEditorPage)getWSEditorAccess().getCurrentPage()).getActionsProvider().getAuthorCommonActions().
  [ro.sync.ecss.extensions.api.component.AuthorComponentProvider.getAuthorExtensionActions()](ro/sync/ecss/extensions/api/component/AuthorComponentProvider.md#getAuthorExtensionActions())
Please use instead the method ((WSAuthorEditorPage)getWSEditorAccess().getCurrentPage()).getActionsProvider().getAuthorExtensionActions().
  [ro.sync.ecss.extensions.api.component.AuthorComponentProvider.setBreadCrumbPopUpCustomizer(PopupMenuCustomizer)](ro/sync/ecss/extensions/api/component/AuthorComponentProvider.md#setBreadCrumbPopUpCustomizer(ro.sync.ecss.extensions.api.component.PopupMenuCustomizer))
Please use instead the method ((WSAuthorComponentEditorPage)getWSEditorAccess().getCurrentPage()).setBreadCrumbPopUpCustomizer();
  [ro.sync.ecss.extensions.api.component.AuthorComponentProvider.setEditorPopUpCustomizer(PopupMenuCustomizer)](ro/sync/ecss/extensions/api/component/AuthorComponentProvider.md#setEditorPopUpCustomizer(ro.sync.ecss.extensions.api.component.PopupMenuCustomizer))
Please use instead the method ((WSAuthorEditorPage)getWSEditorAccess().getCurrentPage())addPopUpMenuCustomizer(AuthorPopupMenuCustomizer popUpCustomizer)
  [ro.sync.ecss.extensions.api.component.AuthorComponentProvider.setOutlinerPopUpCustomizer(PopupMenuCustomizer)](ro/sync/ecss/extensions/api/component/AuthorComponentProvider.md#setOutlinerPopUpCustomizer(ro.sync.ecss.extensions.api.component.PopupMenuCustomizer))
Please use instead the method ((WSAuthorComponentEditorPage)getWSEditorAccess().getCurrentPage()).setOutlinerPopUpCustomizer();
  [ro.sync.ecss.extensions.api.component.AuthorComponentProvider.showBreadCrumb(boolean)](ro/sync/ecss/extensions/api/component/AuthorComponentProvider.md#showBreadCrumb(boolean))
Please use instead the method ((WSAuthorComponentEditorPage)getWSEditorAccess().getCurrentPage()).showBreadCrumbPanel();
  [ro.sync.ecss.extensions.api.component.ditamap.DITAMapTreeComponentProvider.getDITACommonActions()](ro/sync/ecss/extensions/api/component/ditamap/DITAMapTreeComponentProvider.md#getDITACommonActions())
Please use instead the method getDITAAccess().getActionsProvider().getActions().
  [ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation.getFragmentOriginalLocation()](ro/sync/ecss/extensions/api/content/ClipboardFragmentInformation.md#getFragmentOriginalLocation())
from Oxygen 24 because it modifies the system ID at consecutive Paste, setting the systemID as current editor location.
  [ro.sync.ecss.extensions.api.DocumentContentChangedEvent.isSimpleTextEdit()](ro/sync/ecss/extensions/api/DocumentContentChangedEvent.md#isSimpleTextEdit())
Use [DocumentContentChangedEvent.getType()](ro/sync/ecss/extensions/api/DocumentContentChangedEvent.md#getType()) to determine the type of edit.
  [ro.sync.ecss.extensions.api.editor.AuthorInplaceContext.getAttributeToEdit()](ro/sync/ecss/extensions/api/editor/AuthorInplaceContext.md#getAttributeToEdit())
Use [AuthorInplaceContext.getAttributeToEditQName()](ro/sync/ecss/extensions/api/editor/AuthorInplaceContext.md#getAttributeToEditQName()) instead. This method returns the attribute name as it was specified in the CSS. If a QName was specified then this QName might not be valid in the context of the current element. Property [InplaceEditorArgumentKeys.PROPERTY_EDIT_QUALIFIED](ro/sync/ecss/extensions/api/editor/InplaceEditorArgumentKeys.md#PROPERTY_EDIT_QUALIFIED)should be used in these situations.
  [ro.sync.ecss.extensions.api.highlights.ColorHighlightPainter.setStrikeOut(boolean)](ro/sync/ecss/extensions/api/highlights/ColorHighlightPainter.md#setStrikeOut(boolean))
Use [ColorHighlightPainter.setTextDecoration(TextDecoration)](ro/sync/ecss/extensions/api/highlights/ColorHighlightPainter.md#setTextDecoration(ro.sync.ecss.extensions.api.highlights.ColorHighlightPainter.TextDecoration)) instead.
  [ro.sync.ecss.extensions.api.node.AuthorElement.getChild(String)](ro/sync/ecss/extensions/api/node/AuthorElement.md#getChild(java.lang.String))
Use [AuthorElement.getElementsByLocalName(String)](ro/sync/ecss/extensions/api/node/AuthorElement.md#getElementsByLocalName(java.lang.String))[0] instead.
  [ro.sync.ecss.extensions.api.OptionChangedEvent.getNewValue()](ro/sync/ecss/extensions/api/OptionChangedEvent.md#getNewValue())  [ro.sync.ecss.extensions.api.OptionChangedEvent.getOldValue()](ro/sync/ecss/extensions/api/OptionChangedEvent.md#getOldValue())  [ro.sync.ecss.extensions.api.table.operations.AuthorTableOperationsHandler.handleDeleteRow(AuthorTableDeleteRowArguments)](ro/sync/ecss/extensions/api/table/operations/AuthorTableOperationsHandler.md#handleDeleteRow(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowArguments))
Use [AuthorTableOperationsHandler.handleDeleteRows(AuthorTableDeleteRowsArguments)](ro/sync/ecss/extensions/api/table/operations/AuthorTableOperationsHandler.md#handleDeleteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowsArguments)) method instead.
  [ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel.getDPILocation(DocumentPositionedInfo)](ro/sync/ecss/extensions/api/webapp/AuthorDocumentModel.md#getDPILocation(ro.sync.document.DocumentPositionedInfo))
use {[AuthorDocumentModel.getDocumentValidator()](ro/sync/ecss/extensions/api/webapp/AuthorDocumentModel.md#getDocumentValidator()).
  [ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel.getValidationScenarios()](ro/sync/ecss/extensions/api/webapp/AuthorDocumentModel.md#getValidationScenarios())
use {[AuthorDocumentModel.getDocumentValidator()](ro/sync/ecss/extensions/api/webapp/AuthorDocumentModel.md#getDocumentValidator()).
  [ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel.getValidationTask()](ro/sync/ecss/extensions/api/webapp/AuthorDocumentModel.md#getValidationTask())
use {[AuthorDocumentModel.getDocumentValidator()](ro/sync/ecss/extensions/api/webapp/AuthorDocumentModel.md#getDocumentValidator()).
  [ro.sync.ecss.extensions.api.webapp.WebappAuthorDocumentFactory.setPlugins(File)](ro/sync/ecss/extensions/api/webapp/WebappAuthorDocumentFactory.md#setPlugins(java.io.File))
use {[WebappAuthorDocumentFactory.setPlugins(File, File)](ro/sync/ecss/extensions/api/webapp/WebappAuthorDocumentFactory.md#setPlugins(java.io.File,java.io.File)).
  [ro.sync.ecss.extensions.docbook.DocbookAuthorTableOperationsHandler.handleDeleteRow(AuthorTableDeleteRowArguments)](ro/sync/ecss/extensions/docbook/DocbookAuthorTableOperationsHandler.md#handleDeleteRow(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowArguments))

 [ro.sync.exml.workspace.api.editor.page.author.WSAuthorEditorPage.getChangeTrackingController()](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPage.md#getChangeTrackingController())
Use [WSAuthorEditorPage.getReviewController()](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPage.md#getReviewController()) instead.
  [ro.sync.exml.workspace.api.editor.page.author.WSAuthorEditorPageBase.setPopUpMenuCustomizer(AuthorPopupMenuCustomizer)](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#setPopUpMenuCustomizer(ro.sync.ecss.extensions.api.structure.AuthorPopupMenuCustomizer))
This method removes all pop-up menu customizers already registered, please use the "addPopUpMenuCustomizer" method instead.
  [ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionManager.getContextKeyDefinitions()](ro/sync/exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManager.md#getContextKeyDefinitions())
For performance reasons, consider implementing the {[KeyDefinitionManager.getContextKeyDefinitionsMap(URL)](ro/sync/exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManager.md#getContextKeyDefinitionsMap(java.net.URL)) method instead.
  [ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionManager.getContextKeyDefinitions(URL)](ro/sync/exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManager.md#getContextKeyDefinitions(java.net.URL))
For performance reasons, consider implementing the {[KeyDefinitionManager.getContextKeyDefinitionsMap(URL)](ro/sync/exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManager.md#getContextKeyDefinitionsMap(java.net.URL)) method instead.
  [ro.sync.exml.workspace.api.options.WSOptionChangedEvent.getNewValue()](ro/sync/exml/workspace/api/options/WSOptionChangedEvent.md#getNewValue())
The value may not be a plain String, use the "getNewValueObject" instead
  [ro.sync.exml.workspace.api.options.WSOptionChangedEvent.getOldValue()](ro/sync/exml/workspace/api/options/WSOptionChangedEvent.md#getOldValue())
The value may not be a plain String, use the "getOldValueObject" instead
  [ro.sync.exml.workspace.api.options.WSOptionsStorage.setOptionsDoctypePrefix(String)](ro/sync/exml/workspace/api/options/WSOptionsStorage.md#setOptionsDoctypePrefix(java.lang.String))
WARNING: THE USE OF THIS METHOD IS DISCOURAGED AND DEPRECATED

All plugins initially share a common settings namespace. So that would mean that a plugin could read values set by other plugins or it could register to receive value changed events for certain option keys set by other plugins (which may sometimes be useful). But this also means that accidentally a plugin could also overwrite the value for a certain key if more than one plugin use the same key. So ideally your plugin's persisted keys would all be manually prefixed with some unique ID when they are defined. This would be the recommended way of doing things. If you still want to use the method:

Using this method when working with the singleton access to the workspace "PluginWorkspaceProvider.getPluginWorkspace().getOptionsStorage()" will set it for all plugins. So a plugin will globally influence the global prefixes for keys loaded and saved also by other plugins. Which is never a good thing.

But using this method on the WorkspaceAccessPluginExtension.applicationStarted will only set the prefix for your plugin. So as long as your plugin will keep using the "WSOptionsStorage" received on the applicationStarted callback you will not influence other plugins.
  [ro.sync.exml.workspace.api.process.ProcessListener.processStarted(String, String)](ro/sync/exml/workspace/api/process/ProcessListener.md#processStarted(java.lang.String,java.lang.String))
replaced with processAboutToStart in version 23.1.
  [ro.sync.exml.workspace.api.standalone.ui.OKCancelDialog.getHiDPIAwareDimension(Dimension)](ro/sync/exml/workspace/api/standalone/ui/OKCancelDialog.md#getHiDPIAwareDimension(java.awt.Dimension))
Kept for backwards compatibility, no longer necessary with java 9+
  [ro.sync.exml.workspace.api.util.XMLUtilAccess.threeWayAutoMerge(String, String, String, MergeConflictResolutionMethods)](ro/sync/exml/workspace/api/util/XMLUtilAccess.md#threeWayAutoMerge(java.lang.String,java.lang.String,java.lang.String,ro.sync.merge.MergeConflictResolutionMethods))
since 19.1, please use the equivalent [CompareUtilAccess](ro/sync/exml/workspace/api/util/CompareUtilAccess.md) utilities.
  [ro.sync.exml.workspace.api.Workspace.isStandalone()](ro/sync/exml/workspace/api/Workspace.md#isStandalone())
This method returns false also when running inside the WebApp. Use [ApplicationInformationAccess.getPlatform()](ro/sync/exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()) instead.
  [ro.sync.exml.workspace.api.WorkspaceUtilities.clearImageCache()](ro/sync/exml/workspace/api/WorkspaceUtilities.md#clearImageCache())
Replaced by [WorkspaceUtilities.getImageUtilities()](ro/sync/exml/workspace/api/WorkspaceUtilities.md#getImageUtilities())

*   Deprecated Constructors
Constructor

Description
 [ro.sync.ecss.css.URIContent(String, String)](ro/sync/ecss/css/URIContent.md#%3Cinit%3E(java.lang.String,java.lang.String))
Left only for backward compatibility.
  [ro.sync.ecss.extensions.api.OptionChangedEvent(String, String, String)](ro/sync/ecss/extensions/api/OptionChangedEvent.md#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String))  [ro.sync.ecss.extensions.commons.table.operations.TableInfo(Map<String, Object>)](ro/sync/ecss/extensions/commons/table/operations/TableInfo.md#%3Cinit%3E(java.util.Map))
Use [TableInfo(Map, int)](ro/sync/ecss/extensions/commons/table/operations/TableInfo.md#%3Cinit%3E(java.util.Map,int)) instead because the table operation can also convert lists to tables and we need to provide a minimum number of rows.
  [ro.sync.ecss.extensions.dita.conref.DITAConRefResolver(ContextKeyManager)](ro/sync/ecss/extensions/dita/conref/DITAConRefResolver.md#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManager))
use [DITAConRefResolver(ContextKeyManagerProvider)](ro/sync/ecss/extensions/dita/conref/DITAConRefResolver.md#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider)) instead.
  [ro.sync.ecss.extensions.dita.link.DitaLinkTextResolver(ContextKeyManager)](ro/sync/ecss/extensions/dita/link/DitaLinkTextResolver.md#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManager))
use [DitaLinkTextResolver(ContextKeyManagerProvider)](ro/sync/ecss/extensions/dita/link/DitaLinkTextResolver.md#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider)) instead.
  [ro.sync.ecss.extensions.dita.map.topicref.DITAMapRefResolver()](ro/sync/ecss/extensions/dita/map/topicref/DITAMapRefResolver.md#%3Cinit%3E())
use [DITAMapRefResolver(ContextKeyManagerProvider)](ro/sync/ecss/extensions/dita/map/topicref/DITAMapRefResolver.md#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider)) instead, otherwise key resolution will not work in Web Author.
  [ro.sync.ecss.extensions.dita.map.topicref.DITAMapRefResolver(ContextKeyManager)](ro/sync/ecss/extensions/dita/map/topicref/DITAMapRefResolver.md#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManager))
use [DITAMapRefResolver(ContextKeyManagerProvider)](ro/sync/ecss/extensions/dita/map/topicref/DITAMapRefResolver.md#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider)) instead.

*   Deprecated Enum Constants
Enum Constant

Description
 [ro.sync.ecss.extensions.api.CursorType.CURSOR_RESIZE](ro/sync/ecss/extensions/api/CursorType.md#CURSOR_RESIZE)
Use [CursorType.CURSOR_E_RESIZE](ro/sync/ecss/extensions/api/CursorType.md#CURSOR_E_RESIZE) instead.
  [ro.sync.ecss.extensions.api.CursorType.CURSOR_SELECT_ROW](ro/sync/ecss/extensions/api/CursorType.md#CURSOR_SELECT_ROW)
You should use one of the two other constants, specifying the direction.
  [ro.sync.ecss.extensions.api.CursorType.CURSOR_SELECT_TABLE](ro/sync/ecss/extensions/api/CursorType.md#CURSOR_SELECT_TABLE)
You should use one of the two other constants, specifying the direction.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
