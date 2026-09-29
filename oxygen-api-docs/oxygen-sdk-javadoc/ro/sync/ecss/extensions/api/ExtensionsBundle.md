Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class ExtensionsBundle

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.ExtensionsBundle
   All Implemented Interfaces: [Extension](Extension.md)   Direct Known Subclasses: [AntExtensionsBundle](../ant/AntExtensionsBundle.md), [DITAExtensionsBundle](../dita/DITAExtensionsBundle.md), [DITAValExtensionsBundle](../dita/DITAValExtensionsBundle.md), [DocBookExtensionsBundleBase](../docbook/DocBookExtensionsBundleBase.md), [DOTProjectExtensionsBundle](../dita/DOTProjectExtensionsBundle.md), [SchematronExtensionsBundle](../schematron/SchematronExtensionsBundle.md), [TEIExtensionsBundleBase](../tei/TEIExtensionsBundleBase.md), [WSDLExtensionsBundle](../wsdl/WSDLExtensionsBundle.md), [XHTMLExtensionsBundle](../xhtml/XHTMLExtensionsBundle.md), [XSDExtensionsBundle](../xsd/XSDExtensionsBundle.md), [XSLTExtensionsBundle](../xslt/XSLTExtensionsBundle.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ExtensionsBundle extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Extension](Extension.md)
Abstract class representing a bundle for all extensions handlers. Extensions of this class must be defined for every document type association defined in the **Preferences**/**Document type association** section. The bundle is created each time the document type association where it is defined matches the current document opened in an editor or the properties of the enclosing document type have been modified while the document type is active. At most one instance of an extensions bundle exist at a given time in the editor. Note: *References to objects that need to be persistent throughout the existence of an editor must not be kept here.*.

## Constructor Summary
 Constructors
Constructor

Description
 [ExtensionsBundle](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 [AttributesValueEditor](AttributesValueEditor.md) [createAttributesValueEditor](#createAttributesValueEditor(boolean))(boolean forEclipsePlugin)
Creates a new [AttributesValueEditor](AttributesValueEditor.md) instance used to get values for the current attribute.
  [AuthorDnDListener](../../../exml/editor/xmleditor/pageauthor/AuthorDnDListener.md) [createAuthorAWTDndListener](#createAuthorAWTDndListener())()
Creates a new [AuthorDnDListener](../../../exml/editor/xmleditor/pageauthor/AuthorDnDListener.md) instance responsible for handling AWT author drag and drop events.
  [AuthorBreadCrumbCustomizer](structure/AuthorBreadCrumbCustomizer.md) [createAuthorBreadCrumbCustomizer](#createAuthorBreadCrumbCustomizer())()
Create an Author Bread Crumb customizer used for nodes rendering in the Bread Crumb (components path which appears in the top of the Author editor).
  [AuthorExtensionStateListener](AuthorExtensionStateListener.md) [createAuthorExtensionStateListener](#createAuthorExtensionStateListener())()
Returns the [AuthorExtensionStateListener](AuthorExtensionStateListener.md) which will be notified when the Author extension where it is defined is activated and deactivated during the detection process.
  [AuthorOutlineCustomizer](structure/AuthorOutlineCustomizer.md) [createAuthorOutlineCustomizer](#createAuthorOutlineCustomizer())()
Create an Author Outline customizer used for custom filtering and nodes rendering in the Outline.
  [AuthorPreloadProcessor](AuthorPreloadProcessor.md) [createAuthorPreloadProcessor](#createAuthorPreloadProcessor())()
Returns the [AuthorPreloadProcessor](AuthorPreloadProcessor.md) which will be notified before the document is presented in the application.
  [AuthorReferenceResolver](AuthorReferenceResolver.md) [createAuthorReferenceResolver](#createAuthorReferenceResolver())()
Creates a new [AuthorReferenceResolver](AuthorReferenceResolver.md) instance used to expand content references.
  [StylesFilter](StylesFilter.md) [createAuthorStylesFilter](#createAuthorStylesFilter())()
Creates a new [StylesFilter](StylesFilter.md) instance for the CSS styles filtering.
  [AuthorDnDListener](../../../../../com/oxygenxml/editor/editors/author/AuthorDnDListener.md) [createAuthorSWTDndListener](#createAuthorSWTDndListener())()
Creates a new [AuthorDnDListener](../../../../../com/oxygenxml/editor/editors/author/AuthorDnDListener.md) instance responsible for handling SWT author drag and drop events.
  [AuthorTableCellSepProvider](AuthorTableCellSepProvider.md) [createAuthorTableCellSepProvider](#createAuthorTableCellSepProvider())()
Creates a new [AuthorTableCellSepProvider](AuthorTableCellSepProvider.md) instance responsible for providing information about the table cells painting their separators.
  [AuthorTableCellSpanProvider](AuthorTableCellSpanProvider.md) [createAuthorTableCellSpanProvider](#createAuthorTableCellSpanProvider())()
Creates a new [AuthorTableCellSpanProvider](AuthorTableCellSpanProvider.md) instance responsible for providing information about the table cells spanning.
  [AuthorTableColumnWidthProvider](AuthorTableColumnWidthProvider.md) [createAuthorTableColumnWidthProvider](#createAuthorTableColumnWidthProvider())()
Creates a new [AuthorTableColumnWidthProvider](AuthorTableColumnWidthProvider.md) instance responsible for providing information and for handling modifications regarding table width and column widths.
  [CustomAttributeValueEditor](CustomAttributeValueEditor.md) [createCustomAttributeValueEditor](#createCustomAttributeValueEditor(boolean))(boolean forEclipsePlugin)
Creates a new [CustomAttributeValueEditor](CustomAttributeValueEditor.md) instance used to get values for the current attribute.
  [EditPropertiesHandler](EditPropertiesHandler.md) [createEditPropertiesHandler](#createEditPropertiesHandler())()
A custom implementation to handle editing properties of an author node.
  [ElementLocatorProvider](link/ElementLocatorProvider.md) [createElementLocatorProvider](#createElementLocatorProvider())()
Creates a new [ElementLocatorProvider](link/ElementLocatorProvider.md) instance responsible for providing an implementation of an [ElementLocator](link/ElementLocator.md) based on the structure of a link.
  [AuthorExternalObjectInsertionHandler](AuthorExternalObjectInsertionHandler.md) [createExternalObjectInsertionHandler](#createExternalObjectInsertionHandler())()
Create a handler which gets notified when external resources need to be inserted in the Author page.
  [IDTypeRecognizer](link/IDTypeRecognizer.md) [createIDTypeRecognizer](#createIDTypeRecognizer())()
Creates a new [IDTypeRecognizer](link/IDTypeRecognizer.md) instance responsible for providing an implementation which can recognize ID declarations and references.
  [LinkTextResolver](link/LinkTextResolver.md) [createLinkTextResolver](#createLinkTextResolver())()
Creates a new [LinkTextResolver](link/LinkTextResolver.md) instance responsible for resolving a specific link marked in the CSS file and returning a text content from the targeted location.
  [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) [createSchemaManagerFilter](#createSchemaManagerFilter())()
Creates a new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance used to filter the content completion proposals from the schema manager.
  [TextPageExternalObjectInsertionHandler](text/TextPageExternalObjectInsertionHandler.md) [createTextPageExternalObjectInsertionHandler](#createTextPageExternalObjectInsertionHandler())()
Create a handler which gets notified when external resources need to be inserted in the Text page.
  [TextDnDListener](../../../../../com/oxygenxml/editor/editors/TextDnDListener.md) [createTextSWTDndListener](#createTextSWTDndListener())()
Creates a new [TextDnDListener](../../../../../com/oxygenxml/editor/editors/TextDnDListener.md) instance responsible for handling SWT text drag and drop events.
  [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md) [createXMLNodeCustomizer](#createXMLNodeCustomizer())()
Create an XML node customizer used for custom nodes rendering in the Author outline, Text page outline, Author bread crumb, content completion window or the DITA Map view.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [customizeImageTooltipDescription](#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorNode](node/AuthorNode.md) contextNode, [AuthorAccess](AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computedDescription)
Customize the tooltip description when hovering over an image.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [customizeLinkTooltipDescription](#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [AuthorNode](node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computedDescription)
Customize the tooltip description when hovering over a link.
  [AuthorActionEventHandler](AuthorActionEventHandler.md) [getAuthorActionEventHandler](#getAuthorActionEventHandler())()
Creates a special handler for author actions events (such as key events).
  [AuthorImageDecorator](AuthorImageDecorator.md) [getAuthorImageDecorator](#getAuthorImageDecorator())()
Get an [AuthorImageDecorator](AuthorImageDecorator.md).
  [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) [getAuthorSchemaAwareEditingHandler](#getAuthorSchemaAwareEditingHandler())()
If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this support.
  [AuthorTableOperationsHandler](table/operations/AuthorTableOperationsHandler.md) [getAuthorTableOperationsHandler](#getAuthorTableOperationsHandler())()
Get the [AuthorTableOperationsHandler](table/operations/AuthorTableOperationsHandler.md) instance responsible for handling table operations.
  [ClipboardFragmentProcessor](content/ClipboardFragmentProcessor.md) [getClipboardFragmentProcessor](#getClipboardFragmentProcessor())()
Get a processor for Author Document Fragments in the clipboard (which will be pasted, dropped, etc).
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentTypeID](#getDocumentTypeID())()
This should never return null if the [OptionsStorage](OptionsStorage.md)support it is intended to be used.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentTypeName](#getDocumentTypeName())()
Get the name of the document type which created this bundle (as set in the Oxygen -> Preferences -> Document Types.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditorPage)
Get the help page ID for this particular framework extensions bundle.
  [ProfilingConditionalTextProvider](ProfilingConditionalTextProvider.md) [getProfilingConditionalTextProvider](#getProfilingConditionalTextProvider())()
Creates a new [ProfilingConditionalTextProvider](ProfilingConditionalTextProvider.md) instance responsible for providing custom support regarding profiling and conditional text.
  [SpellCheckerHelper](spell/SpellCheckerHelper.md) [getSpellCheckerHelper](#getSpellCheckerHelper())()
Get a helper for the spell checker.
  [UniqueAttributesRecognizer](UniqueAttributesRecognizer.md) [getUniqueAttributesIdentifier](#getUniqueAttributesIdentifier())()
Get an unique attributes creator and identifier.
  [WebappExtensionsProvider](WebappExtensionsProvider.md) [getWebappExtensionsProvier](#getWebappExtensionsProvier())()

 boolean [isContentReference](#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node)
Check if this node references another node which should replace it entirely.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolveCustomAttributeValue](#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext))([CustomAttributeValueContext](CustomAttributeValueContext.md) attributeValueEditingContext)
Resolve a custom attribute value to an URL which will be opened by Oxygen.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolveCustomHref](#resolveCustomHref(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref)
When clicking a href the bundle can custom solve the href to an URL.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolveCustomHref](#resolveCustomHref(java.net.URL,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](AuthorAccess.md) authorAccess)
When clicking a href the bundle can custom solve the href to an URL.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolveCustomHref](#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [AuthorNode](node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](AuthorAccess.md) authorAccess)
When clicking a href the bundle can custom solve the href to an URL.
  void [setDocumentTypeName](#setDocumentTypeName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypeName)
Set the name of the document type which created this bundle.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Constructor Details

### ExtensionsBundle

public ExtensionsBundle()

## Method Details

### createAuthorReferenceResolver

public [AuthorReferenceResolver](AuthorReferenceResolver.md) createAuthorReferenceResolver()

Creates a new [AuthorReferenceResolver](AuthorReferenceResolver.md) instance used to expand content references. The method is called each time an opened document in an Author editor page matches the document type association where the extensions bundle is defined.
  Returns: A new [AuthorReferenceResolver](AuthorReferenceResolver.md) instance.
### createAuthorStylesFilter

public [StylesFilter](StylesFilter.md) createAuthorStylesFilter()

Creates a new [StylesFilter](StylesFilter.md) instance for the CSS styles filtering.

Use this to replace the default styles associated to a node form the document object model, or the styles of the pseudo elements :before and :after.

The method is called each time an opened document in an Author editor page matches the document type association where the extensions bundle is defined.
  Returns: A new [StylesFilter](StylesFilter.md) instance, or null.
### createAuthorTableCellSpanProvider

public [AuthorTableCellSpanProvider](AuthorTableCellSpanProvider.md) createAuthorTableCellSpanProvider()

Creates a new [AuthorTableCellSpanProvider](AuthorTableCellSpanProvider.md) instance responsible for providing information about the table cells spanning. The table cell span provider is not reused between different tables. The method is called for each table in the document so a new instance should be provided each time.
  Returns: A new [AuthorTableCellSpanProvider](AuthorTableCellSpanProvider.md) instance.
### createAuthorTableColumnWidthProvider

public [AuthorTableColumnWidthProvider](AuthorTableColumnWidthProvider.md) createAuthorTableColumnWidthProvider()

Creates a new [AuthorTableColumnWidthProvider](AuthorTableColumnWidthProvider.md) instance responsible for providing information and for handling modifications regarding table width and column widths. The table column width provider is not reused between different tables. The method is called for each table in the document so a new instance should be provided each time.
  Returns: A new [AuthorTableColumnWidthProvider](AuthorTableColumnWidthProvider.md) instance.
### createAuthorTableCellSepProvider

public [AuthorTableCellSepProvider](AuthorTableCellSepProvider.md) createAuthorTableCellSepProvider()

Creates a new [AuthorTableCellSepProvider](AuthorTableCellSepProvider.md) instance responsible for providing information about the table cells painting their separators. The table cell separators provider is not reused between different tables. The method is called for each table in the document so a new instance should be provided each time.
  Returns: A new [AuthorTableCellSepProvider](AuthorTableCellSepProvider.md) instance.
### getAuthorTableOperationsHandler

public [AuthorTableOperationsHandler](table/operations/AuthorTableOperationsHandler.md) getAuthorTableOperationsHandler()

Get the [AuthorTableOperationsHandler](table/operations/AuthorTableOperationsHandler.md) instance responsible for handling table operations.
  Returns: Author table operations handler. Since: 14
### createAuthorExtensionStateListener

public [AuthorExtensionStateListener](AuthorExtensionStateListener.md) createAuthorExtensionStateListener()

Returns the [AuthorExtensionStateListener](AuthorExtensionStateListener.md) which will be notified when the Author extension where it is defined is activated and deactivated during the detection process. This method is called each time the Document Type association where the Author extension and the extensions bundle are defined matches a document opened in an Author page.
  Returns: A new [AuthorExtensionStateListener](AuthorExtensionStateListener.md) instance.
### createAuthorPreloadProcessor

public [AuthorPreloadProcessor](AuthorPreloadProcessor.md) createAuthorPreloadProcessor()

Returns the [AuthorPreloadProcessor](AuthorPreloadProcessor.md) which will be notified before the document is presented in the application.
  Returns: A new [AuthorPreloadProcessor](AuthorPreloadProcessor.md) instance. Since: 23.0
### createAuthorAWTDndListener

public [AuthorDnDListener](../../../exml/editor/xmleditor/pageauthor/AuthorDnDListener.md) createAuthorAWTDndListener()

Creates a new [AuthorDnDListener](../../../exml/editor/xmleditor/pageauthor/AuthorDnDListener.md) instance responsible for handling AWT author drag and drop events. This method is called each time the Document Type association where the extensions bundle is defined matches a document opened in an Author page.
  Returns: The AWT drag and drop listener implementation.
### createAuthorSWTDndListener

public [AuthorDnDListener](../../../../../com/oxygenxml/editor/editors/author/AuthorDnDListener.md) createAuthorSWTDndListener()

Creates a new [AuthorDnDListener](../../../../../com/oxygenxml/editor/editors/author/AuthorDnDListener.md) instance responsible for handling SWT author drag and drop events. This method is called each time the Document Type association where the extensions bundle is defined matches a document opened in an Author page.
  Returns: The SWT drag and drop listener implementation.
### createTextSWTDndListener

public [TextDnDListener](../../../../../com/oxygenxml/editor/editors/TextDnDListener.md) createTextSWTDndListener()

Creates a new [TextDnDListener](../../../../../com/oxygenxml/editor/editors/TextDnDListener.md) instance responsible for handling SWT text drag and drop events. This method is called each time the Document Type association where the extensions bundle is defined matches a document opened in a Text page.
  Returns: The SWT drag and drop listener implementation.
### createElementLocatorProvider

public [ElementLocatorProvider](link/ElementLocatorProvider.md) createElementLocatorProvider()

Creates a new [ElementLocatorProvider](link/ElementLocatorProvider.md) instance responsible for providing an implementation of an [ElementLocator](link/ElementLocator.md) based on the structure of a link. The [ElementLocator](link/ElementLocator.md) is capable of locating an element pointed by the supplied link. This method is called each time an element needs to be located based on a link specification.
  Returns: A new [ElementLocatorProvider](link/ElementLocatorProvider.md) instance.
### createIDTypeRecognizer

public [IDTypeRecognizer](link/IDTypeRecognizer.md) createIDTypeRecognizer()

Creates a new [IDTypeRecognizer](link/IDTypeRecognizer.md) instance responsible for providing an implementation which can recognize ID declarations and references. This method is called each time an ID must be recognized or certain ID-aware searches or refactory actions are performed.
  Returns: A new [IDTypeRecognizer](link/IDTypeRecognizer.md) instance.
### createSchemaManagerFilter

public [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) createSchemaManagerFilter()

Creates a new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance used to filter the content completion proposals from the schema manager. This method is called each time the document type where the extensions bundle is defined matches a document opened in an editor.
  Returns: A new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance.
### createAttributesValueEditor

public [AttributesValueEditor](AttributesValueEditor.md) createAttributesValueEditor(boolean forEclipsePlugin)

Creates a new [AttributesValueEditor](AttributesValueEditor.md) instance used to get values for the current attribute. This is used especially from the "Attributes View" and from attributes editing dialogs available on Author mode and Outliner.
  Parameters: forEclipsePlugin - If true the code is called from the Eclipse plugin. Returns: A new [AttributesValueEditor](AttributesValueEditor.md) instance.
### createCustomAttributeValueEditor

public [CustomAttributeValueEditor](CustomAttributeValueEditor.md) createCustomAttributeValueEditor(boolean forEclipsePlugin)

Creates a new [CustomAttributeValueEditor](CustomAttributeValueEditor.md) instance used to get values for the current attribute. This is used especially from the "Attributes View" and from attributes editing dialogs available on Author mode and Outliner.
  Parameters: forEclipsePlugin - If true the code is called from the Eclipse plugin. Returns: A new [CustomAttributeValueEditor](CustomAttributeValueEditor.md) instance. Since: 15
### getUniqueAttributesIdentifier

public [UniqueAttributesRecognizer](UniqueAttributesRecognizer.md) getUniqueAttributesIdentifier()

Get an unique attributes creator and identifier.
  Returns: The unique attributes identifier
### getClipboardFragmentProcessor

public [ClipboardFragmentProcessor](content/ClipboardFragmentProcessor.md) getClipboardFragmentProcessor()

Get a processor for Author Document Fragments in the clipboard (which will be pasted, dropped, etc).
  Returns: a processor for Author Document Fragments in the clipboard (which will be pasted, dropped, etc). Since: 12.2
### getDocumentTypeID

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentTypeID()

This should never return null if the [OptionsStorage](OptionsStorage.md)support it is intended to be used. If this returns null you will not be able to add [OptionListener](OptionListener.md) or store and retrieve any options at all.
  Returns: The unique identifier of the Document Type.
### resolveCustomAttributeValue

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolveCustomAttributeValue([CustomAttributeValueContext](CustomAttributeValueContext.md) attributeValueEditingContext)

Resolve a custom attribute value to an URL which will be opened by Oxygen. This method is called when the "Open File at Cursor" action is called in the Text editor page.
  Parameters: attributeValueEditingContext - The editing context. Returns: The URL which should be opened as a result of "Open File at Cursor" being invoked on the attribute value. Since: 22
### resolveCustomHref

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolveCustomHref([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

When clicking a href the bundle can custom solve the href to an URL.
  Parameters: linkHref - The link href as derrived from the CSS Returns: The resolved absolute URL if null if the default behavior will be performed Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the link is recognized by the extensions bundle, but could not be mapped to an URL.
### resolveCustomHref

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolveCustomHref([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](AuthorAccess.md) authorAccess)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

When clicking a href the bundle can custom solve the href to an URL.
  Parameters: currentEditorURL - The URL of the current editor. linkHref - The link href as derrived from the CSS authorAccess - The Author Access. Returns: The resolved absolute URL if null if the default behavior will be performed Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the link is recognized by the extensions bundle, but could not be mapped to an URL.
### resolveCustomHref

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolveCustomHref([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [AuthorNode](node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](AuthorAccess.md) authorAccess)throws [CustomResolverException](CustomResolverException.md), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

When clicking a href the bundle can custom solve the href to an URL.
  Parameters: currentEditorURL - The URL of the current editor. contextNode - The context node in which the href needs to be computed. linkHref - The link href as derrived from the CSS authorAccess - The Author Access. Returns: The resolved absolute URL if null if the default behavior will be performed Throws: [CustomResolverException](CustomResolverException.md) - If the link is recognized by the extensions bundle, but could not be mapped to an URL. It offers a solution to the user. This solution is invoked when the user clicks on the error message. [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the link is recognized by the extensions bundle, but could not be mapped to an URL. Since: 15
### customizeLinkTooltipDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) customizeLinkTooltipDescription([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [AuthorNode](node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computedDescription)

Customize the tooltip description when hovering over a link.
  Parameters: currentEditorURL - The current document URL contextNode - The context node linkHref - The link href. authorAccess - The Author access computedDescription - The already computed description. Usually something like: "Click to open: URL" Returns: The customized description. Since: 22.1
### customizeImageTooltipDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) customizeImageTooltipDescription([AuthorNode](node/AuthorNode.md) contextNode, [AuthorAccess](AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computedDescription)

Customize the tooltip description when hovering over an image.
  Parameters: contextNode - The context node authorAccess - The Author access computedDescription - The already computed description. Returns: The customized description. Since: 27
### createAuthorOutlineCustomizer

public [AuthorOutlineCustomizer](structure/AuthorOutlineCustomizer.md) createAuthorOutlineCustomizer()

Create an Author Outline customizer used for custom filtering and nodes rendering in the Outline.
  Returns: The Author Outline customizer.
### createAuthorBreadCrumbCustomizer

public [AuthorBreadCrumbCustomizer](structure/AuthorBreadCrumbCustomizer.md) createAuthorBreadCrumbCustomizer()

Create an Author Bread Crumb customizer used for nodes rendering in the Bread Crumb (components path which appears in the top of the Author editor).
  Returns: The Author Bread Crumb customizer.
### getAuthorSchemaAwareEditingHandler

public [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) getAuthorSchemaAwareEditingHandler()

If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this support. The support can either resolve a specific case, let the default implementation take place or reject the edit entirely by throwing an [InvalidEditException](InvalidEditException.md). It is recommended to extend class [AuthorSchemaAwareEditingHandlerAdapter](AuthorSchemaAwareEditingHandlerAdapter.md) in order to be protected from any API additions that may occur in interface [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md).
  Returns: A custom editing handler for schema aware actions, or null if there is no handler and the default processing should take place.
### createExternalObjectInsertionHandler

public [AuthorExternalObjectInsertionHandler](AuthorExternalObjectInsertionHandler.md) createExternalObjectInsertionHandler()

Create a handler which gets notified when external resources need to be inserted in the Author page. The usual usage for this is to get notified when URLs are dropped from the project or DITA Maps manager in the Author page.
  Returns: The External URLs handler Since: 12
### createTextPageExternalObjectInsertionHandler

public [TextPageExternalObjectInsertionHandler](text/TextPageExternalObjectInsertionHandler.md) createTextPageExternalObjectInsertionHandler()

Create a handler which gets notified when external resources need to be inserted in the Text page. The usual usage for this is to get notified when URLs are dropped from the project or DITA Maps manager in the Text page.
  Returns: The External URLs handler Since: 19
### getDocumentTypeName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentTypeName()

Get the name of the document type which created this bundle (as set in the Oxygen -> Preferences -> Document Types. You can use it in your extensions bundle to see the name of the document type which created this bundle.
  Returns: the name of the document type. Since: 12
### setDocumentTypeName

public void setDocumentTypeName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypeName)

Set the name of the document type which created this bundle. This must not get called by the user code, it is set internal.
  Parameters: documentTypeName - The name of the document type which created this bundle
### isContentReference

public boolean isContentReference([AuthorNode](node/AuthorNode.md) node)

Check if this node references another node which should replace it entirely. This is used in the tables to replace conreffed table rows entirely
  Parameters: node - The node Returns: true if this node references another node which should replace it entirely.
### getProfilingConditionalTextProvider

public [ProfilingConditionalTextProvider](ProfilingConditionalTextProvider.md) getProfilingConditionalTextProvider()

Creates a new [ProfilingConditionalTextProvider](ProfilingConditionalTextProvider.md) instance responsible for providing custom support regarding profiling and conditional text.
  Returns: A new [ProfilingConditionalTextProvider](ProfilingConditionalTextProvider.md) instance. Since: 13.2
### createXMLNodeCustomizer

public [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md) createXMLNodeCustomizer()

Create an XML node customizer used for custom nodes rendering in the Author outline, Text page outline, Author bread crumb, content completion window or the DITA Map view.
  Returns: The XML node customizer. Since: 13.2
### createLinkTextResolver

public [LinkTextResolver](link/LinkTextResolver.md) createLinkTextResolver()

Creates a new [LinkTextResolver](link/LinkTextResolver.md) instance responsible for resolving a specific link marked in the CSS file and returning a text content from the targeted location. This text content will be presented as a static text associated with the link in author page. This resolver will be used when function oxy_link-text() is encountered inside the CSS rules on the 'content' property.
  Returns: A new [LinkTextResolver](link/LinkTextResolver.md) instance. Since: 14.2
### createEditPropertiesHandler

public [EditPropertiesHandler](EditPropertiesHandler.md) createEditPropertiesHandler()

A custom implementation to handle editing properties of an author node. For example when a user double clicks on an element tag we will invoke this extension and a specific dialog can be presented.
  Returns: An implementation that can edit the properties of nodes. Since: 17.1
### getAuthorActionEventHandler

public [AuthorActionEventHandler](AuthorActionEventHandler.md) getAuthorActionEventHandler()

Creates a special handler for author actions events (such as key events). These events normally have built-in handling but this handler gets a chance to perform something different.
  Returns: An event handler. Since: 18
### getAuthorImageDecorator

public [AuthorImageDecorator](AuthorImageDecorator.md) getAuthorImageDecorator()

Get an [AuthorImageDecorator](AuthorImageDecorator.md). Permits decoration of the images that are displayed in the Author view. For instance it can overlay some meta-information over the image.
  Returns: An [AuthorImageDecorator](AuthorImageDecorator.md), or null. Since: 18
### getHelpPageID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditorPage)

Get the help page ID for this particular framework extensions bundle. If the returned help page ID is an URL, a web browser will be opened pointing to that URL when the user presses F1 in the dialog or when using the Help button. If the returned help page ID is an identifier, when help is invoked, the application will open the Oxygen User's Manual and locate this identifier inside it.
  Parameters: currentEditorPage - The current editor page mode (Text/Grid/Author/Schema), one of the constants in the "ro.sync.exml.editor.EditorPageConstants" interface. Returns: The help page ID, by default no help page ID is returned. Since: 18.1 See Also:
        * [HelpPageProvider.getHelpPageID()](../../../ui/application/HelpPageProvider.md#getHelpPageID())

### getWebappExtensionsProvier

public [WebappExtensionsProvider](WebappExtensionsProvider.md) getWebappExtensionsProvier()
  Returns: An object that provides Web Author specific extensions, may be null. Since: 21.1
### getSpellCheckerHelper

public [SpellCheckerHelper](spell/SpellCheckerHelper.md) getSpellCheckerHelper()

Get a helper for the spell checker.
  Returns: Helper utilities implemented at framework level. Since: 26.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
