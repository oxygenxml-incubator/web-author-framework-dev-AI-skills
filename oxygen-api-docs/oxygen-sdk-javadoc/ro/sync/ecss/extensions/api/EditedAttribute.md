Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface EditedAttribute
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface EditedAttribute
Edited attribute information, like QName, element's QName and the proxy namespace mapping.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeQName](#getAttributeQName())()
The attribute QName.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getParentElementQName](#getParentElementQName())()
The parent element QName.
  [ProxyNamespaceMapping](../../../xml/ProxyNamespaceMapping.md) [getProxyNamespaceMapping](#getProxyNamespaceMapping())()
The proxy namespace mapping.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getValue](#getValue())()
The attribute value.

## Method Details

### getAttributeQName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeQName()

The attribute QName.
  Returns: The attribute QName.
### getParentElementQName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getParentElementQName()

The parent element QName.
  Returns: The parent element qname.
### getProxyNamespaceMapping

[ProxyNamespaceMapping](../../../xml/ProxyNamespaceMapping.md) getProxyNamespaceMapping()

The proxy namespace mapping.
  Returns: The proxy namespace mapping.
### getValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getValue()

The attribute value.
  Returns: The attribute value.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
