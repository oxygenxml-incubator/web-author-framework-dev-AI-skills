Package [ro.sync.ecss.extensions.tei](package-summary.md)

# Class TEIExtensionsBundleBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.ExtensionsBundle](../api/ExtensionsBundle.md)
        * ro.sync.ecss.extensions.tei.TEIExtensionsBundleBase
   All Implemented Interfaces: [Extension](../api/Extension.md)   Direct Known Subclasses: [TEI_jteiExtensionsBundle](TEI_jteiExtensionsBundle.md), [TEIP5ExtensionsBundle](TEIP5ExtensionsBundle.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class TEIExtensionsBundleBase extends [ExtensionsBundle](../api/ExtensionsBundle.md)
The TEI framework extensions bundle.

## Constructor Summary
 Constructors
Constructor

Description
 [TEIExtensionsBundleBase](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) [createAuthorTableCellSpanProvider](#createAuthorTableCellSpanProvider())()
Creates a new [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) instance responsible for providing information about the table cells spanning.
  [EditPropertiesHandler](../api/EditPropertiesHandler.md) [createEditPropertiesHandler](#createEditPropertiesHandler())()
A custom implementation to handle editing properties of an author node.
  [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md) [createXMLNodeCustomizer](#createXMLNodeCustomizer())()
Create an XML node customizer used for custom nodes rendering in the Author outline, Text page outline, Author bread crumb, content completion window or the DITA Map view.
  [AuthorActionEventHandler](../api/AuthorActionEventHandler.md) [getAuthorActionEventHandler](#getAuthorActionEventHandler())()
Creates a special handler for author actions events (such as key events).
  [AuthorImageDecorator](../api/AuthorImageDecorator.md) [getAuthorImageDecorator](#getAuthorImageDecorator())()
Get an [AuthorImageDecorator](../api/AuthorImageDecorator.md).
  [AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md) [getAuthorSchemaAwareEditingHandler](#getAuthorSchemaAwareEditingHandler())()
If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this support.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentNamespace](#getDocumentNamespace())()

 [SpellCheckerHelper](../api/spell/SpellCheckerHelper.md) [getSpellCheckerHelper](#getSpellCheckerHelper())()
Get a helper for the spell checker.

### Methods inherited from class ro.sync.ecss.extensions.api.[ExtensionsBundle](../api/ExtensionsBundle.md)
 [createAttributesValueEditor](../api/ExtensionsBundle.md#createAttributesValueEditor(boolean)), [createAuthorAWTDndListener](../api/ExtensionsBundle.md#createAuthorAWTDndListener()), [createAuthorBreadCrumbCustomizer](../api/ExtensionsBundle.md#createAuthorBreadCrumbCustomizer()), [createAuthorExtensionStateListener](../api/ExtensionsBundle.md#createAuthorExtensionStateListener()), [createAuthorOutlineCustomizer](../api/ExtensionsBundle.md#createAuthorOutlineCustomizer()), [createAuthorPreloadProcessor](../api/ExtensionsBundle.md#createAuthorPreloadProcessor()), [createAuthorReferenceResolver](../api/ExtensionsBundle.md#createAuthorReferenceResolver()), [createAuthorStylesFilter](../api/ExtensionsBundle.md#createAuthorStylesFilter()), [createAuthorSWTDndListener](../api/ExtensionsBundle.md#createAuthorSWTDndListener()), [createAuthorTableCellSepProvider](../api/ExtensionsBundle.md#createAuthorTableCellSepProvider()), [createAuthorTableColumnWidthProvider](../api/ExtensionsBundle.md#createAuthorTableColumnWidthProvider()), [createCustomAttributeValueEditor](../api/ExtensionsBundle.md#createCustomAttributeValueEditor(boolean)), [createElementLocatorProvider](../api/ExtensionsBundle.md#createElementLocatorProvider()), [createExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler()), [createIDTypeRecognizer](../api/ExtensionsBundle.md#createIDTypeRecognizer()), [createLinkTextResolver](../api/ExtensionsBundle.md#createLinkTextResolver()), [createSchemaManagerFilter](../api/ExtensionsBundle.md#createSchemaManagerFilter()), [createTextPageExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createTextPageExternalObjectInsertionHandler()), [createTextSWTDndListener](../api/ExtensionsBundle.md#createTextSWTDndListener()), [customizeImageTooltipDescription](../api/ExtensionsBundle.md#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [customizeLinkTooltipDescription](../api/ExtensionsBundle.md#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [getAuthorTableOperationsHandler](../api/ExtensionsBundle.md#getAuthorTableOperationsHandler()), [getClipboardFragmentProcessor](../api/ExtensionsBundle.md#getClipboardFragmentProcessor()), [getDocumentTypeID](../api/ExtensionsBundle.md#getDocumentTypeID()), [getDocumentTypeName](../api/ExtensionsBundle.md#getDocumentTypeName()), [getHelpPageID](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String)), [getProfilingConditionalTextProvider](../api/ExtensionsBundle.md#getProfilingConditionalTextProvider()), [getUniqueAttributesIdentifier](../api/ExtensionsBundle.md#getUniqueAttributesIdentifier()), [getWebappExtensionsProvier](../api/ExtensionsBundle.md#getWebappExtensionsProvier()), [isContentReference](../api/ExtensionsBundle.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)), [resolveCustomAttributeValue](../api/ExtensionsBundle.md#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.lang.String)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [setDocumentTypeName](../api/ExtensionsBundle.md#setDocumentTypeName(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../api/Extension.md)
 [getDescription](../api/Extension.md#getDescription())
## Constructor Details

### TEIExtensionsBundleBase

public TEIExtensionsBundleBase()

## Method Details

### createAuthorTableCellSpanProvider

public [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) createAuthorTableCellSpanProvider()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createAuthorTableCellSpanProvider())
Creates a new [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) instance responsible for providing information about the table cells spanning. The table cell span provider is not reused between different tables. The method is called for each table in the document so a new instance should be provided each time.
  Overrides: [createAuthorTableCellSpanProvider](../api/ExtensionsBundle.md#createAuthorTableCellSpanProvider()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) instance. See Also:
        * [ExtensionsBundle.createAuthorTableCellSpanProvider()](../api/ExtensionsBundle.md#createAuthorTableCellSpanProvider())

### getDocumentNamespace

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentNamespace()
  Returns: The document namespace.
### getAuthorSchemaAwareEditingHandler

public [AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md) getAuthorSchemaAwareEditingHandler()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler())
If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this support. The support can either resolve a specific case, let the default implementation take place or reject the edit entirely by throwing an [InvalidEditException](../api/InvalidEditException.md). It is recommended to extend class [AuthorSchemaAwareEditingHandlerAdapter](../api/AuthorSchemaAwareEditingHandlerAdapter.md) in order to be protected from any API additions that may occur in interface [AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md).
  Overrides: [getAuthorSchemaAwareEditingHandler](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A custom editing handler for schema aware actions, or null if there is no handler and the default processing should take place. See Also:
        * [ExtensionsBundle.getAuthorSchemaAwareEditingHandler()](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler())

### createXMLNodeCustomizer

public [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md) createXMLNodeCustomizer()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createXMLNodeCustomizer())
Create an XML node customizer used for custom nodes rendering in the Author outline, Text page outline, Author bread crumb, content completion window or the DITA Map view.
  Overrides: [createXMLNodeCustomizer](../api/ExtensionsBundle.md#createXMLNodeCustomizer()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: The XML node customizer. See Also:
        * [ExtensionsBundle.createXMLNodeCustomizer()](../api/ExtensionsBundle.md#createXMLNodeCustomizer())

### getAuthorActionEventHandler

public [AuthorActionEventHandler](../api/AuthorActionEventHandler.md) getAuthorActionEventHandler()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getAuthorActionEventHandler())
Creates a special handler for author actions events (such as key events). These events normally have built-in handling but this handler gets a chance to perform something different.
  Overrides: [getAuthorActionEventHandler](../api/ExtensionsBundle.md#getAuthorActionEventHandler()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: An event handler. See Also:
        * [ExtensionsBundle.getAuthorActionEventHandler()](../api/ExtensionsBundle.md#getAuthorActionEventHandler())

### getAuthorImageDecorator

public [AuthorImageDecorator](../api/AuthorImageDecorator.md) getAuthorImageDecorator()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getAuthorImageDecorator())
Get an [AuthorImageDecorator](../api/AuthorImageDecorator.md). Permits decoration of the images that are displayed in the Author view. For instance it can overlay some meta-information over the image.
  Overrides: [getAuthorImageDecorator](../api/ExtensionsBundle.md#getAuthorImageDecorator()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: An [AuthorImageDecorator](../api/AuthorImageDecorator.md), or null. See Also:
        * [ExtensionsBundle.getAuthorImageDecorator()](../api/ExtensionsBundle.md#getAuthorImageDecorator())

### createEditPropertiesHandler

public [EditPropertiesHandler](../api/EditPropertiesHandler.md) createEditPropertiesHandler()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createEditPropertiesHandler())
A custom implementation to handle editing properties of an author node. For example when a user double clicks on an element tag we will invoke this extension and a specific dialog can be presented.
  Overrides: [createEditPropertiesHandler](../api/ExtensionsBundle.md#createEditPropertiesHandler()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: An implementation that can edit the properties of nodes. See Also:
        * [ExtensionsBundle.createEditPropertiesHandler()](../api/ExtensionsBundle.md#createEditPropertiesHandler())

### getSpellCheckerHelper

public [SpellCheckerHelper](../api/spell/SpellCheckerHelper.md) getSpellCheckerHelper()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getSpellCheckerHelper())
Get a helper for the spell checker.
  Overrides: [getSpellCheckerHelper](../api/ExtensionsBundle.md#getSpellCheckerHelper()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: Helper utilities implemented at framework level. See Also:
        * [ExtensionsBundle.getSpellCheckerHelper()](../api/ExtensionsBundle.md#getSpellCheckerHelper())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
