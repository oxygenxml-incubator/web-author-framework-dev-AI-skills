Package [ro.sync.ecss.extensions.docbook](package-summary.md)

# Class DocBookExtensionsBundleBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.ExtensionsBundle](../api/ExtensionsBundle.md)
        * ro.sync.ecss.extensions.docbook.DocBookExtensionsBundleBase
   All Implemented Interfaces: [Extension](../api/Extension.md)   Direct Known Subclasses: [DocBook4ExtensionsBundle](DocBook4ExtensionsBundle.md), [DocBook5ExtensionsBundle](DocBook5ExtensionsBundle.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class DocBookExtensionsBundleBase extends [ExtensionsBundle](../api/ExtensionsBundle.md)
The DocBook framework extensions bundle.

## Constructor Summary
 Constructors
Constructor

Description
 [DocBookExtensionsBundleBase](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorTableCellSepProvider](../api/AuthorTableCellSepProvider.md) [createAuthorTableCellSepProvider](#createAuthorTableCellSepProvider())()
Creates a new [AuthorTableCellSepProvider](../api/AuthorTableCellSepProvider.md) instance responsible for providing information about the table cells painting their separators.
  [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) [createAuthorTableCellSpanProvider](#createAuthorTableCellSpanProvider())()
Creates a new [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) instance responsible for providing information about the table cells spanning.
  [AuthorTableColumnWidthProvider](../api/AuthorTableColumnWidthProvider.md) [createAuthorTableColumnWidthProvider](#createAuthorTableColumnWidthProvider())()
Creates a new [AuthorTableColumnWidthProvider](../api/AuthorTableColumnWidthProvider.md) instance responsible for providing information and for handling modifications regarding table width and column widths.
  [EditPropertiesHandler](../api/EditPropertiesHandler.md) [createEditPropertiesHandler](#createEditPropertiesHandler())()
A custom implementation to handle editing properties of an author node.
  [LinkTextResolver](../api/link/LinkTextResolver.md) [createLinkTextResolver](#createLinkTextResolver())()
Creates a new [LinkTextResolver](../api/link/LinkTextResolver.md) instance responsible for resolving a specific link marked in the CSS file and returning a text content from the targeted location.
  [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) [createSchemaManagerFilter](#createSchemaManagerFilter())()
Creates a new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance used to filter the content completion proposals from the schema manager.
  [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md) [createXMLNodeCustomizer](#createXMLNodeCustomizer())()
Create an XML node customizer used for custom nodes rendering in the Author outline, Text page outline, Author bread crumb, content completion window or the DITA Map view.
  [AuthorActionEventHandler](../api/AuthorActionEventHandler.md) [getAuthorActionEventHandler](#getAuthorActionEventHandler())()
Creates a special handler for author actions events (such as key events).
  [AuthorImageDecorator](../api/AuthorImageDecorator.md) [getAuthorImageDecorator](#getAuthorImageDecorator())()
Get an [AuthorImageDecorator](../api/AuthorImageDecorator.md).
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentNamespace](#getDocumentNamespace())()

 [SpellCheckerHelper](../api/spell/SpellCheckerHelper.md) [getSpellCheckerHelper](#getSpellCheckerHelper())()
Get a helper for the spell checker.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolveCustomHref](#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [AuthorNode](../api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](../api/AuthorAccess.md) authorAccess)
When clicking a href the bundle can custom solve the href to an URL.

### Methods inherited from class ro.sync.ecss.extensions.api.[ExtensionsBundle](../api/ExtensionsBundle.md)
 [createAttributesValueEditor](../api/ExtensionsBundle.md#createAttributesValueEditor(boolean)), [createAuthorAWTDndListener](../api/ExtensionsBundle.md#createAuthorAWTDndListener()), [createAuthorBreadCrumbCustomizer](../api/ExtensionsBundle.md#createAuthorBreadCrumbCustomizer()), [createAuthorExtensionStateListener](../api/ExtensionsBundle.md#createAuthorExtensionStateListener()), [createAuthorOutlineCustomizer](../api/ExtensionsBundle.md#createAuthorOutlineCustomizer()), [createAuthorPreloadProcessor](../api/ExtensionsBundle.md#createAuthorPreloadProcessor()), [createAuthorReferenceResolver](../api/ExtensionsBundle.md#createAuthorReferenceResolver()), [createAuthorStylesFilter](../api/ExtensionsBundle.md#createAuthorStylesFilter()), [createAuthorSWTDndListener](../api/ExtensionsBundle.md#createAuthorSWTDndListener()), [createCustomAttributeValueEditor](../api/ExtensionsBundle.md#createCustomAttributeValueEditor(boolean)), [createElementLocatorProvider](../api/ExtensionsBundle.md#createElementLocatorProvider()), [createExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler()), [createIDTypeRecognizer](../api/ExtensionsBundle.md#createIDTypeRecognizer()), [createTextPageExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createTextPageExternalObjectInsertionHandler()), [createTextSWTDndListener](../api/ExtensionsBundle.md#createTextSWTDndListener()), [customizeImageTooltipDescription](../api/ExtensionsBundle.md#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [customizeLinkTooltipDescription](../api/ExtensionsBundle.md#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [getAuthorSchemaAwareEditingHandler](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler()), [getAuthorTableOperationsHandler](../api/ExtensionsBundle.md#getAuthorTableOperationsHandler()), [getClipboardFragmentProcessor](../api/ExtensionsBundle.md#getClipboardFragmentProcessor()), [getDocumentTypeID](../api/ExtensionsBundle.md#getDocumentTypeID()), [getDocumentTypeName](../api/ExtensionsBundle.md#getDocumentTypeName()), [getHelpPageID](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String)), [getProfilingConditionalTextProvider](../api/ExtensionsBundle.md#getProfilingConditionalTextProvider()), [getUniqueAttributesIdentifier](../api/ExtensionsBundle.md#getUniqueAttributesIdentifier()), [getWebappExtensionsProvier](../api/ExtensionsBundle.md#getWebappExtensionsProvier()), [isContentReference](../api/ExtensionsBundle.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)), [resolveCustomAttributeValue](../api/ExtensionsBundle.md#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.lang.String)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [setDocumentTypeName](../api/ExtensionsBundle.md#setDocumentTypeName(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../api/Extension.md)
 [getDescription](../api/Extension.md#getDescription())
## Constructor Details

### DocBookExtensionsBundleBase

public DocBookExtensionsBundleBase()

## Method Details

### createAuthorTableCellSpanProvider

public [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) createAuthorTableCellSpanProvider()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createAuthorTableCellSpanProvider())
Creates a new [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) instance responsible for providing information about the table cells spanning. The table cell span provider is not reused between different tables. The method is called for each table in the document so a new instance should be provided each time.
  Overrides: [createAuthorTableCellSpanProvider](../api/ExtensionsBundle.md#createAuthorTableCellSpanProvider()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) instance. See Also:
        * [ExtensionsBundle.createAuthorTableCellSpanProvider()](../api/ExtensionsBundle.md#createAuthorTableCellSpanProvider())

### createAuthorTableColumnWidthProvider

public [AuthorTableColumnWidthProvider](../api/AuthorTableColumnWidthProvider.md) createAuthorTableColumnWidthProvider()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createAuthorTableColumnWidthProvider())
Creates a new [AuthorTableColumnWidthProvider](../api/AuthorTableColumnWidthProvider.md) instance responsible for providing information and for handling modifications regarding table width and column widths. The table column width provider is not reused between different tables. The method is called for each table in the document so a new instance should be provided each time.
  Overrides: [createAuthorTableColumnWidthProvider](../api/ExtensionsBundle.md#createAuthorTableColumnWidthProvider()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [AuthorTableColumnWidthProvider](../api/AuthorTableColumnWidthProvider.md) instance. See Also:
        * [ExtensionsBundle.createAuthorTableColumnWidthProvider()](../api/ExtensionsBundle.md#createAuthorTableColumnWidthProvider())

### createAuthorTableCellSepProvider

public [AuthorTableCellSepProvider](../api/AuthorTableCellSepProvider.md) createAuthorTableCellSepProvider()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createAuthorTableCellSepProvider())
Creates a new [AuthorTableCellSepProvider](../api/AuthorTableCellSepProvider.md) instance responsible for providing information about the table cells painting their separators. The table cell separators provider is not reused between different tables. The method is called for each table in the document so a new instance should be provided each time.
  Overrides: [createAuthorTableCellSepProvider](../api/ExtensionsBundle.md#createAuthorTableCellSepProvider()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [AuthorTableCellSepProvider](../api/AuthorTableCellSepProvider.md) instance. See Also:
        * [ExtensionsBundle.createAuthorTableCellSepProvider()](../api/ExtensionsBundle.md#createAuthorTableCellSepProvider())

### getDocumentNamespace

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentNamespace()
  Returns: The document namespace.
### createSchemaManagerFilter

public [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) createSchemaManagerFilter()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createSchemaManagerFilter())
Creates a new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance used to filter the content completion proposals from the schema manager. This method is called each time the document type where the extensions bundle is defined matches a document opened in an editor.
  Overrides: [createSchemaManagerFilter](../api/ExtensionsBundle.md#createSchemaManagerFilter()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance. See Also:
        * [ExtensionsBundle.createSchemaManagerFilter()](../api/ExtensionsBundle.md#createSchemaManagerFilter())

### createXMLNodeCustomizer

public [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md) createXMLNodeCustomizer()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createXMLNodeCustomizer())
Create an XML node customizer used for custom nodes rendering in the Author outline, Text page outline, Author bread crumb, content completion window or the DITA Map view.
  Overrides: [createXMLNodeCustomizer](../api/ExtensionsBundle.md#createXMLNodeCustomizer()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: The XML node customizer. See Also:
        * [ExtensionsBundle.createXMLNodeCustomizer()](../api/ExtensionsBundle.md#createXMLNodeCustomizer())

### createLinkTextResolver

public [LinkTextResolver](../api/link/LinkTextResolver.md) createLinkTextResolver()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createLinkTextResolver())
Creates a new [LinkTextResolver](../api/link/LinkTextResolver.md) instance responsible for resolving a specific link marked in the CSS file and returning a text content from the targeted location. This text content will be presented as a static text associated with the link in author page. This resolver will be used when function oxy_link-text() is encountered inside the CSS rules on the 'content' property.
  Overrides: [createLinkTextResolver](../api/ExtensionsBundle.md#createLinkTextResolver()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [LinkTextResolver](../api/link/LinkTextResolver.md) instance. See Also:
        * [ExtensionsBundle.createLinkTextResolver()](../api/ExtensionsBundle.md#createLinkTextResolver())

### resolveCustomHref

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolveCustomHref([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [AuthorNode](../api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](../api/AuthorAccess.md) authorAccess)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))
When clicking a href the bundle can custom solve the href to an URL.
  Overrides: [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Parameters: currentEditorURL - The URL of the current editor. contextNode - The context node in which the href needs to be computed. linkHref - The link href as derrived from the CSS authorAccess - The Author Access. Returns: The resolved absolute URL if null if the default behavior will be performed Throws: [CustomResolverException](../api/CustomResolverException.md) - If the link is recognized by the extensions bundle, but could not be mapped to an URL. It offers a solution to the user. This solution is invoked when the user clicks on the error message. [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the link is recognized by the extensions bundle, but could not be mapped to an URL. See Also:
        * [ExtensionsBundle.resolveCustomHref(java.net.URL, ro.sync.ecss.extensions.api.node.AuthorNode, java.lang.String, ro.sync.ecss.extensions.api.AuthorAccess)](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))

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
