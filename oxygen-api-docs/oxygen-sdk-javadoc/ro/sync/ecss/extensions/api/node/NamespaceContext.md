Package [ro.sync.ecss.extensions.api.node](package-summary.md)

# Interface NamespaceContext
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface NamespaceContext
Useful interface which can be used to obtain mappings from prefix to namespace and from namespace to prefix in the context of the current element.
  Since: 13
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNamespaceForPrefix](#getNamespaceForPrefix(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix)
Get the namespace corresponding to a prefix in the current element context.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getNamespaces](#getNamespaces())()
Returns all the namespaces active in the current context.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPrefixForNamespace](#getPrefixForNamespace(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Get the prefix which is bound to a specified namespace in the current element context.

## Method Details

### getNamespaceForPrefix

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNamespaceForPrefix([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix)

Get the namespace corresponding to a prefix in the current element context.
  Parameters: prefix - The prefix. Returns: The namespace corresponding to the prefix or null if no mapping was found.
### getPrefixForNamespace

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPrefixForNamespace([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)

Get the prefix which is bound to a specified namespace in the current element context.
  Parameters: namespace - The namespace. Returns: the prefix which is bound to a specified namespace in the current element context or null if no mapping was found.
### getNamespaces

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getNamespaces()

Returns all the namespaces active in the current context.
  Returns: All the namespaces active in the current context. Since: 18
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
