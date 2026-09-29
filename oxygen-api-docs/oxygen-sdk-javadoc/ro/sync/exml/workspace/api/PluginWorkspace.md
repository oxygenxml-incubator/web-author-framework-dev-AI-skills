Package [ro.sync.exml.workspace.api](package-summary.md)

# Interface PluginWorkspace
    All Superinterfaces: [ApplicationInformationAccess](application/ApplicationInformationAccess.md), [ColorThemeUtilities](util/ColorThemeUtilities.md), [GlobalOptionsStorage](options/GlobalOptionsStorage.md), [ReferencesCustomizer](standalone/ReferencesCustomizer.md), [Workspace](Workspace.md), [WorkspaceUtilities](WorkspaceUtilities.md)   All Known Subinterfaces: [EclipsePluginWorkspace](../../../../../com/oxygenxml/workspace/api/eclipse/EclipsePluginWorkspace.md), [StandalonePluginWorkspace](standalone/StandalonePluginWorkspace.md), [WebappPluginWorkspace](../../../ecss/extensions/api/webapp/access/WebappPluginWorkspace.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface PluginWorkspaceextends [Workspace](Workspace.md), [ReferencesCustomizer](standalone/ReferencesCustomizer.md), [GlobalOptionsStorage](options/GlobalOptionsStorage.md)
Access the entire workspace of Oxygen.
  Since: 11.2
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [DITA_MAPS_EDITING_AREA](#DITA_MAPS_EDITING_AREA)
The DITA Maps editing area
  static final int [MAIN_EDITING_AREA](#MAIN_EDITING_AREA)
The main editing area in Oxygen

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addAuthorCSSAlternativesCustomizer](#addAuthorCSSAlternativesCustomizer(ro.sync.exml.workspace.api.editor.page.author.css.AuthorCSSAlternativesCustomizer))([AuthorCSSAlternativesCustomizer](editor/page/author/css/AuthorCSSAlternativesCustomizer.md) cssAlternativesCustomizer)
Add a customizer for the CSS alternatives which the user can choose in the Styles drop-down button when working in the Author visual editing mode.
  void [addBatchOperationsListener](#addBatchOperationsListener(ro.sync.exml.workspace.api.listeners.BatchOperationsListener))([BatchOperationsListener](listeners/BatchOperationsListener.md) listener)
Add a batch operations listener, listener notified before and after large modification operations start in Oxygen, for example when the Replace All in Files is started.
  void [addEditorChangeListener](#addEditorChangeListener(ro.sync.exml.workspace.api.listeners.WSEditorChangeListener,int))([WSEditorChangeListener](listeners/WSEditorChangeListener.md) editorListener, int editingArea)
Add listener for editor related events(for example editor opened, closed, page changed).
  [AuthorDocumentProvider](../../../ecss/extensions/api/node/AuthorDocumentProvider.md) [createAuthorDocumentProvider](#createAuthorDocumentProvider(java.net.URL,java.io.Reader))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemId, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) documentReader)
Creates a provider for a given resource specified by URL and/or Reader.
  [AuthorDocumentProvider](../../../ecss/extensions/api/node/AuthorDocumentProvider.md) [createAuthorDocumentProvider](#createAuthorDocumentProvider(java.net.URL,java.io.Reader,boolean))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemId, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) documentReader, boolean expandReferences)
Creates a provider for a given resource specified by URL and/or Reader.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] [getAllEditorLocations](#getAllEditorLocations(int))(int editingArea)
Get all the editor locations.Based on its settings, the application may choose not to fully load documents in the editor tabs until the user switches to them.
  [BatchOperationsListener](listeners/BatchOperationsListener.md) [getBatchOperationsListenersAccess](#getBatchOperationsListenersAccess())()
Get access to a wrapper which notifies all batch operation listeners registered using the "addBatchOperationsListener" API if a third party plugin intends to make batch changes to a set of resources.
  [CompareUtilAccess](util/CompareUtilAccess.md) [getCompareUtilAccess](#getCompareUtilAccess())()
Access to Comparison utilities.
  [IComponentsProvider](componentscollector/IComponentsProvider.md) [getComponentsProvider](#getComponentsProvider())()
Creates a components provider for editors.
  [WSEditor](editor/WSEditor.md) [getCurrentEditorAccess](#getCurrentEditorAccess(int))(int editingArea)
Get access to the current selected editor.
  [WSEditor](editor/WSEditor.md) [getEditorAccess](#getEditorAccess(java.net.URL,int))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) location, int editingArea)
Find an editor access by location
  [WSEditorChangeListener](listeners/WSEditorChangeListener.md)[] [getEditorChangeListeners](#getEditorChangeListeners(int))(int editingArea)
Return a list with all registered editor changed listeners, never null.
  [WSOptionsStorage](options/WSOptionsStorage.md) [getOptionsStorage](#getOptionsStorage())()
This interface can be used to save and persist in the Oxygen preferences user-defined keys and values.
  [ResultsManager](results/ResultsManager.md) [getResultsManager](#getResultsManager())()
Get the results manager, that can be used to present operation results to the user inside a dedicated view.
  [UtilAccess](util/UtilAccess.md) [getUtilAccess](#getUtilAccess())()
Get access to utility methods.
  [ValidationUtilAccess](util/validation/ValidationUtilAccess.md) [getValidationUtilAccess](#getValidationUtilAccess())()
Get access to validation utilities.
  [XMLRefactorUtilAccess](util/refactor/XMLRefactorUtilAccess.md) [getXMLRefactorUtilAccess](#getXMLRefactorUtilAccess())()
Get access to XML refactoring utilities.
  [XMLUtilAccess](util/XMLUtilAccess.md) [getXMLUtilAccess](#getXMLUtilAccess())()
Access to XML utilities.
  void [removeAuthorCSSAlternativesCustomizer](#removeAuthorCSSAlternativesCustomizer(ro.sync.exml.workspace.api.editor.page.author.css.AuthorCSSAlternativesCustomizer))([AuthorCSSAlternativesCustomizer](editor/page/author/css/AuthorCSSAlternativesCustomizer.md) cssAlternativesCustomizer)
Remove a customizer for the CSS alternatives which the user can choose in the Styles drop-down button when working in the Author visual editing mode.
  void [removeBatchOperationsListener](#removeBatchOperationsListener(ro.sync.exml.workspace.api.listeners.BatchOperationsListener))([BatchOperationsListener](listeners/BatchOperationsListener.md) listener)
Remove a batch operations listener.
  void [removeEditorChangeListener](#removeEditorChangeListener(ro.sync.exml.workspace.api.listeners.WSEditorChangeListener,int))([WSEditorChangeListener](listeners/WSEditorChangeListener.md) editorListener, int editingArea)
Remove listener for editor related events.
  void [setDITAKeyDefinitionManager](#setDITAKeyDefinitionManager(ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionManager))([KeyDefinitionManager](editor/page/ditamap/keys/KeyDefinitionManager.md) keyDefitionManager)
By default key definitions are gathered from DITA Maps opened in the DITA Maps Manager.

### Methods inherited from interface ro.sync.exml.workspace.api.application.[ApplicationInformationAccess](application/ApplicationInformationAccess.md)
 [getApplicationName](application/ApplicationInformationAccess.md#getApplicationName()), [getApplicationType](application/ApplicationInformationAccess.md#getApplicationType()), [getLicenseInformationProvider](application/ApplicationInformationAccess.md#getLicenseInformationProvider()), [getPlatform](application/ApplicationInformationAccess.md#getPlatform()), [getPreferencesDirectory](application/ApplicationInformationAccess.md#getPreferencesDirectory()), [getUserInterfaceLanguage](application/ApplicationInformationAccess.md#getUserInterfaceLanguage()), [getVersion](application/ApplicationInformationAccess.md#getVersion()), [getVersionBuildID](application/ApplicationInformationAccess.md#getVersionBuildID())
### Methods inherited from interface ro.sync.exml.workspace.api.util.[ColorThemeUtilities](util/ColorThemeUtilities.md)
 [getColorTheme](util/ColorThemeUtilities.md#getColorTheme()), [getImageInverter](util/ColorThemeUtilities.md#getImageInverter())
### Methods inherited from interface ro.sync.exml.workspace.api.options.[GlobalOptionsStorage](options/GlobalOptionsStorage.md)
 [addGlobalOptionListener](options/GlobalOptionsStorage.md#addGlobalOptionListener(ro.sync.ecss.extensions.api.OptionListener)), [deserializePersistentObject](options/GlobalOptionsStorage.md#deserializePersistentObject(java.lang.String)), [getGlobalObjectProperty](options/GlobalOptionsStorage.md#getGlobalObjectProperty(java.lang.String)), [importGlobalOptions](options/GlobalOptionsStorage.md#importGlobalOptions(java.io.File)), [importGlobalOptions](options/GlobalOptionsStorage.md#importGlobalOptions(java.io.File,boolean)), [removeGlobalOptionListener](options/GlobalOptionsStorage.md#removeGlobalOptionListener(ro.sync.ecss.extensions.api.OptionListener)), [saveGlobalOptions](options/GlobalOptionsStorage.md#saveGlobalOptions()), [serializePersistentObject](options/GlobalOptionsStorage.md#serializePersistentObject(java.lang.Object)), [setGlobalObjectProperty](options/GlobalOptionsStorage.md#setGlobalObjectProperty(java.lang.String,java.lang.Object)), [showPreferencesPages](options/GlobalOptionsStorage.md#showPreferencesPages(java.lang.String%5B%5D,java.lang.String,boolean))
### Methods inherited from interface ro.sync.exml.workspace.api.standalone.[ReferencesCustomizer](standalone/ReferencesCustomizer.md)
 [addInputURLChooserCustomizer](standalone/ReferencesCustomizer.md#addInputURLChooserCustomizer(ro.sync.exml.workspace.api.standalone.InputURLChooserCustomizer)), [addRelativeReferencesResolver](standalone/ReferencesCustomizer.md#addRelativeReferencesResolver(java.lang.String,ro.sync.exml.workspace.api.util.RelativeReferenceResolver))
### Methods inherited from interface ro.sync.exml.workspace.api.[Workspace](Workspace.md)
 [close](Workspace.md#close(java.net.URL)), [closeAll](Workspace.md#closeAll()), [createNewEditor](Workspace.md#createNewEditor(java.lang.String,java.lang.String,java.lang.String)), [createNewEditor](Workspace.md#createNewEditor(java.net.URL,java.lang.String,java.lang.String,java.lang.String)), [delete](Workspace.md#delete(java.net.URL)), [isStandalone](Workspace.md#isStandalone()), [open](Workspace.md#open(java.net.URL)), [open](Workspace.md#open(java.net.URL,java.lang.String)), [open](Workspace.md#open(java.net.URL,java.lang.String,java.lang.String)), [refreshInProject](Workspace.md#refreshInProject(java.net.URL)), [saveAll](Workspace.md#saveAll()), [setParentFrameTitle](Workspace.md#setParentFrameTitle(java.lang.String))
### Methods inherited from interface ro.sync.exml.workspace.api.[WorkspaceUtilities](WorkspaceUtilities.md)
 [chooseDirectory](WorkspaceUtilities.md#chooseDirectory()), [chooseDirectory](WorkspaceUtilities.md#chooseDirectory(java.io.File)), [chooseFile](WorkspaceUtilities.md#chooseFile(java.io.File,java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)), [chooseFile](WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseFile](WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)), [chooseFiles](WorkspaceUtilities.md#chooseFiles(java.io.File,java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURL](WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURL](WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String)), [chooseURL](WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String,java.lang.String,java.lang.String)), [chooseURLPath](WorkspaceUtilities.md#chooseURLPath(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURLPath](WorkspaceUtilities.md#chooseURLPath(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String)), [clearImageCache](WorkspaceUtilities.md#clearImageCache()), [createJavaProcess](WorkspaceUtilities.md#createJavaProcess(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String,java.util.Map,java.io.File,ro.sync.exml.workspace.api.process.ProcessListener)), [createProcess](WorkspaceUtilities.md#createProcess(ro.sync.exml.workspace.api.process.ProcessListener,java.lang.String,java.io.File,java.lang.String,boolean)), [getDataSourceAccess](WorkspaceUtilities.md#getDataSourceAccess()), [getImageUtilities](WorkspaceUtilities.md#getImageUtilities()), [getParentFrame](WorkspaceUtilities.md#getParentFrame()), [getTemplateManager](WorkspaceUtilities.md#getTemplateManager()), [openInExternalApplication](WorkspaceUtilities.md#openInExternalApplication(java.lang.String,boolean,java.lang.String)), [openInExternalApplication](WorkspaceUtilities.md#openInExternalApplication(java.net.URL,boolean)), [openInExternalApplication](WorkspaceUtilities.md#openInExternalApplication(java.net.URL,boolean,java.lang.String)), [showConfirmDialog](WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)), [showConfirmDialog](WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D,int)), [showErrorMessage](WorkspaceUtilities.md#showErrorMessage(java.lang.String)), [showErrorMessage](WorkspaceUtilities.md#showErrorMessage(java.lang.String,java.lang.Throwable)), [showInformationMessage](WorkspaceUtilities.md#showInformationMessage(java.lang.String)), [showStatusMessage](WorkspaceUtilities.md#showStatusMessage(java.lang.String)), [showStatusMessage](WorkspaceUtilities.md#showStatusMessage(java.lang.String,ro.sync.exml.workspace.api.OperationStatus)), [showWarningDialog](WorkspaceUtilities.md#showWarningDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)), [showWarningDialog](WorkspaceUtilities.md#showWarningDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D,int)), [showWarningMessage](WorkspaceUtilities.md#showWarningMessage(java.lang.String)), [startProcess](WorkspaceUtilities.md#startProcess(java.lang.String,java.io.File,java.lang.String,boolean))
## Field Details

### MAIN_EDITING_AREA

static final int MAIN_EDITING_AREA

The main editing area in Oxygen
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.workspace.api.PluginWorkspace.MAIN_EDITING_AREA)

### DITA_MAPS_EDITING_AREA

static final int DITA_MAPS_EDITING_AREA

The DITA Maps editing area
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.workspace.api.PluginWorkspace.DITA_MAPS_EDITING_AREA)

## Method Details

### getAllEditorLocations

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] getAllEditorLocations(int editingArea)

Get all the editor locations.Based on its settings, the application may choose not to fully load documents in the editor tabs until the user switches to them. In such cases the URLs for these not yet instantiated editors are not returned by this method.
  Parameters: editingArea - One of the constants in this class:  [MAIN_EDITING_AREA](#MAIN_EDITING_AREA) - for the editors in the main Oxygen workspace area.  [DITA_MAPS_EDITING_AREA](#DITA_MAPS_EDITING_AREA) - for the editors in the DITA Maps Manager view workspace area.  Returns: All the editor locations or empty array if no editor is opened
### getEditorAccess

[WSEditor](editor/WSEditor.md) getEditorAccess([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) location, int editingArea)

Find an editor access by location
  Parameters: location - The editor location editingArea - One of the constants in this class:  [MAIN_EDITING_AREA](#MAIN_EDITING_AREA) - for the editors in the main Oxygen workspace area.  [DITA_MAPS_EDITING_AREA](#DITA_MAPS_EDITING_AREA) - for the editors in the DITA Maps Manager view workspace area.  Returns: access to the found editor or null if no editor found with that location URL.
### getCurrentEditorAccess

[WSEditor](editor/WSEditor.md) getCurrentEditorAccess(int editingArea)

Get access to the current selected editor.
  Parameters: editingArea - One of the constants in this class:  [MAIN_EDITING_AREA](#MAIN_EDITING_AREA) - for the editors in the main Oxygen workspace area.  [DITA_MAPS_EDITING_AREA](#DITA_MAPS_EDITING_AREA) - for the editors in the DITA Maps Manager view workspace area.  Returns: access to the current editor or null if no editor is opened.
### getXMLUtilAccess

[XMLUtilAccess](util/XMLUtilAccess.md) getXMLUtilAccess()

Access to XML utilities.
  Returns: Access to XML utilities.
### getCompareUtilAccess

[CompareUtilAccess](util/CompareUtilAccess.md) getCompareUtilAccess()

Access to Comparison utilities.
  Returns: Access to comparison utilities. Since: 19.1
### getUtilAccess

[UtilAccess](util/UtilAccess.md) getUtilAccess()

Get access to utility methods.
  Returns: access to utility methods.
### getValidationUtilAccess

[ValidationUtilAccess](util/validation/ValidationUtilAccess.md) getValidationUtilAccess()

Get access to validation utilities.
  Returns: access to validation utility methods. Since: 25
### getXMLRefactorUtilAccess

[XMLRefactorUtilAccess](util/refactor/XMLRefactorUtilAccess.md) getXMLRefactorUtilAccess()

Get access to XML refactoring utilities.
  Returns: access to xml refactoring utilities. Since: 28  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

### getResultsManager

[ResultsManager](results/ResultsManager.md) getResultsManager()

Get the results manager, that can be used to present operation results to the user inside a dedicated view.
  Returns: the results manager. Since: 19.0
### addEditorChangeListener

void addEditorChangeListener([WSEditorChangeListener](listeners/WSEditorChangeListener.md) editorListener, int editingArea)

Add listener for editor related events(for example editor opened, closed, page changed).
  Parameters: editorListener - The listener notified when an editor is added, removed or the editor page is changed. editingArea - One of the constants in this class:  [MAIN_EDITING_AREA](#MAIN_EDITING_AREA) - for the editors in the main Oxygen workspace area.  [DITA_MAPS_EDITING_AREA](#DITA_MAPS_EDITING_AREA) - for the editors in the DITA Maps Manager view workspace area.
### removeEditorChangeListener

void removeEditorChangeListener([WSEditorChangeListener](listeners/WSEditorChangeListener.md) editorListener, int editingArea)

Remove listener for editor related events.
  Parameters: editingArea - One of the constants in this class:  [MAIN_EDITING_AREA](#MAIN_EDITING_AREA) - for the editors in the main Oxygen workspace area.  [DITA_MAPS_EDITING_AREA](#DITA_MAPS_EDITING_AREA) - for the editors in the DITA Maps Manager view workspace area.  editorListener - The listener notified when an editor is added, removed or the editor page is changed.
### getEditorChangeListeners

[WSEditorChangeListener](listeners/WSEditorChangeListener.md)[] getEditorChangeListeners(int editingArea)

Return a list with all registered editor changed listeners, never null.
  Parameters: editingArea - One of the constants in this class:  [MAIN_EDITING_AREA](#MAIN_EDITING_AREA) - for the editors in the main Oxygen workspace area.  [DITA_MAPS_EDITING_AREA](#DITA_MAPS_EDITING_AREA) - for the editors in the DITA Maps Manager view workspace area. Returns: a list with all registered editor changed listeners, never null. Since: 16
### getOptionsStorage

[WSOptionsStorage](options/WSOptionsStorage.md) getOptionsStorage()

This interface can be used to save and persist in the Oxygen preferences user-defined keys and values. It is also responsible for adding and removing listeners that are notified about the option changes. These keys are common to all plugin implementations.
  Returns: The object that manages the custom user options stored in the Oxygen preferences from the plugin implementations. Since: 12.1
### setDITAKeyDefinitionManager

void setDITAKeyDefinitionManager([KeyDefinitionManager](editor/page/ditamap/keys/KeyDefinitionManager.md) keyDefitionManager)

By default key definitions are gathered from DITA Maps opened in the DITA Maps Manager. This API can be used by the developer to take control over the key definitions which will be used to resolve keyrefs and conkeyrefs for topics opened in the Author page.
  Parameters: keyDefitionManager - The key definition manager Since: 14
### addAuthorCSSAlternativesCustomizer

void addAuthorCSSAlternativesCustomizer([AuthorCSSAlternativesCustomizer](editor/page/author/css/AuthorCSSAlternativesCustomizer.md) cssAlternativesCustomizer)

Add a customizer for the CSS alternatives which the user can choose in the Styles drop-down button when working in the Author visual editing mode.
  Parameters: cssAlternativesCustomizer - The CSS alternatives customizer. Since: 17
### removeAuthorCSSAlternativesCustomizer

void removeAuthorCSSAlternativesCustomizer([AuthorCSSAlternativesCustomizer](editor/page/author/css/AuthorCSSAlternativesCustomizer.md) cssAlternativesCustomizer)

Remove a customizer for the CSS alternatives which the user can choose in the Styles drop-down button when working in the Author visual editing mode.
  Parameters: cssAlternativesCustomizer - The CSS alternatives customizer. Since: 17
### addBatchOperationsListener

void addBatchOperationsListener([BatchOperationsListener](listeners/BatchOperationsListener.md) listener)

Add a batch operations listener, listener notified before and after large modification operations start in Oxygen, for example when the Replace All in Files is started. The listener is only called with REPLACE_ALL events for the standalone version of Oxygen.
  Parameters: listener - The batch operations listener. Since: 18.1
### removeBatchOperationsListener

void removeBatchOperationsListener([BatchOperationsListener](listeners/BatchOperationsListener.md) listener)

Remove a batch operations listener.
  Parameters: listener - The batch operations listener. Since: 18.1
### getBatchOperationsListenersAccess

[BatchOperationsListener](listeners/BatchOperationsListener.md) getBatchOperationsListenersAccess()

Get access to a wrapper which notifies all batch operation listeners registered using the "addBatchOperationsListener" API if a third party plugin intends to make batch changes to a set of resources.
  Returns: A BatchOperationsListener wrapper which notifies all BatchOperationsListener listeners added by other plugins using the "addBatchOperationsListener" API method Since: 26.1
### createAuthorDocumentProvider

[AuthorDocumentProvider](../../../ecss/extensions/api/node/AuthorDocumentProvider.md) createAuthorDocumentProvider([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemId, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) documentReader)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Creates a provider for a given resource specified by URL and/or Reader. References are not expanded. The provider creates a structure of AuthorNodes and allows it to be manipulated via an [AuthorDocumentController](../../../ecss/extensions/api/AuthorDocumentController.md). Such an API may be useful if you want to load XML content and use Author API to make changes to it. Afterwards you can serialize the structure back to XML. The parsing of the XML content to Author Nodes is quite fast and may also be used to batch change sets of XML resources by using the [AuthorDocumentController](../../../ecss/extensions/api/AuthorDocumentController.md) API.
  Parameters: systemId - The system id of the resource. If null, the reader must be provided and relative DTD entity references will not be properly resolved. documentReader - The document reader. If null, the reader will be created internally. Returns: The provider which gives access to the non-visual [AuthorDocumentController](../../../ecss/extensions/api/AuthorDocumentController.md) representation of the resource. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If any exception occurs during the loading, for example IO exception due to incorrect system id, unsupported encodings, files saving permission, etc Since: 22.1
### createAuthorDocumentProvider

[AuthorDocumentProvider](../../../ecss/extensions/api/node/AuthorDocumentProvider.md) createAuthorDocumentProvider([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemId, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) documentReader, boolean expandReferences)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Creates a provider for a given resource specified by URL and/or Reader. The provider creates a structure of AuthorNodes and allows it to be manipulated via an [AuthorDocumentController](../../../ecss/extensions/api/AuthorDocumentController.md). Such an API may be useful if you want to load XML content and use Author API to make changes to it. Afterwards you can serialize the structure back to XML. The parsing of the XML content to Author Nodes is quite fast and may also be used to batch change sets of XML resources by using the [AuthorDocumentController](../../../ecss/extensions/api/AuthorDocumentController.md) API.
  Parameters: systemId - The system id of the resource. If null, the reader must be provided and relative DTD entity references will not be properly resolved. documentReader - The document reader. If null, the reader will be created internally. expandReferences - true to expand references in the created document. Returns: The provider which gives access to the non-visual [AuthorDocumentController](../../../ecss/extensions/api/AuthorDocumentController.md) representation of the resource. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If any exception occurs during the loading, for example IO exception due to incorrect system id, unsupported encodings, files saving permission, etc Since: 24.0
### getComponentsProvider

[IComponentsProvider](componentscollector/IComponentsProvider.md) getComponentsProvider()

Creates a components provider for editors. The provider allows you to obtain the components from an editor.
  Returns: The provider which gives you access to the editor components. Since: 27
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
