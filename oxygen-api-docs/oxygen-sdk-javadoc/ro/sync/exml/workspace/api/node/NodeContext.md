Package [ro.sync.exml.workspace.api.node](package-summary.md)

# Class NodeContext

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.node.NodeContext
   Direct Known Subclasses: [NodeRendererCustomizerContext](customizer/NodeRendererCustomizerContext.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public abstract class NodeContext extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Provide information like node name, node namespace, attributes (if available), that will be used for Author outline, Author bread crumb, Text page outline, content completion proposals window or DITA Map view rendering customization.
  Since: 15.2
## Constructor Summary
 Constructors
Constructor

Description
 [NodeContext](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeNamespace](#getAttributeNamespace(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrQName)
Get namespace URI for a given attribute qualified name.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeQName](#getAttributeQName(int))(int index)
Get the qualified attribute name at index.
  abstract int [getAttributesCount](#getAttributesCount())()
Returns the number of the element attributes.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeValue](#getAttributeValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrQName)
Get attribute value for given attribute qualified name.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNodeName](#getNodeName())()
Get the node name.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNodeNamespace](#getNodeNamespace())()
Get the node namespace.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getParentNodeName](#getParentNodeName())()
Get the parent node name.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getParentNodeNamespace](#getParentNodeNamespace())()
Get the parent node namespace.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### NodeContext

public NodeContext()

## Method Details

### getNodeName

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNodeName()

Get the node name.
  Returns: Returns the node name.
### getNodeNamespace

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNodeNamespace()

Get the node namespace.
  Returns: Returns the node namespace.
### getParentNodeName

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getParentNodeName()

Get the parent node name.
  Returns: Returns the parent node name.
### getParentNodeNamespace

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getParentNodeNamespace()

Get the parent node namespace.
  Returns: Returns the parent node namespace.
### getAttributesCount

public abstract int getAttributesCount()

Returns the number of the element attributes.
  Returns: The number of the element attributes.
### getAttributeQName

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeQName(int index)

Get the qualified attribute name at index.
  Parameters: index - Index of the attribute. Returns: The qualified attribute name at index.
### getAttributeValue

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrQName)

Get attribute value for given attribute qualified name.
  Parameters: attrQName - The qualified attribute name. Returns: The attribute value.
### getAttributeNamespace

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeNamespace([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrQName)

Get namespace URI for a given attribute qualified name.
  Parameters: attrQName - The attribute qualified name. Returns: The attribute namespace URI.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
