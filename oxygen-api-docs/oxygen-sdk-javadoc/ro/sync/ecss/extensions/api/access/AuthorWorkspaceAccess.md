Package [ro.sync.ecss.extensions.api.access](package-summary.md)

# Interface AuthorWorkspaceAccess
    All Superinterfaces: [ApplicationInformationAccess](../../../../exml/workspace/api/application/ApplicationInformationAccess.md), [ColorThemeUtilities](../../../../exml/workspace/api/util/ColorThemeUtilities.md), [Workspace](../../../../exml/workspace/api/Workspace.md), [WorkspaceUtilities](../../../../exml/workspace/api/WorkspaceUtilities.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorWorkspaceAccessextends [Workspace](../../../../exml/workspace/api/Workspace.md)
Provides access to workspace specific information and actions.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] [getAllEditorLocations](#getAllEditorLocations())()
Get all the editor locations.
  [WSEditor](../../../../exml/workspace/api/editor/WSEditor.md) [getEditorAccess](#getEditorAccess(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) location)
Find an editor access by location.
  boolean [open](#open(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) file)  Deprecated.
Use [Workspace.open(URL)](../../../../exml/workspace/api/Workspace.md#open(java.net.URL)) instead.

### Methods inherited from interface ro.sync.exml.workspace.api.application.[ApplicationInformationAccess](../../../../exml/workspace/api/application/ApplicationInformationAccess.md)
 [getApplicationName](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getApplicationName()), [getApplicationType](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getApplicationType()), [getLicenseInformationProvider](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getLicenseInformationProvider()), [getPlatform](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()), [getPreferencesDirectory](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPreferencesDirectory()), [getUserInterfaceLanguage](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getUserInterfaceLanguage()), [getVersion](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getVersion()), [getVersionBuildID](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getVersionBuildID())
### Methods inherited from interface ro.sync.exml.workspace.api.util.[ColorThemeUtilities](../../../../exml/workspace/api/util/ColorThemeUtilities.md)
 [getColorTheme](../../../../exml/workspace/api/util/ColorThemeUtilities.md#getColorTheme()), [getImageInverter](../../../../exml/workspace/api/util/ColorThemeUtilities.md#getImageInverter())
### Methods inherited from interface ro.sync.exml.workspace.api.[Workspace](../../../../exml/workspace/api/Workspace.md)
 [close](../../../../exml/workspace/api/Workspace.md#close(java.net.URL)), [closeAll](../../../../exml/workspace/api/Workspace.md#closeAll()), [createNewEditor](../../../../exml/workspace/api/Workspace.md#createNewEditor(java.lang.String,java.lang.String,java.lang.String)), [createNewEditor](../../../../exml/workspace/api/Workspace.md#createNewEditor(java.net.URL,java.lang.String,java.lang.String,java.lang.String)), [delete](../../../../exml/workspace/api/Workspace.md#delete(java.net.URL)), [isStandalone](../../../../exml/workspace/api/Workspace.md#isStandalone()), [open](../../../../exml/workspace/api/Workspace.md#open(java.net.URL)), [open](../../../../exml/workspace/api/Workspace.md#open(java.net.URL,java.lang.String)), [open](../../../../exml/workspace/api/Workspace.md#open(java.net.URL,java.lang.String,java.lang.String)), [refreshInProject](../../../../exml/workspace/api/Workspace.md#refreshInProject(java.net.URL)), [saveAll](../../../../exml/workspace/api/Workspace.md#saveAll()), [setParentFrameTitle](../../../../exml/workspace/api/Workspace.md#setParentFrameTitle(java.lang.String))
### Methods inherited from interface ro.sync.exml.workspace.api.[WorkspaceUtilities](../../../../exml/workspace/api/WorkspaceUtilities.md)
 [chooseDirectory](../../../../exml/workspace/api/WorkspaceUtilities.md#chooseDirectory()), [chooseDirectory](../../../../exml/workspace/api/WorkspaceUtilities.md#chooseDirectory(java.io.File)), [chooseFile](../../../../exml/workspace/api/WorkspaceUtilities.md#chooseFile(java.io.File,java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)), [chooseFile](../../../../exml/workspace/api/WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseFile](../../../../exml/workspace/api/WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)), [chooseFiles](../../../../exml/workspace/api/WorkspaceUtilities.md#chooseFiles(java.io.File,java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURL](../../../../exml/workspace/api/WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURL](../../../../exml/workspace/api/WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String)), [chooseURL](../../../../exml/workspace/api/WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String,java.lang.String,java.lang.String)), [chooseURLPath](../../../../exml/workspace/api/WorkspaceUtilities.md#chooseURLPath(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURLPath](../../../../exml/workspace/api/WorkspaceUtilities.md#chooseURLPath(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String)), [clearImageCache](../../../../exml/workspace/api/WorkspaceUtilities.md#clearImageCache()), [createJavaProcess](../../../../exml/workspace/api/WorkspaceUtilities.md#createJavaProcess(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String,java.util.Map,java.io.File,ro.sync.exml.workspace.api.process.ProcessListener)), [createProcess](../../../../exml/workspace/api/WorkspaceUtilities.md#createProcess(ro.sync.exml.workspace.api.process.ProcessListener,java.lang.String,java.io.File,java.lang.String,boolean)), [getDataSourceAccess](../../../../exml/workspace/api/WorkspaceUtilities.md#getDataSourceAccess()), [getImageUtilities](../../../../exml/workspace/api/WorkspaceUtilities.md#getImageUtilities()), [getParentFrame](../../../../exml/workspace/api/WorkspaceUtilities.md#getParentFrame()), [getTemplateManager](../../../../exml/workspace/api/WorkspaceUtilities.md#getTemplateManager()), [openInExternalApplication](../../../../exml/workspace/api/WorkspaceUtilities.md#openInExternalApplication(java.lang.String,boolean,java.lang.String)), [openInExternalApplication](../../../../exml/workspace/api/WorkspaceUtilities.md#openInExternalApplication(java.net.URL,boolean)), [openInExternalApplication](../../../../exml/workspace/api/WorkspaceUtilities.md#openInExternalApplication(java.net.URL,boolean,java.lang.String)), [showConfirmDialog](../../../../exml/workspace/api/WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)), [showConfirmDialog](../../../../exml/workspace/api/WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D,int)), [showErrorMessage](../../../../exml/workspace/api/WorkspaceUtilities.md#showErrorMessage(java.lang.String)), [showErrorMessage](../../../../exml/workspace/api/WorkspaceUtilities.md#showErrorMessage(java.lang.String,java.lang.Throwable)), [showInformationMessage](../../../../exml/workspace/api/WorkspaceUtilities.md#showInformationMessage(java.lang.String)), [showStatusMessage](../../../../exml/workspace/api/WorkspaceUtilities.md#showStatusMessage(java.lang.String)), [showStatusMessage](../../../../exml/workspace/api/WorkspaceUtilities.md#showStatusMessage(java.lang.String,ro.sync.exml.workspace.api.OperationStatus)), [showWarningDialog](../../../../exml/workspace/api/WorkspaceUtilities.md#showWarningDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)), [showWarningDialog](../../../../exml/workspace/api/WorkspaceUtilities.md#showWarningDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D,int)), [showWarningMessage](../../../../exml/workspace/api/WorkspaceUtilities.md#showWarningMessage(java.lang.String)), [startProcess](../../../../exml/workspace/api/WorkspaceUtilities.md#startProcess(java.lang.String,java.io.File,java.lang.String,boolean))
## Method Details

### open

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) boolean open([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) file)
 Deprecated.
Use [Workspace.open(URL)](../../../../exml/workspace/api/Workspace.md#open(java.net.URL)) instead.

Opens the specified [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) in a new editor.
  Parameters: file - The file to be opened. Returns: true if the operation has succeeded.
### getAllEditorLocations

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] getAllEditorLocations()

Get all the editor locations.
  Returns: All the editor locations in the main editing area or empty array if no editor is opened. Since: 13.2
### getEditorAccess

[WSEditor](../../../../exml/workspace/api/editor/WSEditor.md) getEditorAccess([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) location)

Find an editor access by location.
  Parameters: location - The editor location  Returns: access to the found editor or null if no editor found with that location URL. Since: 13.2
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
