Package [ro.sync.ecss.extensions.api.link](package-summary.md)

# Interface ElementLocatorProvider
    All Superinterfaces: [Extension](../Extension.md)   All Known Implementing Classes: [DefaultElementLocatorProvider](../../commons/DefaultElementLocatorProvider.md), [DITAElementLocatorProvider](../../dita/DITAElementLocatorProvider.md), [XHTMLElementLocatorProvider](../../xhtml/XHTMLElementLocatorProvider.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface ElementLocatorProviderextends [Extension](../Extension.md)
This class is able to provide an implementation of an [ElementLocator](ElementLocator.md) based on the structure of a link. The [ElementLocator](ElementLocator.md) is capable of locating an element pointed by the supplied link.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [ElementLocator](ElementLocator.md) [getElementLocator](#getElementLocator(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String))([IDTypeVerifier](IDTypeVerifier.md) idVerifier, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)
Get an element locator capable of locating the element pointed by this link.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../Extension.md)
 [getDescription](../Extension.md#getDescription())
## Method Details

### getElementLocator

[ElementLocator](ElementLocator.md) getElementLocator([IDTypeVerifier](IDTypeVerifier.md) idVerifier, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)

Get an element locator capable of locating the element pointed by this link.
  Parameters: idVerifier - Verifies if a given attribute type is ID. link - The link that points to the element. Returns: An [ElementLocator](ElementLocator.md) capable of locating the element indicated by the given link.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
