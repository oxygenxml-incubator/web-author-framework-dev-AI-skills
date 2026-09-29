Package [ro.sync.exml.plugin.urlstreamhandler](package-summary.md)

# Interface URLChooserPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md), [URLChooserMenuExtension](URLChooserMenuExtension.md)   [@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html)@API(type=EXTENDABLE, src=PUBLIC) public interface URLChooserPluginExtensionextends [URLChooserMenuExtension](URLChooserMenuExtension.md), [PluginExtension](../PluginExtension.md) Deprecated.
This approach will continue to work but it is recommanded to use the **ro.sync.exml.plugin.urlstreamhandler.URLChooserPluginExtension2** interface which also receives access to the Oxygen workspace.

URL chooser plugin extension. Allows the user to browse a repository of resources (usually by displaying a chooser dialog) and to select one or more resources for opening in Oxygen.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] [chooseURLs](#chooseURLs())()  Deprecated.
Choose a set of URLs with the corresponding protocol.

### Methods inherited from interface ro.sync.exml.plugin.urlstreamhandler.[URLChooserMenuExtension](URLChooserMenuExtension.md)
 [getMenuName](URLChooserMenuExtension.md#getMenuName())
## Method Details

### chooseURLs

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] chooseURLs()
 Deprecated.
Choose a set of URLs with the corresponding protocol.
  Returns: The chosen array of URLs or null if the user rejects the selection.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
