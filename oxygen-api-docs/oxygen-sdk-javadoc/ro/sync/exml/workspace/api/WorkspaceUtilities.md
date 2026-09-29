Package [ro.sync.exml.workspace.api](package-summary.md)

# Interface WorkspaceUtilities
    All Superinterfaces: [ApplicationInformationAccess](application/ApplicationInformationAccess.md), [ColorThemeUtilities](util/ColorThemeUtilities.md)   All Known Subinterfaces: [AuthorWorkspaceAccess](../../../ecss/extensions/api/access/AuthorWorkspaceAccess.md), [EclipsePluginWorkspace](../../../../../com/oxygenxml/workspace/api/eclipse/EclipsePluginWorkspace.md), [PluginWorkspace](PluginWorkspace.md), [StandalonePluginWorkspace](standalone/StandalonePluginWorkspace.md), [WebappPluginWorkspace](../../../ecss/extensions/api/webapp/access/WebappPluginWorkspace.md), [Workspace](Workspace.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WorkspaceUtilitiesextends [ColorThemeUtilities](util/ColorThemeUtilities.md), [ApplicationInformationAccess](application/ApplicationInformationAccess.md)
Provides access to global utility methods.
  Since: 15
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [chooseDirectory](#chooseDirectory())()
Displays a directory chooser for selecting a directory.
  [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [chooseDirectory](#chooseDirectory(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) startingDir)
Displays a directory chooser.
  [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [chooseFile](#chooseFile(java.io.File,java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) currentFileContext, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr, boolean usedForSave)
Displays a file chooser for selecting a [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html).
  [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [chooseFile](#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr)
Displays a file chooser for selecting a [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html).
  [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [chooseFile](#chooseFile(java.lang.String,java.lang.String%5B%5D,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr, boolean openForSave)
Displays a file chooser for selecting a [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html).
  [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] [chooseFiles](#chooseFiles(java.io.File,java.lang.String,java.lang.String%5B%5D,java.lang.String))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) currentFileContext, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr)
Displays a file chooser for selecting multiple [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)s.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [chooseURL](#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr)
Displays an URL chooser for selecting an [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [chooseURL](#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialURL)
Displays an URL chooser for selecting an [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [chooseURL](#chooseURL(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) urlLabel, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) okLabel)
Displays an URL chooser for selecting an [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [chooseURLPath](#chooseURLPath(java.lang.String,java.lang.String%5B%5D,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr)
Displays an URL chooser for selecting an [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [chooseURLPath](#chooseURLPath(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialURL)
Displays an URL chooser for selecting an [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  void [clearImageCache](#clearImageCache())()  Deprecated.
Replaced by [getImageUtilities()](#getImageUtilities())
   [ProcessController](process/ProcessController.md) [createJavaProcess](#createJavaProcess(java.lang.String,java.lang.String%5B%5D,java.lang.String,java.lang.String,java.util.Map,java.io.File,ro.sync.exml.workspace.api.process.ProcessListener))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalJavaArguments, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] classpath, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mainClass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalArguments, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> environmentalVariables, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) startDirectory, [ProcessListener](process/ProcessListener.md) processListener)
Prepare a Java process for execution.
  [ProcessController](process/ProcessController.md) [createProcess](#createProcess(ro.sync.exml.workspace.api.process.ProcessListener,java.lang.String,java.io.File,java.lang.String,boolean))([ProcessListener](process/ProcessListener.md) processListener, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) workingDirectory, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cmdLine, boolean showConsole)
Create a process that executes a given command line.
  ro.sync.exml.workspace.api.options.DataSourceAccess [getDataSourceAccess](#getDataSourceAccess())()
Get information about the configured data source connections.
  [ImageUtilities](images/ImageUtilities.md) [getImageUtilities](#getImageUtilities())()
Get access to image related utilities, support to register custom image handlers or to reset the images cache.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getParentFrame](#getParentFrame())()
Get the parent main frame.
  [TemplateManager](templates/TemplateManager.md) [getTemplateManager](#getTemplateManager())()
Get access to all new file templates.
  void [openInExternalApplication](#openInExternalApplication(java.lang.String,boolean,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url, boolean preferAssociatedApplication, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mediaType)
Open in the associated system application.
  void [openInExternalApplication](#openInExternalApplication(java.net.URL,boolean))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, boolean preferAssociatedApplication)
Open in the associated system application
  void [openInExternalApplication](#openInExternalApplication(java.net.URL,boolean,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, boolean preferAssociatedApplication, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mediaType)
Open in the associated system application
  int [showConfirmDialog](#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] buttonNames, int[] buttonIds)
Shows a question message dialog.
  int [showConfirmDialog](#showConfirmDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] buttonNames, int[] buttonIds, int initialSelectedIndex)
Shows a question message dialog.
  void [showErrorMessage](#showErrorMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)
Presents an error message dialog.
  void [showErrorMessage](#showErrorMessage(java.lang.String,java.lang.Throwable))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html) exception)
Presents an error message dialog.
  void [showInformationMessage](#showInformationMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)
Presents an information message dialog.
  void [showStatusMessage](#showStatusMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) statusMessage)
Show a status message.
  void [showStatusMessage](#showStatusMessage(java.lang.String,ro.sync.exml.workspace.api.OperationStatus))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) statusMessage, [OperationStatus](OperationStatus.md) status)
Show a status message and set a corresponding status color.
  int [showWarningDialog](#showWarningDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] buttonNames, int[] buttonIds)
Shows a warning message dialog.
  int [showWarningDialog](#showWarningDialog(java.lang.String,java.lang.String,java.lang.String%5B%5D,int%5B%5D,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] buttonNames, int[] buttonIds, int initialSelectedIndex)
Shows a warning message dialog.
  void [showWarningMessage](#showWarningMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)
Presents a warning message dialog.
  void [startProcess](#startProcess(java.lang.String,java.io.File,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) workingDirectory, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cmdLine, boolean showConsole)
Start a process that executes a given command line.

### Methods inherited from interface ro.sync.exml.workspace.api.application.[ApplicationInformationAccess](application/ApplicationInformationAccess.md)
 [getApplicationName](application/ApplicationInformationAccess.md#getApplicationName()), [getApplicationType](application/ApplicationInformationAccess.md#getApplicationType()), [getLicenseInformationProvider](application/ApplicationInformationAccess.md#getLicenseInformationProvider()), [getPlatform](application/ApplicationInformationAccess.md#getPlatform()), [getPreferencesDirectory](application/ApplicationInformationAccess.md#getPreferencesDirectory()), [getUserInterfaceLanguage](application/ApplicationInformationAccess.md#getUserInterfaceLanguage()), [getVersion](application/ApplicationInformationAccess.md#getVersion()), [getVersionBuildID](application/ApplicationInformationAccess.md#getVersionBuildID())
### Methods inherited from interface ro.sync.exml.workspace.api.util.[ColorThemeUtilities](util/ColorThemeUtilities.md)
 [getColorTheme](util/ColorThemeUtilities.md#getColorTheme()), [getImageInverter](util/ColorThemeUtilities.md#getImageInverter())
## Method Details

### getParentFrame

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getParentFrame()

Get the parent main frame.
  Returns: The parent frame ({javax.swing.JFrame or java.awt.Frame (when running as a JApplet)}) of the Oxygen application or the parent shell ({org.eclipse.swt.widgets.Shell}) if this is the Eclipse implementation.
### chooseFile

[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) chooseFile([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr, boolean openForSave)

Displays a file chooser for selecting a [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html).
  Parameters: title - The file chooser title. allowedExtensions - Allowed file extensions. Can be null if you want all files filter. Example: new String[] {"xml", "dita"}. filterDescr - Description for the file filter. openForSave - true when the file chooser is used for saving, false if it is used for opening an existing file. Returns: The chosen file or null if the user canceled the dialog.
### chooseFile

[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) chooseFile([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) currentFileContext, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr, boolean usedForSave)

Displays a file chooser for selecting a [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html).
  Parameters: currentFileContext - The file which will be selected in the file chooser. If it is a directory, it will be used as a default directory. If it is a file (even non-existing) and the file chooser is shown for a save operation its name will also be selected in the chooser. Can be set null in order to use the default behavior. title - The file chooser title. allowedExtensions - Allowed file extensions. Can be null if you want all files filter. Example: new String[] {"xml", "dita"}. filterDescr - Description for the file filter. usedForSave - true when the file chooser is used for saving, false if it is used for opening an existing file. Returns: The chosen file or null if the user canceled the dialog. Since: 14
### chooseFile

[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) chooseFile([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr)

Displays a file chooser for selecting a [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html).
  Parameters: title - The file chooser title. allowedExtensions - Allowed file extensions. Can be null if you want all files filter. Example: new String[] {"xml", "dita"}. filterDescr - Description for the file filter. Returns: The chosen file or null if the user canceled the dialog.
### chooseFiles

[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] chooseFiles([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) currentFileContext, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr)

Displays a file chooser for selecting multiple [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)s.
  Parameters: currentFileContext - The file which will be selected in the file chooser. If it is a directory, it will be used as a default directory. If it is a file (even non-existing) and the file chooser is shown for a save operation its name will also be selected in the chooser. Can be set null in order to use the default behavior. title - The file chooser title. allowedExtensions - Allowed file extensions. Can be null if you want all files filter. Example: new String[] {"xml", "dita"}. filterDescr - Description for the file filter. Returns: The chosen files or null if the user canceled the dialog. Since: 15.2
### chooseDirectory

[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) chooseDirectory()

Displays a directory chooser for selecting a directory.
  Returns: The chosen directory or null if the user canceled the dialog. Since: 15
### chooseDirectory

[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) chooseDirectory([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) startingDir)

Displays a directory chooser. Available for the stand-alone oXygen and the Eclipse plugin.
  Parameters: startingDir - The starting directory. May be null. Returns: The chosen directory or null if the user canceled the dialog. Since: 21.1
### chooseURL

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) chooseURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr)

Displays an URL chooser for selecting an [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  Parameters: title - The chooser dialog title. allowedExtensions - Allowed extensions. filterDescr - Description for the filter. Returns: The chosen URL or null if the user canceled the dialog.
### chooseURL

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) chooseURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialURL)

Displays an URL chooser for selecting an [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  Parameters: title - The chooser dialog title. allowedExtensions - Allowed extensions. filterDescr - Description for the filter. initialURL - Default value for the URL (given as string). Can be null. Returns: The chosen URL or null if the user canceled the dialog. Since: 14.2
### chooseURL

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) chooseURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) urlLabel, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) okLabel)

Displays an URL chooser for selecting an [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  Parameters: title - The chooser dialog title. allowedExtensions - Allowed extensions. filterDescr - Description for the filter. initialURL - Default value for the URL (given as string). Can be null. urlLabel - The label used for describing the URL field. If null, the value will be: "URL:". okLabel - The label of the "OK" button. If null the value will be "OK". Returns: The chosen URL or null if the user canceled the dialog. Since: 25.0
### chooseURLPath

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) chooseURLPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr)

Displays an URL chooser for selecting an [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html). If the user sets a relative path in the chooser, that path will be returned.
  Parameters: title - The chooser dialog title. allowedExtensions - Allowed extensions. filterDescr - Description for the filter. Returns: The chosen URL as String or null if the user canceled the dialog. Since: 14
### chooseURLPath

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) chooseURLPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedExtensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filterDescr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialURL)

Displays an URL chooser for selecting an [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html). If the user sets a relative path in the chooser, that path will be returned.
  Parameters: title - The chooser dialog title. allowedExtensions - Allowed extensions. filterDescr - Description for the filter. initialURL - The initial URL to set in the field. Returns: The chosen URL as String or null if the user canceled the dialog. Since: 16.1
### showWarningDialog

int showWarningDialog([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] buttonNames, int[] buttonIds)

Shows a warning message dialog.
  Parameters: title - The dialog title. message - The message to be presented to the user. buttonNames - The names of the buttons representing the choices in the dialog. buttonIds - The id for each button. Used to identify which button was pressed. All Ids must be greater or equal to 0. Returns: the id of the pressed button or -1 if the dialog was closed by other means. Since: 26.0
### showWarningDialog

int showWarningDialog([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] buttonNames, int[] buttonIds, int initialSelectedIndex)

Shows a warning message dialog.
  Parameters: title - The dialog title. message - The message to be presented to the user. buttonNames - The names of the buttons representing the choices in the dialog. buttonIds - The id for each button. Used to identify which button was pressed. initialSelectedIndex - The index of the initial selected button. 0 based. All Ids must be greater or equal to 0. Returns: the id of the pressed button or -1 if the dialog was closed by other means. Since: 26.0
### showConfirmDialog

int showConfirmDialog([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] buttonNames, int[] buttonIds)

Shows a question message dialog.
  Parameters: title - The dialog title. message - The message to be presented to the user. buttonNames - The names of the buttons representing the choices in the dialog. buttonIds - The id for each button. Used to identify which button was pressed. All Ids must be greater or equal to 0. Returns: the id of the pressed button or -1 if the dialog was closed by other means.
### showConfirmDialog

int showConfirmDialog([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] buttonNames, int[] buttonIds, int initialSelectedIndex)

Shows a question message dialog.
  Parameters: title - The dialog title. message - The message to be presented to the user. buttonNames - The names of the buttons representing the choices in the dialog. buttonIds - The id for each button. Used to identify which button was pressed. initialSelectedIndex - The index of the initial selected button. 0 based. All Ids must be greater or equal to 0. Returns: the id of the pressed button or -1 if the dialog was closed by other means. Since: 13.1
### showErrorMessage

void showErrorMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)

Presents an error message dialog.
  Parameters: message - The error message.
### showErrorMessage

void showErrorMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html) exception)

Presents an error message dialog.
  Parameters: message - The error message. exception - An exception for which the stack trace will be shown when the "More details" link is clicked. In more recent application versions due to security related decisions the exception stack trace is no longer shown. Since: 19.1
### showWarningMessage

void showWarningMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)

Presents a warning message dialog.
  Parameters: message - The warning message. Since: 17.1
### showInformationMessage

void showInformationMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)

Presents an information message dialog.
  Parameters: message - The information message.
### showStatusMessage

void showStatusMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) statusMessage)

Show a status message.
  Parameters: statusMessage - The status message
### showStatusMessage

void showStatusMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) statusMessage, [OperationStatus](OperationStatus.md) status)

Show a status message and set a corresponding status color.
  Parameters: statusMessage - The message. status - The status that gives the color. Since: 20
### openInExternalApplication

void openInExternalApplication([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, boolean preferAssociatedApplication)

Open in the associated system application
  Parameters: url - The URL to open. preferAssociatedApplication - If true will prefer the system associated application and if this fails, open in the browser if false will open in the browser. Since: 12
### openInExternalApplication

void openInExternalApplication([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, boolean preferAssociatedApplication, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mediaType)

Open in the associated system application
  Parameters: url - The URL to open. preferAssociatedApplication - If true will prefer the system associated application and if this fails, open in the browser if false will open in the browser. mediaType - The media type of the URL to open. Since: 18.1
### openInExternalApplication

void openInExternalApplication([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url, boolean preferAssociatedApplication, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mediaType)

Open in the associated system application.
  Parameters: url - The URL to open. preferAssociatedApplication - If true, it will prefer the system associated application and if this fails, it will open in the browser. If falsethe resource will be opened in the browser. mediaType - The media type of the URL to open. Since: 19.1
### createJavaProcess

[ProcessController](process/ProcessController.md) createJavaProcess([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalJavaArguments, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] classpath, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mainClass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalArguments, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> environmentalVariables, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) startDirectory, [ProcessListener](process/ProcessListener.md) processListener)

Prepare a Java process for execution. It also sets on the Java process the Oxygen HTTP proxy configuration.
  Parameters: additionalJavaArguments - Additional Java arguments like "-Xmx256m" classpath - The classpath. mainClass - The main class additionalArguments - The additional process arguments environmentalVariables - Additional environmental variables. Can be null startDirectory - The directory where the process should start. Can be null processListener - The process listener. Can be null Returns: Access to the process. Sample usage:  ProcessListener processListener = new ProcessListener() {public void newErrorLine(String line) {System.err.println("Error from process " + line);}public void processCouldNotStart(String message) {System.err.println("Could not start process " + message);}public void processEnded(int exitCode) {System.err.println("Process ended " + exitCode);}public void newOutputLine(String line) {System.out.println("Output from process: " + line);}};final ProcessController processController = standalonePluginWorkspace.createJavaProcess("-Xmx256m", new String[] {"lib/oxygen.jar", "classes"}, //The main Oxygen class"ro.sync.exml.Oxygen", //The URL which Oxygen will attempt to load on startup"file:/D:/projects/eXml/samples/dita/flowers/topics/copyright.xml",//Environmental variables to set to the process, none in mu casenull, new File("."), processListener);//You can start a new thread here and send messages to the process using the ProcessControler //Start the process, will block until process has finishedprocessController.start(); Since: 12.1
### startProcess

void startProcess([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) workingDirectory, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cmdLine, boolean showConsole)

Start a process that executes a given command line. If the process is already running, it will not be started again. **Does not wait for the process to finish.**
  Parameters: name - The name of the process. workingDirectory - The directory where the process is started. cmdLine - The command line to be executed. Can contain editor variables. showConsole - True to show the console. Since: 18.1
### createProcess

[ProcessController](process/ProcessController.md) createProcess([ProcessListener](process/ProcessListener.md) processListener, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) workingDirectory, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cmdLine, boolean showConsole)

Create a process that executes a given command line.
  Parameters: processListener - The process handler name - The name of the process. workingDirectory - The directory where the process is started. cmdLine - The command line to be executed. Can contain editor variables. showConsole - True to show the console. Returns: The process controller of the started process if process could be started, otherwise null if for example the process is already running. Since: 23.1
### clearImageCache

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void clearImageCache()
 Deprecated.
Replaced by [getImageUtilities()](#getImageUtilities())

Clear the cache of images used to display images fast in the Author page. You can use the [ImageUtilities](images/ImageUtilities.md) API to clear the image cache.
  Since: 13
### getDataSourceAccess

ro.sync.exml.workspace.api.options.DataSourceAccess getDataSourceAccess()

Get information about the configured data source connections.
  Returns: The DataSourceAccess capable of providing information about the data source connections. Since: 14.1
### getImageUtilities

[ImageUtilities](images/ImageUtilities.md) getImageUtilities()

Get access to image related utilities, support to register custom image handlers or to reset the images cache.
  Returns: access to image related utilities. Since: 18
### getTemplateManager

[TemplateManager](templates/TemplateManager.md) getTemplateManager()

Get access to all new file templates.
  Returns: access to all new file templates. Since: 18
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
