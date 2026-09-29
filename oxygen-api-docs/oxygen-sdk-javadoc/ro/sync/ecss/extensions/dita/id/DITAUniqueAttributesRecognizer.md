Package [ro.sync.ecss.extensions.dita.id](package-summary.md)

# Class DITAUniqueAttributesRecognizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.id.DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md)
        * ro.sync.ecss.extensions.dita.id.DITAUniqueAttributesRecognizer
   All Implemented Interfaces: [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md), [ClipboardFragmentProcessor](../../api/content/ClipboardFragmentProcessor.md), [Extension](../../api/Extension.md), [UniqueAttributesProcessor](../../api/UniqueAttributesProcessor.md), [UniqueAttributesRecognizer](../../api/UniqueAttributesRecognizer.md)   @API(type=INTERNAL, src=PUBLIC) public class DITAUniqueAttributesRecognizer extends [DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md)
Unique attributes recognizer for DITA.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.id.[DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md)
 [authorAccess](../../commons/id/DefaultUniqueAttributesRecognizer.md#authorAccess), [idAttrQname](../../commons/id/DefaultUniqueAttributesRecognizer.md#idAttrQname)
## Constructor Summary
 Constructors
Constructor

Description
 [DITAUniqueAttributesRecognizer](#%3Cinit%3E())()
Constructor

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [copyAttributeOnSplit](#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrQName, [AuthorElement](../../api/node/AuthorElement.md) element)
Checks if the attribute specified by QName can be considered as a valid attribute to copy when the element is split.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getGenerateIDAttributeQName](#getGenerateIDAttributeQName(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,boolean))([AuthorElement](../../api/node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elemsWithAutoGeneration, boolean forceGeneration)

 void [process](#process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation))([ClipboardFragmentInformation](../../api/content/ClipboardFragmentInformation.md) fragmentInformation)
Process a fragment in the clipboard before inserting it in the document.

### Methods inherited from class ro.sync.ecss.extensions.commons.id.[DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md)
 [activated](../../commons/id/DefaultUniqueAttributesRecognizer.md#activated(ro.sync.ecss.extensions.api.AuthorAccess)), [assignUniqueIDs](../../commons/id/DefaultUniqueAttributesRecognizer.md#assignUniqueIDs(int,int,boolean)), [deactivated](../../commons/id/DefaultUniqueAttributesRecognizer.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess)), [generateUniqueIDFor](../../commons/id/DefaultUniqueAttributesRecognizer.md#generateUniqueIDFor(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement)), [getDefaultOptions](../../commons/id/DefaultUniqueAttributesRecognizer.md#getDefaultOptions()), [getDefaultOptionsXMLResourceName](../../commons/id/DefaultUniqueAttributesRecognizer.md#getDefaultOptionsXMLResourceName()), [getGenerateIDElementsInfo](../../commons/id/DefaultUniqueAttributesRecognizer.md#getGenerateIDElementsInfo()), [isAutoIDGenerationActive](../../commons/id/DefaultUniqueAttributesRecognizer.md#isAutoIDGenerationActive()), [preserveIDsWhenPastingBetweenResources](../../commons/id/DefaultUniqueAttributesRecognizer.md#preserveIDsWhenPastingBetweenResources(int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAUniqueAttributesRecognizer

public DITAUniqueAttributesRecognizer()

Constructor

## Method Details

### copyAttributeOnSplit

public boolean copyAttributeOnSplit([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrQName, [AuthorElement](../../api/node/AuthorElement.md) element)
 Description copied from interface: [UniqueAttributesProcessor](../../api/UniqueAttributesProcessor.md#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))
Checks if the attribute specified by QName can be considered as a valid attribute to copy when the element is split.
  Specified by: [copyAttributeOnSplit](../../api/UniqueAttributesProcessor.md#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [UniqueAttributesProcessor](../../api/UniqueAttributesProcessor.md) Overrides: [copyAttributeOnSplit](../../commons/id/DefaultUniqueAttributesRecognizer.md#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement)) in class [DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md) Parameters: attrQName - The attribute qualified name. element - The element. Returns: true if the attribute should be copied when Split is performed. See Also:
        * [DefaultUniqueAttributesRecognizer.copyAttributeOnSplit(java.lang.String, ro.sync.ecss.extensions.api.node.AuthorElement)](../../commons/id/DefaultUniqueAttributesRecognizer.md#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../api/Extension.md#getDescription()) in interface [Extension](../../api/Extension.md) Overrides: [getDescription](../../commons/id/DefaultUniqueAttributesRecognizer.md#getDescription()) in class [DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

### getGenerateIDAttributeQName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getGenerateIDAttributeQName([AuthorElement](../../api/node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elemsWithAutoGeneration, boolean forceGeneration)
  Overrides: [getGenerateIDAttributeQName](../../commons/id/DefaultUniqueAttributesRecognizer.md#getGenerateIDAttributeQName(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,boolean)) in class [DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md) Parameters: element - The current element. elemsWithAutoGeneration - The array of elements for which generation is activated forceGeneration - Force ID generation if there is no selection. Returns: The name of the attribute for which to generate the ID or null (default behavior). See Also:
        * [DefaultUniqueAttributesRecognizer.getGenerateIDAttributeQName(ro.sync.ecss.extensions.api.node.AuthorElement, java.lang.String[], boolean)](../../commons/id/DefaultUniqueAttributesRecognizer.md#getGenerateIDAttributeQName(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,boolean))

### process

public void process([ClipboardFragmentInformation](../../api/content/ClipboardFragmentInformation.md) fragmentInformation)
 Description copied from interface: [ClipboardFragmentProcessor](../../api/content/ClipboardFragmentProcessor.md#process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation))
Process a fragment in the clipboard before inserting it in the document.
  Specified by: [process](../../api/content/ClipboardFragmentProcessor.md#process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation)) in interface [ClipboardFragmentProcessor](../../api/content/ClipboardFragmentProcessor.md) Overrides: [process](../../commons/id/DefaultUniqueAttributesRecognizer.md#process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation)) in class [DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md) Parameters: fragmentInformation - Information about a fragment in the clipboard. See Also:
        * [DefaultUniqueAttributesRecognizer.process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation)](../../commons/id/DefaultUniqueAttributesRecognizer.md#process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
