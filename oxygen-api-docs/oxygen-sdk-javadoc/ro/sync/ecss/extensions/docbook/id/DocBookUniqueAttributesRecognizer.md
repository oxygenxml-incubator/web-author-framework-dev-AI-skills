Package [ro.sync.ecss.extensions.docbook.id](package-summary.md)

# Class DocBookUniqueAttributesRecognizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.id.DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md)
        * ro.sync.ecss.extensions.docbook.id.DocBookUniqueAttributesRecognizer
   All Implemented Interfaces: [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md), [ClipboardFragmentProcessor](../../api/content/ClipboardFragmentProcessor.md), [Extension](../../api/Extension.md), [UniqueAttributesProcessor](../../api/UniqueAttributesProcessor.md), [UniqueAttributesRecognizer](../../api/UniqueAttributesRecognizer.md)   Direct Known Subclasses: [Docbook4UniqueAttributesRecognizer](Docbook4UniqueAttributesRecognizer.md), [Docbook5UniqueAttributesRecognizer](Docbook5UniqueAttributesRecognizer.md)   @API(type=INTERNAL, src=PUBLIC) public class DocBookUniqueAttributesRecognizer extends [DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md)
Unique attributes recognizer for DocBook.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.id.[DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md)
 [authorAccess](../../commons/id/DefaultUniqueAttributesRecognizer.md#authorAccess), [idAttrQname](../../commons/id/DefaultUniqueAttributesRecognizer.md#idAttrQname)
## Constructor Summary
 Constructors
Constructor

Description
 [DocBookUniqueAttributesRecognizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [preserveIDsWhenPastingBetweenResources](#preserveIDsWhenPastingBetweenResources(int))(int fragmentPurpose)
Check if we should preserve IDs when pasting between resources.

### Methods inherited from class ro.sync.ecss.extensions.commons.id.[DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md)
 [activated](../../commons/id/DefaultUniqueAttributesRecognizer.md#activated(ro.sync.ecss.extensions.api.AuthorAccess)), [assignUniqueIDs](../../commons/id/DefaultUniqueAttributesRecognizer.md#assignUniqueIDs(int,int,boolean)), [copyAttributeOnSplit](../../commons/id/DefaultUniqueAttributesRecognizer.md#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement)), [deactivated](../../commons/id/DefaultUniqueAttributesRecognizer.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess)), [generateUniqueIDFor](../../commons/id/DefaultUniqueAttributesRecognizer.md#generateUniqueIDFor(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement)), [getDefaultOptions](../../commons/id/DefaultUniqueAttributesRecognizer.md#getDefaultOptions()), [getDefaultOptionsXMLResourceName](../../commons/id/DefaultUniqueAttributesRecognizer.md#getDefaultOptionsXMLResourceName()), [getDescription](../../commons/id/DefaultUniqueAttributesRecognizer.md#getDescription()), [getGenerateIDAttributeQName](../../commons/id/DefaultUniqueAttributesRecognizer.md#getGenerateIDAttributeQName(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,boolean)), [getGenerateIDElementsInfo](../../commons/id/DefaultUniqueAttributesRecognizer.md#getGenerateIDElementsInfo()), [isAutoIDGenerationActive](../../commons/id/DefaultUniqueAttributesRecognizer.md#isAutoIDGenerationActive()), [process](../../commons/id/DefaultUniqueAttributesRecognizer.md#process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DocBookUniqueAttributesRecognizer

public DocBookUniqueAttributesRecognizer()

## Method Details

### preserveIDsWhenPastingBetweenResources

protected boolean preserveIDsWhenPastingBetweenResources(int fragmentPurpose)
 Description copied from class: [DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md#preserveIDsWhenPastingBetweenResources(int))
Check if we should preserve IDs when pasting between resources.
  Overrides: [preserveIDsWhenPastingBetweenResources](../../commons/id/DefaultUniqueAttributesRecognizer.md#preserveIDsWhenPastingBetweenResources(int)) in class [DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md) Parameters: fragmentPurpose - The fragment purpose. On of the [AuthorSchemaAwareEditingHandler](../../api/AuthorSchemaAwareEditingHandler.md) purposes. Returns: true if we should preserve IDs when pasting between resources. By default the base method returns true. See Also:
        * [DefaultUniqueAttributesRecognizer.preserveIDsWhenPastingBetweenResources(int)](../../commons/id/DefaultUniqueAttributesRecognizer.md#preserveIDsWhenPastingBetweenResources(int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
