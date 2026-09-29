Package [ro.sync.exml.plugin.ai](package-summary.md)

# Interface AIConnectorsPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AIConnectorsPluginExtensionextends [PluginExtension](../PluginExtension.md)
Plug-in extension that provides external AI connectors to AI services
  Since: 27.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<com.oxygenxml.positron.api.connector.AIConnector> [getExternalAIConnectors](#getExternalAIConnectors())()
Get the custom/external AI connectors to external AI services.

## Method Details

### getExternalAIConnectors

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<com.oxygenxml.positron.api.connector.AIConnector> getExternalAIConnectors()

Get the custom/external AI connectors to external AI services.
  Returns: The custom AI connectors to external AI services.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
