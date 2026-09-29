Package [ro.sync.ecss.extensions.api.component](package-summary.md)

# Class AuthorComponentFactory

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.component.AuthorComponentFactory
   All Implemented Interfaces: [MathFlowConfigurator](../../../../exml/workspace/api/math/MathFlowConfigurator.md), [ReferencesCustomizer](../../../../exml/workspace/api/standalone/ReferencesCustomizer.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class AuthorComponentFactory extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ReferencesCustomizer](../../../../exml/workspace/api/standalone/ReferencesCustomizer.md), [MathFlowConfigurator](../../../../exml/workspace/api/math/MathFlowConfigurator.md)
This factory creates author components.
The recommended way to license the author component is:

1. Set up a floating license servlet, as explained [here](http://oxygenxml.com/doc/help.php?pageId=installation-setting-up-license-server)
2. Let each user paste their named user license key in the License Key Dialog displayed automatically when no license information is provided to the factory.
Here is a small sample showing how to load an XML document into an Author page. For more samples see the sample projects available in the SDK. Read about accessing the SDK API and samples [here](http://www.oxygenxml.com/oxygen_sdk.html).
```

           // These two zips should be packed in some jar files from the classpath.
           URL frameworksZipURL = Reviewer.class.getResource("/frameworks.zip");  
           URL optionsZipURL = Reviewer.class.getResource("/options.zip");

           // Getting the component factory
           AuthorComponentFactory factory = AuthorComponentFactory.getInstance();
           factory.init(new URL[] {frameworksZipURL}, optionsZipURL, null, null, 
               // A null license key triggers the display of the license key dialog.
               // You can use a floating license servlet by invoking other init methods. 
               null);

           // Create the AuthorComponent provider
           EditorComponentProvider componentProvider = factory.createEditorComponentProvider(
               new String[] { EditorPageConstants.PAGE_AUTHOR },
               // The initial page
               EditorPageConstants.PAGE_AUTHOR);

           // This is the Author API starting point
           // You can access the document, selection, move caret, perform edits, etc..
           WSAuthorComponentEditorPage authorPage = (WSAuthorComponentEditorPage) componentProvider.getWSEditorAccess()
               .getCurrentPage();

           // Load a document.
           URL url = new File("D:/projects/eXml/samples/personal.xml").toURI().toURL();
           Reader reader = new InputStreamReader(url.openStream(), "UTF-8");     
           componentProvider.load(url, reader);

           // Show the component in a frame.
           JFrame frame = new JFrame("Author Component Sample Reviewer Application");
           frame.setSize(600, 400);
           frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
           frame.getContentPane().add(componentProvider.getEditorComponent());
           frame.setVisible(true);

```

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorComponentFactory](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addDITAMapTreeTargetInformationProvider](#addDITAMapTreeTargetInformationProvider(java.lang.String,ro.sync.exml.workspace.api.standalone.ditamap.TopicRefTargetInfoProvider))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol, [TopicRefTargetInfoProvider](../../../../exml/workspace/api/standalone/ditamap/TopicRefTargetInfoProvider.md) targetInformationProvider)
Add a provider which can resolve certain information for each topic ref, without the component needing to parse that topic reference.
  void [addInputURLChooserCustomizer](#addInputURLChooserCustomizer(ro.sync.exml.workspace.api.standalone.InputURLChooserCustomizer))([InputURLChooserCustomizer](../../../../exml/workspace/api/standalone/InputURLChooserCustomizer.md) inputURLChooserCustomizer)
Adds a customizer which can modify the list of "Browse" actions.
  void [addRelativeReferencesResolver](#addRelativeReferencesResolver(java.lang.String,ro.sync.exml.workspace.api.util.RelativeReferenceResolver))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol, [RelativeReferenceResolver](../../../../exml/workspace/api/util/RelativeReferenceResolver.md) resolver)
Add a relative reference resolver for a certain URL protocol.
  [DITAMapTreeComponentProvider](ditamap/DITAMapTreeComponentProvider.md) [createDITAMapTreeComponentProvider](#createDITAMapTreeComponentProvider())()
Creates a new DITA Map tree component provider.
  [EditorComponentProvider](EditorComponentProvider.md) [createEditorComponentProvider](#createEditorComponentProvider(java.lang.String%5B%5D,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage)
Creates a new author component
  [EditorComponentProvider](EditorComponentProvider.md) [createEditorComponentProvider](#createEditorComponentProvider(java.lang.String%5B%5D,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
Creates a new editor component
  void [dispose](#dispose())()
It is advisable to call this method when the Author Component Factory is no longer in use.
  void [disposeDITAMapComponentProvider](#disposeDITAMapComponentProvider(ro.sync.ecss.extensions.api.component.ditamap.DITAMapTreeComponentProvider))([DITAMapTreeComponentProvider](ditamap/DITAMapTreeComponentProvider.md) provider)
Remove the handlers the factory has to the component used to notify for changes.
  void [disposeEditorComponentProvider](#disposeEditorComponentProvider(ro.sync.ecss.extensions.api.component.EditorComponentProvider))([EditorComponentProvider](EditorComponentProvider.md) provider)
Remove the handlers the factory has to the component used to notify for changes.
  static [AuthorComponentFactory](AuthorComponentFactory.md) [getInstance](#getInstance())()
Get the singleton instance.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[MenuBarCustomizer](../../../../exml/workspace/api/standalone/MenuBarCustomizer.md)> [getPluginMenubarCustomizers](#getPluginMenubarCustomizers())()
Get the menu bar customizers which were added by all the installed plugins.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ToolbarComponentsCustomizer](../../../../exml/workspace/api/standalone/ToolbarComponentsCustomizer.md)> [getPluginToolbarCustomizers](#getPluginToolbarCustomizers())()
Get the toolbar customizers which were added by all installed plugins.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ViewComponentCustomizer](../../../../exml/workspace/api/standalone/ViewComponentCustomizer.md)> [getPluginViewCustomizers](#getPluginViewCustomizers())()
Get the view customizers which were added by all the installed plugins.
  [PluginWorkspace](../../../../exml/workspace/api/PluginWorkspace.md) [getPluginWorkspace](#getPluginWorkspace())()
Get access to API used to control the created editor components.
  ro.sync.azcheck.ui.SpellCheckOptions [getSpellCheckOptions](#getSpellCheckOptions())()
Get the spell check options which are currently used for the components.
  [UtilAccess](../../../../exml/workspace/api/util/UtilAccess.md) [getUtilAccess](#getUtilAccess())()
Get access to utility methods.
  [WorkspaceUtilities](../../../../exml/workspace/api/WorkspaceUtilities.md) [getWorkspaceUtilities](#getWorkspaceUtilities())()
Get access to various workspace utilities.
  [XMLUtilAccess](../../../../exml/workspace/api/util/XMLUtilAccess.md) [getXMLUtilAccess](#getXMLUtilAccess())()
Access to XML utilities.
  void [init](#init(java.io.File,java.net.URL,java.net.URL,java.lang.String,java.lang.String,java.lang.String,java.lang.String))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworksAndPluginsFolder, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) optionsZipURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) appletCodeBase, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) appletID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) servletURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) userName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) password)
This method should get called as soon as possible before calling any other methods from this class.
  void [init](#init(java.net.URL%5B%5D,java.net.URL,java.net.URL,java.lang.String,java.lang.String,java.lang.String,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] frameworksZIPURLs, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) optionsZipURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) appletCodeBase, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) appletID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) servletURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) userName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) password)
This method should get called as soon as possible before calling any other methods from this class.
  void [setAutoCorrectState](#setAutoCorrectState(boolean))(boolean enabled)
Enable or disable the auto correct feature.
  void [setDITAKeyDefinitionManager](#setDITAKeyDefinitionManager(ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionManager))([KeyDefinitionManager](../../../../exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManager.md) keyDefitionManager)
By default key definitions are gathered from DITA Maps opened in the DITA Maps Manager.
  void [setMathFlowFixedLicenseFile](#setMathFlowFixedLicenseFile(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) licenseFile)
Set the path to a license file.
  void [setMathFlowFixedLicenseKeyForComposer](#setMathFlowFixedLicenseKeyForComposer(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fixedKey)
Set a fixed key for licensing the MathFlow composer used to view embedded MathML equations.
  void [setMathFlowFixedLicenseKeyForEditor](#setMathFlowFixedLicenseKeyForEditor(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fixedKey)
Set a fixed key for licensing the MathFlow editor dialog used to edit embedded MathML equations.
  void [setMathFlowInstallationFolder](#setMathFlowInstallationFolder(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) installationFolder)
Set the path to the MathFlow installation folder.
  void [setObjectProperty](#setObjectProperty(java.lang.String,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)
Sets a property in the Oxygen preferences.
  void [setOpenURLHandler](#setOpenURLHandler(ro.sync.ecss.extensions.api.component.listeners.OpenURLHandler))([OpenURLHandler](listeners/OpenURLHandler.md) openURLHandler)
Set a handler which will be notified when an URL should be opened.
  void [setParentFrame](#setParentFrame(java.awt.Frame))([Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) parentFrame)
Set the parent frame to the Author Component Factory.
  void [setSpellCheckOptions](#setSpellCheckOptions(ro.sync.azcheck.ui.SpellCheckOptions))(ro.sync.azcheck.ui.SpellCheckOptions newSpellCheckOptions)
Set the spell check options which are currently used for the components.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorComponentFactory

public AuthorComponentFactory()

## Method Details

### getInstance

public static [AuthorComponentFactory](AuthorComponentFactory.md) getInstance()

Get the singleton instance.
  Returns: The singleton instance.
### dispose

public void dispose()

It is advisable to call this method when the Author Component Factory is no longer in use. For example, if the author component is using a floating license, this method should get called in the applet when the destroy() callback is received in order to quickly release the license to the license server.
  Since: 13.2
### init

public void init([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworksAndPluginsFolder, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) optionsZipURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) appletCodeBase, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) appletID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) servletURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) userName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) password)throws [AuthorComponentException](AuthorComponentException.md)

#### This method should get called as soon as possible before calling any other methods from this class. Please use it only if you have set up a license servlet on a J2EE server which distributes floating licenses:https://www.oxygenxml.com/doc/ug-editor/index.html#topics/component_licensing.htmlhttps://www.oxygenxml.com/doc/ug-editor/index.html#topic_l1g_lhy_x4.html#topic_l1g_lhy_x4
Initialize the component. Will have effect only once.
  Parameters: frameworksAndPluginsFolder - The folder containing the framework and plugin folders to be used. optionsZipURL - URL to the options ZIP. appletCodeBase - Code base when run from an applet, can be null when using the author component in a standalone application appletID - ID when run from Applet, can be null, used to store the frameworks associated with the applet. servletURL - The URL to connect to a HTTP license server userName - User name to connect to the license server. password - Password to connect to the license server. Throws: [AuthorComponentException](AuthorComponentException.md) Since: 22
### init

public void init([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] frameworksZIPURLs, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) optionsZipURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) appletCodeBase, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) appletID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) servletURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) userName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) password)throws [AuthorComponentException](AuthorComponentException.md)

#### This method should get called as soon as possible before calling any other methods from this class. Please use it only if you have set up a license servlet on a J2EE server which distributes floating licenses:https://www.oxygenxml.com/doc/ug-editor/index.html#topics/component_licensing.htmlhttps://www.oxygenxml.com/doc/ug-editor/index.html#topic_l1g_lhy_x4.html#topic_l1g_lhy_x4
Initialize the component. Will have effect only once.
  Parameters: frameworksZIPURLs - The set of ZIPs which contain the frameworks optionsZipURL - URL to the options ZIP. appletCodeBase - Code base when run from an applet, can be null when using the author component in a standalone application appletID - ID when run from Applet, can be null, used to store the frameworks associated with the applet. servletURL - The URL to connect to a HTTP license server userName - User name to connect to the license server. password - Password to connect to the license server. Throws: [AuthorComponentException](AuthorComponentException.md) Since: 12.1
### setObjectProperty

public void setObjectProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)

Sets a property in the Oxygen preferences.
  Parameters: key - The key from the Oxygen options value - Value for the key.
### createEditorComponentProvider

public [EditorComponentProvider](EditorComponentProvider.md) createEditorComponentProvider([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage)throws [AuthorComponentException](AuthorComponentException.md)

Creates a new author component
  Parameters: allowedPages - The pages which will be used in the editor. One of the constant fields: [EditorPageConstants.PAGE_TEXT](../../../../exml/editor/EditorPageConstants.md#PAGE_TEXT), [EditorPageConstants.PAGE_AUTHOR](../../../../exml/editor/EditorPageConstants.md#PAGE_AUTHOR), [EditorPageConstants.PAGE_GRID](../../../../exml/editor/EditorPageConstants.md#PAGE_GRID) initialPage - The initial page in which the component will edit. Can be null in order to auto detect it. Returns: the new author component Throws: [AuthorComponentException](AuthorComponentException.md) Since: 14.2
### createEditorComponentProvider

public [EditorComponentProvider](EditorComponentProvider.md) createEditorComponentProvider([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)throws [AuthorComponentException](AuthorComponentException.md)

Creates a new editor component
  Parameters: allowedPages - The pages which will be used in the editor. One of the constant fields: [EditorPageConstants.PAGE_TEXT](../../../../exml/editor/EditorPageConstants.md#PAGE_TEXT), [EditorPageConstants.PAGE_AUTHOR](../../../../exml/editor/EditorPageConstants.md#PAGE_AUTHOR), [EditorPageConstants.PAGE_GRID](../../../../exml/editor/EditorPageConstants.md#PAGE_GRID), , [EditorPageConstants.PAGE_DESIGN](../../../../exml/editor/EditorPageConstants.md#PAGE_DESIGN) initialPage - The initial page in which the component will edit. Can be null in order to auto detect it. contentType - The editor content type. One of ContentTypes constants Returns: the new author component Throws: [AuthorComponentException](AuthorComponentException.md) Since: 26.0
### createDITAMapTreeComponentProvider

public [DITAMapTreeComponentProvider](ditamap/DITAMapTreeComponentProvider.md) createDITAMapTreeComponentProvider() throws [AuthorComponentException](AuthorComponentException.md)

Creates a new DITA Map tree component provider. Provides access to showing a DITA Map URL in a tree-like fashion (like the DITA Maps Manager view).
  Returns: the new DITA Map tree component provider. Throws: [AuthorComponentException](AuthorComponentException.md) Since: 14
### disposeEditorComponentProvider

public void disposeEditorComponentProvider([EditorComponentProvider](EditorComponentProvider.md) provider)

Remove the handlers the factory has to the component used to notify for changes. It is important to call this method when creating multiple author components in a multiple editor component where editors are sometimes closed. When an editor is closed, this method should get called in order to avoid memory leaks.
  Parameters: provider - The provider to release.
### disposeDITAMapComponentProvider

public void disposeDITAMapComponentProvider([DITAMapTreeComponentProvider](ditamap/DITAMapTreeComponentProvider.md) provider)

Remove the handlers the factory has to the component used to notify for changes. It is important to call this method when creating multiple DITA Map components in a multiple editor component where editors are sometimes closed. When an editor is closed, this method should get called in order to avoid memory leaks.
  Parameters: provider - The provider to release.
### getSpellCheckOptions

public ro.sync.azcheck.ui.SpellCheckOptions getSpellCheckOptions()

Get the spell check options which are currently used for the components.
  Returns: the spell check options which are currently used for the components.
### setSpellCheckOptions

public void setSpellCheckOptions(ro.sync.azcheck.ui.SpellCheckOptions newSpellCheckOptions)

Set the spell check options which are currently used for the components. All options can be changed except the spell checker which is fixed to Hunspell.
  Parameters: newSpellCheckOptions - The new spell check options to set.
### setAutoCorrectState

public void setAutoCorrectState(boolean enabled)

Enable or disable the auto correct feature. By default it is disabled.
  Parameters: enabled - true to enable the auto correct feature, false to disable it.
### setOpenURLHandler

public void setOpenURLHandler([OpenURLHandler](listeners/OpenURLHandler.md) openURLHandler)

Set a handler which will be notified when an URL should be opened. For example the user clicked a link in the Author page.
  Parameters: openURLHandler - The open URLs handler. Since: 12.2
### addInputURLChooserCustomizer

public void addInputURLChooserCustomizer([InputURLChooserCustomizer](../../../../exml/workspace/api/standalone/InputURLChooserCustomizer.md) inputURLChooserCustomizer)
 Description copied from interface: [ReferencesCustomizer](../../../../exml/workspace/api/standalone/ReferencesCustomizer.md#addInputURLChooserCustomizer(ro.sync.exml.workspace.api.standalone.InputURLChooserCustomizer))
Adds a customizer which can modify the list of "Browse" actions. These actions are available in Oxygen, in any control or dialog that contains an URL input box.  **IMPORTANT** This customizer must be set early, when the plugin extension's **applicationStarted** method gets called or after the AuthorComponentFactory was initialized (if running the Author component).  *Example:* If a CMS developer wants the user to choose the URL from their custom CMS chooser then it will add a new action (possibly removing the others). When the new action gets called the custom code shows the custom chooser and at the end it can call the **ro.sync.exml.workspace.api.standalone.InputURLChooser** interface to set the new URL in the combo box.
  Specified by: [addInputURLChooserCustomizer](../../../../exml/workspace/api/standalone/ReferencesCustomizer.md#addInputURLChooserCustomizer(ro.sync.exml.workspace.api.standalone.InputURLChooserCustomizer)) in interface [ReferencesCustomizer](../../../../exml/workspace/api/standalone/ReferencesCustomizer.md) Parameters: inputURLChooserCustomizer - The input URL chooser customizer. Since: 13 See Also:
        * [ReferencesCustomizer.addInputURLChooserCustomizer(ro.sync.exml.workspace.api.standalone.InputURLChooserCustomizer)](../../../../exml/workspace/api/standalone/ReferencesCustomizer.md#addInputURLChooserCustomizer(ro.sync.exml.workspace.api.standalone.InputURLChooserCustomizer))

### addRelativeReferencesResolver

public void addRelativeReferencesResolver([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol, [RelativeReferenceResolver](../../../../exml/workspace/api/util/RelativeReferenceResolver.md) resolver)
 Description copied from interface: [ReferencesCustomizer](../../../../exml/workspace/api/standalone/ReferencesCustomizer.md#addRelativeReferencesResolver(java.lang.String,ro.sync.exml.workspace.api.util.RelativeReferenceResolver))
Add a relative reference resolver for a certain URL protocol. This method can be used by a CMS implementor to take control over the way Oxygen is computing relative references for a certain URL protocol. For example when inserting in a DITA Topic a reference to an image Oxygen will try to make the reference relative to the current XML document. If the DITA Topic is opened using your custom URL protocol you can take control over they way in which the relative path is computed.
  Specified by: [addRelativeReferencesResolver](../../../../exml/workspace/api/standalone/ReferencesCustomizer.md#addRelativeReferencesResolver(java.lang.String,ro.sync.exml.workspace.api.util.RelativeReferenceResolver)) in interface [ReferencesCustomizer](../../../../exml/workspace/api/standalone/ReferencesCustomizer.md) Parameters: protocol - The URL protocol for which you want to take control over the relativization. resolver - The custom resolver. Since: 13 See Also:
        * [ReferencesCustomizer.addRelativeReferencesResolver(java.lang.String, ro.sync.exml.workspace.api.util.RelativeReferenceResolver)](../../../../exml/workspace/api/standalone/ReferencesCustomizer.md#addRelativeReferencesResolver(java.lang.String,ro.sync.exml.workspace.api.util.RelativeReferenceResolver))

### addDITAMapTreeTargetInformationProvider

public void addDITAMapTreeTargetInformationProvider([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol, [TopicRefTargetInfoProvider](../../../../exml/workspace/api/standalone/ditamap/TopicRefTargetInfoProvider.md) targetInformationProvider)

Add a provider which can resolve certain information for each topic ref, without the component needing to parse that topic reference.
  Parameters: protocol - The protocol for which the provider is registered targetInformationProvider - The topic reference target information provider provider. Since: 14
### setMathFlowFixedLicenseKeyForEditor

public void setMathFlowFixedLicenseKeyForEditor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fixedKey)

Set a fixed key for licensing the MathFlow editor dialog used to edit embedded MathML equations.
  Specified by: [setMathFlowFixedLicenseKeyForEditor](../../../../exml/workspace/api/math/MathFlowConfigurator.md#setMathFlowFixedLicenseKeyForEditor(java.lang.String)) in interface [MathFlowConfigurator](../../../../exml/workspace/api/math/MathFlowConfigurator.md) Parameters: fixedKey - The fixed key. The key needs to be obtained from MathFlow: http://dessci.com/ and has the following format: MFSCKKK-KKKKKK-KKKKK If no editor key will be given then MathFlow will be used neither for editing nor for rendering. Since: 14
### setMathFlowFixedLicenseKeyForComposer

public void setMathFlowFixedLicenseKeyForComposer([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fixedKey)

Set a fixed key for licensing the MathFlow composer used to view embedded MathML equations.
  Specified by: [setMathFlowFixedLicenseKeyForComposer](../../../../exml/workspace/api/math/MathFlowConfigurator.md#setMathFlowFixedLicenseKeyForComposer(java.lang.String)) in interface [MathFlowConfigurator](../../../../exml/workspace/api/math/MathFlowConfigurator.md) Parameters: fixedKey - The fixed key. The key needs to be obtained from MathFlow: http://dessci.com/ and has the following format: MFSEKKK-KKKKKK-KKKKK If no composer key will be given then the fallback for rendering will be the Apache JEuclid library. Since: 14
### setMathFlowFixedLicenseFile

public void setMathFlowFixedLicenseFile([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) licenseFile)

Set the path to a license file.
  Specified by: [setMathFlowFixedLicenseFile](../../../../exml/workspace/api/math/MathFlowConfigurator.md#setMathFlowFixedLicenseFile(java.io.File)) in interface [MathFlowConfigurator](../../../../exml/workspace/api/math/MathFlowConfigurator.md) Parameters: licenseFile - The path to the MathFlow license file. If the file contains both a license for the composer and for the editor, then both rendering and editing is supported. If the file contains a license only for the editor, rendering will be done using the open source JEuclid library. Since: 16
### setMathFlowInstallationFolder

public void setMathFlowInstallationFolder([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) installationFolder)

Set the path to the MathFlow installation folder.
  Specified by: [setMathFlowInstallationFolder](../../../../exml/workspace/api/math/MathFlowConfigurator.md#setMathFlowInstallationFolder(java.io.File)) in interface [MathFlowConfigurator](../../../../exml/workspace/api/math/MathFlowConfigurator.md) Parameters: installationFolder - The MathFlow installation folder Since: 16
### getXMLUtilAccess

public [XMLUtilAccess](../../../../exml/workspace/api/util/XMLUtilAccess.md) getXMLUtilAccess()

Access to XML utilities.
  Returns: Access to XML utilities. Since: 14.2
### getUtilAccess

public [UtilAccess](../../../../exml/workspace/api/util/UtilAccess.md) getUtilAccess()

Get access to utility methods.
  Returns: access to utility methods. Since: 14.2
### getPluginToolbarCustomizers

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ToolbarComponentsCustomizer](../../../../exml/workspace/api/standalone/ToolbarComponentsCustomizer.md)> getPluginToolbarCustomizers()

Get the toolbar customizers which were added by all installed plugins.
  Returns: Returns the toolbar customizers which were added by all installed plugins. Since: 14.2
### getPluginViewCustomizers

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ViewComponentCustomizer](../../../../exml/workspace/api/standalone/ViewComponentCustomizer.md)> getPluginViewCustomizers()

Get the view customizers which were added by all the installed plugins.
  Returns: Returns the view customizers which were added by all installed plugins. Since: 14.2
### getPluginMenubarCustomizers

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[MenuBarCustomizer](../../../../exml/workspace/api/standalone/MenuBarCustomizer.md)> getPluginMenubarCustomizers()

Get the menu bar customizers which were added by all the installed plugins.
  Returns: Returns the menu bar customizers which were added by all installed plugins. Since: 14.2
### setDITAKeyDefinitionManager

public void setDITAKeyDefinitionManager([KeyDefinitionManager](../../../../exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManager.md) keyDefitionManager)

By default key definitions are gathered from DITA Maps opened in the DITA Maps Manager. This API can be used by the developer to take control over the key definitions which will be used to resolve keyrefs and conkeyrefs for topics opened in the Author page.
  Parameters: keyDefitionManager - The key definition manager Since: 15
### getWorkspaceUtilities

public [WorkspaceUtilities](../../../../exml/workspace/api/WorkspaceUtilities.md) getWorkspaceUtilities()

Get access to various workspace utilities.
  Returns: Access to various workspace utilities. Since: 15
### getPluginWorkspace

public [PluginWorkspace](../../../../exml/workspace/api/PluginWorkspace.md) getPluginWorkspace()

Get access to API used to control the created editor components. This API may not implement all the functionality available in the standalone editor.
  Returns: Returns the pluginWorkspace. Since: 16
### setParentFrame

public void setParentFrame([Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) parentFrame)

Set the parent frame to the Author Component Factory. Will be used as a parent when dialogs are shown from framework-related actions.
  Parameters: parentFrame - The parent frame. Must not be null. Since: 20.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
