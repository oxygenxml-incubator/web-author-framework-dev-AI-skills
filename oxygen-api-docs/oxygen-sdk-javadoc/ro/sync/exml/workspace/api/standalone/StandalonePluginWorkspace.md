Package [ro.sync.exml.workspace.api.standalone](package-summary.md)

# Interface StandalonePluginWorkspace
    All Superinterfaces: [ApplicationInformationAccess](../application/ApplicationInformationAccess.md), [ColorThemeUtilities](../util/ColorThemeUtilities.md), [DiffAndMergeTools](DiffAndMergeTools.md), [GlobalOptionsStorage](../options/GlobalOptionsStorage.md), [MathFlowConfigurator](../math/MathFlowConfigurator.md), [PluginWorkspace](../PluginWorkspace.md), [ReferencesCustomizer](ReferencesCustomizer.md), [Workspace](../Workspace.md), [WorkspaceUtilities](../WorkspaceUtilities.md)   All Known Subinterfaces: [WebappPluginWorkspace](../../../../ecss/extensions/api/webapp/access/WebappPluginWorkspace.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface StandalonePluginWorkspaceextends [PluginWorkspace](../PluginWorkspace.md), [MathFlowConfigurator](../math/MathFlowConfigurator.md), [DiffAndMergeTools](DiffAndMergeTools.md)
The **Plugin Workspace** offers the possibility to customize the Workspace toolbars, menu bars or views, to access utility methods or to access (and add listeners for) all opened editors from the Main editing area or from the DITA Maps editing area. Each opened editor contains one or more pages. The current editor page can be accessed trough the [WSEditor.getCurrentPage()](../editor/WSEditor.md#getCurrentPage())method that returns specific editor implementations for Author and Text pages:
*  [WSAuthorEditorPage](../editor/page/author/WSAuthorEditorPage.md) that provides access to Author editor page document controller or change tracking controller
*  [WSTextEditorPage](../editor/page/text/WSTextEditorPage.md) that offers access to the edited document.
Both text based editor pages provides informations and actions regarding the caret position or the document current selection.
  Since: 11.2
## Field Summary

### Fields inherited from interface ro.sync.exml.workspace.api.[PluginWorkspace](../PluginWorkspace.md)
 [DITA_MAPS_EDITING_AREA](../PluginWorkspace.md#DITA_MAPS_EDITING_AREA), [MAIN_EDITING_AREA](../PluginWorkspace.md#MAIN_EDITING_AREA)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addMenuBarCustomizer](#addMenuBarCustomizer(ro.sync.exml.workspace.api.standalone.MenuBarCustomizer))([MenuBarCustomizer](MenuBarCustomizer.md) menuBarCustomizer)
Adds a customizer which can contribute to or modify existing menu components.
  void [addMenusAndToolbarsContributorCustomizer](#addMenusAndToolbarsContributorCustomizer(ro.sync.exml.workspace.api.standalone.actions.MenusAndToolbarsContributorCustomizer))([MenusAndToolbarsContributorCustomizer](actions/MenusAndToolbarsContributorCustomizer.md) customizer)
Add a customizer for menus and toolbars.
  void [addPluginExtension](#addPluginExtension(java.lang.String,ro.sync.exml.plugin.PluginExtension))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) extensionType, [PluginExtension](../../../plugin/PluginExtension.md) pluginExtension)
Adds a plug-in extension of a specified type.
  void [addToolbarComponentsCustomizer](#addToolbarComponentsCustomizer(ro.sync.exml.workspace.api.standalone.ToolbarComponentsCustomizer))([ToolbarComponentsCustomizer](ToolbarComponentsCustomizer.md) componentsCustomizer)
Adds a customizer which can contribute to or modify existing toolbars or contribute to the reserved **Plugins** toolbar.
  void [addTopicRefTargetInfoProvider](#addTopicRefTargetInfoProvider(java.lang.String,ro.sync.exml.workspace.api.standalone.ditamap.TopicRefTargetInfoProvider))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol, [TopicRefTargetInfoProvider](ditamap/TopicRefTargetInfoProvider.md) targetInfoProvider)
Add a target information provider to the DITA Maps Manager view.
  void [addViewComponentCustomizer](#addViewComponentCustomizer(ro.sync.exml.workspace.api.standalone.ViewComponentCustomizer))([ViewComponentCustomizer](ViewComponentCustomizer.md) viewComponentCustomizer)
Adds a customizer which can contribute to or modify existing views or contribute to the reserved custom view.
  [AuthorPreviewComponentProvider](../editor/page/author/AuthorPreviewComponentProvider.md) [createAuthorPreviewComponentProvider](#createAuthorPreviewComponentProvider())()
Create a lightweight not editable Author preview component.
  [EditorComponentProvider](../../../../ecss/extensions/api/component/EditorComponentProvider.md) [createEditorComponentProvider](#createEditorComponentProvider(java.lang.String%5B%5D,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage)
Creates a new editor component.
  [EditorComponentProvider](../../../../ecss/extensions/api/component/EditorComponentProvider.md) [createEditorComponentProvider](#createEditorComponentProvider(java.lang.String%5B%5D,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
Creates a new editor component.
  [ActionsProvider](actions/ActionsProvider.md) [getActionsProvider](#getActionsProvider())()
Provides access to global actions defined in the application.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOxygenActionID](#getOxygenActionID(javax.swing.Action))([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action)
Get an unique ID (which does not depend on the action name) for an action Oxygen has mounted on the main JMenuBar or on the toolbars.
  [ProjectController](project/ProjectController.md) [getProjectManager](#getProjectManager())()
Get access to Project related API.
  [ProxyDetailsProvider](proxy/ProxyDetailsProvider.md) [getProxyDetailsProvider](#getProxyDetailsProvider())()
Get access to currently configured network proxy information.
  [PluginResourceBundle](../PluginResourceBundle.md) [getResourceBundle](#getResourceBundle())()
A message bundle that holds all the internationalized messages displayed in all the plugins for a language set in Preferences.
  void [hideToolbar](#hideToolbar(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toolbarID)
Hide a toolbar specified by the toolbar ID.
  void [hideView](#hideView(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) viewID)
Hide a view specified by the view ID.
  boolean [isToolbarShowing](#isToolbarShowing(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toolbarID)
Check if a toolbar is showing or hidden.
  boolean [isViewAvailable](#isViewAvailable(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) viewID)
Check if a view with a certain ID is available in the application.
  boolean [isViewShowing](#isViewShowing(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) viewID)
Check if a view is showing or hidden.
  void [removeMenusAndToolbarsContributorCustomizer](#removeMenusAndToolbarsContributorCustomizer(ro.sync.exml.workspace.api.standalone.actions.MenusAndToolbarsContributorCustomizer))([MenusAndToolbarsContributorCustomizer](actions/MenusAndToolbarsContributorCustomizer.md) customizer)
Remove a customizer for menus and toolbars.
  void [showToolbar](#showToolbar(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toolbarID)
Show a toolbar specified by the toolbar ID.
  void [showView](#showView(java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) viewID, boolean requestFocus)
Show a view specified by the view ID.

### Methods inherited from interface ro.sync.exml.workspace.api.application.[ApplicationInformationAccess](../application/ApplicationInformationAccess.md)
 [getApplicationName](../application/ApplicationInformationAccess.md#getApplicationName()), [getApplicationType](../application/ApplicationInformationAccess.md#getApplicationType()), [getLicenseInformationProvider](../application/ApplicationInformationAccess.md#getLicenseInformationProvider()), [getPlatform](../application/ApplicationInformationAccess.md#getPlatform()), [getPreferencesDirectory](../application/ApplicationInformationAccess.md#getPreferencesDirectory()), [getUserInterfaceLanguage](../application/ApplicationInformationAccess.md#getUserInterfaceLanguage()), [getVersion](../application/ApplicationInformationAccess.md#getVersion()), [getVersionBuildID](../application/ApplicationInformationAccess.md#getVersionBuildID())
### Methods inherited from interface ro.sync.exml.workspace.api.util.[ColorThemeUtilities](../util/ColorThemeUtilities.md)
 [getColorTheme](../util/ColorThemeUtilities.md#getColorTheme()), [getImageInverter](../util/ColorThemeUtilities.md#getImageInverter())
### Methods inherited from interface ro.sync.exml.workspace.api.standalone.[DiffAndMergeTools](DiffAndMergeTools.md)
 [openDiffFilesApplication](DiffAndMergeTools.md#openDiffFilesApplication(java.lang.String,java.net.URL,java.lang.String,java.net.URL)), [openDiffFilesApplication](DiffAndMergeTools.md#openDiffFilesApplication(java.lang.String,java.net.URL,java.lang.String,java.net.URL,java.net.URL,boolean)), [openDiffFilesApplication](DiffAndMergeTools.md#openDiffFilesApplication(java.net.URL,java.net.URL)), [openDiffFilesApplication](DiffAndMergeTools.md#openDiffFilesApplication(java.net.URL,java.net.URL,java.net.URL)), [openMergeApplication](DiffAndMergeTools.md#openMergeApplication(java.io.File,java.io.File,java.io.File,java.util.Map)), [openMergeApplication](DiffAndMergeTools.md#openMergeApplication(java.lang.String,java.lang.String,boolean,java.lang.String,java.net.URL,boolean,boolean,java.lang.String,java.net.URL,boolean,boolean,java.net.URL)), [openPreviewDialog](DiffAndMergeTools.md#openPreviewDialog(java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.util.LinkedHashMap)), [openPreviewDialog](DiffAndMergeTools.md#openPreviewDialog(java.lang.String,java.lang.String,java.util.LinkedHashMap))
### Methods inherited from interface ro.sync.exml.workspace.api.options.[GlobalOptionsStorage](../options/GlobalOptionsStorage.md)
 [addGlobalOptionListener](../options/GlobalOptionsStorage.md#addGlobalOptionListener(ro.sync.ecss.extensions.api.OptionListener)), [deserializePersistentObject](../options/GlobalOptionsStorage.md#deserializePersistentObject(java.lang.String)), [getGlobalObjectProperty](../options/GlobalOptionsStorage.md#getGlobalObjectProperty(java.lang.String)), [importGlobalOptions](../options/GlobalOptionsStorage.md#importGlobalOptions(java.io.File)), [importGlobalOptions](../options/GlobalOptionsStorage.md#importGlobalOptions(java.io.File,boolean)), [removeGlobalOptionListener](../options/GlobalOptionsStorage.md#removeGlobalOptionListener(ro.sync.ecss.extensions.api.OptionListener)), [saveGlobalOptions](../options/GlobalOptionsStorage.md#saveGlobalOptions()), [serializePersistentObject](../options/GlobalOptionsStorage.md#serializePersistentObject(java.lang.Object)), [setGlobalObjectProperty](../options/GlobalOptionsStorage.md#setGlobalObjectProperty(java.lang.String,java.lang.Object)), [showPreferencesPages](../options/GlobalOptionsStorage.md#showPreferencesPages(java.lang.String%5B%5D,java.lang.String,boolean))
### Methods inherited from interface ro.sync.exml.workspace.api.math.[MathFlowConfigurator](../math/MathFlowConfigurator.md)
 [setMathFlowFixedLicenseFile](../math/MathFlowConfigurator.md#setMathFlowFixedLicenseFile(java.io.File)), [setMathFlowFixedLicenseKeyForComposer](../math/MathFlowConfigurator.md#setMathFlowFixedLicenseKeyForComposer(java.lang.String)), [setMathFlowFixedLicenseKeyForEditor](../math/MathFlowConfigurator.md#setMathFlowFixedLicenseKeyForEditor(java.lang.String)), [setMathFlowInstallationFolder](../math/MathFlowConfigurator.md#setMathFlowInstallationFolder(java.io.File))
### Methods inherited from interface ro.sync.exml.workspace.api.[PluginWorkspace](../PluginWorkspace.md)
 [addAuthorCSSAlternativesCustomizer](../PluginWorkspace.md#addAuthorCSSAlternativesCustomizer(ro.sync.exml.workspace.api.editor.page.author.css.AuthorCSSAlternativesCustomizer)), [addBatchOperationsListener](../PluginWorkspace.md#addBatchOperationsListener(ro.sync.exml.workspace.api.listeners.BatchOperationsListener)), [addEditorChangeListener](../PluginWorkspace.md#addEditorChangeListener(ro.sync.exml.workspace.api.listeners.WSEditorChangeListener,int)), [createAuthorDocumentProvider](../PluginWorkspace.md#createAuthorDocumentProvider(java.net.URL,java.io.Reader)), [createAuthorDocumentProvider](../PluginWorkspace.md#createAuthorDocumentProvider(java.net.URL,java.io.Reader,boolean)), [getAllEditorLocations](../PluginWorkspace.md#getAllEditorLocations(int)), [getBatchOperationsListenersAccess](../PluginWorkspace.md#getBatchOperationsListenersAccess()), [getCompareUtilAccess](../PluginWorkspace.md#getCompareUtilAccess()), [getComponentsProvider](../PluginWorkspace.md#getComponentsProvider()), [getCurrentEditorAccess](../PluginWorkspace.md#getCurrentEditorAccess(int)), [getEditorAccess](../PluginWorkspace.md#getEditorAccess(java.net.URL,int)), [getEditorChangeListeners](../PluginWorkspace.md#getEditorChangeListeners(int)), [getOptionsStorage](../PluginWorkspace.md#getOptionsStorage()), [getResultsManager](../PluginWorkspace.md#getResultsManager()), [getUtilAccess](../PluginWorkspace.md#getUtilAccess()), [getValidationUtilAccess](../PluginWorkspace.md#getValidationUtilAccess()), [getXMLRefactorUtilAccess](../PluginWorkspace.md#getXMLRefactorUtilAccess()), [getXMLUtilAccess](../PluginWorkspace.md#getXMLUtilAccess()), [removeAuthorCSSAlternativesCustomizer](../PluginWorkspace.md#removeAuthorCSSAlternativesCustomizer(ro.sync.exml.workspace.api.editor.page.author.css.AuthorCSSAlternativesCustomizer)), [removeBatchOperationsListener](../PluginWorkspace.md#removeBatchOperationsListener(ro.sync.exml.workspace.api.listeners.BatchOperationsListener)), [removeEditorChangeListener](../PluginWorkspace.md#removeEditorChangeListener(ro.sync.exml.workspace.api.listeners.WSEditorChangeListener,int)), [setDITAKeyDefinitionManager](../PluginWorkspace.md#setDITAKeyDefinitionManager(ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionManager))
### Methods inherited from interface ro.sync.exml.workspace.api.standalone.[ReferencesCustomizer](ReferencesCustomizer.md)
 [addInputURLChooserCustomizer](ReferencesCustomizer.md#addInputURLChooserCustomizer(ro.sync.exml.workspace.api.standalone.InputURLChooserCustomizer)), [addRelativeReferencesResolver](ReferencesCustomizer.md#addRelativeReferencesResolver(java.lang.String,ro.sync.exml.workspace.api.util.RelativeReferenceResolver))
### Methods inherited from interface ro.sync.exml.workspace.api.[Workspace](../Workspace.md)
 [close](../Workspace.md#close(java.net.URL)), [closeAll](../Workspace.md#closeAll()), [createNewEditor](../Workspace.md#createNewEditor(java.lang.String,java.lang.String,java.lang.String)), [createNewEditor](../Workspace.md#createNewEditor(java.net.URL,java.lang.String,java.lang.String,java.lang.String)), [delete](../Workspace.md#delete(java.net.URL)), [isStandalone](../Workspace.md#isStandalone()), [open](../Workspace.md#open(java.net.URL)), [open](../Workspace.md#open(java.net.URL,java.lang.String)), [open](../Workspace.md#open(java.net.URL,java.lang.String,java.lang.String)), [refreshInProject](../Workspace.md#refreshInProject(java.net.URL)), [saveAll](../Workspace.md#saveAll()), [setParentFrameTitle](../Workspace.md#setParentFrameTitle(java.lang.String))
### Methods inherited from interface ro.sync.exml.workspace.api.[WorkspaceUtilities](../WorkspaceUtilities.md)
 [chooseDirectory](../WorkspaceUtilities.md#chooseDirectory()), [chooseDirectory](../WorkspaceUtilities.md#chooseDirectory(java.io.File)), [chooseFile](../WorkspaceUtilities.md#chooseFile(java.io.File,java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)), [chooseFile](../WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseFile](../WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)), [chooseFiles](../WorkspaceUtilities.md#chooseFiles(java.io.File,java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURL](../WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURL](../WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String)), [chooseURL](../WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String,java.lang.String,java.lang.String)), [chooseURLPath](../WorkspaceUtilities.md#chooseURLPath(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURLPath](../WorkspaceUtilities.md#chooseURLPath(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String)), [clearImageCache](../WorkspaceUtilities.md#clearImageCache()), [createJavaProcess](../WorkspaceUtilities.md#createJavaProcess(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String,java.util.Map,java.io.File,ro.sync.exml.workspace.api.process.ProcessListener)), [createProcess](../WorkspaceUtilities.md#createProcess(ro.sync.exml.workspace.api.process.ProcessListener,java.lang.String,java.io.File,java.lang.String,boolean)), [getDataSourceAccess](../WorkspaceUtilities.md#getDataSourceAccess()), [getImageUtilities](../WorkspaceUtilities.md#getImageUtilities()), [getParentFrame](../WorkspaceUtilities.md#getParentFrame()), [getTemplateManager](../WorkspaceUtilities.md#getTemplateManager()), [openInExternalApplication](../WorkspaceUtilities.md#openInExternalApplication(java.lang.String,boolean,java.lang.String)), [openInExternalApplication](../WorkspaceUtilities.md#openInExternalApplication(java.net.URL,boolean)), [openInExternalApplication](../WorkspaceUtilities.md#openInExternalApplication(java.net.URL,boolean,java.lang.String)), [showConfirmDialog](../WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)), [showConfirmDialog](../WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D,int)), [showErrorMessage](../WorkspaceUtilities.md#showErrorMessage(java.lang.String)), [showErrorMessage](../WorkspaceUtilities.md#showErrorMessage(java.lang.String,java.lang.Throwable)), [showInformationMessage](../WorkspaceUtilities.md#showInformationMessage(java.lang.String)), [showStatusMessage](../WorkspaceUtilities.md#showStatusMessage(java.lang.String)), [showStatusMessage](../WorkspaceUtilities.md#showStatusMessage(java.lang.String,ro.sync.exml.workspace.api.OperationStatus)), [showWarningDialog](../WorkspaceUtilities.md#showWarningDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)), [showWarningDialog](../WorkspaceUtilities.md#showWarningDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D,int)), [showWarningMessage](../WorkspaceUtilities.md#showWarningMessage(java.lang.String)), [startProcess](../WorkspaceUtilities.md#startProcess(java.lang.String,java.io.File,java.lang.String,boolean))
## Method Details

### addToolbarComponentsCustomizer

void addToolbarComponentsCustomizer([ToolbarComponentsCustomizer](ToolbarComponentsCustomizer.md) componentsCustomizer)

Adds a customizer which can contribute to or modify existing toolbars or contribute to the reserved **Plugins** toolbar.  **IMPORTANT** This customizer must be set early, when the plugin extension's **applicationStarted** method gets called.  **NOTICE** You will also receive notification for the Author extension toolbars (which are dynamically constructed based on the document type of the current selected XML file). The notifications will be received before the toolbars are constructed after an XML editor which is opened in the Author page was selected. Such toolbar IDs have the prefix "Author_custom_actions" and the suffix is a number depending on how many toolbars were created for that specific document type. In this way you can dynamically filter or add to toolbar buttons already declared in the document type associated to the XML editor.
  Parameters: componentsCustomizer - The tool bar components customizer.
### addViewComponentCustomizer

void addViewComponentCustomizer([ViewComponentCustomizer](ViewComponentCustomizer.md) viewComponentCustomizer)

Adds a customizer which can contribute to or modify existing views or contribute to the reserved custom view.  **IMPORTANT** This customizer must be set early, when the plugin extension's **applicationStarted** method gets called.
  Parameters: viewComponentCustomizer - The views component customizer.
### addMenuBarCustomizer

void addMenuBarCustomizer([MenuBarCustomizer](MenuBarCustomizer.md) menuBarCustomizer)

Adds a customizer which can contribute to or modify existing menu components.  **IMPORTANT** This customizer must be set early, when the plugin extension's **applicationStarted** method gets called.
  Parameters: menuBarCustomizer - The menu bar components customizer.
### addTopicRefTargetInfoProvider

void addTopicRefTargetInfoProvider([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol, [TopicRefTargetInfoProvider](ditamap/TopicRefTargetInfoProvider.md) targetInfoProvider)

Add a target information provider to the DITA Maps Manager view. This method can be used by a CMS implementor to take control over the way Oxygen is gathering information about each topic reference. The protocol is the protocol of the URL of the opened DITA Map. For example when a DITA Map is opened in the DITA Maps Manager view the CMS can get called to compute titles for all topic references instead of the default Oxygen behavior (requesting the entire content for the referenced URL).
  Parameters: protocol - The custom protocol of the opened DITA Map for which the plugin will compute the topic reference titles and auxiliary information. targetInfoProvider - Gets called to resolve the title for the topic references in the DITA Map. Since: 12.2
### showView

void showView([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) viewID, boolean requestFocus)

Show a view specified by the view ID. If the view is hidden, this method brings it to front. If the view is in auto-hide state, this method removes its auto-hide state and bring it to front.
  Parameters: viewID - The view ID. requestFocus - True to request the focus inside the view after show. Since: 12
### hideView

void hideView([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) viewID)

Hide a view specified by the view ID.
  Parameters: viewID - The view ID. Since: 15
### isViewShowing

boolean isViewShowing([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) viewID)

Check if a view is showing or hidden.
  Parameters: viewID - The view ID. Returns: true if the view is showing Since: 15
### isViewAvailable

boolean isViewAvailable([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) viewID)

Check if a view with a certain ID is available in the application.
  Parameters: viewID - The view ID. Returns: true if the view is available in the application Since: 22
### hideToolbar

void hideToolbar([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toolbarID)

Hide a toolbar specified by the toolbar ID.
  Parameters: toolbarID - The toolbar ID. Since: 15
### showToolbar

void showToolbar([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toolbarID)

Show a toolbar specified by the toolbar ID. If the toolbar is hidden, this method shows it.
  Parameters: toolbarID - The toolbar ID. You can install a toolbar component customizer and see all available IDs. Since: 12
### isToolbarShowing

boolean isToolbarShowing([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toolbarID)

Check if a toolbar is showing or hidden.
  Parameters: toolbarID - The toolbar ID. Returns: true if the toolbar is showing Since: 15
### getOxygenActionID

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOxygenActionID([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action)

Get an unique ID (which does not depend on the action name) for an action Oxygen has mounted on the main JMenuBar or on the toolbars. If the action appears on a contextual menu but is not installed on a main menu it will pe prefixed with the constant "ACTION_WITH_NO_SHORTCUT/"
  Parameters: action - The action for which to retrieve the ID. Returns: The unique ID or null if the action is not one provided by Oxygen. Since: 12.2
### getActionsProvider

[ActionsProvider](actions/ActionsProvider.md) getActionsProvider()

Provides access to global actions defined in the application. It might be null when called in certain contexts (for example from the webapp application).
  Returns: access to global actions defined in the application. Since: 18
### addMenusAndToolbarsContributorCustomizer

void addMenusAndToolbarsContributorCustomizer([MenusAndToolbarsContributorCustomizer](actions/MenusAndToolbarsContributorCustomizer.md) customizer)

Add a customizer for menus and toolbars. It will be notified to customize various menus and toolbars.
  Parameters: customizer - The customizer which will be notified to customize menus and toolbars. Since: 18
### removeMenusAndToolbarsContributorCustomizer

void removeMenusAndToolbarsContributorCustomizer([MenusAndToolbarsContributorCustomizer](actions/MenusAndToolbarsContributorCustomizer.md) customizer)

Remove a customizer for menus and toolbars.
  Parameters: customizer - The customizer to remove. Since: 18
### createEditorComponentProvider

[EditorComponentProvider](../../../../ecss/extensions/api/component/EditorComponentProvider.md) createEditorComponentProvider([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage)throws [AuthorComponentException](../../../../ecss/extensions/api/component/AuthorComponentException.md)

Creates a new editor component. Such a component is a small XML editing container which can have all editing modes and can be added to a custom Swing-based dialog created by the developer in order for example to preview content from various target files.
  Parameters: allowedPages - The pages which will be used in the editor. One of the constant fields: [EditorPageConstants.PAGE_TEXT](../../../editor/EditorPageConstants.md#PAGE_TEXT), [EditorPageConstants.PAGE_AUTHOR](../../../editor/EditorPageConstants.md#PAGE_AUTHOR), [EditorPageConstants.PAGE_GRID](../../../editor/EditorPageConstants.md#PAGE_GRID) initialPage - The initial page in which the component will edit. Returns: the new editor component. Throws: [AuthorComponentException](../../../../ecss/extensions/api/component/AuthorComponentException.md) - The component was not initialized properly. Since: 18.1
### createEditorComponentProvider

[EditorComponentProvider](../../../../ecss/extensions/api/component/EditorComponentProvider.md) createEditorComponentProvider([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)throws [AuthorComponentException](../../../../ecss/extensions/api/component/AuthorComponentException.md)

Creates a new editor component. Such a component is a small editing container which can have all editing modes and can be added to a custom Swing-based dialog created by the developer in order for example to preview content from various target files.
  Parameters: allowedPages - The pages which will be used in the editor. One of the constant fields: [EditorPageConstants.PAGE_TEXT](../../../editor/EditorPageConstants.md#PAGE_TEXT), [EditorPageConstants.PAGE_AUTHOR](../../../editor/EditorPageConstants.md#PAGE_AUTHOR), [EditorPageConstants.PAGE_GRID](../../../editor/EditorPageConstants.md#PAGE_GRID) initialPage - The initial page in which the component will edit. contentType - The proposed content type for the component, null to fall back to XML content type. Returns: the new editor component. Throws: [AuthorComponentException](../../../../ecss/extensions/api/component/AuthorComponentException.md) - The component was not initialized properly. Since: 26.1
### createAuthorPreviewComponentProvider

[AuthorPreviewComponentProvider](../editor/page/author/AuthorPreviewComponentProvider.md) createAuthorPreviewComponentProvider()

Create a lightweight not editable Author preview component.
  Returns: An author preview component. Since: 27
### getResourceBundle

[PluginResourceBundle](../PluginResourceBundle.md) getResourceBundle()

A message bundle that holds all the internationalized messages displayed in all the plugins for a language set in Preferences. It works as a map in which any message is accessed by a specific key. The translation file must be located in a directory named "i18n" (placed in the plugin's root directory). The translation file name must be: **translation\*.xml** Here is a small sample of an translation XML file structure:
```


 <translation>
     <languageList>
       <language description="English US" lang="en_US"/>
       <language description="German" lang="de_DE"/>
       <language description="French" lang="fr_FR"/>
    </languageList>
    <key value="key_name1">
       <comment>key description1</comment>
      <val lang="en_US">en_US_translation1</val>
      <val lang="de_DE">de_DE_translation1</val>
      <val lang="fr_FR">fr_FR_translation1</val>
  </key>
   <key value="key_name2">
       <comment>key description2</comment>
      <val lang="en_US">en_US_translation2</val>
      <val lang="de_DE">de_DE_translation2</val>
      <val lang="fr_FR">fr_FR_translation2</val>
  </key>
  ........................
 </translation>


```

  Returns: The message bundle used to get the translation of messages used in the plugin. Since: 18.1
### getProxyDetailsProvider

[ProxyDetailsProvider](proxy/ProxyDetailsProvider.md) getProxyDetailsProvider()

Get access to currently configured network proxy information.
  Returns: access to currently configured network proxy information. Since: 19.1
### getProjectManager

[ProjectController](project/ProjectController.md) getProjectManager()

Get access to Project related API.
  Returns: The project manager API Since: 19.1
### addPluginExtension

void addPluginExtension([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) extensionType, [PluginExtension](../../../plugin/PluginExtension.md) pluginExtension)

Adds a plug-in extension of a specified type.
  Parameters: extensionType - The type of the plugin extension; can be a constant from . pluginExtension - The plugin extension implementation to be added. Since: 24.0
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
