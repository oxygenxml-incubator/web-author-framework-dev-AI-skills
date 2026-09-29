Package [ro.sync.exml.plugin.ai](package-summary.md)

# Interface AIHooksHandlerPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AIHooksHandlerPluginExtensionextends [PluginExtension](../PluginExtension.md)
Plug-in extension that provides a handler for the AI hooks
  Since: 28.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 com.oxygenxml.positron.api.hook.AIHooksHandler [getHooksHandler](#getHooksHandler())()
Returns the AIHooksHandler instance contributed by this plugin extension.

## Method Details

### getHooksHandler

com.oxygenxml.positron.api.hook.AIHooksHandler getHooksHandler()

Returns the AIHooksHandler instance contributed by this plugin extension.
The returned handler will be registered by the AI integration layer and invoked for each lifecycle hook emitted by Positron (e.g. session start/end, prompt submission, tool invocation events, stop events).

  Returns: the AIHooksHandler implementation provided by this extension; never null
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
