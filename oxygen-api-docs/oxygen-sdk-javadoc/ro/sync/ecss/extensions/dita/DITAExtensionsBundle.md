Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DITAExtensionsBundle

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.ExtensionsBundle](../api/ExtensionsBundle.md)
        * ro.sync.ecss.extensions.dita.DITAExtensionsBundle
   All Implemented Interfaces: [ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md), [Extension](../api/Extension.md)   Direct Known Subclasses: [DITAMapExtensionsBundle](map/DITAMapExtensionsBundle.md), [LWDITAExtensionsBundle](LWDITAExtensionsBundle.md)   @API(type=INTERNAL, src=PUBLIC) public class DITAExtensionsBundle extends [ExtensionsBundle](../api/ExtensionsBundle.md)implements [ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md)
The DITA framework extensions bundle.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [ContextKeyManager](../../dita/ContextKeyManager.md) [keyManager](#keyManager)
The key manager that is context aware and is used to resolve key refs.
  protected final [ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) [keyManagerProvider](#keyManagerProvider)
The provider for the key manager which is context aware and is used to resolve key refs.

## Constructor Summary
 Constructors
Constructor

Description
 [DITAExtensionsBundle](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) [createAuthorExtensionStateListener](#createAuthorExtensionStateListener())()
Returns the [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) which will be notified when the Author extension where it is defined is activated and deactivated during the detection process.
  [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) [createAuthorReferenceResolver](#createAuthorReferenceResolver())()
Creates a new [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) instance used to expand content references.
  [AuthorTableCellSepProvider](../api/AuthorTableCellSepProvider.md) [createAuthorTableCellSepProvider](#createAuthorTableCellSepProvider())()
Creates a new [AuthorTableCellSepProvider](../api/AuthorTableCellSepProvider.md) instance responsible for providing information about the table cells painting their separators.
  [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) [createAuthorTableCellSpanProvider](#createAuthorTableCellSpanProvider())()
Creates a new [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) instance responsible for providing information about the table cells spanning.
  [AuthorTableColumnWidthProvider](../api/AuthorTableColumnWidthProvider.md) [createAuthorTableColumnWidthProvider](#createAuthorTableColumnWidthProvider())()
Creates a new [AuthorTableColumnWidthProvider](../api/AuthorTableColumnWidthProvider.md) instance responsible for providing information and for handling modifications regarding table width and column widths.
  protected [ContextKeyManager](../../dita/ContextKeyManager.md) [createContextKeyManager](#createContextKeyManager(ro.sync.ecss.extensions.api.access.EditingSessionContext))([EditingSessionContext](../api/access/EditingSessionContext.md) context)
Create a context key manager to be used when resolving keyrefs.
  [EditPropertiesHandler](../api/EditPropertiesHandler.md) [createEditPropertiesHandler](#createEditPropertiesHandler())()
A custom implementation to handle editing properties of an author node.
  [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) [createElementLocatorProvider](#createElementLocatorProvider())()
Creates a new [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) instance responsible for providing an implementation of an [ElementLocator](../api/link/ElementLocator.md) based on the structure of a link.
  [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) [createExternalObjectInsertionHandler](#createExternalObjectInsertionHandler())()
Create a handler which gets notified when external resources need to be inserted in the Author page.
  [IDTypeRecognizer](../api/link/IDTypeRecognizer.md) [createIDTypeRecognizer](#createIDTypeRecognizer())()
Creates a new [IDTypeRecognizer](../api/link/IDTypeRecognizer.md) instance responsible for providing an implementation which can recognize ID declarations and references.
  [LinkTextResolver](../api/link/LinkTextResolver.md) [createLinkTextResolver](#createLinkTextResolver())()
Creates a new [LinkTextResolver](../api/link/LinkTextResolver.md) instance responsible for resolving a specific link marked in the CSS file and returning a text content from the targeted location.
  [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) [createSchemaManagerFilter](#createSchemaManagerFilter())()
Creates a new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance used to filter the content completion proposals from the schema manager.
  [TextPageExternalObjectInsertionHandler](../api/text/TextPageExternalObjectInsertionHandler.md) [createTextPageExternalObjectInsertionHandler](#createTextPageExternalObjectInsertionHandler())()
Create a handler which gets notified when external resources need to be inserted in the Text page.
  [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md) [createXMLNodeCustomizer](#createXMLNodeCustomizer())()
Create an XML node customizer used for custom nodes rendering in the Author outline, Text page outline, Author bread crumb, content completion window or the DITA Map view.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [customizeImageTooltipDescription](#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorNode](../api/node/AuthorNode.md) contextNode, [AuthorAccess](../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computedDescription)
Customize the tooltip description when hovering over an image.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [customizeLinkTooltipDescription](#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [AuthorNode](../api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computedDescription)
Customize the tooltip description when hovering over a link.
  [AuthorActionEventHandler](../api/AuthorActionEventHandler.md) [getAuthorActionEventHandler](#getAuthorActionEventHandler())()
Creates a special handler for author actions events (such as key events).
  [AuthorImageDecorator](../api/AuthorImageDecorator.md) [getAuthorImageDecorator](#getAuthorImageDecorator())()
Get an [AuthorImageDecorator](../api/AuthorImageDecorator.md).
  [AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md) [getAuthorSchemaAwareEditingHandler](#getAuthorSchemaAwareEditingHandler())()
If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this support.
  [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) [getAuthorTableOperationsHandler](#getAuthorTableOperationsHandler())()
Get the [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) instance responsible for handling table operations.
  [ClipboardFragmentProcessor](../api/content/ClipboardFragmentProcessor.md) [getClipboardFragmentProcessor](#getClipboardFragmentProcessor())()
Get a processor for Author Document Fragments in the clipboard (which will be pasted, dropped, etc).
  [ContextKeyManager](../../dita/ContextKeyManager.md) [getContextKeyManager](#getContextKeyManager())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentTypeID](#getDocumentTypeID())()
This should never return null if the [OptionsStorage](../api/OptionsStorage.md)support it is intended to be used.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditorPage)
Get the help page ID for this particular framework extensions bundle.
  [ContextKeyManager](../../dita/ContextKeyManager.md) [getKeyManager](#getKeyManager())()
Returns the keys manager.
  [ProfilingConditionalTextProvider](../api/ProfilingConditionalTextProvider.md) [getProfilingConditionalTextProvider](#getProfilingConditionalTextProvider())()
Creates a new [ProfilingConditionalTextProvider](../api/ProfilingConditionalTextProvider.md) instance responsible for providing custom support regarding profiling and conditional text.
  [SpellCheckerHelper](../api/spell/SpellCheckerHelper.md) [getSpellCheckerHelper](#getSpellCheckerHelper())()
Get a helper for the spell checker.
  [UniqueAttributesRecognizer](../api/UniqueAttributesRecognizer.md) [getUniqueAttributesIdentifier](#getUniqueAttributesIdentifier())()
Get an unique attributes creator and identifier.
  boolean [isContentReference](#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Check if this node references another node which should replace it entirely.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolveCustomAttributeValue](#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext))([CustomAttributeValueContext](../api/CustomAttributeValueContext.md) attributeValueEditingContext)
Resolve a custom attribute value to an URL which will be opened by Oxygen.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolveCustomHref](#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [AuthorNode](../api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](../api/AuthorAccess.md) authorAccess)
When clicking a href the bundle can custom solve the href to an URL.

### Methods inherited from class ro.sync.ecss.extensions.api.[ExtensionsBundle](../api/ExtensionsBundle.md)
 [createAttributesValueEditor](../api/ExtensionsBundle.md#createAttributesValueEditor(boolean)), [createAuthorAWTDndListener](../api/ExtensionsBundle.md#createAuthorAWTDndListener()), [createAuthorBreadCrumbCustomizer](../api/ExtensionsBundle.md#createAuthorBreadCrumbCustomizer()), [createAuthorOutlineCustomizer](../api/ExtensionsBundle.md#createAuthorOutlineCustomizer()), [createAuthorPreloadProcessor](../api/ExtensionsBundle.md#createAuthorPreloadProcessor()), [createAuthorStylesFilter](../api/ExtensionsBundle.md#createAuthorStylesFilter()), [createAuthorSWTDndListener](../api/ExtensionsBundle.md#createAuthorSWTDndListener()), [createCustomAttributeValueEditor](../api/ExtensionsBundle.md#createCustomAttributeValueEditor(boolean)), [createTextSWTDndListener](../api/ExtensionsBundle.md#createTextSWTDndListener()), [getDocumentTypeName](../api/ExtensionsBundle.md#getDocumentTypeName()), [getWebappExtensionsProvier](../api/ExtensionsBundle.md#getWebappExtensionsProvier()), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.lang.String)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [setDocumentTypeName](../api/ExtensionsBundle.md#setDocumentTypeName(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### keyManager

protected [ContextKeyManager](../../dita/ContextKeyManager.md) keyManager

The key manager that is context aware and is used to resolve key refs.

### keyManagerProvider

protected final [ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) keyManagerProvider

The provider for the key manager which is context aware and is used to resolve key refs.

## Constructor Details

### DITAExtensionsBundle

public DITAExtensionsBundle()

## Method Details

### createAuthorExtensionStateListener

public [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) createAuthorExtensionStateListener()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createAuthorExtensionStateListener())
Returns the [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) which will be notified when the Author extension where it is defined is activated and deactivated during the detection process. This method is called each time the Document Type association where the Author extension and the extensions bundle are defined matches a document opened in an Author page.
  Overrides: [createAuthorExtensionStateListener](../api/ExtensionsBundle.md#createAuthorExtensionStateListener()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) instance. See Also:
        * [ExtensionsBundle.createAuthorExtensionStateListener()](../api/ExtensionsBundle.md#createAuthorExtensionStateListener())

### createContextKeyManager

protected [ContextKeyManager](../../dita/ContextKeyManager.md) createContextKeyManager([EditingSessionContext](../api/access/EditingSessionContext.md) context)

Create a context key manager to be used when resolving keyrefs. The key manager may resolve keys depending on the editing session context. The current implementation checks the [DITAAccess.DITA_ROOT_MAP_URL_ATTRIBUTE](../../dita/DITAAccess.md#DITA_ROOT_MAP_URL_ATTRIBUTE)and if it was set, the specified map is used. Otherwise, it uses the default ditamap in Autor.
  Parameters: context - The editing session context. Returns: The key manager.
### getClipboardFragmentProcessor

public [ClipboardFragmentProcessor](../api/content/ClipboardFragmentProcessor.md) getClipboardFragmentProcessor()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getClipboardFragmentProcessor())
Get a processor for Author Document Fragments in the clipboard (which will be pasted, dropped, etc).
  Overrides: [getClipboardFragmentProcessor](../api/ExtensionsBundle.md#getClipboardFragmentProcessor()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: a processor for Author Document Fragments in the clipboard (which will be pasted, dropped, etc). See Also:
        * [ExtensionsBundle.getClipboardFragmentProcessor()](../api/ExtensionsBundle.md#getClipboardFragmentProcessor())

### createAuthorReferenceResolver

public [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) createAuthorReferenceResolver()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createAuthorReferenceResolver())
Creates a new [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) instance used to expand content references. The method is called each time an opened document in an Author editor page matches the document type association where the extensions bundle is defined.
  Overrides: [createAuthorReferenceResolver](../api/ExtensionsBundle.md#createAuthorReferenceResolver()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) instance. See Also:
        * [ExtensionsBundle.createAuthorReferenceResolver()](../api/ExtensionsBundle.md#createAuthorReferenceResolver())

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

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../api/Extension.md#getDescription()) in interface [Extension](../api/Extension.md) Returns: The description of the extension. See Also:
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

### createElementLocatorProvider

public [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) createElementLocatorProvider()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createElementLocatorProvider())
Creates a new [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) instance responsible for providing an implementation of an [ElementLocator](../api/link/ElementLocator.md) based on the structure of a link. The [ElementLocator](../api/link/ElementLocator.md) is capable of locating an element pointed by the supplied link. This method is called each time an element needs to be located based on a link specification.
  Overrides: [createElementLocatorProvider](../api/ExtensionsBundle.md#createElementLocatorProvider()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [ElementLocatorProvider](../api/link/ElementLocatorProvider.md) instance. See Also:
        * [ExtensionsBundle.createElementLocatorProvider()](../api/ExtensionsBundle.md#createElementLocatorProvider())

### customizeLinkTooltipDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) customizeLinkTooltipDescription([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [AuthorNode](../api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computedDescription)
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))
Customize the tooltip description when hovering over a link.
  Overrides: [customizeLinkTooltipDescription](../api/ExtensionsBundle.md#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Parameters: currentEditorURL - The current document URL contextNode - The context node linkHref - The link href. authorAccess - The Author access computedDescription - The already computed description. Usually something like: "Click to open: URL" Returns: The customized description. See Also:
        * [ExtensionsBundle.customizeLinkTooltipDescription(java.net.URL, ro.sync.ecss.extensions.api.node.AuthorNode, java.lang.String, ro.sync.ecss.extensions.api.AuthorAccess, java.lang.String)](../api/ExtensionsBundle.md#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))

### customizeImageTooltipDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) customizeImageTooltipDescription([AuthorNode](../api/node/AuthorNode.md) contextNode, [AuthorAccess](../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computedDescription)
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))
Customize the tooltip description when hovering over an image.
  Overrides: [customizeImageTooltipDescription](../api/ExtensionsBundle.md#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Parameters: contextNode - The context node authorAccess - The Author access computedDescription - The already computed description. Returns: The customized description. See Also:
        * [ExtensionsBundle.customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode, ro.sync.ecss.extensions.api.AuthorAccess, java.lang.String)](../api/ExtensionsBundle.md#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))

### resolveCustomHref

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolveCustomHref([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [AuthorNode](../api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](../api/AuthorAccess.md) authorAccess)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [CustomResolverException](../api/CustomResolverException.md)
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))
When clicking a href the bundle can custom solve the href to an URL.
  Overrides: [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Parameters: currentEditorURL - The URL of the current editor. contextNode - The context node in which the href needs to be computed. linkHref - The link href as derrived from the CSS authorAccess - The Author Access. Returns: The resolved absolute URL if null if the default behavior will be performed Throws: [CustomResolverException](../api/CustomResolverException.md) - If the link is recognized by the extensions bundle, but could not be mapped to an URL. It offers a solution to the user. This solution is invoked when the user clicks on the error message. [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the link is recognized by the extensions bundle, but could not be mapped to an URL. See Also:
        * [ExtensionsBundle.resolveCustomHref(java.net.URL, ro.sync.ecss.extensions.api.node.AuthorNode, java.lang.String, ro.sync.ecss.extensions.api.AuthorAccess)](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))

### getAuthorSchemaAwareEditingHandler

public [AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md) getAuthorSchemaAwareEditingHandler()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler())
If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this support. The support can either resolve a specific case, let the default implementation take place or reject the edit entirely by throwing an [InvalidEditException](../api/InvalidEditException.md). It is recommended to extend class [AuthorSchemaAwareEditingHandlerAdapter](../api/AuthorSchemaAwareEditingHandlerAdapter.md) in order to be protected from any API additions that may occur in interface [AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md).
  Overrides: [getAuthorSchemaAwareEditingHandler](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A custom editing handler for schema aware actions, or null if there is no handler and the default processing should take place. See Also:
        * [ExtensionsBundle.getAuthorSchemaAwareEditingHandler()](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler())

### createSchemaManagerFilter

public [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) createSchemaManagerFilter()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createSchemaManagerFilter())
Creates a new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance used to filter the content completion proposals from the schema manager. This method is called each time the document type where the extensions bundle is defined matches a document opened in an editor.
  Overrides: [createSchemaManagerFilter](../api/ExtensionsBundle.md#createSchemaManagerFilter()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance. See Also:
        * [ExtensionsBundle.createSchemaManagerFilter()](../api/ExtensionsBundle.md#createSchemaManagerFilter())

### createExternalObjectInsertionHandler

public [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) createExternalObjectInsertionHandler()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler())
Create a handler which gets notified when external resources need to be inserted in the Author page. The usual usage for this is to get notified when URLs are dropped from the project or DITA Maps manager in the Author page.
  Overrides: [createExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: The External URLs handler See Also:
        * [ExtensionsBundle.createExternalObjectInsertionHandler()](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler())

### createTextPageExternalObjectInsertionHandler

public [TextPageExternalObjectInsertionHandler](../api/text/TextPageExternalObjectInsertionHandler.md) createTextPageExternalObjectInsertionHandler()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createTextPageExternalObjectInsertionHandler())
Create a handler which gets notified when external resources need to be inserted in the Text page. The usual usage for this is to get notified when URLs are dropped from the project or DITA Maps manager in the Text page.
  Overrides: [createTextPageExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createTextPageExternalObjectInsertionHandler()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: The External URLs handler See Also:
        * [ExtensionsBundle.createTextPageExternalObjectInsertionHandler()](../api/ExtensionsBundle.md#createTextPageExternalObjectInsertionHandler())

### isContentReference

public boolean isContentReference([AuthorNode](../api/node/AuthorNode.md) node)
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if this node references another node which should replace it entirely. This is used in the tables to replace conreffed table rows entirely
  Overrides: [isContentReference](../api/ExtensionsBundle.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Parameters: node - The node Returns: true if this node references another node which should replace it entirely. See Also:
        * [ExtensionsBundle.isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)](../api/ExtensionsBundle.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode))

### getProfilingConditionalTextProvider

public [ProfilingConditionalTextProvider](../api/ProfilingConditionalTextProvider.md) getProfilingConditionalTextProvider()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getProfilingConditionalTextProvider())
Creates a new [ProfilingConditionalTextProvider](../api/ProfilingConditionalTextProvider.md) instance responsible for providing custom support regarding profiling and conditional text.
  Overrides: [getProfilingConditionalTextProvider](../api/ExtensionsBundle.md#getProfilingConditionalTextProvider()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [ProfilingConditionalTextProvider](../api/ProfilingConditionalTextProvider.md) instance. See Also:
        * [ExtensionsBundle.getProfilingConditionalTextProvider()](../api/ExtensionsBundle.md#getProfilingConditionalTextProvider())

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

### createLinkTextResolver

public [LinkTextResolver](../api/link/LinkTextResolver.md) createLinkTextResolver()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createLinkTextResolver())
Creates a new [LinkTextResolver](../api/link/LinkTextResolver.md) instance responsible for resolving a specific link marked in the CSS file and returning a text content from the targeted location. This text content will be presented as a static text associated with the link in author page. This resolver will be used when function oxy_link-text() is encountered inside the CSS rules on the 'content' property.
  Overrides: [createLinkTextResolver](../api/ExtensionsBundle.md#createLinkTextResolver()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [LinkTextResolver](../api/link/LinkTextResolver.md) instance. See Also:
        * [ExtensionsBundle.createLinkTextResolver()](../api/ExtensionsBundle.md#createLinkTextResolver())

### createIDTypeRecognizer

public [IDTypeRecognizer](../api/link/IDTypeRecognizer.md) createIDTypeRecognizer()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createIDTypeRecognizer())
Creates a new [IDTypeRecognizer](../api/link/IDTypeRecognizer.md) instance responsible for providing an implementation which can recognize ID declarations and references. This method is called each time an ID must be recognized or certain ID-aware searches or refactory actions are performed.
  Overrides: [createIDTypeRecognizer](../api/ExtensionsBundle.md#createIDTypeRecognizer()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [IDTypeRecognizer](../api/link/IDTypeRecognizer.md) instance. See Also:
        * [ExtensionsBundle.createIDTypeRecognizer()](../api/ExtensionsBundle.md#createIDTypeRecognizer())

### getKeyManager

public [ContextKeyManager](../../dita/ContextKeyManager.md) getKeyManager()

Returns the keys manager.
  Returns: Returns the keys manager.
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

### getContextKeyManager

public [ContextKeyManager](../../dita/ContextKeyManager.md) getContextKeyManager()
  Specified by: [getContextKeyManager](../../dita/ContextKeyManagerProvider.md#getContextKeyManager()) in interface [ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) Returns: The context key manager. See Also:
        * [ContextKeyManagerProvider.getContextKeyManager()](../../dita/ContextKeyManagerProvider.md#getContextKeyManager())

### resolveCustomAttributeValue

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolveCustomAttributeValue([CustomAttributeValueContext](../api/CustomAttributeValueContext.md) attributeValueEditingContext)
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext))
Resolve a custom attribute value to an URL which will be opened by Oxygen. This method is called when the "Open File at Cursor" action is called in the Text editor page.
  Overrides: [resolveCustomAttributeValue](../api/ExtensionsBundle.md#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext)) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Parameters: attributeValueEditingContext - The editing context. Returns: The URL which should be opened as a result of "Open File at Cursor" being invoked on the attribute value. See Also:
        * [ExtensionsBundle.resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext)](../api/ExtensionsBundle.md#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext))

### getSpellCheckerHelper

public [SpellCheckerHelper](../api/spell/SpellCheckerHelper.md) getSpellCheckerHelper()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getSpellCheckerHelper())
Get a helper for the spell checker.
  Overrides: [getSpellCheckerHelper](../api/ExtensionsBundle.md#getSpellCheckerHelper()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: Helper utilities implemented at framework level. See Also:
        * [ExtensionsBundle.getSpellCheckerHelper()](../api/ExtensionsBundle.md#getSpellCheckerHelper())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
