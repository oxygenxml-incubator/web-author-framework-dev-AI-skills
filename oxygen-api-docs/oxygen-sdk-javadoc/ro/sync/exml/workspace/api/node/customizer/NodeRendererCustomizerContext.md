Package [ro.sync.exml.workspace.api.node.customizer](package-summary.md)

# Class NodeRendererCustomizerContext

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.workspace.api.node.NodeContext](../NodeContext.md)
        * ro.sync.exml.workspace.api.node.customizer.NodeRendererCustomizerContext
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public abstract class NodeRendererCustomizerContext extends [NodeContext](../NodeContext.md)
Provide information like node name, node namespace, attributes (if available), that will be used for Author outline, Author bread crumb, Text page outline, content completion proposals window or DITA Map view rendering customization.
  Since: 13.2
## Constructor Summary
 Constructors
Constructor

Description
 [NodeRendererCustomizerContext](#%3Cinit%3E())()

## Method Summary

### Methods inherited from class ro.sync.exml.workspace.api.node.[NodeContext](../NodeContext.md)
 [getAttributeNamespace](../NodeContext.md#getAttributeNamespace(java.lang.String)), [getAttributeQName](../NodeContext.md#getAttributeQName(int)), [getAttributesCount](../NodeContext.md#getAttributesCount()), [getAttributeValue](../NodeContext.md#getAttributeValue(java.lang.String)), [getNodeName](../NodeContext.md#getNodeName()), [getNodeNamespace](../NodeContext.md#getNodeNamespace()), [getParentNodeName](../NodeContext.md#getParentNodeName()), [getParentNodeNamespace](../NodeContext.md#getParentNodeNamespace())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### NodeRendererCustomizerContext

public NodeRendererCustomizerContext()

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
