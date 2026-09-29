Package [ro.sync.exml.workspace.api.componentscollector](package-summary.md)

# Interface IComponentsProvider
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface IComponentsProvider
The components provider interface.
  Since: 27
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[IComponentInfo](IComponentInfo.md)> [getAllComponents](#getAllComponents(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorUrl)
Get all components from the editor of the specified URL.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[INamespaceInfo](INamespaceInfo.md)> [getAllNamespaces](#getAllNamespaces(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorUrl)
Get all namespaces from the editor of the specified URL.

## Method Details

### getAllComponents

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[IComponentInfo](IComponentInfo.md)> getAllComponents([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorUrl)

Get all components from the editor of the specified URL.
  Parameters: editorUrl - The editor URL. Returns: The list of components. Might be null if the editor is not opened for editing in TEXT page.
### getAllNamespaces

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[INamespaceInfo](INamespaceInfo.md)> getAllNamespaces([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorUrl)

Get all namespaces from the editor of the specified URL.
  Parameters: editorUrl - The editor URL. Returns: The list of namespaces. Might be null if the editor is not opened for editing in TEXT page.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
