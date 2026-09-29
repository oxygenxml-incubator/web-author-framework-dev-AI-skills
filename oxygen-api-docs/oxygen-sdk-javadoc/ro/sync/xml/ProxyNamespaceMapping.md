Package [ro.sync.xml](package-summary.md)

# Class ProxyNamespaceMapping

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.basic.xml.ProxyNamespaceMapping
        * ro.sync.xml.ProxyNamespaceMapping
   All Implemented Interfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)   @API(type=EXTENDABLE, src=PRIVATE) public class ProxyNamespaceMapping extends ro.sync.basic.xml.ProxyNamespaceMapping
Stores the mappings between the namespace prefixes and the URI's. It is mainly used in the content completion process. The implementation consists in two lists. The modifying operations are performed at the end of the lists. Note that duplicates can exist in the mappings.

## Field Summary

### Fields inherited from class ro.sync.basic.xml.ProxyNamespaceMapping
 namespaces, prefixes
## Constructor Summary
 Constructors
Modifier

Constructor

Description
   [ProxyNamespaceMapping](#%3Cinit%3E())()
Constructor.
  protected  [ProxyNamespaceMapping](#%3Cinit%3E(java.util.List,java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> prefixies, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> namespaces)
Private constructor.
    [ProxyNamespaceMapping](#%3Cinit%3E(org.w3c.dom.Node))([Node](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/w3c/dom/Node.html) node)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()
Clones the prefix namespace mapping.
  protected [ProxyNamespaceMapping](ProxyNamespaceMapping.md) [createProxyNamespaceMapping](#createProxyNamespaceMapping())()

 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

### Methods inherited from class ro.sync.basic.xml.ProxyNamespaceMapping
 addMapping, clear, getMappingsFromAncestor, getNamespaceForAttributePrefix, getNamespaceForPrefix, getNamespaces, getPrefixesForNamespace, getPrefixesForNamespace, getPrefixForAttributeNamespace, getPrefixForNamespace, getPrefixForNamespace, getProxies, removeByNamespace, removeByPrefix, removeLastMapping, toString, update, updateNamespaceProxyMapping
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ProxyNamespaceMapping

public ProxyNamespaceMapping([Node](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/w3c/dom/Node.html) node)

Constructor. Adds the default namespace mapping.
  Parameters: node - The context node, DOM Level 1, the prefix namespace mapping will be populated based on the xmlns attributes, starting with the root element.
### ProxyNamespaceMapping

protected ProxyNamespaceMapping([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> prefixies, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> namespaces)

Private constructor. Used to clone a prefix-namespace mapping.
  Parameters: prefixies - The prefixes list. namespaces - The namespaces list.
### ProxyNamespaceMapping

public ProxyNamespaceMapping()

Constructor. Adds the default namespace.

## Method Details

### createProxyNamespaceMapping

protected [ProxyNamespaceMapping](ProxyNamespaceMapping.md) createProxyNamespaceMapping()
  Overrides: createProxyNamespaceMapping in class ro.sync.basic.xml.ProxyNamespaceMapping
### clone

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone()

Clones the prefix namespace mapping.
  Overrides: clone in class ro.sync.basic.xml.ProxyNamespaceMapping
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
