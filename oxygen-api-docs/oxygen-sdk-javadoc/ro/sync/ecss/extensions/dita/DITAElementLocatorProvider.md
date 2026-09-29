Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DITAElementLocatorProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.DefaultElementLocatorProvider](../commons/DefaultElementLocatorProvider.md)
        * ro.sync.ecss.extensions.dita.DITAElementLocatorProvider
   All Implemented Interfaces: [Extension](../api/Extension.md), [ElementLocatorProvider](../api/link/ElementLocatorProvider.md)   @API(type=INTERNAL, src=PUBLIC) public class DITAElementLocatorProvider extends [DefaultElementLocatorProvider](../commons/DefaultElementLocatorProvider.md)
Implementation for locating elements based on a link from a DITA document. See:  [http://docs.oasis-open.org/dita/v1.0/langspec/relatedl.html ](http://docs.oasis-open.org/dita/v1.0/langspec/relatedl.html)  [http://docs.oasis-open.org/dita/v1.1/OS/langspec/common/theconrefattribute.html ](http://docs.oasis-open.org/dita/v1.1/OS/langspec/common/theconrefattribute.html)  [http://docs.oasis-open.org/dita/v1.0/langspec/xref.html ](http://docs.oasis-open.org/dita/v1.0/langspec/xref.html)

## Constructor Summary
 Constructors
Constructor

Description
 [DITAElementLocatorProvider](#%3Cinit%3E())()
Default constructor.
  [DITAElementLocatorProvider](#%3Cinit%3E(boolean))(boolean locateInsideDITAMap)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [ElementLocator](../api/link/ElementLocator.md) [getElementLocator](#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String))([IDTypeVerifier](../api/link/IDTypeVerifier.md) idVerifier, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)
Get an element locator capable of locating the element pointed by this link.

### Methods inherited from class ro.sync.ecss.extensions.commons.[DefaultElementLocatorProvider](../commons/DefaultElementLocatorProvider.md)
 [getDescription](../commons/DefaultElementLocatorProvider.md#getDescription())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAElementLocatorProvider

public DITAElementLocatorProvider()

Default constructor.

### DITAElementLocatorProvider

public DITAElementLocatorProvider(boolean locateInsideDITAMap)

Constructor.
  Parameters: locateInsideDITAMap - true if we need to locate inside a DITA Map
## Method Details

### getElementLocator

public [ElementLocator](../api/link/ElementLocator.md) getElementLocator([IDTypeVerifier](../api/link/IDTypeVerifier.md) idVerifier, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)
 Description copied from interface: [ElementLocatorProvider](../api/link/ElementLocatorProvider.md#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String))
Get an element locator capable of locating the element pointed by this link.
  Specified by: [getElementLocator](../api/link/ElementLocatorProvider.md#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String)) in interface [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) Overrides: [getElementLocator](../commons/DefaultElementLocatorProvider.md#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String)) in class [DefaultElementLocatorProvider](../commons/DefaultElementLocatorProvider.md) Parameters: idVerifier - Verifies if a given attribute type is ID. link - The link that points to the element. Returns: An [ElementLocator](../api/link/ElementLocator.md) capable of locating the element indicated by the given link. See Also:
        * [DefaultElementLocatorProvider.getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier, java.lang.String)](../commons/DefaultElementLocatorProvider.md#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
