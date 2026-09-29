Package [ro.sync.ecss.extensions.tei](package-summary.md)

# Class TEIP5ExtensionsBundle

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.ExtensionsBundle](../api/ExtensionsBundle.md)
        * [ro.sync.ecss.extensions.tei.TEIExtensionsBundleBase](TEIExtensionsBundleBase.md)
            * ro.sync.ecss.extensions.tei.TEIP5ExtensionsBundle
   All Implemented Interfaces: [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class TEIP5ExtensionsBundle extends [TEIExtensionsBundleBase](TEIExtensionsBundleBase.md)
The TEI P5 framework extensions bundle.

## Constructor Summary
 Constructors
Constructor

Description
 [TEIP5ExtensionsBundle](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) [createAuthorExtensionStateListener](#createAuthorExtensionStateListener())()
Returns the [AuthorExtensionStateListener](../api/AuthorExtensionStateListener.md) which will be notified when the Author extension where it is defined is activated and deactivated during the detection process.
  [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) [createExternalObjectInsertionHandler](#createExternalObjectInsertionHandler())()
Create a handler which gets notified when external resources need to be inserted in the Author page.
  [IDTypeRecognizer](../api/link/IDTypeRecognizer.md) [createIDTypeRecognizer](#createIDTypeRecognizer())()
Creates a new [IDTypeRecognizer](../api/link/IDTypeRecognizer.md) instance responsible for providing an implementation which can recognize ID declarations and references.
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
  [UniqueAttributesRecognizer](../api/UniqueAttributesRecognizer.md) [getUniqueAttributesIdentifier](#getUniqueAttributesIdentifier())()
Get an unique attributes creator and identifier.

### Methods inherited from class ro.sync.ecss.extensions.tei.[TEIExtensionsBundleBase](TEIExtensionsBundleBase.md)
 [createAuthorTableCellSpanProvider](TEIExtensionsBundleBase.md#createAuthorTableCellSpanProvider()), [createEditPropertiesHandler](TEIExtensionsBundleBase.md#createEditPropertiesHandler()), [createXMLNodeCustomizer](TEIExtensionsBundleBase.md#createXMLNodeCustomizer()), [getAuthorActionEventHandler](TEIExtensionsBundleBase.md#getAuthorActionEventHandler()), [getAuthorImageDecorator](TEIExtensionsBundleBase.md#getAuthorImageDecorator()), [getAuthorSchemaAwareEditingHandler](TEIExtensionsBundleBase.md#getAuthorSchemaAwareEditingHandler()), [getSpellCheckerHelper](TEIExtensionsBundleBase.md#getSpellCheckerHelper())
### Methods inherited from class ro.sync.ecss.extensions.api.[ExtensionsBundle](../api/ExtensionsBundle.md)
 [createAttributesValueEditor](../api/ExtensionsBundle.md#createAttributesValueEditor(boolean)), [createAuthorAWTDndListener](../api/ExtensionsBundle.md#createAuthorAWTDndListener()), [createAuthorBreadCrumbCustomizer](../api/ExtensionsBundle.md#createAuthorBreadCrumbCustomizer()), [createAuthorOutlineCustomizer](../api/ExtensionsBundle.md#createAuthorOutlineCustomizer()), [createAuthorPreloadProcessor](../api/ExtensionsBundle.md#createAuthorPreloadProcessor()), [createAuthorReferenceResolver](../api/ExtensionsBundle.md#createAuthorReferenceResolver()), [createAuthorStylesFilter](../api/ExtensionsBundle.md#createAuthorStylesFilter()), [createAuthorSWTDndListener](../api/ExtensionsBundle.md#createAuthorSWTDndListener()), [createAuthorTableCellSepProvider](../api/ExtensionsBundle.md#createAuthorTableCellSepProvider()), [createAuthorTableColumnWidthProvider](../api/ExtensionsBundle.md#createAuthorTableColumnWidthProvider()), [createCustomAttributeValueEditor](../api/ExtensionsBundle.md#createCustomAttributeValueEditor(boolean)), [createElementLocatorProvider](../api/ExtensionsBundle.md#createElementLocatorProvider()), [createLinkTextResolver](../api/ExtensionsBundle.md#createLinkTextResolver()), [createSchemaManagerFilter](../api/ExtensionsBundle.md#createSchemaManagerFilter()), [createTextPageExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createTextPageExternalObjectInsertionHandler()), [createTextSWTDndListener](../api/ExtensionsBundle.md#createTextSWTDndListener()), [customizeImageTooltipDescription](../api/ExtensionsBundle.md#customizeImageTooltipDescription(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [customizeLinkTooltipDescription](../api/ExtensionsBundle.md#customizeLinkTooltipDescription(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [getDocumentTypeName](../api/ExtensionsBundle.md#getDocumentTypeName()), [getProfilingConditionalTextProvider](../api/ExtensionsBundle.md#getProfilingConditionalTextProvider()), [getWebappExtensionsProvier](../api/ExtensionsBundle.md#getWebappExtensionsProvier()), [isContentReference](../api/ExtensionsBundle.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)), [resolveCustomAttributeValue](../api/ExtensionsBundle.md#resolveCustomAttributeValue(ro.sync.ecss.extensions.api.CustomAttributeValueContext)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.lang.String)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [resolveCustomHref](../api/ExtensionsBundle.md#resolveCustomHref(java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess)), [setDocumentTypeName](../api/ExtensionsBundle.md#setDocumentTypeName(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TEIP5ExtensionsBundle

public TEIP5ExtensionsBundle()

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
  Specified by: [getDocumentNamespace](TEIExtensionsBundleBase.md#getDocumentNamespace()) in class [TEIExtensionsBundleBase](TEIExtensionsBundleBase.md) Returns: The document namespace. See Also:
        * [TEIExtensionsBundleBase.getDocumentNamespace()](TEIExtensionsBundleBase.md#getDocumentNamespace())

### createExternalObjectInsertionHandler

public [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) createExternalObjectInsertionHandler()
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler())
Create a handler which gets notified when external resources need to be inserted in the Author page. The usual usage for this is to get notified when URLs are dropped from the project or DITA Maps manager in the Author page.
  Overrides: [createExternalObjectInsertionHandler](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler()) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Returns: The External URLs handler See Also:
        * [ExtensionsBundle.createExternalObjectInsertionHandler()](../api/ExtensionsBundle.md#createExternalObjectInsertionHandler())

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

### getHelpPageID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditorPage)
 Description copied from class: [ExtensionsBundle](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String))
Get the help page ID for this particular framework extensions bundle. If the returned help page ID is an URL, a web browser will be opened pointing to that URL when the user presses F1 in the dialog or when using the Help button. If the returned help page ID is an identifier, when help is invoked, the application will open the Oxygen User's Manual and locate this identifier inside it.
  Overrides: [getHelpPageID](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String)) in class [ExtensionsBundle](../api/ExtensionsBundle.md) Parameters: currentEditorPage - The current editor page mode (Text/Grid/Author/Schema), one of the constants in the "ro.sync.exml.editor.EditorPageConstants" interface. Returns: The help page ID, by default no help page ID is returned. See Also:
        * [ExtensionsBundle.getHelpPageID(java.lang.String)](../api/ExtensionsBundle.md#getHelpPageID(java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
