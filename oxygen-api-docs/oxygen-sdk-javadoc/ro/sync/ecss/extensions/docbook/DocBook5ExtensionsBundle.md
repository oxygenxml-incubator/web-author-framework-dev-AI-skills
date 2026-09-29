Package [ro.sync.ecss.extensions.docbook](package-summary.md)

# Class DocBook5ExtensionsBundle

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.ExtensionsBundle](../api/ExtensionsBundle.md)
        * [ro.sync.ecss.extensions.docbook.DocBookExtensionsBundleBase](DocBookExtensionsBundleBase.md)
            * ro.sync.ecss.extensions.docbook.DocBook5ExtensionsBundle
   All Implemented Interfaces: [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DocBook5ExtensionsBundle extends [DocBookExtensionsBundleBase](DocBookExtensionsBundleBase.md)
The DocBook 5 framework extensions bundle.

## Constructor Summary
 Constructors
Constructor

Description
 [DocBook5ExtensionsBundle](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) [createAuthorExtensionStateListener](#createAuthorExtensionStateListener())()
Returns the [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) which will be notified when the Author extension where it is defined is activated and deactivated during the detection process.
  [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) [createExternalObjectInsertionHandler](#createExternalObjectInsertionHandler())()
Create a handler which gets notified when external resources need to be inserted in the Author page.
  [AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md) [getAuthorSchemaAwareEditingHandler](#getAuthorSchemaAwareEditingHandler())()
If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this support.
  [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) [getAuthorTableOperationsHandler](#getAuthorTableOperationsHandler())()
Get the [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) instance responsible for handling table operations.
  [ClipboardFragmentProcessor](../api/content/ClipboardFragmentProcessor.md) [getClipboardFragmentProcessor](#getClipboardFragmentProcessor())()
Get a processor for Author Document Fragments in the clipboard (which will be pasted, dropped, etc).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentNamespace](#getDocumentNamespace())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentTypeID](#getDocumentTypeID())()
This should never return null if the [OptionsStorage](../api/OptionsStorage.md)support it is intended to be used.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditorPage)
Get the help page ID for this particular framework extensions bundle.
  [ProfilingConditionalTextProvider](../api/ProfilingConditionalTextProvider.md) [getProfilingConditionalTextProvider](#getProfilingConditionalTextProvider())()
Creates a new [ProfilingConditionalTextProvider](../api/ProfilingConditionalTextProvider.md) instance responsible for providing custom support regarding profiling and conditional text.
  [UniqueAttributesRecognizer](../api/UniqueAttributesRecognizer.md) [getUniqueAttributesIdentifier](#getUniqueAttributesIdentifier())()
Get an unique attributes creator and identifier.

### Methods inherited from class ro.sync.ecss.extensions.docbook.[DocBookExtensionsBundleBase](DocBookExtensionsBundleBase.md)
 [createAuthorTableCellSepProvider](DocBookExtensionsBundleBase.md#createAuthorTableCellSepProvider()), [createAuthorTableCellSpanProvider](DocBookExtensionsBundleBase.md#createAuthorTableCellSpanProvider()), [createAuthorTableColumnWidthProvider](DocBookExtensionsBundleBase.md#createAuthorTableColumnWidthProvider()), [createEditPropertiesHandler](DocBookExtensionsBundleBase.md#createEditPropertiesHandler()), [createLinkTextResolver](DocBookExtensionsBundleBase.md#createLinkTextResolver()), [createSchemaManagerFilter](DocBookExtensionsBundleBase.md#createSchemaManagerFilter()), [createXMLNodeCustomizer](DocBookExtensionsBundleBase.md#createXMLNodeCustomizer()), [getAuthorActionEventHandler](DocBookExtensionsBundleBase.md#getAuthorActionEventHandler()), [getAuthorImageDecorator](DocBookExtensionsBundleBase.md#getAuthorImageDecorator()), [getSpellCheckerHelper](DocBookExtensionsBundleBase.md#getSpellCheckerHelper()), [resolveCustomHref](DocBookExtensionsBundleBase.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))
### Methods inherited from class ro.sync.ecss.extensions.api.[ExtensionsBundle](../api/ExtensionsBundle.md)
 [createAttributesValueEditor](../api/ExtensionsBundle.md#createAttributesValueEditor(boolean)), [createAuthorAWTDndListener](../api/ExtensionsBundle.md#createAuthorAWTDndListener()), [createAuthorBreadCrumbCustomizer](../api/ExtensionsBundle.md#createAuthorBreadCrumbCustomizer()), [createAuthorOutlineCustomizer](../api/ExtensionsBundle.md#createAuthorOutlineCustomizer()), [createAuthorPreloadProcessor](../api/ExtensionsBundle.md#createAuthorPreloadProcessor()), [createAuthorReferenceResolver](../api/ExtensionsBundle.md#createAuthorReferenceResolver()), [createAuthorStylesFilter](../api/ExtensionsBundle.md#createAuthorStylesFilter()), [createAuthorSWTDndListener](../api/ExtensionsBundle.md#createAuthorSWTDndListener()), [createCustomAttributeValueEditor](../api/ExtensionsBundle.md#createCustomAttributeValueEditor(boolean)), [createElementLocatorProvider](../api/ExtensionsBundle.md#createElementLocatorProvider()), [createIDTypeRecognizer](../api/ExtensionsBundle.md#createIDTypeRecognizer()), [createTextPageExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createTextPageExternalObjectInsertionHandler()), [createTextSWTDndListener](../api/ExtensionsBundle.md#createTextSWTDndListener()), [customizeImageTooltipDescription](../api/ExtensionsBundle.md#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [customizeLinkTooltipDescription](../api/ExtensionsBundle.md#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [getDocumentTypeName](../api/ExtensionsBundle.md#getDocumentTypeName()), [getWebappExtensionsProvier](../api/ExtensionsBundle.md#getWebappExtensionsProvier()), [isContentReference](../api/ExtensionsBundle.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)), [resolveCustomAttributeValue](../api/ExtensionsBundle.md#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.lang.String)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [setDocumentTypeName](../api/ExtensionsBundle.md#setDocumentTypeName(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DocBook5ExtensionsBundle

public DocBook5ExtensionsBundle()

## Method Details

### createAuthorExtensionStateListener

public [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) createAuthorExtensionStateListener()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createAuthorExtensionStateListener())
Returns the [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) which will be notified when the Author extension where it is defined is activated and deactivated during the detection process. This method is called each time the Document Type association where the Author extension and the extensions bundle are defined matches a document opened in an Author page.
  Overrides: [createAuthorExtensionStateListener](../api/ExtensionsBundle.md#createAuthorExtensionStateListener()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) instance. See Also:
        * [ExtensionsBundle.createAuthorExtensionStateListener()](../api/ExtensionsBundle.md#createAuthorExtensionStateListener())

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

### getDocumentNamespace

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentNamespace()
  Specified by: [getDocumentNamespace](DocBookExtensionsBundleBase.md#getDocumentNamespace()) in class [DocBookExtensionsBundleBase](DocBookExtensionsBundleBase.md) Returns: The document namespace. See Also:
        * [DocBookExtensionsBundleBase.getDocumentNamespace()](DocBookExtensionsBundleBase.md#getDocumentNamespace())

### getAuthorSchemaAwareEditingHandler

public [AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md) getAuthorSchemaAwareEditingHandler()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler())
If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this support. The support can either resolve a specific case, let the default implementation take place or reject the edit entirely by throwing an [InvalidEditException](../api/InvalidEditException.md). It is recommended to extend class [AuthorSchemaAwareEditingHandlerAdapter](../api/AuthorSchemaAwareEditingHandlerAdapter.md) in order to be protected from any API additions that may occur in interface [AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md).
  Overrides: [getAuthorSchemaAwareEditingHandler](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A custom editing handler for schema aware actions, or null if there is no handler and the default processing should take place. See Also:
        * [ExtensionsBundle.getAuthorSchemaAwareEditingHandler()](../api/ExtensionsBundle.md#getAuthorSchemaAwareEditingHandler())

### createExternalObjectInsertionHandler

public [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) createExternalObjectInsertionHandler()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler())
Create a handler which gets notified when external resources need to be inserted in the Author page. The usual usage for this is to get notified when URLs are dropped from the project or DITA Maps manager in the Author page.
  Overrides: [createExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: The External URLs handler See Also:
        * [ExtensionsBundle.createExternalObjectInsertionHandler()](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler())

### getProfilingConditionalTextProvider

public [ProfilingConditionalTextProvider](../api/ProfilingConditionalTextProvider.md) getProfilingConditionalTextProvider()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getProfilingConditionalTextProvider())
Creates a new [ProfilingConditionalTextProvider](../api/ProfilingConditionalTextProvider.md) instance responsible for providing custom support regarding profiling and conditional text.
  Overrides: [getProfilingConditionalTextProvider](../api/ExtensionsBundle.md#getProfilingConditionalTextProvider()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: A new [ProfilingConditionalTextProvider](../api/ProfilingConditionalTextProvider.md) instance. See Also:
        * [ExtensionsBundle.getProfilingConditionalTextProvider()](../api/ExtensionsBundle.md#getProfilingConditionalTextProvider())

### getAuthorTableOperationsHandler

public [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) getAuthorTableOperationsHandler()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getAuthorTableOperationsHandler())
Get the [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) instance responsible for handling table operations.
  Overrides: [getAuthorTableOperationsHandler](../api/ExtensionsBundle.md#getAuthorTableOperationsHandler()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: Author table operations handler. See Also:
        * [ExtensionsBundle.getAuthorTableOperationsHandler()](../api/ExtensionsBundle.md#getAuthorTableOperationsHandler())

### getHelpPageID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditorPage)
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String))
Get the help page ID for this particular framework extensions bundle. If the returned help page ID is an URL, a web browser will be opened pointing to that URL when the user presses F1 in the dialog or when using the Help button. If the returned help page ID is an identifier, when help is invoked, the application will open the Oxygen User's Manual and locate this identifier inside it.
  Overrides: [getHelpPageID](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String)) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Parameters: currentEditorPage - The current editor page mode (Text/Grid/Author/Schema), one of the constants in the "ro.sync.exml.editor.EditorPageConstants" interface. Returns: The help page ID, by default no help page ID is returned. See Also:
        * [ExtensionsBundle.getHelpPageID(java.lang.String)](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
