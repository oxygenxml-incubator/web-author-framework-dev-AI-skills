Package [ro.sync.ecss.extensions.commons.id](package-summary.md)

# Class DefaultUniqueAttributesRecognizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.id.DefaultUniqueAttributesRecognizer
   All Implemented Interfaces: [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md), [ClipboardFragmentProcessor](../../api/content/ClipboardFragmentProcessor.md), [Extension](../../api/Extension.md), [UniqueAttributesProcessor](../../api/UniqueAttributesProcessor.md), [UniqueAttributesRecognizer](../../api/UniqueAttributesRecognizer.md)   Direct Known Subclasses: [DITAUniqueAttributesRecognizer](../../dita/id/DITAUniqueAttributesRecognizer.md), [DocBookUniqueAttributesRecognizer](../../docbook/id/DocBookUniqueAttributesRecognizer.md), [TEIP5UniqueAttributesRecognizer](../../tei/id/TEIP5UniqueAttributesRecognizer.md), [XHTMLUniqueAttributesRecognizer](../../xhtml/id/XHTMLUniqueAttributesRecognizer.md)   @API(type=INTERNAL, src=PUBLIC) public class DefaultUniqueAttributesRecognizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [UniqueAttributesRecognizer](../../api/UniqueAttributesRecognizer.md), [ClipboardFragmentProcessor](../../api/content/ClipboardFragmentProcessor.md)
Default unique attributes recognizer

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [AuthorAccess](../../api/AuthorAccess.md) [authorAccess](#authorAccess)
The author access
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [idAttrQname](#idAttrQname)
The ID attribute qname

## Constructor Summary
 Constructors
Constructor

Description
 [DefaultUniqueAttributesRecognizer](#%3Cinit%3E())()
Default constructor.
  [DefaultUniqueAttributesRecognizer](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idAttrQname)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [activated](#activated(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Method called when the Author extension was activated.
  void [assignUniqueIDs](#assignUniqueIDs(int,int,boolean))(int startOffset, int endOffset, boolean forceGeneration)
Assigns unique IDs between a start and an end offset in the document.
  boolean [copyAttributeOnSplit](#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrQName, [AuthorElement](../../api/node/AuthorElement.md) element)
Checks if the attribute specified by QName can be considered as a valid attribute to copy when the element is split.
  void [deactivated](#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Method called when the Author extension was deactivated.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [generateUniqueIDFor](#generateUniqueIDFor(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idGenerationPattern, [AuthorElement](../../api/node/AuthorElement.md) element)
Generate an unique ID for an element
  protected [GenerateIDElementsInfo](GenerateIDElementsInfo.md) [getDefaultOptions](#getDefaultOptions())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultOptionsXMLResourceName](#getDefaultOptionsXMLResourceName())()
Get the name of the XML resource from which to load the default options.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getGenerateIDAttributeQName](#getGenerateIDAttributeQName(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,boolean))([AuthorElement](../../api/node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elemsWithAutoGeneration, boolean forceGeneration)

 [GenerateIDElementsInfo](GenerateIDElementsInfo.md) [getGenerateIDElementsInfo](#getGenerateIDElementsInfo())()

 boolean [isAutoIDGenerationActive](#isAutoIDGenerationActive())()

 protected boolean [preserveIDsWhenPastingBetweenResources](#preserveIDsWhenPastingBetweenResources(int))(int fragmentPurpose)
Check if we should preserve IDs when pasting between resources.
  void [process](#process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation))([ClipboardFragmentInformation](../../api/content/ClipboardFragmentInformation.md) fragmentInformation)
Process a fragment in the clipboard before inserting it in the document.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### idAttrQname

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idAttrQname

The ID attribute qname

### authorAccess

protected [AuthorAccess](../../api/AuthorAccess.md) authorAccess

The author access

## Constructor Details

### DefaultUniqueAttributesRecognizer

public DefaultUniqueAttributesRecognizer()

Default constructor.

### DefaultUniqueAttributesRecognizer

public DefaultUniqueAttributesRecognizer([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idAttrQname)

Constructor.
  Parameters: idAttrQname - The ID attribute qname
## Method Details

### copyAttributeOnSplit

public boolean copyAttributeOnSplit([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrQName, [AuthorElement](../../api/node/AuthorElement.md) element)
 Description copied from interface: [UniqueAttributesProcessor](../../api/UniqueAttributesProcessor.md#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))
Checks if the attribute specified by QName can be considered as a valid attribute to copy when the element is split.
  Specified by: [copyAttributeOnSplit](../../api/UniqueAttributesProcessor.md#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [UniqueAttributesProcessor](../../api/UniqueAttributesProcessor.md) Parameters: attrQName - The attribute qualified name. element - The element. Returns: true if the attribute should be copied when Split is performed. See Also:
        * [UniqueAttributesProcessor.copyAttributeOnSplit(java.lang.String, ro.sync.ecss.extensions.api.node.AuthorElement)](../../api/UniqueAttributesProcessor.md#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))

### activated

public void activated([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
 Description copied from interface: [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md#activated(ro.sync.ecss.extensions.api.AuthorAccess))
Method called when the Author extension was activated. This event is triggered when the Author extension where this listener is defined was activated in relation with a document opened in Author page. Listeners like [AuthorMouseListener](../../api/AuthorMouseListener.md) or [AuthorListener](../../api/AuthorListener.md) can be added at this point.
  Specified by: [activated](../../api/AuthorExtensionStateListener.md#activated(ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md) Parameters: authorAccess - The [AuthorAccess](../../api/AuthorAccess.md) of the Author page where the listener was activated. See Also:
        * [AuthorExtensionStateListener.activated(ro.sync.ecss.extensions.api.AuthorAccess)](../../api/AuthorExtensionStateListener.md#activated(ro.sync.ecss.extensions.api.AuthorAccess))

### deactivated

public void deactivated([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
 Description copied from interface: [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))
Method called when the Author extension was deactivated. This event is triggered when another Author extension corresponding to the the current document opened in Author page was activated, the user switches to another editor page or the editor is closed.
  Specified by: [deactivated](../../api/AuthorExtensionStateListener.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md) Parameters: authorAccess - The [AuthorAccess](../../api/AuthorAccess.md) of the Author page where the listener was deactivated. See Also:
        * [AuthorExtensionStateListener.deactivated(ro.sync.ecss.extensions.api.AuthorAccess)](../../api/AuthorExtensionStateListener.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))

### getDefaultOptions

protected [GenerateIDElementsInfo](GenerateIDElementsInfo.md) getDefaultOptions()
  Returns: The default generation options
### getDefaultOptionsXMLResourceName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultOptionsXMLResourceName()

Get the name of the XML resource from which to load the default options.
  Returns: the name of the XML resource from which to load the default options.
### isAutoIDGenerationActive

public boolean isAutoIDGenerationActive()
  Specified by: [isAutoIDGenerationActive](../../api/UniqueAttributesRecognizer.md#isAutoIDGenerationActive()) in interface [UniqueAttributesRecognizer](../../api/UniqueAttributesRecognizer.md) Returns: true if auto generation is active and we have elements for which to generate.
### getGenerateIDAttributeQName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getGenerateIDAttributeQName([AuthorElement](../../api/node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elemsWithAutoGeneration, boolean forceGeneration)
  Parameters: element - The current element. elemsWithAutoGeneration - The array of elements for which generation is activated forceGeneration - Force ID generation if there is no selection. Returns: The name of the attribute for which to generate the ID or null (default behavior).
### generateUniqueIDFor

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) generateUniqueIDFor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idGenerationPattern, [AuthorElement](../../api/node/AuthorElement.md) element)

Generate an unique ID for an element
  Parameters: idGenerationPattern - The pattern for id generation. element - The element Returns: The unique ID
### assignUniqueIDs

public void assignUniqueIDs(int startOffset, int endOffset, boolean forceGeneration)
 Description copied from interface: [UniqueAttributesProcessor](../../api/UniqueAttributesProcessor.md#assignUniqueIDs(int,int,boolean))
Assigns unique IDs between a start and an end offset in the document.
  Specified by: [assignUniqueIDs](../../api/UniqueAttributesProcessor.md#assignUniqueIDs(int,int,boolean)) in interface [UniqueAttributesProcessor](../../api/UniqueAttributesProcessor.md) Parameters: startOffset - Start offset. endOffset - End offset. forceGeneration - true to generate ID even if the ID generation pattern list does not match. See Also:
        * [UniqueAttributesProcessor.assignUniqueIDs(int, int, boolean)](../../api/UniqueAttributesProcessor.md#assignUniqueIDs(int,int,boolean))

### getGenerateIDElementsInfo

public [GenerateIDElementsInfo](GenerateIDElementsInfo.md) getGenerateIDElementsInfo()
  Returns: Returns the autoGenerateElementsInfo.
### process

public void process([ClipboardFragmentInformation](../../api/content/ClipboardFragmentInformation.md) fragmentInformation)
 Description copied from interface: [ClipboardFragmentProcessor](../../api/content/ClipboardFragmentProcessor.md#process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation))
Process a fragment in the clipboard before inserting it in the document.
  Specified by: [process](../../api/content/ClipboardFragmentProcessor.md#process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation)) in interface [ClipboardFragmentProcessor](../../api/content/ClipboardFragmentProcessor.md) Parameters: fragmentInformation - Information about a fragment in the clipboard. See Also:
        * [ClipboardFragmentProcessor.process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation)](../../api/content/ClipboardFragmentProcessor.md#process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation))

### preserveIDsWhenPastingBetweenResources

protected boolean preserveIDsWhenPastingBetweenResources(int fragmentPurpose)

Check if we should preserve IDs when pasting between resources.
  Parameters: fragmentPurpose - The fragment purpose. On of the [AuthorSchemaAwareEditingHandler](../../api/AuthorSchemaAwareEditingHandler.md) purposes. Returns: true if we should preserve IDs when pasting between resources. By default the base method returns true.
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../api/Extension.md#getDescription()) in interface [Extension](../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
