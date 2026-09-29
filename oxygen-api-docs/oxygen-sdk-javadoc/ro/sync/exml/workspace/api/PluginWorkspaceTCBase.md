Package [ro.sync.exml.workspace.api](package-summary.md)

# Class PluginWorkspaceTCBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * junit.framework.Assert
        * junit.framework.TestCase
            * junit.extensions.jfcunit.JFCTestCase
                * ro.sync.exml.workspace.api.PluginWorkspaceTCBase
   All Implemented Interfaces: junit.framework.Test   @API(type=EXTENDABLE, src=PRIVATE) public abstract class PluginWorkspaceTCBase extends junit.extensions.jfcunit.JFCTestCase
Base class for testing plugins and frameworks. For more details please read the topic called "Creating and Running Automated Tests" from the user manual: https://www.oxygenxml.com/doc/ug-oxygen/topics/automated-tests.html
  Since: 14.1 See Also:
* "https://www.oxygenxml.com/doc/ug-oxygen/topics/automated-tests.html"

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [JSON_EDITOR_PRODUCT](#JSON_EDITOR_PRODUCT)
JSON Editor
  static final int [XML_AUTHOR_PRODUCT](#XML_AUTHOR_PRODUCT)
XML Author
  static final int [XML_DEVELOPER_PRODUCT](#XML_DEVELOPER_PRODUCT)
XML Developer
  static final int [XML_EDITOR_PRODUCT](#XML_EDITOR_PRODUCT)
XML Editor

## Constructor Summary
 Constructors
Constructor

Description
 [PluginWorkspaceTCBase](#%3Cinit%3E(java.io.File,java.io.File,java.io.File,java.io.File,java.lang.String))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) installationFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworksFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) pluginsFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) optionsFolder, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) licenseKey)
Constructor.
  [PluginWorkspaceTCBase](#%3Cinit%3E(java.io.File,java.io.File,java.io.File,java.io.File,java.lang.String,int))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) installationFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworksFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) pluginsFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) optionsFolder, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) licenseKey, int productID)
Constructor.
  [PluginWorkspaceTCBase](#%3Cinit%3E(java.io.File,java.io.File,java.lang.String))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworksFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) pluginsFolder, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) licenseKey)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [WSAuthorEditorPage](editor/page/author/WSAuthorEditorPage.md) [getCurrentAuthorEditorPageAccess](#getCurrentAuthorEditorPageAccess())()
Get the WSAuthorEditorPage for the current edited file.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCurrentEditorXMLContent](#getCurrentEditorXMLContent())()
Get the XML content currently loaded in the current editor.
  [StandalonePluginWorkspace](standalone/StandalonePluginWorkspace.md) [getPluginWorkspace](#getPluginWorkspace())()
Get the plugin workspace.
  protected void [invokeAuthorExtensionActionForID](#invokeAuthorExtensionActionForID(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) id)
Invoke action with a certain ID on the AWT thread.
  protected void [moveCaretRelativeTo](#moveCaretRelativeTo(java.lang.String,int,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, int relativePosition, boolean select)
Move caret relative to a text already existing in the author page.
  [WSEditor](editor/WSEditor.md) [open](#open(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Open an URL.
  protected void [setUp](#setUp())()

 protected void [tearDown](#tearDown())()

### Methods inherited from class junit.extensions.jfcunit.JFCTestCase
 awtSleep, awtSleep, createNoExitSecurityManager, flushAWT, getAssertExit, getError, getHelper, getLockWait, hasError, isAWTRunning, pause, pauseAWT, resetError, resetForcedWait, resetSleepTime, resumeAWT, runBare, runCode, runTest, setAssertExit, setError, setForcedWait, setHelper, setLockWait, setSleepTime, sleep
### Methods inherited from class junit.framework.TestCase
 assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertEquals, assertFalse, assertFalse, assertNotNull, assertNotNull, assertNotSame, assertNotSame, assertNull, assertNull, assertSame, assertSame, assertTrue, assertTrue, countTestCases, createResult, fail, fail, failNotEquals, failNotSame, failSame, format, getName, run, run, setName, toString
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### XML_AUTHOR_PRODUCT

public static final int XML_AUTHOR_PRODUCT

XML Author
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.workspace.api.PluginWorkspaceTCBase.XML_AUTHOR_PRODUCT)

### XML_EDITOR_PRODUCT

public static final int XML_EDITOR_PRODUCT

XML Editor
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.workspace.api.PluginWorkspaceTCBase.XML_EDITOR_PRODUCT)

### XML_DEVELOPER_PRODUCT

public static final int XML_DEVELOPER_PRODUCT

XML Developer
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.workspace.api.PluginWorkspaceTCBase.XML_DEVELOPER_PRODUCT)

### JSON_EDITOR_PRODUCT

public static final int JSON_EDITOR_PRODUCT

JSON Editor
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.workspace.api.PluginWorkspaceTCBase.JSON_EDITOR_PRODUCT)

## Constructor Details

### PluginWorkspaceTCBase

public PluginWorkspaceTCBase([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworksFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) pluginsFolder, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) licenseKey)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Constructor. The installation folder will be assumed to be the folder in which the JVM has started (new File(".")).
  Parameters: frameworksFolder - The folder from where to load the frameworks. If null it will default to the folder "frameworks" in the installationFolder. pluginsFolder - The folder from where to load the plugins. If null it will default to the folder "plugins" in the installationFolder. licenseKey - The license key used to license the test Oxygen application. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - The folder parameters are incorrect.
### PluginWorkspaceTCBase

public PluginWorkspaceTCBase([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) installationFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworksFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) pluginsFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) optionsFolder, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) licenseKey)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Constructor.
  Parameters: installationFolder - The folder where Oxygen is installed. If null it will default to the folder in which the JVM started (new File(".")). frameworksFolder - The folder from where to load the frameworks. If null it will default to the folder "frameworks" in the installationFolder. pluginsFolder - The folder from where to load the plugins. If null it will default to the folder "plugins" in the installationFolder. optionsFolder - The folder from where to load the Oxygen options. Set to null to use the default options folder on your specific platform (located in the user home). licenseKey - The license key used to license the test Oxygen application. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - The folder parameters are incorrect.
### PluginWorkspaceTCBase

public PluginWorkspaceTCBase([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) installationFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworksFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) pluginsFolder, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) optionsFolder, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) licenseKey, int productID)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Constructor.
  Parameters: installationFolder - The folder where Oxygen is installed. If null it will default to the folder in which the JVM started (new File(".")). frameworksFolder - The folder from where to load the frameworks. If null it will default to the folder "frameworks" in the installationFolder. pluginsFolder - The folder from where to load the plugins. If null it will default to the folder "plugins" in the installationFolder. optionsFolder - The folder from where to load the Oxygen options. Set to null to use the default options folder on your specific platform (located in the user home). licenseKey - The license key used to license the test Oxygen application. productID - ID of the product which should be started, one of [XML_AUTHOR_PRODUCT](#XML_AUTHOR_PRODUCT), [XML_EDITOR_PRODUCT](#XML_EDITOR_PRODUCT) or [XML_DEVELOPER_PRODUCT](#XML_DEVELOPER_PRODUCT). The ID of the product should match the type of Oxygen installation that you are using to start the test case. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - The folder parameters are incorrect.
## Method Details

### tearDown

protected void tearDown() throws [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
  Overrides: tearDown in class junit.extensions.jfcunit.JFCTestCase Throws: [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) See Also:
        * JFCTestCase.tearDown()

### setUp

protected void setUp() throws [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
  Overrides: setUp in class junit.extensions.jfcunit.JFCTestCase Throws: [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) See Also:
        * JFCTestCase.setUp()

### getPluginWorkspace

public [StandalonePluginWorkspace](standalone/StandalonePluginWorkspace.md) getPluginWorkspace()

Get the plugin workspace.
  Returns: Returns the plugin workspace.
### open

public [WSEditor](editor/WSEditor.md) open([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)throws [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

Open an URL.
  Parameters: url - The URL to open. Returns: The author page. Throws: [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) - If an I/O exception occurs.
### getCurrentEditorXMLContent

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCurrentEditorXMLContent() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Get the XML content currently loaded in the current editor.
  Returns: The XML content. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If an I/O exception occurs.
### getCurrentAuthorEditorPageAccess

public [WSAuthorEditorPage](editor/page/author/WSAuthorEditorPage.md) getCurrentAuthorEditorPageAccess() throws [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

Get the WSAuthorEditorPage for the current edited file.
  Returns: the WSAuthorEditorPage for the current edited file. Can throw class cast exception if the current editor is not opened in the author page. Throws: [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) - Problems while accessing the current editor page.
### invokeAuthorExtensionActionForID

protected void invokeAuthorExtensionActionForID([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) id)throws [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

Invoke action with a certain ID on the AWT thread.
  Parameters: id - The id The action ID as defined in the framework. Throws: [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) - Problems while accessing the current editor page.
### moveCaretRelativeTo

protected void moveCaretRelativeTo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, int relativePosition, boolean select)throws [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

Move caret relative to a text already existing in the author page.
  Parameters: text - The text to search relativePosition - The delta to move the caret with after finding the text. Throws: [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) - The anchor text was not found in the document.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
