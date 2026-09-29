Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DITAValExtensionsBundle

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.ExtensionsBundle](../api/ExtensionsBundle.md)
        * ro.sync.ecss.extensions.dita.DITAValExtensionsBundle
   All Implemented Interfaces: [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DITAValExtensionsBundle extends [ExtensionsBundle](../api/ExtensionsBundle.md)
The DITAVal extensions bundle

## Constructor Summary
 Constructors
Constructor

Description
 [DITAValExtensionsBundle](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) [createSchemaManagerFilter](#createSchemaManagerFilter())()
Creates a new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance used to filter the content completion proposals from the schema manager.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentTypeID](#getDocumentTypeID())()
This should never return null if the [OptionsStorage](../api/OptionsStorage.md)support it is intended to be used.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditorPage)
Get the help page ID for this particular framework extensions bundle.

### Methods inherited from class ro.sync.ecss.extensions.api.[ExtensionsBundle](../api/ExtensionsBundle.md)
 [createAttributesValueEditor](../api/ExtensionsBundle.md#createAttributesValueEditor(boolean)), [createAuthorAWTDndListener](../api/ExtensionsBundle.md#createAuthorAWTDndListener()), [createAuthorBreadCrumbCustomizer](../api/ExtensionsBundle.md#createAuthorBreadCrumbCustomizer()), [createAuthorExtensionStateListener](../api/ExtensionsBundle.md#createAuthorExtensionStateListener()), [createAuthorOutlineCustomizer](../api/ExtensionsBundle.md#createAuthorOutlineCustomizer()), [createAuthorPreloadProcessor](../api/ExtensionsBundle.md#createAuthorPreloadProcessor()), [createAuthorReferenceResolver](../api/ExtensionsBundle.md#createAuthorReferenceResolver()), [createAuthorStylesFilter](../api/ExtensionsBundle.md#createAuthorStylesFilter()), [createAuthorSWTDndListener](../api/ExtensionsBundle.md#createAuthorSWTDndListener()), [createAuthorTableCellSepProvider](../api/ExtensionsBundle.md#createAuthorTableCellSepProvider()), [createAuthorTableCellSpanProvider](../api/ExtensionsBundle.md#createAuthorTableCellSpanProvider()), [createAuthorTableColumnWidthProvider](../api/ExtensionsBundle.md#createAuthorTableColumnWidthProvider()), [createCustomAttributeValueEditor](../api/ExtensionsBundle.md#createCustomAttributeValueEditor(boolean)), [createEditPropertiesHandler](../api/ExtensionsBundle.md#createEditPropertiesHandler()), [createElementLocatorProvider](../api/ExtensionsBundle.md#createElementLocatorProvider()), [createExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler()), [createIDTypeRecognizer](../api/ExtensionsBundle.md#createIDTypeRecognizer()), [createLinkTextResolver](../api/ExtensionsBundle.md#createLinkTextResolver()), [createTextPageExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createTextPageExternalObjectInsertionHandler()), [createTextSWTDndListener](../api/ExtensionsBundle.md#createTextSWTDndListener()), [createXMLNodeCustomizer](../api/ExtensionsBundle.md#createXMLNodeCustomizer()), [customizeImageTooltipDescription](../api/ExtensionsBundle.md#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [customizeLinkTooltipDescription](../api/ExtensionsBundle.md#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [getAuthorActionEventHandler](../api/ExtensionsBundle.md#getAuthorActionEventHandler()), [getAuthorImageDecorator](../api/ExtensionsBundle.md#getAuthorImageDecorator()), [getAuthorSchemaAwareEditingHandler](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler()), [getAuthorTableOperationsHandler](../api/ExtensionsBundle.md#getAuthorTableOperationsHandler()), [getClipboardFragmentProcessor](../api/ExtensionsBundle.md#getClipboardFragmentProcessor()), [getDocumentTypeName](../api/ExtensionsBundle.md#getDocumentTypeName()), [getProfilingConditionalTextProvider](../api/ExtensionsBundle.md#getProfilingConditionalTextProvider()), [getSpellCheckerHelper](../api/ExtensionsBundle.md#getSpellCheckerHelper()), [getUniqueAttributesIdentifier](../api/ExtensionsBundle.md#getUniqueAttributesIdentifier()), [getWebappExtensionsProvier](../api/ExtensionsBundle.md#getWebappExtensionsProvier()), [isContentReference](../api/ExtensionsBundle.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)), [resolveCustomAttributeValue](../api/ExtensionsBundle.md#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.lang.String)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [setDocumentTypeName](../api/ExtensionsBundle.md#setDocumentTypeName(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAValExtensionsBundle

public DITAValExtensionsBundle()

## Method Details

### createSchemaManagerFilter

public [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) createSchemaManagerFilter()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createSchemaManagerFilter())
Creates a new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance used to filter the content completion proposals from the schema manager. This method is called each time the document type where the extensions bundle is defined matches a document opened in an editor.
  Overrides: [createSchemaManagerFilter](../api/ExtensionsBundle.md#createSchemaManagerFilter()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) instance. See Also:
        * [ExtensionsBundle.createSchemaManagerFilter()](../api/ExtensionsBundle.md#createSchemaManagerFilter())

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

### getHelpPageID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditorPage)
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String))
Get the help page ID for this particular framework extensions bundle. If the returned help page ID is an URL, a web browser will be opened pointing to that URL when the user presses F1 in the dialog or when using the Help button. If the returned help page ID is an identifier, when help is invoked, the application will open the Oxygen User's Manual and locate this identifier inside it.
  Overrides: [getHelpPageID](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String)) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Parameters: currentEditorPage - The current editor page mode (Text/Grid/Author/Schema), one of the constants in the "ro.sync.exml.editor.EditorPageConstants" interface. Returns: The help page ID, by default no help page ID is returned. See Also:
        * [ExtensionsBundle.getHelpPageID(java.lang.String)](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
