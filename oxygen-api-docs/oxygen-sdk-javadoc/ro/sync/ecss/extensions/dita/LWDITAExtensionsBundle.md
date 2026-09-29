Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class LWDITAExtensionsBundle

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.ExtensionsBundle](../api/ExtensionsBundle.md)
        * [ro.sync.ecss.extensions.dita.DITAExtensionsBundle](DITAExtensionsBundle.md)
            * ro.sync.ecss.extensions.dita.LWDITAExtensionsBundle
   All Implemented Interfaces: [ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md), [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class LWDITAExtensionsBundle extends [DITAExtensionsBundle](DITAExtensionsBundle.md)
The Lightweight DITA framework extensions bundle.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.dita.[DITAExtensionsBundle](DITAExtensionsBundle.md)
 [keyManager](DITAExtensionsBundle.md#keyManager), [keyManagerProvider](DITAExtensionsBundle.md#keyManagerProvider)
## Constructor Summary
 Constructors
Constructor

Description
 [LWDITAExtensionsBundle](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentTypeID](#getDocumentTypeID())()
This should never return null if the [OptionsStorage](../api/OptionsStorage.md)support it is intended to be used.

### Methods inherited from class ro.sync.ecss.extensions.dita.[DITAExtensionsBundle](DITAExtensionsBundle.md)
 [createAuthorExtensionStateListener](DITAExtensionsBundle.md#createAuthorExtensionStateListener()), [createAuthorReferenceResolver](DITAExtensionsBundle.md#createAuthorReferenceResolver()), [createAuthorTableCellSepProvider](DITAExtensionsBundle.md#createAuthorTableCellSepProvider()), [createAuthorTableCellSpanProvider](DITAExtensionsBundle.md#createAuthorTableCellSpanProvider()), [createAuthorTableColumnWidthProvider](DITAExtensionsBundle.md#createAuthorTableColumnWidthProvider()), [createContextKeyManager](DITAExtensionsBundle.md#createContextKeyManager(ro.sync.ecss.extensions.api.access.EditingSessionContext)), [createEditPropertiesHandler](DITAExtensionsBundle.md#createEditPropertiesHandler()), [createElementLocatorProvider](DITAExtensionsBundle.md#createElementLocatorProvider()), [createExternalObjectInsertionHandler](DITAExtensionsBundle.md#createExternalObjectInsertionHandler()), [createIDTypeRecognizer](DITAExtensionsBundle.md#createIDTypeRecognizer()), [createLinkTextResolver](DITAExtensionsBundle.md#createLinkTextResolver()), [createSchemaManagerFilter](DITAExtensionsBundle.md#createSchemaManagerFilter()), [createTextPageExternalObjectInsertionHandler](DITAExtensionsBundle.md#createTextPageExternalObjectInsertionHandler()), [createXMLNodeCustomizer](DITAExtensionsBundle.md#createXMLNodeCustomizer()), [customizeImageTooltipDescription](DITAExtensionsBundle.md#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [customizeLinkTooltipDescription](DITAExtensionsBundle.md#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [getAuthorActionEventHandler](DITAExtensionsBundle.md#getAuthorActionEventHandler()), [getAuthorImageDecorator](DITAExtensionsBundle.md#getAuthorImageDecorator()), [getAuthorSchemaAwareEditingHandler](DITAExtensionsBundle.md#getAuthorSchemaAwareEditingHandler()), [getAuthorTableOperationsHandler](DITAExtensionsBundle.md#getAuthorTableOperationsHandler()), [getClipboardFragmentProcessor](DITAExtensionsBundle.md#getClipboardFragmentProcessor()), [getContextKeyManager](DITAExtensionsBundle.md#getContextKeyManager()), [getHelpPageID](DITAExtensionsBundle.md#getHelpPageID(java.lang.String)), [getKeyManager](DITAExtensionsBundle.md#getKeyManager()), [getProfilingConditionalTextProvider](DITAExtensionsBundle.md#getProfilingConditionalTextProvider()), [getSpellCheckerHelper](DITAExtensionsBundle.md#getSpellCheckerHelper()), [getUniqueAttributesIdentifier](DITAExtensionsBundle.md#getUniqueAttributesIdentifier()), [isContentReference](DITAExtensionsBundle.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)), [resolveCustomAttributeValue](DITAExtensionsBundle.md#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext)), [resolveCustomHref](DITAExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))
### Methods inherited from class ro.sync.ecss.extensions.api.[ExtensionsBundle](../api/ExtensionsBundle.md)
 [createAttributesValueEditor](../api/ExtensionsBundle.md#createAttributesValueEditor(boolean)), [createAuthorAWTDndListener](../api/ExtensionsBundle.md#createAuthorAWTDndListener()), [createAuthorBreadCrumbCustomizer](../api/ExtensionsBundle.md#createAuthorBreadCrumbCustomizer()), [createAuthorOutlineCustomizer](../api/ExtensionsBundle.md#createAuthorOutlineCustomizer()), [createAuthorPreloadProcessor](../api/ExtensionsBundle.md#createAuthorPreloadProcessor()), [createAuthorStylesFilter](../api/ExtensionsBundle.md#createAuthorStylesFilter()), [createAuthorSWTDndListener](../api/ExtensionsBundle.md#createAuthorSWTDndListener()), [createCustomAttributeValueEditor](../api/ExtensionsBundle.md#createCustomAttributeValueEditor(boolean)), [createTextSWTDndListener](../api/ExtensionsBundle.md#createTextSWTDndListener()), [getDocumentTypeName](../api/ExtensionsBundle.md#getDocumentTypeName()), [getWebappExtensionsProvier](../api/ExtensionsBundle.md#getWebappExtensionsProvier()), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.lang.String)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [setDocumentTypeName](../api/ExtensionsBundle.md#setDocumentTypeName(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### LWDITAExtensionsBundle

public LWDITAExtensionsBundle()

## Method Details

### getDocumentTypeID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentTypeID()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getDocumentTypeID())
This should never return null if the [OptionsStorage](../api/OptionsStorage.md)support it is intended to be used. If this returns null you will not be able to add [OptionListener](../api/OptionListener.md) or store and retrieve any options at all.
  Overrides: [getDocumentTypeID](DITAExtensionsBundle.md#getDocumentTypeID()) in class [DITAExtensionsBundle](DITAExtensionsBundle.md) Returns: The unique identifier of the Document Type. See Also:
        * [ExtensionsBundle.getDocumentTypeID()](../api/ExtensionsBundle.md#getDocumentTypeID())

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../api/Extension.md#getDescription()) in interface [Extension](../api/Extension.md) Overrides: [getDescription](DITAExtensionsBundle.md#getDescription()) in class [DITAExtensionsBundle](DITAExtensionsBundle.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
