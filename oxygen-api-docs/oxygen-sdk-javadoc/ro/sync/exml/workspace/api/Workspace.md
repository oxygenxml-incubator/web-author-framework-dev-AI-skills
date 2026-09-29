Package [ro.sync.exml.workspace.api](package-summary.md)

# Interface Workspace
    All Superinterfaces: [ApplicationInformationAccess](application/ApplicationInformationAccess.md), [ColorThemeUtilities](util/ColorThemeUtilities.md), [WorkspaceUtilities](WorkspaceUtilities.md)   All Known Subinterfaces: [AuthorWorkspaceAccess](../../../ecss/extensions/api/access/AuthorWorkspaceAccess.md), [EclipsePluginWorkspace](../../../../../com/oxygenxml/workspace/api/eclipse/EclipsePluginWorkspace.md), [PluginWorkspace](PluginWorkspace.md), [StandalonePluginWorkspace](standalone/StandalonePluginWorkspace.md), [WebappPluginWorkspace](../../../ecss/extensions/api/webapp/access/WebappPluginWorkspace.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface Workspaceextends [WorkspaceUtilities](WorkspaceUtilities.md)
Provides access to workspace specific information and actions.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 boolean [close](#close(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Closes the editor specified by the URL.
  boolean [closeAll](#closeAll())()
Closes all the editors.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [createNewEditor](#createNewEditor(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) extension, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) content)
This is available only in the standalone Oxygen version (not available in the Oxygen Eclipse plugin).Create a new "Untitled" editor.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [createNewEditor](#createNewEditor(java.net.URL,java.lang.String,java.lang.String,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) saveTo, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) extension, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) content)
This is available only in the standalone Oxygen version (not available in the Oxygen Eclipse plugin).Create a new "Untitled" editor.
  void [delete](#delete(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Delete the resource identified by the specified [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  boolean [isStandalone](#isStandalone())()  Deprecated.
This method returns false also when running inside the WebApp.
   boolean [open](#open(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Opens the file at the specified [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) in a new editor.
  boolean [open](#open(java.net.URL,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imposedPage)
Opens the file at the specified [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) in a new editor.
  boolean [open](#open(java.net.URL,java.lang.String,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imposedPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imposedContentType)
Opens the file at the specified [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) in a new editor by specifying an imposed page and an imposed content type.
  void [refreshInProject](#refreshInProject(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
If a new file appeared as a child of a folder in the project, use this method to refresh the parent folder.
  void [saveAll](#saveAll())()
Saves the content of all opened and unsaved editors.
  void [setParentFrameTitle](#setParentFrameTitle(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentFrameTitle)
Set a title on the parent frame.

### Methods inherited from interface ro.sync.exml.workspace.api.application.[ApplicationInformationAccess](application/ApplicationInformationAccess.md)
 [getApplicationName](application/ApplicationInformationAccess.md#getApplicationName()), [getApplicationType](application/ApplicationInformationAccess.md#getApplicationType()), [getLicenseInformationProvider](application/ApplicationInformationAccess.md#getLicenseInformationProvider()), [getPlatform](application/ApplicationInformationAccess.md#getPlatform()), [getPreferencesDirectory](application/ApplicationInformationAccess.md#getPreferencesDirectory()), [getUserInterfaceLanguage](application/ApplicationInformationAccess.md#getUserInterfaceLanguage()), [getVersion](application/ApplicationInformationAccess.md#getVersion()), [getVersionBuildID](application/ApplicationInformationAccess.md#getVersionBuildID())
### Methods inherited from interface ro.sync.exml.workspace.api.util.[ColorThemeUtilities](util/ColorThemeUtilities.md)
 [getColorTheme](util/ColorThemeUtilities.md#getColorTheme()), [getImageInverter](util/ColorThemeUtilities.md#getImageInverter())
### Methods inherited from interface ro.sync.exml.workspace.api.[WorkspaceUtilities](WorkspaceUtilities.md)
 [chooseDirectory](WorkspaceUtilities.md#chooseDirectory()), [chooseDirectory](WorkspaceUtilities.md#chooseDirectory(java.io.File)), [chooseFile](WorkspaceUtilities.md#chooseFile(java.io.File,java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)), [chooseFile](WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseFile](WorkspaceUtilities.md#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean)), [chooseFiles](WorkspaceUtilities.md#chooseFiles(java.io.File,java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURL](WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURL](WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String)), [chooseURL](WorkspaceUtilities.md#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String,java.lang.String,java.lang.String)), [chooseURLPath](WorkspaceUtilities.md#chooseURLPath(java.lang.String,java.lang.String%5B%5D,java.lang.String)), [chooseURLPath](WorkspaceUtilities.md#chooseURLPath(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String)), [clearImageCache](WorkspaceUtilities.md#clearImageCache()), [createJavaProcess](WorkspaceUtilities.md#createJavaProcess(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String,java.util.Map,java.io.File,ro.sync.exml.workspace.api.process.ProcessListener)), [createProcess](WorkspaceUtilities.md#createProcess(ro.sync.exml.workspace.api.process.ProcessListener,java.lang.String,java.io.File,java.lang.String,boolean)), [getDataSourceAccess](WorkspaceUtilities.md#getDataSourceAccess()), [getImageUtilities](WorkspaceUtilities.md#getImageUtilities()), [getParentFrame](WorkspaceUtilities.md#getParentFrame()), [getTemplateManager](WorkspaceUtilities.md#getTemplateManager()), [openInExternalApplication](WorkspaceUtilities.md#openInExternalApplication(java.lang.String,boolean,java.lang.String)), [openInExternalApplication](WorkspaceUtilities.md#openInExternalApplication(java.net.URL,boolean)), [openInExternalApplication](WorkspaceUtilities.md#openInExternalApplication(java.net.URL,boolean,java.lang.String)), [showConfirmDialog](WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)), [showConfirmDialog](WorkspaceUtilities.md#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D,int)), [showErrorMessage](WorkspaceUtilities.md#showErrorMessage(java.lang.String)), [showErrorMessage](WorkspaceUtilities.md#showErrorMessage(java.lang.String,java.lang.Throwable)), [showInformationMessage](WorkspaceUtilities.md#showInformationMessage(java.lang.String)), [showStatusMessage](WorkspaceUtilities.md#showStatusMessage(java.lang.String)), [showStatusMessage](WorkspaceUtilities.md#showStatusMessage(java.lang.String,ro.sync.exml.workspace.api.OperationStatus)), [showWarningDialog](WorkspaceUtilities.md#showWarningDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D)), [showWarningDialog](WorkspaceUtilities.md#showWarningDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D,int)), [showWarningMessage](WorkspaceUtilities.md#showWarningMessage(java.lang.String)), [startProcess](WorkspaceUtilities.md#startProcess(java.lang.String,java.io.File,java.lang.String,boolean))
## Method Details

### open

boolean open([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Opens the file at the specified [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) in a new editor. If the URL is already opened, the editor tab which contains it will be brought to front.
  Parameters: url - The URL of the file to be opened. Returns: true if the operation has succeeded.
### open

boolean open([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imposedPage)

Opens the file at the specified [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) in a new editor. If the URL is already opened, the editor tab which contains it will be brought to front.
  Parameters: url - The URL of the file to be opened. imposedPage - The imposed page for opening the URL. One of the page related constants from [EditorPageConstants](../../editor/EditorPageConstants.md). Returns: true if the operation has succeeded. Since: 13
### open

boolean open([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imposedPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imposedContentType)

Opens the file at the specified [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) in a new editor by specifying an imposed page and an imposed content type. If the URL is already opened, the editor tab which contains it will be brought to front. The imposed content type is used only in the Oxygen standalone application, it is not used in the Author Component and Eclipse plugin applications.
  Parameters: url - The URL of the file to be opened. imposedPage - The imposed page for opening the URL. Can be null to perform the default behavior. imposedContentType - The imposed content type, one of the constants in the interface ro.sync.exml.editor.ContentTypes. This is useful if for example the URL does not have a file extension (maybe it is a CMS resource) but the caller of the API knows that it is XML. In this case the caller can provide the "text/xml" imposed content type for it to avoid Oxygen asking what type of resource the URL is.Another use case is for DITA Map URLs without an extension. The caller can pass the "application/ditamap" content type value to the API. In the standalone application Oxygen will ask the user where to open the DITA Map (DITA Maps Manager or the main editor) and will continue the open procedure. In the Oxygen Eclipse plugin the DITA Map will be opened directly in the DITA Maps Manager view. Can be null to perform the default behavior. Returns: true if the operation has succeeded. Since: 15.2
### saveAll

void saveAll()

Saves the content of all opened and unsaved editors.

### close

boolean close([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Closes the editor specified by the URL.
If the editor has unsaved content, the user will be given the opportunity to save it.

  Parameters: url - The url of the editor to be closed. Returns: true if the editor was successfully closed, and false if the editor could not be closed.
### closeAll

boolean closeAll()

Closes all the editors.
If there are editors with unsaved content, the user will be given the opportunity to save them.

  Returns: true if the editors were successfully closed, and false if the editors are still open.
### delete

void delete([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Delete the resource identified by the specified [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html). Currently supported protocols are:
        * file://
        * zip://
        * ftp://
        * sftp://
        * http://
        * https://

  Parameters: url - The URL from where to delete a resource. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If an I/O exception occurs.
### refreshInProject

void refreshInProject([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

If a new file appeared as a child of a folder in the project, use this method to refresh the parent folder.
  Parameters: url - The new resource
### createNewEditor

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) createNewEditor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) extension, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) content)

This is available only in the standalone Oxygen version (not available in the Oxygen Eclipse plugin).Create a new "Untitled" editor. The editor content is not saved on disk, this method is equivalent to using the "File -> New" action.
  Parameters: extension - The editor extension ("xml" or "dita" or "xsl" or "xsd", etc...) contentType - The content type which can take values like: "text/xml" or "text/xsl" or "text/xsd", etc... If NULL, the content type will be automatically detected from the extension. content - The XML content will be used to load the new editor from. Returns: The URL of the created new editor. Since: 12.1
### createNewEditor

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) createNewEditor([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) saveTo, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) extension, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) content)

This is available only in the standalone Oxygen version (not available in the Oxygen Eclipse plugin).Create a new "Untitled" editor. The editor content is not saved on disk, this method is equivalent to using the "File -> New" action.
  Parameters: saveTo - The URL where the new file will be saved when the save operation is invoked for the first time. extension - The editor extension ("xml" or "dita" or "xsl" or "xsd", etc...). May be null if the saveTo URL is specified. contentType - The content type which can take values like: "text/xml" or "text/xsl" or "text/xsd", etc... If NULL, the content type will be automatically detected from the extension. content - The XML content will be used to load the new editor from. Returns: The URL of the created new editor. Can be null if the URL is already opened in the application. Since: 22
### isStandalone

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) boolean isStandalone()
 Deprecated.
This method returns false also when running inside the WebApp. Use [ApplicationInformationAccess.getPlatform()](application/ApplicationInformationAccess.md#getPlatform()) instead.

Check if the extension is used in the Oxygen stand alone or Eclipse plugin version.
  Returns: true if this is the stand-alone Oxygen version or false if it is the Oxygen Eclipse plug-in version.
### setParentFrameTitle

void setParentFrameTitle([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentFrameTitle)

Set a title on the parent frame. This is available only in the standalone Oxygen version (not available in the Oxygen Eclipse plugin). If NULL, will reset to the default title.
  Parameters: parentFrameTitle - The new title to set on the parent frame. If NULL, will reset to the default title. Since: 12.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
