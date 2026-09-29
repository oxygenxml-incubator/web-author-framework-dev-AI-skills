Package [ro.sync.ecss.extensions.commons](package-summary.md)

# Class DefaultElementLocatorProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.DefaultElementLocatorProvider
   All Implemented Interfaces: [Extension](../api/Extension.md), [ElementLocatorProvider](../api/link/ElementLocatorProvider.md)   Direct Known Subclasses: [DITAElementLocatorProvider](../dita/DITAElementLocatorProvider.md)   @API(type=INTERNAL, src=PUBLIC) public class DefaultElementLocatorProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ElementLocatorProvider](../api/link/ElementLocatorProvider.md)
Default implementation for locating elements based on a given link. Depending on the link structure the following cases are covered: - XInclude element scheme : element(/1/2)  see [http://www.w3.org/TR/2003/REC-xptr-element-20030325/](http://www.w3.org/TR/2003/REC-xptr-element-20030325/) - ID based links : the link represents the value of an attribute of type ID.

## Constructor Summary
 Constructors
Constructor

Description
 [DefaultElementLocatorProvider](#%3Cinit%3E())()

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

### DefaultElementLocatorProvider

public DefaultElementLocatorProvider()

## Method Details

### getElementLocator

public [ElementLocator](../api/link/ElementLocator.md) getElementLocator([IDTypeVerifier](../api/link/IDTypeVerifier.md) idVerifier, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)
 Description copied from interface: [ElementLocatorProvider](../api/link/ElementLocatorProvider.md#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String))
Get an element locator capable of locating the element pointed by this link.
  Specified by: [getElementLocator](../api/link/ElementLocatorProvider.md#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String)) in interface [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) Parameters: idVerifier - Verifies if a given attribute type is ID. link - The link that points to the element. Returns: An [ElementLocator](../api/link/ElementLocator.md) capable of locating the element indicated by the given link. See Also:
        * [ElementLocatorProvider.getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier, java.lang.String)](../api/link/ElementLocatorProvider.md#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../api/Extension.md#getDescription()) in interface [Extension](../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
