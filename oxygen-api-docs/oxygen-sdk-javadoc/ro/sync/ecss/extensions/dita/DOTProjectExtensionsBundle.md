Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DOTProjectExtensionsBundle

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.ExtensionsBundle](../api/ExtensionsBundle.md)
        * ro.sync.ecss.extensions.dita.DOTProjectExtensionsBundle
   All Implemented Interfaces: [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DOTProjectExtensionsBundle extends [ExtensionsBundle](../api/ExtensionsBundle.md)
Extensions bundle for a DITA OT Project.

## Constructor Summary
 Constructors
Constructor

Description
 [DOTProjectExtensionsBundle](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) [createAuthorReferenceResolver](#createAuthorReferenceResolver())()
Creates a new [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) instance used to expand content references.
  [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) [createElementLocatorProvider](#createElementLocatorProvider())()
Creates a new [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) instance responsible for providing an implementation of an [ElementLocator](../api/link/ElementLocator.md) based on the structure of a link.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentTypeID](#getDocumentTypeID())()
This should never return null if the [OptionsStorage](../api/OptionsStorage.md)support it is intended to be used.

### Methods inherited from class ro.sync.ecss.extensions.api.[ExtensionsBundle](../api/ExtensionsBundle.md)
 [createAttributesValueEditor](../api/ExtensionsBundle.md#createAttributesValueEditor(boolean)), [createAuthorAWTDndListener](../api/ExtensionsBundle.md#createAuthorAWTDndListener()), [createAuthorBreadCrumbCustomizer](../api/ExtensionsBundle.md#createAuthorBreadCrumbCustomizer()), [createAuthorExtensionStateListener](../api/ExtensionsBundle.md#createAuthorExtensionStateListener()), [createAuthorOutlineCustomizer](../api/ExtensionsBundle.md#createAuthorOutlineCustomizer()), [createAuthorPreloadProcessor](../api/ExtensionsBundle.md#createAuthorPreloadProcessor()), [createAuthorStylesFilter](../api/ExtensionsBundle.md#createAuthorStylesFilter()), [createAuthorSWTDndListener](../api/ExtensionsBundle.md#createAuthorSWTDndListener()), [createAuthorTableCellSepProvider](../api/ExtensionsBundle.md#createAuthorTableCellSepProvider()), [createAuthorTableCellSpanProvider](../api/ExtensionsBundle.md#createAuthorTableCellSpanProvider()), [createAuthorTableColumnWidthProvider](../api/ExtensionsBundle.md#createAuthorTableColumnWidthProvider()), [createCustomAttributeValueEditor](../api/ExtensionsBundle.md#createCustomAttributeValueEditor(boolean)), [createEditPropertiesHandler](../api/ExtensionsBundle.md#createEditPropertiesHandler()), [createExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler()), [createIDTypeRecognizer](../api/ExtensionsBundle.md#createIDTypeRecognizer()), [createLinkTextResolver](../api/ExtensionsBundle.md#createLinkTextResolver()), [createSchemaManagerFilter](../api/ExtensionsBundle.md#createSchemaManagerFilter()), [createTextPageExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createTextPageExternalObjectInsertionHandler()), [createTextSWTDndListener](../api/ExtensionsBundle.md#createTextSWTDndListener()), [createXMLNodeCustomizer](../api/ExtensionsBundle.md#createXMLNodeCustomizer()), [customizeImageTooltipDescription](../api/ExtensionsBundle.md#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [customizeLinkTooltipDescription](../api/ExtensionsBundle.md#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [getAuthorActionEventHandler](../api/ExtensionsBundle.md#getAuthorActionEventHandler()), [getAuthorImageDecorator](../api/ExtensionsBundle.md#getAuthorImageDecorator()), [getAuthorSchemaAwareEditingHandler](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler()), [getAuthorTableOperationsHandler](../api/ExtensionsBundle.md#getAuthorTableOperationsHandler()), [getClipboardFragmentProcessor](../api/ExtensionsBundle.md#getClipboardFragmentProcessor()), [getDocumentTypeName](../api/ExtensionsBundle.md#getDocumentTypeName()), [getHelpPageID](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String)), [getProfilingConditionalTextProvider](../api/ExtensionsBundle.md#getProfilingConditionalTextProvider()), [getSpellCheckerHelper](../api/ExtensionsBundle.md#getSpellCheckerHelper()), [getUniqueAttributesIdentifier](../api/ExtensionsBundle.md#getUniqueAttributesIdentifier()), [getWebappExtensionsProvier](../api/ExtensionsBundle.md#getWebappExtensionsProvier()), [isContentReference](../api/ExtensionsBundle.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)), [resolveCustomAttributeValue](../api/ExtensionsBundle.md#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.lang.String)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [setDocumentTypeName](../api/ExtensionsBundle.md#setDocumentTypeName(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DOTProjectExtensionsBundle

public DOTProjectExtensionsBundle()

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../api/Extension.md#getDescription())

### getDocumentTypeID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentTypeID()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getDocumentTypeID())
This should never return null if the [OptionsStorage](../api/OptionsStorage.md)support it is intended to be used. If this returns null you will not be able to add [OptionListener](../api/OptionListener.md) or store and retrieve any options at all.
  Specified by: [getDocumentTypeID](../api/ExtensionsBundle.md#getDocumentTypeID()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: The unique identifier of the Document Type. See Also:
        * [ExtensionsBundle.getDocumentTypeID()](../api/ExtensionsBundle.md#getDocumentTypeID())

### createElementLocatorProvider

public [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) createElementLocatorProvider()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createElementLocatorProvider())
Creates a new [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) instance responsible for providing an implementation of an [ElementLocator](../api/link/ElementLocator.md) based on the structure of a link. The [ElementLocator](../api/link/ElementLocator.md) is capable of locating an element pointed by the supplied link. This method is called each time an element needs to be located based on a link specification.
  Overrides: [createElementLocatorProvider](../api/ExtensionsBundle.md#createElementLocatorProvider()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) instance. See Also:
        * [ExtensionsBundle.createElementLocatorProvider()](../api/ExtensionsBundle.md#createElementLocatorProvider())

### createAuthorReferenceResolver

public [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) createAuthorReferenceResolver()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createAuthorReferenceResolver())
Creates a new [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) instance used to expand content references. The method is called each time an opened document in an Author editor page matches the document type association where the extensions bundle is defined.
  Overrides: [createAuthorReferenceResolver](../api/ExtensionsBundle.md#createAuthorReferenceResolver()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) instance. See Also:
        * [ExtensionsBundle.createAuthorReferenceResolver()](../api/ExtensionsBundle.md#createAuthorReferenceResolver())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
