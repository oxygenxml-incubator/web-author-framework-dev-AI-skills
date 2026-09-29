Package [ro.sync.exml.plugin.general](package-summary.md)

# Interface GeneralPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface GeneralPluginExtensionextends [PluginExtension](../PluginExtension.md)
Plugin interface.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [process](#process(ro.sync.exml.plugin.general.GeneralPluginContext))([GeneralPluginContext](GeneralPluginContext.md) context)
Main plugin method.

## Method Details

### process

void process([GeneralPluginContext](GeneralPluginContext.md) context)

Main plugin method. It receives the current context and it should return the processed content.
  Parameters: context - The context the plugin was invoked in.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
