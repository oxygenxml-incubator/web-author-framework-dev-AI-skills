Package [ro.sync.ecss.extensions.dita.map](package-summary.md)

# Class DITAMapExtensionsBundle

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.ExtensionsBundle](../../api/ExtensionsBundle.md)
        * [ro.sync.ecss.extensions.dita.DITAExtensionsBundle](../DITAExtensionsBundle.md)
            * ro.sync.ecss.extensions.dita.map.DITAMapExtensionsBundle
   All Implemented Interfaces: [ContextKeyManagerProvider](../../../dita/ContextKeyManagerProvider.md), [Extension](../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DITAMapExtensionsBundle extends [DITAExtensionsBundle](../DITAExtensionsBundle.md)
DITA Map extensions bundle

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.dita.[DITAExtensionsBundle](../DITAExtensionsBundle.md)
 [keyManager](../DITAExtensionsBundle.md#keyManager), [keyManagerProvider](../DITAExtensionsBundle.md#keyManagerProvider)
## Constructor Summary
 Constructors
Constructor

Description
 [DITAMapExtensionsBundle](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md) [createAuthorExtensionStateListener](#createAuthorExtensionStateListener())()
Returns the [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md) which will be notified when the Author extension where it is defined is activated and deactivated during the detection process.
  [AuthorPreloadProcessor](../../api/AuthorPreloadProcessor.md) [createAuthorPreloadProcessor](#createAuthorPreloadProcessor())()
Returns the [AuthorPreloadProcessor](../../api/AuthorPreloadProcessor.md) which will be notified before the document is presented in the application.
  [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md) [createAuthorReferenceResolver](#createAuthorReferenceResolver())()
Creates a new [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md) instance used to expand content references.
  [EditPropertiesHandler](../../api/EditPropertiesHandler.md) [createEditPropertiesHandler](#createEditPropertiesHandler())()
A custom implementation to handle editing properties of an author node.
  [ElementLocatorProvider](../../api/link/ElementLocatorProvider.md) [createElementLocatorProvider](#createElementLocatorProvider())()
Creates a new [ElementLocatorProvider](../../api/link/ElementLocatorProvider.md) instance responsible for providing an implementation of an [ElementLocator](../../api/link/ElementLocator.md) based on the structure of a link.
  [AuthorExternalObjectInsertionHandler](../../api/AuthorExternalObjectInsertionHandler.md) [createExternalObjectInsertionHandler](#createExternalObjectInsertionHandler())()
Create a handler which gets notified when external resources need to be inserted in the Author page.
  [TextPageExternalObjectInsertionHandler](../../api/text/TextPageExternalObjectInsertionHandler.md) [createTextPageExternalObjectInsertionHandler](#createTextPageExternalObjectInsertionHandler())()
Create a handler which gets notified when external resources need to be inserted in the Text page.
  [AuthorSchemaAwareEditingHandler](../../api/AuthorSchemaAwareEditingHandler.md) [getAuthorSchemaAwareEditingHandler](#getAuthorSchemaAwareEditingHandler())()
If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this support.
  [AuthorTableOperationsHandler](../../api/table/operations/AuthorTableOperationsHandler.md) [getAuthorTableOperationsHandler](#getAuthorTableOperationsHandler())()
Get the [AuthorTableOperationsHandler](../../api/table/operations/AuthorTableOperationsHandler.md) instance responsible for handling table operations.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditorPage)
Get the help page ID for this particular framework extensions bundle.

### Methods inherited from class ro.sync.ecss.extensions.dita.[DITAExtensionsBundle](../DITAExtensionsBundle.md)
 [createAuthorTableCellSepProvider](../DITAExtensionsBundle.md#createAuthorTableCellSepProvider()), [createAuthorTableCellSpanProvider](../DITAExtensionsBundle.md#createAuthorTableCellSpanProvider()), [createAuthorTableColumnWidthProvider](../DITAExtensionsBundle.md#createAuthorTableColumnWidthProvider()), [createContextKeyManager](../DITAExtensionsBundle.md#createContextKeyManager(ro.sync.ecss.extensions.api.access.EditingSessionContext)), [createIDTypeRecognizer](../DITAExtensionsBundle.md#createIDTypeRecognizer()), [createLinkTextResolver](../DITAExtensionsBundle.md#createLinkTextResolver()), [createSchemaManagerFilter](../DITAExtensionsBundle.md#createSchemaManagerFilter()), [createXMLNodeCustomizer](../DITAExtensionsBundle.md#createXMLNodeCustomizer()), [customizeImageTooltipDescription](../DITAExtensionsBundle.md#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [customizeLinkTooltipDescription](../DITAExtensionsBundle.md#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [getAuthorActionEventHandler](../DITAExtensionsBundle.md#getAuthorActionEventHandler()), [getAuthorImageDecorator](../DITAExtensionsBundle.md#getAuthorImageDecorator()), [getClipboardFragmentProcessor](../DITAExtensionsBundle.md#getClipboardFragmentProcessor()), [getContextKeyManager](../DITAExtensionsBundle.md#getContextKeyManager()), [getDescription](../DITAExtensionsBundle.md#getDescription()), [getDocumentTypeID](../DITAExtensionsBundle.md#getDocumentTypeID()), [getKeyManager](../DITAExtensionsBundle.md#getKeyManager()), [getProfilingConditionalTextProvider](../DITAExtensionsBundle.md#getProfilingConditionalTextProvider()), [getSpellCheckerHelper](../DITAExtensionsBundle.md#getSpellCheckerHelper()), [getUniqueAttributesIdentifier](../DITAExtensionsBundle.md#getUniqueAttributesIdentifier()), [isContentReference](../DITAExtensionsBundle.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)), [resolveCustomAttributeValue](../DITAExtensionsBundle.md#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext)), [resolveCustomHref](../DITAExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))
### Methods inherited from class ro.sync.ecss.extensions.api.[ExtensionsBundle](../../api/ExtensionsBundle.md)
 [createAttributesValueEditor](../../api/ExtensionsBundle.md#createAttributesValueEditor(boolean)), [createAuthorAWTDndListener](../../api/ExtensionsBundle.md#createAuthorAWTDndListener()), [createAuthorBreadCrumbCustomizer](../../api/ExtensionsBundle.md#createAuthorBreadCrumbCustomizer()), [createAuthorOutlineCustomizer](../../api/ExtensionsBundle.md#createAuthorOutlineCustomizer()), [createAuthorStylesFilter](../../api/ExtensionsBundle.md#createAuthorStylesFilter()), [createAuthorSWTDndListener](../../api/ExtensionsBundle.md#createAuthorSWTDndListener()), [createCustomAttributeValueEditor](../../api/ExtensionsBundle.md#createCustomAttributeValueEditor(boolean)), [createTextSWTDndListener](../../api/ExtensionsBundle.md#createTextSWTDndListener()), [getDocumentTypeName](../../api/ExtensionsBundle.md#getDocumentTypeName()), [getWebappExtensionsProvier](../../api/ExtensionsBundle.md#getWebappExtensionsProvier()), [resolveCustomHref](../../api/ExtensionsBundle.md#resolveCustomHref(java.lang.String)), [resolveCustomHref](../../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [setDocumentTypeName](../../api/ExtensionsBundle.md#setDocumentTypeName(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAMapExtensionsBundle

public DITAMapExtensionsBundle()

## Method Details

### createAuthorExtensionStateListener

public [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md) createAuthorExtensionStateListener()
 Description copied from class: [ExtensionsBundle](../../api/ExtensionsBundle.md#createAuthorExtensionStateListener())
Returns the [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md) which will be notified when the Author extension where it is defined is activated and deactivated during the detection process. This method is called each time the Document Type association where the Author extension and the extensions bundle are defined matches a document opened in an Author page.
  Overrides: [createAuthorExtensionStateListener](../DITAExtensionsBundle.md#createAuthorExtensionStateListener()) in class [DITAExtensionsBundle](../DITAExtensionsBundle.md) Returns: A new [AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md) instance. See Also:
        * [DITAExtensionsBundle.createAuthorExtensionStateListener()](../DITAExtensionsBundle.md#createAuthorExtensionStateListener())

### createAuthorPreloadProcessor

public [AuthorPreloadProcessor](../../api/AuthorPreloadProcessor.md) createAuthorPreloadProcessor()
 Description copied from class: [ExtensionsBundle](../../api/ExtensionsBundle.md#createAuthorPreloadProcessor())
Returns the [AuthorPreloadProcessor](../../api/AuthorPreloadProcessor.md) which will be notified before the document is presented in the application.
  Overrides: [createAuthorPreloadProcessor](../../api/ExtensionsBundle.md#createAuthorPreloadProcessor()) in class [ExtensionsBundle](../../api/ExtensionsBundle.md) Returns: A new [AuthorPreloadProcessor](../../api/AuthorPreloadProcessor.md) instance. See Also:
        * [ExtensionsBundle.createAuthorPreloadProcessor()](../../api/ExtensionsBundle.md#createAuthorPreloadProcessor())

### createAuthorReferenceResolver

public [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md) createAuthorReferenceResolver()
 Description copied from class: [ExtensionsBundle](../../api/ExtensionsBundle.md#createAuthorReferenceResolver())
Creates a new [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md) instance used to expand content references. The method is called each time an opened document in an Author editor page matches the document type association where the extensions bundle is defined.
  Overrides: [createAuthorReferenceResolver](../DITAExtensionsBundle.md#createAuthorReferenceResolver()) in class [DITAExtensionsBundle](../DITAExtensionsBundle.md) Returns: A new [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md) instance. See Also:
        * [ExtensionsBundle.createAuthorReferenceResolver()](../../api/ExtensionsBundle.md#createAuthorReferenceResolver())

### createExternalObjectInsertionHandler

public [AuthorExternalObjectInsertionHandler](../../api/AuthorExternalObjectInsertionHandler.md) createExternalObjectInsertionHandler()
 Description copied from class: [ExtensionsBundle](../../api/ExtensionsBundle.md#createExternalObjectInsertionHandler())
Create a handler which gets notified when external resources need to be inserted in the Author page. The usual usage for this is to get notified when URLs are dropped from the project or DITA Maps manager in the Author page.
  Overrides: [createExternalObjectInsertionHandler](../DITAExtensionsBundle.md#createExternalObjectInsertionHandler()) in class [DITAExtensionsBundle](../DITAExtensionsBundle.md) Returns: The External URLs handler See Also:
        * [DITAExtensionsBundle.createExternalObjectInsertionHandler()](../DITAExtensionsBundle.md#createExternalObjectInsertionHandler())

### createElementLocatorProvider

public [ElementLocatorProvider](../../api/link/ElementLocatorProvider.md) createElementLocatorProvider()
 Description copied from class: [ExtensionsBundle](../../api/ExtensionsBundle.md#createElementLocatorProvider())
Creates a new [ElementLocatorProvider](../../api/link/ElementLocatorProvider.md) instance responsible for providing an implementation of an [ElementLocator](../../api/link/ElementLocator.md) based on the structure of a link. The [ElementLocator](../../api/link/ElementLocator.md) is capable of locating an element pointed by the supplied link. This method is called each time an element needs to be located based on a link specification.
  Overrides: [createElementLocatorProvider](../DITAExtensionsBundle.md#createElementLocatorProvider()) in class [DITAExtensionsBundle](../DITAExtensionsBundle.md) Returns: A new [ElementLocatorProvider](../../api/link/ElementLocatorProvider.md) instance. See Also:
        * [DITAExtensionsBundle.createElementLocatorProvider()](../DITAExtensionsBundle.md#createElementLocatorProvider())

### getAuthorTableOperationsHandler

public [AuthorTableOperationsHandler](../../api/table/operations/AuthorTableOperationsHandler.md) getAuthorTableOperationsHandler()
 Description copied from class: [ExtensionsBundle](../../api/ExtensionsBundle.md#getAuthorTableOperationsHandler())
Get the [AuthorTableOperationsHandler](../../api/table/operations/AuthorTableOperationsHandler.md) instance responsible for handling table operations.
  Overrides: [getAuthorTableOperationsHandler](../DITAExtensionsBundle.md#getAuthorTableOperationsHandler()) in class [DITAExtensionsBundle](../DITAExtensionsBundle.md) Returns: Author table operations handler. See Also:
        * [ExtensionsBundle.getAuthorTableOperationsHandler()](../../api/ExtensionsBundle.md#getAuthorTableOperationsHandler())

### createEditPropertiesHandler

public [EditPropertiesHandler](../../api/EditPropertiesHandler.md) createEditPropertiesHandler()
 Description copied from class: [ExtensionsBundle](../../api/ExtensionsBundle.md#createEditPropertiesHandler())
A custom implementation to handle editing properties of an author node. For example when a user double clicks on an element tag we will invoke this extension and a specific dialog can be presented.
  Overrides: [createEditPropertiesHandler](../DITAExtensionsBundle.md#createEditPropertiesHandler()) in class [DITAExtensionsBundle](../DITAExtensionsBundle.md) Returns: An implementation that can edit the properties of nodes. See Also:
        * [ExtensionsBundle.createEditPropertiesHandler()](../../api/ExtensionsBundle.md#createEditPropertiesHandler())

### createTextPageExternalObjectInsertionHandler

public [TextPageExternalObjectInsertionHandler](../../api/text/TextPageExternalObjectInsertionHandler.md) createTextPageExternalObjectInsertionHandler()
 Description copied from class: [ExtensionsBundle](../../api/ExtensionsBundle.md#createTextPageExternalObjectInsertionHandler())
Create a handler which gets notified when external resources need to be inserted in the Text page. The usual usage for this is to get notified when URLs are dropped from the project or DITA Maps manager in the Text page.
  Overrides: [createTextPageExternalObjectInsertionHandler](../DITAExtensionsBundle.md#createTextPageExternalObjectInsertionHandler()) in class [DITAExtensionsBundle](../DITAExtensionsBundle.md) Returns: The External URLs handler See Also:
        * [DITAExtensionsBundle.createTextPageExternalObjectInsertionHandler()](../DITAExtensionsBundle.md#createTextPageExternalObjectInsertionHandler())

### getHelpPageID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditorPage)
 Description copied from class: [ExtensionsBundle](../../api/ExtensionsBundle.md#getHelpPageID(java.lang.String))
Get the help page ID for this particular framework extensions bundle. If the returned help page ID is an URL, a web browser will be opened pointing to that URL when the user presses F1 in the dialog or when using the Help button. If the returned help page ID is an identifier, when help is invoked, the application will open the Oxygen User's Manual and locate this identifier inside it.
  Overrides: [getHelpPageID](../DITAExtensionsBundle.md#getHelpPageID(java.lang.String)) in class [DITAExtensionsBundle](../DITAExtensionsBundle.md) Parameters: currentEditorPage - The current editor page mode (Text/Grid/Author/Schema), one of the constants in the "ro.sync.exml.editor.EditorPageConstants" interface. Returns: The help page ID, by default no help page ID is returned. See Also:
        * [ExtensionsBundle.getHelpPageID(java.lang.String)](../../api/ExtensionsBundle.md#getHelpPageID(java.lang.String))

### getAuthorSchemaAwareEditingHandler

public [AuthorSchemaAwareEditingHandler](../../api/AuthorSchemaAwareEditingHandler.md) getAuthorSchemaAwareEditingHandler()
 Description copied from class: [ExtensionsBundle](../../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler())
If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this support. The support can either resolve a specific case, let the default implementation take place or reject the edit entirely by throwing an [InvalidEditException](../../api/InvalidEditException.md). It is recommended to extend class [AuthorSchemaAwareEditingHandlerAdapter](../../api/AuthorSchemaAwareEditingHandlerAdapter.md) in order to be protected from any API additions that may occur in interface [AuthorSchemaAwareEditingHandler](../../api/AuthorSchemaAwareEditingHandler.md).
  Overrides: [getAuthorSchemaAwareEditingHandler](../DITAExtensionsBundle.md#getAuthorSchemaAwareEditingHandler()) in class [DITAExtensionsBundle](../DITAExtensionsBundle.md) Returns: A custom editing handler for schema aware actions, or null if there is no handler and the default processing should take place. See Also:
        * [ExtensionsBundle.getAuthorSchemaAwareEditingHandler()](../../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
