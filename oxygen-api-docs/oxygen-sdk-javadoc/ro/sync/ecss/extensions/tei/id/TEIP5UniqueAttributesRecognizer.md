Package [ro.sync.ecss.extensions.tei.id](package-summary.md)

# Class TEIP5UniqueAttributesRecognizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.id.DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md)
        * ro.sync.ecss.extensions.tei.id.TEIP5UniqueAttributesRecognizer
   All Implemented Interfaces: [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md), [ClipboardFragmentProcessor](../../api/content/ClipboardFragmentProcessor.md), [Extension](../../api/Extension.md), [UniqueAttributesProcessor](../../api/UniqueAttributesProcessor.md), [UniqueAttributesRecognizer](../../api/UniqueAttributesRecognizer.md)   @API(type=INTERNAL, src=PUBLIC) public class TEIP5UniqueAttributesRecognizer extends [DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md)
Unique attributes recognizer

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.id.[DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md)
 [authorAccess](../../commons/id/DefaultUniqueAttributesRecognizer.md#authorAccess), [idAttrQname](../../commons/id/DefaultUniqueAttributesRecognizer.md#idAttrQname)
## Constructor Summary
 Constructors
Constructor

Description
 [TEIP5UniqueAttributesRecognizer](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultOptionsXMLResourceName](#getDefaultOptionsXMLResourceName())()
Get the name of the XML resource from which to load the default options.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

### Methods inherited from class ro.sync.ecss.extensions.commons.id.[DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md)
 [activated](../../commons/id/DefaultUniqueAttributesRecognizer.md#activated(ro.sync.ecss.extensions.api.AuthorAccess)), [assignUniqueIDs](../../commons/id/DefaultUniqueAttributesRecognizer.md#assignUniqueIDs(int,int,boolean)), [copyAttributeOnSplit](../../commons/id/DefaultUniqueAttributesRecognizer.md#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement)), [deactivated](../../commons/id/DefaultUniqueAttributesRecognizer.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess)), [generateUniqueIDFor](../../commons/id/DefaultUniqueAttributesRecognizer.md#generateUniqueIDFor(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement)), [getDefaultOptions](../../commons/id/DefaultUniqueAttributesRecognizer.md#getDefaultOptions()), [getGenerateIDAttributeQName](../../commons/id/DefaultUniqueAttributesRecognizer.md#getGenerateIDAttributeQName(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,boolean)), [getGenerateIDElementsInfo](../../commons/id/DefaultUniqueAttributesRecognizer.md#getGenerateIDElementsInfo()), [isAutoIDGenerationActive](../../commons/id/DefaultUniqueAttributesRecognizer.md#isAutoIDGenerationActive()), [preserveIDsWhenPastingBetweenResources](../../commons/id/DefaultUniqueAttributesRecognizer.md#preserveIDsWhenPastingBetweenResources(int)), [process](../../commons/id/DefaultUniqueAttributesRecognizer.md#process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TEIP5UniqueAttributesRecognizer

public TEIP5UniqueAttributesRecognizer()

Constructor.

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../api/Extension.md#getDescription()) in interface [Extension](../../api/Extension.md) Overrides: [getDescription](../../commons/id/DefaultUniqueAttributesRecognizer.md#getDescription()) in class [DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

### getDefaultOptionsXMLResourceName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultOptionsXMLResourceName()

Get the name of the XML resource from which to load the default options.
  Overrides: [getDefaultOptionsXMLResourceName](../../commons/id/DefaultUniqueAttributesRecognizer.md#getDefaultOptionsXMLResourceName()) in class [DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md) Returns: the name of the XML resource from which to load the default options.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
