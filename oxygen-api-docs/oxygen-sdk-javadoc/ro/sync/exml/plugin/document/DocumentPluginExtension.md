Package [ro.sync.exml.plugin.document](package-summary.md)

# Interface DocumentPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface DocumentPluginExtensionextends [PluginExtension](../PluginExtension.md)
Plugin extension. The document plugin can be called from the contextual menu. The context containing the document is passed to the plugin process method and the result is processed by the editor.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [DocumentPluginResult](DocumentPluginResult.md) [process](#process(ro.sync.exml.plugin.document.DocumentPluginContext))([DocumentPluginContext](DocumentPluginContext.md) context)
Main plugin method.

## Method Details

### process

[DocumentPluginResult](DocumentPluginResult.md) process([DocumentPluginContext](DocumentPluginContext.md) context)

Main plugin method. It receives the current context and it should return the processed content.
  Parameters: context - The context the plugin was invoked in. Returns: The processed data or null if it cannot/does not want to process the data.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
