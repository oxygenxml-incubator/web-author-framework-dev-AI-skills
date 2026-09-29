Package [ro.sync.ecss.extensions.xhtml](package-summary.md)

# Class XHTMLElementLocatorProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.xhtml.XHTMLElementLocatorProvider
   All Implemented Interfaces: [Extension](../api/Extension.md), [ElementLocatorProvider](../api/link/ElementLocatorProvider.md)   @API(type=INTERNAL, src=PUBLIC) public class XHTMLElementLocatorProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ElementLocatorProvider](../api/link/ElementLocatorProvider.md)
In XHTML the reference can point to an ID type attribute and also to the name attribute of the a element.

## Constructor Summary
 Constructors
Constructor

Description
 [XHTMLElementLocatorProvider](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [ElementLocator](../api/link/ElementLocator.md) [getElementLocator](#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String))([IDTypeVerifier](../api/link/IDTypeVerifier.md) idVerifier, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)
Get an element locator capable of locating the element pointed by this link.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XHTMLElementLocatorProvider

public XHTMLElementLocatorProvider()

## Method Details

### getElementLocator

public [ElementLocator](../api/link/ElementLocator.md) getElementLocator([IDTypeVerifier](../api/link/IDTypeVerifier.md) idVerifier, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)
 Description copied from interface: [ElementLocatorProvider](../api/link/ElementLocatorProvider.md#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String))
Get an element locator capable of locating the element pointed by this link.
  Specified by: [getElementLocator](../api/link/ElementLocatorProvider.md#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String)) in interface [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) Parameters: idVerifier - Verifies if a given attribute type is ID. link - The link that points to the element. Returns: An [ElementLocator](../api/link/ElementLocator.md) capable of locating the element indicated by the given link. See Also:
        * [DefaultElementLocatorProvider.getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier, java.lang.String)](../commons/DefaultElementLocatorProvider.md#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../api/Extension.md#getDescription()) in interface [Extension](../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
