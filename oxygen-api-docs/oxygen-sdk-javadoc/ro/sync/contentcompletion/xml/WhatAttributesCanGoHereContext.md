Package [ro.sync.contentcompletion.xml](package-summary.md)

# Class WhatAttributesCanGoHereContext

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.contentcompletion.xml.Context](Context.md)
        * ro.sync.contentcompletion.xml.WhatContextInParent
            * ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext
   All Implemented Interfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)   @API(type=EXTENDABLE, src=PRIVATE) public class WhatAttributesCanGoHereContext extends ro.sync.contentcompletion.xml.WhatContextInParent
Used by the schema manager to find out the attributes that can be inserted in a given context.

## Field Summary

### Fields inherited from class ro.sync.contentcompletion.xml.WhatContextInParent
 parentElement
### Fields inherited from class ro.sync.contentcompletion.xml.[Context](Context.md)
 [elementStack](Context.md#elementStack), [idValuesList](Context.md#idValuesList), [infoProvider](Context.md#infoProvider), [nextSiblingElements](Context.md#nextSiblingElements), [prefixNamespaceMapping](Context.md#prefixNamespaceMapping), [previousSiblingElements](Context.md#previousSiblingElements), [xmlReader](Context.md#xmlReader)
## Constructor Summary
 Constructors
Constructor

Description
 [WhatAttributesCanGoHereContext](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()

### Methods inherited from class ro.sync.contentcompletion.xml.WhatContextInParent
 getParentElement, getPreviousAttributeNames, getPreviousAttributes, getPreviousAttributesList, getRootAttributes, pushContextElement, setParentElement, toString
### Methods inherited from class ro.sync.contentcompletion.xml.[Context](Context.md)
 [computeContextXPathExpression](Context.md#computeContextXPathExpression()), [equals](Context.md#equals(java.lang.Object)), [executeXPath](Context.md#executeXPath(java.lang.String,java.lang.String%5B%5D)), [executeXPath](Context.md#executeXPath(java.lang.String,java.lang.String%5B%5D,boolean)), [getDefaultAttributeValue](Context.md#getDefaultAttributeValue(ro.sync.contentcompletion.xml.ContextElement,java.lang.String)), [getElementStack](Context.md#getElementStack()), [getIdValuesList](Context.md#getIdValuesList()), [getNextSiblingElements](Context.md#getNextSiblingElements()), [getPrefixNamespaceMapping](Context.md#getPrefixNamespaceMapping()), [getPreviousSiblingElements](Context.md#getPreviousSiblingElements()), [getProxyNamespaceMapping](Context.md#getProxyNamespaceMapping(ro.sync.contentcompletion.xml.Context)), [getSystemID](Context.md#getSystemID()), [setAdditionalContextInformationProvider](Context.md#setAdditionalContextInformationProvider(ro.sync.contentcompletion.xml.AdditionalContextInformationProvider)), [setElementStack](Context.md#setElementStack(java.util.Stack)), [setIdValuesList](Context.md#setIdValuesList(java.util.List)), [setNextSiblingElements](Context.md#setNextSiblingElements(java.util.List)), [setPrefixNamespaceMapping](Context.md#setPrefixNamespaceMapping(ro.sync.xml.ProxyNamespaceMapping)), [setPreviousSiblingElements](Context.md#setPreviousSiblingElements(java.util.List)), [setXMLReader](Context.md#setXMLReader(org.xml.sax.XMLReader))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WhatAttributesCanGoHereContext

public WhatAttributesCanGoHereContext()

## Method Details

### clone

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone()
  Overrides: clone in class ro.sync.contentcompletion.xml.WhatContextInParent See Also:
        * WhatContextInParent.clone()

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
