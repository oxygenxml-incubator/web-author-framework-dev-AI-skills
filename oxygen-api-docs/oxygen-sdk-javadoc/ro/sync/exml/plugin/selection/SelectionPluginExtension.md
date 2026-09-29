Package [ro.sync.exml.plugin.selection](package-summary.md)

# Interface SelectionPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface SelectionPluginExtensionextends [PluginExtension](../PluginExtension.md)
Plugin extension. This is intended to work as follows: the user makes a selection in the editor and then goes to the contextual menu and selects from the Plugins entry one of the available plugin modules. The context containing the selection is passed to the process plugin method and the result is processed by the editor eventually replacing the selection. Of course other ways of calling the plugins can be found, like a Plugins main menu for instance.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [SelectionPluginResult](SelectionPluginResult.md) [process](#process(ro.sync.exml.plugin.selection.SelectionPluginContext))([SelectionPluginContext](SelectionPluginContext.md) context)
Main plugin method.

## Method Details

### process

[SelectionPluginResult](SelectionPluginResult.md) process([SelectionPluginContext](SelectionPluginContext.md) context)

Main plugin method. It receives the current context and it should return the processed content.
  Parameters: context - The context the plugin was invoked in. Returns: The processed data or null if it cannot/does not want to process the data.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
