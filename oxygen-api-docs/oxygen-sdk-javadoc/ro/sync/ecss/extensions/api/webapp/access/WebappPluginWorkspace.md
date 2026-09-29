Package [ro.sync.ecss.extensions.api.webapp.access](package-summary.md)

# Interface WebappPluginWorkspace
    All Superinterfaces: [ApplicationInformationAccess](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md), [ColorThemeUtilities](../../../../../exml/workspace/api/util/ColorThemeUtilities.md), [DiffAndMergeTools](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md), [GlobalOptionsStorage](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md), [MathFlowConfigurator](../../../../../exml/workspace/api/math/MathFlowConfigurator.md), [PluginWorkspace](../../../../../exml/workspace/api/PluginWorkspace.md), [ReferencesCustomizer](../../../../../exml/workspace/api/standalone/ReferencesCustomizer.md), [StandalonePluginWorkspace](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md), [Workspace](../../../../../exml/workspace/api/Workspace.md), [WorkspaceUtilities](../../../../../exml/workspace/api/WorkspaceUtilities.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WebappPluginWorkspaceextends [StandalonePluginWorkspace](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md)
Plugin workspace access API with webapp-specific features. To obtain an instance of this class, one can either register a [WorkspaceAccessPluginExtension](../../../../../exml/plugin/workspace/WorkspaceAccessPluginExtension.md) or use [PluginWorkspaceProvider](../../../../../exml/workspace/api/PluginWorkspaceProvider.md).
  Since: 17
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OXYGEN_WEBAPP_DATA_DIR](#OXYGEN_WEBAPP_DATA_DIR)
Servlet context attribute used to retrieve the data directory.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [restApiVersion](#restApiVersion)
The web-app REST api version

### Fields inherited from interface ro.sync.exml.workspace.api.[PluginWorkspace](../../../../../exml/workspace/api/PluginWorkspace.md)
 [DITA_MAPS_EDITING_AREA](../../../../../exml/workspace/api/PluginWorkspace.md#DITA_MAPS_EDITING_AREA), [MAIN_EDITING_AREA](../../../../../exml/workspace/api/PluginWorkspace.md#MAIN_EDITING_AREA)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addDITAMapEditingSessionLifecycleListener](#addDITAMapEditingSessionLifecycleListener(ro.sync.ecss.extensions.api.webapp.access.WebappEditingSessionLifecycleListener))([WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md) listener)
Registers a listener for the lifecycle events of the editing sessions for an editable DITA Map opened in the DITA Maps Manager component.
  void [addEditingSessionLifecycleListener](#addEditingSessionLifecycleListener(ro.sync.ecss.extensions.api.webapp.access.WebappEditingSessionLifecycleListener))([WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md) listener)
Registers a listener for the lifecycle events of the editing sessions.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md)> [getAllDITAMapEditingSessionLifecycleListeners](#getAllDITAMapEditingSessionLifecycleListeners())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md)> [getAllEditingSessionLifecycleListeners](#getAllEditingSessionLifecycleListeners())()

 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getMonitoringStats](#getMonitoringStats())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<javax.servlet.Filter> [getServletFilters](#getServletFilters())()

 [SessionStore](../SessionStore.md) [getSessionStore](#getSessionStore())()
A store which can remember key, values on a given session.
  void [removeDITAMapEditingSessionLifecycleListener](#removeDITAMapEditingSessionLifecycleListener(ro.sync.ecss.extensions.api.webapp.access.WebappEditingSessionLifecycleListener))([WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md) listener)
Removes the listener for an editable DITA Map's editing session for an editable DITA Map opened in the DITA Maps Manager component.
  void [removeEditingSessionLifecycleListener](#removeEditingSessionLifecycleListener(ro.sync.ecss.extensions.api.webapp.access.WebappEditingSessionLifecycleListener))([WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md) listener)
Removes the listener.
  void [setDITAKeyDefinitionManagerProvider](#setDITAKeyDefinitionManagerProvider(ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionManagerProvider))([KeyDefinitionManagerProvider](../../../../../exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManagerProvider.md) keyDefinitionManagerProvider)
Sets an object that provides a DITA keys manager for each opened document.

### Methods inherited from interface ro.sync.exml.workspace.api.application.[ApplicationInformationAccess](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md)
 [getApplicationName](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getApplicationName()), [getApplicationType](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getApplicationType()), [getLicenseInformationProvider](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getLicenseInformationProvider()), [getPlatform](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()), [getPreferencesDirectory](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPreferencesDirectory()), [getUserInterfaceLanguage](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getUserInterfaceLanguage()), [getVersion](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getVersion()), [getVersionBuildID](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getVersionBuildID())
### Methods inherited from interface ro.sync.exml.workspace.api.util.[ColorThemeUtilities](../../../../../exml/workspace/api/util/ColorThemeUtilities.md)
 [getColorTheme](../../../../../exml/workspace/api/util/ColorThemeUtilities.md#getColorTheme()), [getImageInverter](../../../../../exml/workspace/api/util/ColorThemeUtilities.md#getImageInverter())
### Methods inherited from interface ro.sync.exml.workspace.api.standalone.[DiffAndMergeTools](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md)
 [openDiffFilesApplication](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md#openDiffFilesApplication(java.lang.String,java.net.URL,java.lang.String,java.net.URL)), [openDiffFilesApplication](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md#openDiffFilesApplication(java.lang.String,java.net.URL,java.lang.String,java.net.URL,java.net.URL,boolean)), [openDiffFilesApplication](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md#openDiffFilesApplication(java.net.URL,java.net.URL)), [openDiffFilesApplication](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md#openDiffFilesApplication(java.net.URL,java.net.URL,java.net.URL)), [openMergeApplication](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md#openMergeApplication(java.io.File,java.io.File,java.io.File,java.util.Map)), [openMergeApplication](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md#openMergeApplication(java.lang.String,java.lang.String,boolean,java.lang.String,java.net.URL,boolean,boolean,java.lang.String,java.net.URL,boolean,boolean,java.net.URL)), [openPreviewDialog](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md#openPreviewDialog(java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.util.LinkedHashMap)), [openPreviewDialog](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md#openPreviewDialog(java.lang.String,java.lang.String,java.util.LinkedHashMap))
### Methods inherited from interface ro.sync.exml.workspace.api.options.[GlobalOptionsStorage](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md)
 [addGlobalOptionListener](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md#addGlobalOptionListener(ro.sync.ecss.extensions.api.OptionListener)), [deserializePersistentObject](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md#deserializePersistentObject(java.lang.String)), [getGlobalObjectProperty](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md#getGlobalObjectProperty(java.lang.String)), [importGlobalOptions](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md#importGlobalOptions(java.io.File)), [importGlobalOptions](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md#importGlobalOptions(java.io.File,boolean)), [removeGlobalOptionListener](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md#removeGlobalOptionListener(ro.sync.ecss.extensions.api.OptionListener)), [saveGlobalOptions](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md#saveGlobalOptions()), [serializePersistentObject](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md#serializePersistentObject(java.lang.Object)), [setGlobalObjectProperty](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md#setGlobalObjectProperty(java.lang.String,java.lang.Object)), [showPreferencesPages](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md#showPreferencesPages(java.lang.String%5B%5D,java.lang.String,boolean))
### Methods inherited from interface ro.sync.exml.workspace.api.math.[MathFlowConfigurator](../../../../../exml/workspace/api/math/MathFlowConfigurator.md)
 [setMathFlowFixedLicenseFile](../../../../../exml/workspace/api/math/MathFlowConfigurator.md#setMathFlowFixedLicenseFile(java.io.File)), [setMathFlowFixedLicenseKeyForComposer](../../../../../exml/workspace/api/math/MathFlowConfigurator.md#setMathFlowFixedLicenseKeyForComposer(java.lang.String)), [setMathFlowFixedLicenseKeyForEditor](../../../../../exml/workspace/api/math/MathFlowConfigurator.md#setMathFlowFixedLicenseKeyForEditor(java.lang.String)), [setMathFlowInstallationFolder](../../../../../exml/workspace/api/math/MathFlowConfigurator.md#setMathFlowInstallationFolder(java.io.File))
### Methods inherited from interface ro.sync.exml.workspace.api.[PluginWorkspace](../../../../../exml/workspace/api/PluginWorkspace.md)
 [addAuthorCSSAlternativesCustomizer](../../../../../exml/workspace/api/PluginWorkspace.md#addAuthorCSSAlternativesCustomizer(ro.sync.exml.workspace.api.editor.page.author.css.AuthorCSSAlternativesCustomizer)), [addBatchOperationsListener](../../../../../exml/workspace/api/PluginWorkspace.md#addBatchOperationsListener(ro.sync.exml.workspace.api.listeners.BatchOperationsListener)), [addEditorChangeListener](../../../../../exml/workspace/api/PluginWorkspace.md#addEditorChangeListener(ro.sync.exml.workspace.api.listeners.WSEditorChangeListener,int)), [createAuthorDocumentProvider](../../../../../exml/workspace/api/PluginWorkspace.md#createAuthorDocumentProvider(java.net.URL,java.io.Reader)), [createAuthorDocumentProvider](../../../../../exml/workspace/api/PluginWorkspace.md#createAuthorDocumentProvider(java.net.URL,java.io.Reader,boolean)), [getAllEditorLocations](../../../../../exml/workspace/api/PluginWorkspace.md#getAllEditorLocations(int)), [getBatchOperationsListenersAccess](../../../../../exml/workspace/api/PluginWorkspace.md#getBatchOperationsListenersAccess()), [getCompareUtilAccess](../../../../../exml/workspace/api/PluginWorkspace.md#getCompareUtilAccess()), [getComponentsProvider](../../../../../exml/workspace/api/PluginWorkspace.md#getComponentsProvider()), [getCurrentEditorAccess](../../../../../exml/workspace/api/PluginWorkspace.md#getCurrentEditorAccess(int)), [getEditorAccess](../../../../../exml/workspace/api/PluginWorkspace.md#getEditorAccess(java.net.URL,int)), [getEditorChangeListeners](../../../../../exml/workspace/api/PluginWorkspace.md#getEditorChangeListeners(int)), [getOptionsStorage](../../../../../exml/workspace/api/PluginWorkspace.md#getOptionsStorage()), [getResultsManager](../../../../../exml/workspace/api/PluginWorkspace.md#getResultsManager()), [getUtilAccess](../../../../../exml/workspace/api/PluginWorkspace.md#getUtilAccess()), [getValidationUtilAccess](../../../../../exml/workspace/api/PluginWorkspace.md#getValidationUtilAccess()), [getXMLRefactorUtilAccess](../../../../../exml/workspace/api/PluginWorkspace.md#getXMLRefactorUtilAccess()), [getXMLUtilAccess](../../../../../exml/workspace/api/PluginWorkspace.md#getXMLUtilAccess()), [removeAuthorCSSAlternativesCustomizer](../../../../../exml/workspace/api/PluginWorkspace.md#removeAuthorCSSAlternativesCustomizer(ro.sync.exml.workspace.api.editor.page.author.css.AuthorCSSAlternativesCustomizer)), [removeBatchOperationsListener](../../../../../exml/workspace/api/PluginWorkspace.md#removeBatchOperationsListener(ro.sync.exml.workspace.api.listeners.BatchOperationsListener)), [removeEditorChangeListener](../../../../../exml/workspace/api/PluginWorkspace.md#removeEditorChangeListener(ro.sync.exml.workspace.api.listeners.WSEditorChangeListener,int)), [setDITAKeyDefinitionManager](../../../../../exml/workspace/api/PluginWorkspace.md#setDITAKeyDefinitionManager(ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionManager))
### Methods inherited from interface ro.sync.exml.workspace.api.standalone.[ReferencesCustomizer](../../../../../exml/workspace/api/standalone/ReferencesCustomizer.md)
 [addInputURLChooserCustomizer](../../../../../exml/workspace/api/standalone/ReferencesCustomizer.md#addInputURLChooserCustomizer(ro.sync.exml.workspace.api.standalone.InputURLChooserCustomizer)), [addRelativeReferencesResolver](../../../../../exml/workspace/api/standalone/ReferencesCustomizer.md#addRelativeReferencesResolver(java.lang.String,ro.sync.exml.workspace.api.util.RelativeReferenceResolver))
### Methods inherited from interface ro.sync.exml.workspace.api.standalone.[StandalonePluginWorkspace](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md)
 [addMenuBarCustomizer](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#addMenuBarCustomizer(ro.sync.exml.workspace.api.standalone.MenuBarCustomizer)), [addMenusAndToolbarsContributorCustomizer](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#addMenusAndToolbarsContributorCustomizer(ro.sync.exml.workspace.api.standalone.actions.MenusAndToolbarsContributorCustomizer)), [addPluginExtension](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#addPluginExtension(java.lang.String,ro.sync.exml.plugin.PluginExtension)), [addToolbarComponentsCustomizer](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#addToolbarComponentsCustomizer(ro.sync.exml.workspace.api.standalone.ToolbarComponentsCustomizer)), [addTopicRefTargetInfoProvider](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#addTopicRefTargetInfoProvider(java.lang.String,ro.sync.exml.workspace.api.standalone.ditamap.TopicRefTargetInfoProvider)), [addViewComponentCustomizer](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#addViewComponentCustomizer(ro.sync.exml.workspace.api.standalone.ViewComponentCustomizer)), [createAuthorPreviewComponentProvider](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#createAuthorPreviewComponentProvider()), [createEditorComponentProvider](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#createEditorComponentProvider(java.lang.String%5B%5D,java.lang.String)), [createEditorComponentProvider](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#createEditorComponentProvider(java.lang.String%5B%5D,java.lang.String,java.lang.String)), [getActionsProvider](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#getActionsProvider()), [getOxygenActionID](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#getOxygenActionID(javax.swing.Action)), [getProjectManager](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#getProjectManager()), [getProxyDetailsProvider](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#getProxyDetailsProvider()), [getResourceBundle](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#getResourceBundle()), [hideToolbar](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#hideToolbar(java.lang.String)), [hideView](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#hideView(java.lang.String)), [isToolbarShowing](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#isToolbarShowing(java.lang.String)), [isViewAvailable](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#isViewAvailable(java.lang.String)), [isViewShowing](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#isViewShowing(java.lang.String)), [removeMenusAndToolbarsContributorCustomizer](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#removeMenusAndToolbarsContributorCustomizer(ro.sync.exml.workspace.api.standalone.actions.MenusAndToolbarsContributorCustomizer)), [showToolbar](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#showToolbar(java.lang.String)), [showView](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md#showView(java.lang.String,boolean))
### Methods inherited from interface ro.sync.exml.workspace.api.[Workspace](../../../../../exml/workspace/api/Workspace.md)
 [close](../../../../../exml/workspace/api/Workspace.md#close(java.net.URL)), [closeAll](../../../../../exml/workspace/api/Workspace.md#closeAll()), [createNewEditor](../../../../../exml/workspace/api/Workspace.md#createNewEditor(java.lang.String,java.lang.String,java.lang.String)), [createNewEditor](../../../../../exml/workspace/api/Workspace.md#createNewEditor(java.net.URL,java.lang.String,java.lang.String,java.lang.String)), [delete](../../../../../exml/workspace/api/Workspace.md#delete(java.net.URL)), [isStandalone](../../../../../exml/workspace/api/Workspace.md#isStandalone()), [open](../../../../../exml/workspace/api/Workspace.md#open(java.net.URL)), [open](../../../../../exml/workspace/api/Workspace.md#open(java.net.URL,java.lang.String)), [open](../../../../../exml/workspace/api/Workspace.md#open(java.net.URL,java.lang.String,java.lang.String)), [refreshInProject](../../../../../exml/workspace/api/Workspace.md#refreshInProject(java.net.URL)), [saveAll](../../../../../exml/workspace/api/Workspace.md#saveAll()), [setParentFrameTitle](../../../../../exml/workspace/api/Workspace.md#setParentFrameTitle(java.lang.String))
### Methods inherited from interface ro.sync.exml.workspace.api.[WorkspaceUtilities](../../../../../exml/workspace/api/WorkspaceUtilities.md)
 [chooseDirectory](../../../../../exml/workspace/api/WorkspaceUtilities.md#chooseDirectory()), [chooseDirectory](../../../../../exml/workspace/api/WorkspaceUtilities.md#chooseDirectory(java.io.File)), [chooseFile](../../../../../exml/workspace/api/WorkspaceUtilities.md#chooseFile(java.io.File,java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)), [chooseFile](../../../../../exml/workspace/api/WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseFile](../../../../../exml/workspace/api/WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)), [chooseFiles](../../../../../exml/workspace/api/WorkspaceUtilities.md#chooseFiles(java.io.File,java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURL](../../../../../exml/workspace/api/WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURL](../../../../../exml/workspace/api/WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String)), [chooseURL](../../../../../exml/workspace/api/WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String,java.lang.String,java.lang.String)), [chooseURLPath](../../../../../exml/workspace/api/WorkspaceUtilities.md#chooseURLPath(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURLPath](../../../../../exml/workspace/api/WorkspaceUtilities.md#chooseURLPath(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String)), [clearImageCache](../../../../../exml/workspace/api/WorkspaceUtilities.md#clearImageCache()), [createJavaProcess](../../../../../exml/workspace/api/WorkspaceUtilities.md#createJavaProcess(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String,java.util.Map,java.io.File,ro.sync.exml.workspace.api.process.ProcessListener)), [createProcess](../../../../../exml/workspace/api/WorkspaceUtilities.md#createProcess(ro.sync.exml.workspace.api.process.ProcessListener,java.lang.String,java.io.File,java.lang.String,boolean)), [getDataSourceAccess](../../../../../exml/workspace/api/WorkspaceUtilities.md#getDataSourceAccess()), [getImageUtilities](../../../../../exml/workspace/api/WorkspaceUtilities.md#getImageUtilities()), [getParentFrame](../../../../../exml/workspace/api/WorkspaceUtilities.md#getParentFrame()), [getTemplateManager](../../../../../exml/workspace/api/WorkspaceUtilities.md#getTemplateManager()), [openInExternalApplication](../../../../../exml/workspace/api/WorkspaceUtilities.md#openInExternalApplication(java.lang.String,boolean,java.lang.String)), [openInExternalApplication](../../../../../exml/workspace/api/WorkspaceUtilities.md#openInExternalApplication(java.net.URL,boolean)), [openInExternalApplication](../../../../../exml/workspace/api/WorkspaceUtilities.md#openInExternalApplication(java.net.URL,boolean,java.lang.String)), [showConfirmDialog](../../../../../exml/workspace/api/WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)), [showConfirmDialog](../../../../../exml/workspace/api/WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D,int)), [showErrorMessage](../../../../../exml/workspace/api/WorkspaceUtilities.md#showErrorMessage(java.lang.String)), [showErrorMessage](../../../../../exml/workspace/api/WorkspaceUtilities.md#showErrorMessage(java.lang.String,java.lang.Throwable)), [showInformationMessage](../../../../../exml/workspace/api/WorkspaceUtilities.md#showInformationMessage(java.lang.String)), [showStatusMessage](../../../../../exml/workspace/api/WorkspaceUtilities.md#showStatusMessage(java.lang.String)), [showStatusMessage](../../../../../exml/workspace/api/WorkspaceUtilities.md#showStatusMessage(java.lang.String,ro.sync.exml.workspace.api.OperationStatus)), [showWarningDialog](../../../../../exml/workspace/api/WorkspaceUtilities.md#showWarningDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)), [showWarningDialog](../../../../../exml/workspace/api/WorkspaceUtilities.md#showWarningDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D,int)), [showWarningMessage](../../../../../exml/workspace/api/WorkspaceUtilities.md#showWarningMessage(java.lang.String)), [startProcess](../../../../../exml/workspace/api/WorkspaceUtilities.md#startProcess(java.lang.String,java.io.File,java.lang.String,boolean))
## Field Details

### restApiVersion

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) restApiVersion

The web-app REST api version
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.access.WebappPluginWorkspace.restApiVersion)

### OXYGEN_WEBAPP_DATA_DIR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OXYGEN_WEBAPP_DATA_DIR

Servlet context attribute used to retrieve the data directory. This directory contains:
        * frameworks
        * plugins
        * configuration files

  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.access.WebappPluginWorkspace.OXYGEN_WEBAPP_DATA_DIR)

## Method Details

### addEditingSessionLifecycleListener

void addEditingSessionLifecycleListener([WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md) listener)

Registers a listener for the lifecycle events of the editing sessions.
  Parameters: listener - The listener to be added.
### addDITAMapEditingSessionLifecycleListener

void addDITAMapEditingSessionLifecycleListener([WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md) listener)

Registers a listener for the lifecycle events of the editing sessions for an editable DITA Map opened in the DITA Maps Manager component.
  Parameters: listener - The listener to be added. Since: 26.1
### removeEditingSessionLifecycleListener

void removeEditingSessionLifecycleListener([WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md) listener)

Removes the listener.
  Parameters: listener - The listener to be removed.
### removeDITAMapEditingSessionLifecycleListener

void removeDITAMapEditingSessionLifecycleListener([WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md) listener)

Removes the listener for an editable DITA Map's editing session for an editable DITA Map opened in the DITA Maps Manager component.
  Parameters: listener - The listener to be removed. Since: 26.1
### getAllEditingSessionLifecycleListeners

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md)> getAllEditingSessionLifecycleListeners()
  Returns: Returns all the listeners for lifecycle events of the editing sessions.
### getAllDITAMapEditingSessionLifecycleListeners

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md)> getAllDITAMapEditingSessionLifecycleListeners()
  Returns: Returns all the listeners for lifecycle events of editable DITA Maps opened in the DITA Maps Manager component. Since: 26.1
### getServletFilters

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<javax.servlet.Filter> getServletFilters()
  Returns: The list of Servlet filters registered by plugins.
### getMonitoringStats

[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getMonitoringStats()
  Returns: A map with statistics that can be used for monitoring. Since: 19.1
### setDITAKeyDefinitionManagerProvider

void setDITAKeyDefinitionManagerProvider([KeyDefinitionManagerProvider](../../../../../exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManagerProvider.md) keyDefinitionManagerProvider)

Sets an object that provides a DITA keys manager for each opened document.
  Parameters: keyDefinitionManagerProvider - The provider of the keys manager for opened documents. Since: 19.1
### getSessionStore

[SessionStore](../SessionStore.md) getSessionStore()

A store which can remember key, values on a given session. The values expire automatically when the session expires.
  Returns: A store which can remember key, values on a given session. The values expire automatically when the session expires. Since: 20.0
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
