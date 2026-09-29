Package [ro.sync.exml.plugin.urlstreamhandler](package-summary.md)

# Interface URLChooserPluginExtension2
    All Superinterfaces: [PluginExtension](../PluginExtension.md), [URLChooserMenuExtension](URLChooserMenuExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface URLChooserPluginExtension2extends [URLChooserMenuExtension](URLChooserMenuExtension.md), [PluginExtension](../PluginExtension.md)
URL chooser plugin extension. Allows the user to browse a repository of resources (usually by displaying a chooser dialog) and to select one or more resources for opening in Oxygen. The user can access the entire workspace API.
  Since: 12.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] [chooseURLs](#chooseURLs(ro.sync.exml.workspace.api.standalone.StandalonePluginWorkspace))([StandalonePluginWorkspace](../../workspace/api/standalone/StandalonePluginWorkspace.md) workspaceAccess)
Choose a set of URLs with the corresponding protocol.

### Methods inherited from interface ro.sync.exml.plugin.urlstreamhandler.[URLChooserMenuExtension](URLChooserMenuExtension.md)
 [getMenuName](URLChooserMenuExtension.md#getMenuName())
## Method Details

### chooseURLs

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] chooseURLs([StandalonePluginWorkspace](../../workspace/api/standalone/StandalonePluginWorkspace.md) workspaceAccess)

Choose a set of URLs with the corresponding protocol.
  Parameters: workspaceAccess - Access to the Oxygen workspace. Returns: The chosen array of URLs or null if the user rejects the selection.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
