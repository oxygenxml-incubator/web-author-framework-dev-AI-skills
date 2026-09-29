Package [ro.sync.exml.plugin.option](package-summary.md)

# Class OptionPagePluginExtension

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.plugin.option.OptionPagePluginExtension
   All Implemented Interfaces: [PluginExtension](../PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class OptionPagePluginExtension extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [PluginExtension](../PluginExtension.md)
Class used to create plugin option page extension. It receives callbacks for saving options, restoring default options and loading options. The GUI for this option page must be built in order to associated the options with their corresponding GUI components.
  Since: 15
## Constructor Summary
 Constructors
Constructor

Description
 [OptionPagePluginExtension](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract void [apply](#apply(ro.sync.exml.workspace.api.PluginWorkspace))([PluginWorkspace](../../workspace/api/PluginWorkspace.md) pluginWorkspace)
This method is called when "Apply" or "OK" button are pressed in from the GUI option page.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageURL](#getHelpPageURL())()
Get the help URL for this page.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getKey](#getKey())()
Retrieves the option page key.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getProjectLevelOptionKeys](#getProjectLevelOptionKeys())()
The options that will be saved inside the project file when this page is switched to project level inside the preferences dialog.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTitle](#getTitle())()
Retrieves the option page title.
  abstract [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) [init](#init(ro.sync.exml.workspace.api.PluginWorkspace))([PluginWorkspace](../../workspace/api/PluginWorkspace.md) pluginWorkspace)
Initializes the GUI for the option page and loads the stored option values.This method may be called multiple times on the same "OptionPagePluginExtension" implementation.For example it's called when the end user cancels the "Preferences" dialog and you need to reload your custom UI settings from the options storage.So you could for example create the custom Swing component only when the first "init" is called and on subsequent calls return the already created component.But on each "init" callback you always need to reload your page's GUI settings (e.g.
  abstract void [restoreDefaults](#restoreDefaults())()
This method is called when "Restore defaults" button is pressed from the GUI option page.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### OptionPagePluginExtension

public OptionPagePluginExtension()

## Method Details

### apply

public abstract void apply([PluginWorkspace](../../workspace/api/PluginWorkspace.md) pluginWorkspace)

This method is called when "Apply" or "OK" button are pressed in from the GUI option page. All options associated with the option page must be saved on this method.
  Parameters: pluginWorkspace - Access the entire workspace of Oxygen. It can be used to retrieve the [OptionsStorage](../../../ecss/extensions/api/OptionsStorage.md) and perform options save operations on it.
### restoreDefaults

public abstract void restoreDefaults()

This method is called when "Restore defaults" button is pressed from the GUI option page. All options associated with the option page must be restored to their default values.

### getTitle

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTitle()

Retrieves the option page title.
  Returns: The option page title used in GUI.
### getKey

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getKey()

Retrieves the option page key. Can be overridden in order to pass the returned value to [GlobalOptionsStorage.showPreferencesPages(String[], String, boolean)](../../workspace/api/options/GlobalOptionsStorage.md#showPreferencesPages(java.lang.String%5B%5D,java.lang.String,boolean)), which is used for displaying the preferences dialog with certain pages in the table of contents.
  Returns: The option page key. Since: 17.1
### init

public abstract [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) init([PluginWorkspace](../../workspace/api/PluginWorkspace.md) pluginWorkspace)

Initializes the GUI for the option page and loads the stored option values.This method may be called multiple times on the same "OptionPagePluginExtension" implementation.For example it's called when the end user cancels the "Preferences" dialog and you need to reload your custom UI settings from the options storage.So you could for example create the custom Swing component only when the first "init" is called and on subsequent calls return the already created component.But on each "init" callback you always need to reload your page's GUI settings (e.g. checkboxes) from the option stored in the options storage. (ro.sync.exml.workspace.api.PluginWorkspace.getOptionsStorage()).If certain settings can also be changed in other parts of the code, on the first "init" callback you can add an options storage listener (ro.sync.exml.workspace.api.options.WSOptionsStorage.addOptionListener(WSOptionListener)) and update your UI's settingswhen the stored keys are changed in other parts of the code.
  Parameters: pluginWorkspace - Access the entire workspace of Oxygen. It can be used to retrieve the [OptionsStorage](../../../ecss/extensions/api/OptionsStorage.md) and perform options save/load operations it. Returns: The GUI component of the option page.
### getProjectLevelOptionKeys

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getProjectLevelOptionKeys()

The options that will be saved inside the project file when this page is switched to project level inside the preferences dialog.
  Returns: The options presented in this page. Since: 24.0
### getHelpPageURL

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageURL()

Get the help URL for this page. Use null if no help page is available for the dialog (no help is shown).
  Returns: the help URL for this page. If not needed please return null. Since: 27.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
