Package [ro.sync.ecss.extensions.xhtml](package-summary.md)

# Class XHTMLExtensionsBundle

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.ExtensionsBundle](../api/ExtensionsBundle.md)
        * ro.sync.ecss.extensions.xhtml.XHTMLExtensionsBundle
   All Implemented Interfaces: [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class XHTMLExtensionsBundle extends [ExtensionsBundle](../api/ExtensionsBundle.md)
The XHTML framework extensions bundle.

## Constructor Summary
 Constructors
Constructor

Description
 [XHTMLExtensionsBundle](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) [createAuthorExtensionStateListener](#createAuthorExtensionStateListener())()
Returns the [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) which will be notified when the Author extension where it is defined is activated and deactivated during the detection process.
  [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) [createAuthorTableCellSpanProvider](#createAuthorTableCellSpanProvider())()
Creates a new [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) instance responsible for providing information about the table cells spanning.
  [AuthorTableColumnWidthProvider](../api/AuthorTableColumnWidthProvider.md) [createAuthorTableColumnWidthProvider](#createAuthorTableColumnWidthProvider())()
Creates a new [AuthorTableColumnWidthProvider](../api/AuthorTableColumnWidthProvider.md) instance responsible for providing information and for handling modifications regarding table width and column widths.
  [EditPropertiesHandler](../api/EditPropertiesHandler.md) [createEditPropertiesHandler](#createEditPropertiesHandler())()
A custom implementation to handle editing properties of an author node.
  [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) [createElementLocatorProvider](#createElementLocatorProvider())()
Creates a new [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) instance responsible for providing an implementation of an [ElementLocator](../api/link/ElementLocator.md) based on the structure of a link.
  [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) [createExternalObjectInsertionHandler](#createExternalObjectInsertionHandler())()
Create a handler which gets notified when external resources need to be inserted in the Author page.
  [IDTypeRecognizer](../api/link/IDTypeRecognizer.md) [createIDTypeRecognizer](#createIDTypeRecognizer())()
Creates a new [IDTypeRecognizer](../api/link/IDTypeRecognizer.md) instance responsible for providing an implementation which can recognize ID declarations and references.
  [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) [createSchemaManagerFilter](#createSchemaManagerFilter())()
Creates a new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance used to filter the content completion proposals from the schema manager.
  [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md) [createXMLNodeCustomizer](#createXMLNodeCustomizer())()
Create an XML node customizer used for custom nodes rendering in the Author outline, Text page outline, Author bread crumb, content completion window or the DITA Map view.
  [AuthorActionEventHandler](../api/AuthorActionEventHandler.md) [getAuthorActionEventHandler](#getAuthorActionEventHandler())()
Creates a special handler for author actions events (such as key events).
  [AuthorImageDecorator](../api/AuthorImageDecorator.md) [getAuthorImageDecorator](#getAuthorImageDecorator())()
Get an [AuthorImageDecorator](../api/AuthorImageDecorator.md).
  [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) [getAuthorTableOperationsHandler](#getAuthorTableOperationsHandler())()
Get the [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) instance responsible for handling table operations.
  [ClipboardFragmentProcessor](../api/content/ClipboardFragmentProcessor.md) [getClipboardFragmentProcessor](#getClipboardFragmentProcessor())()
Get a processor for Author Document Fragments in the clipboard (which will be pasted, dropped, etc).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentTypeID](#getDocumentTypeID())()
This should never return null if the [OptionsStorage](../api/OptionsStorage.md)support it is intended to be used.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditorPage)
Get the help page ID for this particular framework extensions bundle.
  [UniqueAttributesRecognizer](../api/UniqueAttributesRecognizer.md) [getUniqueAttributesIdentifier](#getUniqueAttributesIdentifier())()
Get an unique attributes creator and identifier.

### Methods inherited from class ro.sync.ecss.extensions.api.[ExtensionsBundle](../api/ExtensionsBundle.md)
 [createAttributesValueEditor](../api/ExtensionsBundle.md#createAttributesValueEditor(boolean)), [createAuthorAWTDndListener](../api/ExtensionsBundle.md#createAuthorAWTDndListener()), [createAuthorBreadCrumbCustomizer](../api/ExtensionsBundle.md#createAuthorBreadCrumbCustomizer()), [createAuthorOutlineCustomizer](../api/ExtensionsBundle.md#createAuthorOutlineCustomizer()), [createAuthorPreloadProcessor](../api/ExtensionsBundle.md#createAuthorPreloadProcessor()), [createAuthorReferenceResolver](../api/ExtensionsBundle.md#createAuthorReferenceResolver()), [createAuthorStylesFilter](../api/ExtensionsBundle.md#createAuthorStylesFilter()), [createAuthorSWTDndListener](../api/ExtensionsBundle.md#createAuthorSWTDndListener()), [createAuthorTableCellSepProvider](../api/ExtensionsBundle.md#createAuthorTableCellSepProvider()), [createCustomAttributeValueEditor](../api/ExtensionsBundle.md#createCustomAttributeValueEditor(boolean)), [createLinkTextResolver](../api/ExtensionsBundle.md#createLinkTextResolver()), [createTextPageExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createTextPageExternalObjectInsertionHandler()), [createTextSWTDndListener](../api/ExtensionsBundle.md#createTextSWTDndListener()), [customizeImageTooltipDescription](../api/ExtensionsBundle.md#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [customizeLinkTooltipDescription](../api/ExtensionsBundle.md#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [getAuthorSchemaAwareEditingHandler](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler()), [getDocumentTypeName](../api/ExtensionsBundle.md#getDocumentTypeName()), [getProfilingConditionalTextProvider](../api/ExtensionsBundle.md#getProfilingConditionalTextProvider()), [getSpellCheckerHelper](../api/ExtensionsBundle.md#getSpellCheckerHelper()), [getWebappExtensionsProvier](../api/ExtensionsBundle.md#getWebappExtensionsProvier()), [isContentReference](../api/ExtensionsBundle.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)), [resolveCustomAttributeValue](../api/ExtensionsBundle.md#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.lang.String)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [setDocumentTypeName](../api/ExtensionsBundle.md#setDocumentTypeName(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XHTMLExtensionsBundle

public XHTMLExtensionsBundle()

## Method Details

### createAuthorExtensionStateListener

public [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) createAuthorExtensionStateListener()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createAuthorExtensionStateListener())
Returns the [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) which will be notified when the Author extension where it is defined is activated and deactivated during the detection process. This method is called each time the Document Type association where the Author extension and the extensions bundle are defined matches a document opened in an Author page.
  Overrides: [createAuthorExtensionStateListener](../api/ExtensionsBundle.md#createAuthorExtensionStateListener()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) instance. See Also:
        * [ExtensionsBundle.createAuthorExtensionStateListener()](../api/ExtensionsBundle.md#createAuthorExtensionStateListener())

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

### getUniqueAttributesIdentifier

public [UniqueAttributesRecognizer](../api/UniqueAttributesRecognizer.md) getUniqueAttributesIdentifier()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getUniqueAttributesIdentifier())
Get an unique attributes creator and identifier.
  Overrides: [getUniqueAttributesIdentifier](../api/ExtensionsBundle.md#getUniqueAttributesIdentifier()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: The unique attributes identifier See Also:
        * [ExtensionsBundle.getUniqueAttributesIdentifier()](../api/ExtensionsBundle.md#getUniqueAttributesIdentifier())

### getClipboardFragmentProcessor

public [ClipboardFragmentProcessor](../api/content/ClipboardFragmentProcessor.md) getClipboardFragmentProcessor()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getClipboardFragmentProcessor())
Get a processor for Author Document Fragments in the clipboard (which will be pasted, dropped, etc).
  Overrides: [getClipboardFragmentProcessor](../api/ExtensionsBundle.md#getClipboardFragmentProcessor()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: a processor for Author Document Fragments in the clipboard (which will be pasted, dropped, etc). See Also:
        * [ExtensionsBundle.getClipboardFragmentProcessor()](../api/ExtensionsBundle.md#getClipboardFragmentProcessor())

### createElementLocatorProvider

public [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) createElementLocatorProvider()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createElementLocatorProvider())
Creates a new [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) instance responsible for providing an implementation of an [ElementLocator](../api/link/ElementLocator.md) based on the structure of a link. The [ElementLocator](../api/link/ElementLocator.md) is capable of locating an element pointed by the supplied link. This method is called each time an element needs to be located based on a link specification.
  Overrides: [createElementLocatorProvider](../api/ExtensionsBundle.md#createElementLocatorProvider()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) instance. See Also:
        * [ExtensionsBundle.createElementLocatorProvider()](../api/ExtensionsBundle.md#createElementLocatorProvider())

### createExternalObjectInsertionHandler

public [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) createExternalObjectInsertionHandler()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler())
Create a handler which gets notified when external resources need to be inserted in the Author page. The usual usage for this is to get notified when URLs are dropped from the project or DITA Maps manager in the Author page.
  Overrides: [createExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: The External URLs handler See Also:
        * [ExtensionsBundle.createExternalObjectInsertionHandler()](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler())

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

### getAuthorTableOperationsHandler

public [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) getAuthorTableOperationsHandler()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getAuthorTableOperationsHandler())
Get the [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) instance responsible for handling table operations.
  Overrides: [getAuthorTableOperationsHandler](../api/ExtensionsBundle.md#getAuthorTableOperationsHandler()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: Author table operations handler. See Also:
        * [ExtensionsBundle.getAuthorTableOperationsHandler()](../api/ExtensionsBundle.md#getAuthorTableOperationsHandler())

### createIDTypeRecognizer

public [IDTypeRecognizer](../api/link/IDTypeRecognizer.md) createIDTypeRecognizer()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createIDTypeRecognizer())
Creates a new [IDTypeRecognizer](../api/link/IDTypeRecognizer.md) instance responsible for providing an implementation which can recognize ID declarations and references. This method is called each time an ID must be recognized or certain ID-aware searches or refactory actions are performed.
  Overrides: [createIDTypeRecognizer](../api/ExtensionsBundle.md#createIDTypeRecognizer()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [IDTypeRecognizer](../api/link/IDTypeRecognizer.md) instance. See Also:
        * [ExtensionsBundle.createIDTypeRecognizer()](../api/ExtensionsBundle.md#createIDTypeRecognizer())

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

### getHelpPageID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditorPage)
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String))
Get the help page ID for this particular framework extensions bundle. If the returned help page ID is an URL, a web browser will be opened pointing to that URL when the user presses F1 in the dialog or when using the Help button. If the returned help page ID is an identifier, when help is invoked, the application will open the Oxygen User's Manual and locate this identifier inside it.
  Overrides: [getHelpPageID](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String)) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Parameters: currentEditorPage - The current editor page mode (Text/Grid/Author/Schema), one of the constants in the "ro.sync.exml.editor.EditorPageConstants" interface. Returns: The help page ID, by default no help page ID is returned. See Also:
        * [ExtensionsBundle.getHelpPageID(java.lang.String)](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
