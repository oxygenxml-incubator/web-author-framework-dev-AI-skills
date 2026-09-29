Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorExternalObjectInsertionHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorExternalObjectInsertionHandler
   All Implemented Interfaces: [Extension](Extension.md), [ExternalObjectInsertionSources](ExternalObjectInsertionSources.md)   Direct Known Subclasses: [DITAExternalObjectInsertionHandler](../dita/DITAExternalObjectInsertionHandler.md), [Docbook4ExternalObjectInsertionHandler](../docbook/Docbook4ExternalObjectInsertionHandler.md), [Docbook5ExternalObjectInsertionHandler](../docbook/Docbook5ExternalObjectInsertionHandler.md), [TEI_jteiExternalObjectInsertionHandler](../tei/TEI_jteiExternalObjectInsertionHandler.md), [TEIP5ExternalObjectInsertionHandler](../tei/TEIP5ExternalObjectInsertionHandler.md), [XHTMLExternalObjectInsertionHandler](../xhtml/XHTMLExternalObjectInsertionHandler.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorExternalObjectInsertionHandler extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ExternalObjectInsertionSources](ExternalObjectInsertionSources.md), [Extension](Extension.md)
This class is notified when URLs are dropped or pasted to an Author Editor page or when XHTML fragments are pasted or dropped from external applications (like web browsers or office applications) to the Author page.If you want to use a stylesheet to convert the pasted XHTML to your own XML vocabulary you can just overwrite the method: "ro.sync.ecss.extensions.api.AuthorExternalObjectInsertionHandler.getImporterStylesheetFileName(AuthorAccess)" and return the file name of the stylesheet which will be applied. The path to the importer stylesheet must be added in the Classpath tab in the Document Type Association edit dialog (as an example you can see the DITA and Docbook document types).
  Since: 12
## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[ExternalObjectInsertionSources](ExternalObjectInsertionSources.md)
 [DND_DB_TREE](ExternalObjectInsertionSources.md#DND_DB_TREE), [DND_DITA_COMPONENTS_TAB](ExternalObjectInsertionSources.md#DND_DITA_COMPONENTS_TAB), [DND_DITA_KEYS_VIEW](ExternalObjectInsertionSources.md#DND_DITA_KEYS_VIEW), [DND_DITA_MAPS_MANAGER](ExternalObjectInsertionSources.md#DND_DITA_MAPS_MANAGER), [DND_DITA_MEDIA_TAB](ExternalObjectInsertionSources.md#DND_DITA_MEDIA_TAB), [DND_EXTERNAL](ExternalObjectInsertionSources.md#DND_EXTERNAL), [DND_IMAGE_PREVIEW](ExternalObjectInsertionSources.md#DND_IMAGE_PREVIEW), [DND_PROJECT_TREE](ExternalObjectInsertionSources.md#DND_PROJECT_TREE), [PASTE](ExternalObjectInsertionSources.md#PASTE)
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorExternalObjectInsertionHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [acceptSource](#acceptSource(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](AuthorAccess.md) authorAccess, int source)
Confirm that the source of URLs is interesting to this handler.
  boolean [acceptURLs](#acceptURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,int))([AuthorAccess](AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, int source)
Confirm that the list of URLs is interesting to this handler.
  protected boolean [checkImportedXHTMLContentIsPreservedEntirely](#checkImportedXHTMLContentIsPreservedEntirely())()
Overwrite this method if you want to check the text data is preserved on paste after applying the conversion XSL stylesheet.
  protected static boolean [containOnlyBinaryResources](#containOnlyBinaryResources(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List))([AuthorAccess](AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urlList)
Verify if the provided URLs are only binary rsources.
  protected static boolean [containOnlyImages](#containOnlyImages(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List))([AuthorAccess](AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urlList)
Verify if the provided URLs are only images.
  protected [StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) [createImporterStylesheetSource](#createImporterStylesheetSource(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Create the [StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) for the main XSLT stylesheet which will do the importing (transforming from the XHTML content to content valid in the current framework).
  protected static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getBaseURLAtCaretPosition](#getBaseURLAtCaretPosition(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Get the base URL for the node located at caret position.
  protected [StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) [getClassStylesheetResource](#getClassStylesheetResource(java.lang.Class,java.lang.String))([Class](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Class.html) clazz, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourcePath)
Find the stylesheet resource in the class package with the given file name.
  protected static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getContextPathNamesAndUris](#getContextPathNamesAndUris(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Get the list of parent elements of insertion point in Author document.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected [StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) [getFilterContentOfOutputStylesheet](#getFilterContentOfOutputStylesheet())()
Gets an XSLT stylesheet that can filter non text content from the output XML.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getImporterStylesheetFileName](#getImporterStylesheetFileName(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Get the file name of the main Author paste stylesheet.
  protected [StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) [getOnlyTextContentStylesheet](#getOnlyTextContentStylesheet(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Gets an XSLT stylesheet that can extract the entire text content (and only the text content) from any input XML.
  protected void [insertImportedContent](#insertImportedContent(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) importedContent)
Insert the content imported by applying the XSLT stylesheet directly in the document.
  void [insertURLs](#insertURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,int))([AuthorAccess](AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, int source)
A list of URLs need to be inserted at the caret position, probably as links.
  void [insertURLs](#insertURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,java.util.List,int))([AuthorAccess](AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ReferenceType](ReferenceType.md)> types, int source)
A list of URLs need to be inserted at the caret position, probably as links.
  void [insertXHTMLFragment](#insertXHTMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,java.io.Reader))([AuthorAccess](AuthorAccess.md) authorAccess, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) xhtmlContentReader)
Insert an XHTML fragment
  protected static void [setParametersToTransform](#setParametersToTransform(javax.xml.transform.Transformer,ro.sync.ecss.extensions.api.AuthorAccess,boolean))([Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) transformer, [AuthorAccess](AuthorAccess.md) authorAccess, boolean copyWordImageResources)
Set the parameters on the XSLT transform engine.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [simpleTransform](#simpleTransform(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String))([AuthorAccess](AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xml, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xsl)
Transform the specified XML input with the specified XSLT stylesheet using Saxon HE processor.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [simpleTransform](#simpleTransform(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,javax.xml.transform.stream.StreamSource))([AuthorAccess](AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xml, [StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) xsl)
Transform the specified XML input with the specified XSLT stylesheet using Saxon HE processor.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorExternalObjectInsertionHandler

public AuthorExternalObjectInsertionHandler()

## Method Details

### insertURLs

public void insertURLs([AuthorAccess](AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, int source)throws [AuthorOperationException](AuthorOperationException.md)

A list of URLs need to be inserted at the caret position, probably as links. The source of the insertion can be a paste event or a drag and drop event. This call back is received if [acceptURLs(AuthorAccess, List, int)](#acceptURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,int))returned true for the same source and urls list. You can use it to link to those specific files/URLs.
  Parameters: authorAccess - The author access urls - The list of URLs. source - The source of the URLs, one of the [AuthorExternalObjectInsertionHandler](AuthorExternalObjectInsertionHandler.md) constants. Throws: [AuthorOperationException](AuthorOperationException.md)
### insertURLs

public void insertURLs([AuthorAccess](AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ReferenceType](ReferenceType.md)> types, int source)throws [AuthorOperationException](AuthorOperationException.md)

A list of URLs need to be inserted at the caret position, probably as links. The source of the insertion can be a paste event or a drag and drop event. This call back is received if [acceptURLs(AuthorAccess, List, int)](#acceptURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,int))returned true for the same source and urls list. You can use it to link to those specific files/URLs.
  Parameters: authorAccess - The author access urls - The list of URLs. types - The type of the URL reference - if null, the type will be inferred. source - The source of the URLs, one of the [AuthorExternalObjectInsertionHandler](AuthorExternalObjectInsertionHandler.md) constants. Throws: [AuthorOperationException](AuthorOperationException.md) Since: 18.0
### acceptURLs

public boolean acceptURLs([AuthorAccess](AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, int source)

Confirm that the list of URLs is interesting to this handler. The source of the insertion can be a paste event or a drag and drop event. If the source is of drag and drop type and it is accepted, the caret will be moved to the drop position. By default accepts the URLs from external sources if the URLs are only images or binary files and all URLs from paste events and drops from the Oxygen Project and DITA Maps Manager. It calls the "acceptSource" method to check if a certain source of the operation is accepted.
  Parameters: authorAccess - The author access. urls - The list of URLs. source - The source of the URLs, one of the [AuthorExternalObjectInsertionHandler](AuthorExternalObjectInsertionHandler.md) constants. Returns: true if the provided URLs are interesting.
### acceptSource

public boolean acceptSource([AuthorAccess](AuthorAccess.md) authorAccess, int source)

Confirm that the source of URLs is interesting to this handler. The source of the insertion can be a paste event or a drag and drop event. If the source is of drag and drop type and it is accepted, the caret will be moved to the drag position. By default accepts paste sources and drags from the Oxygen Project and DITA Maps Manager.
  Parameters: authorAccess - The author access. source - The source of the URLs, one of the [AuthorExternalObjectInsertionHandler](AuthorExternalObjectInsertionHandler.md) constants (that represents a paste or a drag and drop event) Returns: true if the insert URLs are interesting.
### containOnlyImages

protected static boolean containOnlyImages([AuthorAccess](AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urlList)

Verify if the provided URLs are only images.
  Parameters: urlList - The list of URLs Returns: true if the URLs are only images.
### containOnlyBinaryResources

protected static boolean containOnlyBinaryResources([AuthorAccess](AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urlList)

Verify if the provided URLs are only binary rsources.
  Parameters: urlList - The list of URLs Returns: true if the URLs are only binary resources.
### insertXHTMLFragment

public void insertXHTMLFragment([AuthorAccess](AuthorAccess.md) authorAccess, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) xhtmlContentReader)throws [AuthorOperationException](AuthorOperationException.md)

Insert an XHTML fragment
  Parameters: authorAccess - The author access xhtmlContentReader - The XTHML content reader Throws: [AuthorOperationException](AuthorOperationException.md) Since: 12.1
### insertImportedContent

protected void insertImportedContent([AuthorAccess](AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) importedContent)throws [AuthorOperationException](AuthorOperationException.md)

Insert the content imported by applying the XSLT stylesheet directly in the document. The insertion is done schema aware.
  Parameters: authorAccess - The author access. importedContent - The imported content. Throws: [AuthorOperationException](AuthorOperationException.md)
### getOnlyTextContentStylesheet

protected [StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) getOnlyTextContentStylesheet([AuthorAccess](AuthorAccess.md) authorAccess)

Gets an XSLT stylesheet that can extract the entire text content (and only the text content) from any input XML.
  Parameters: authorAccess - The author access Returns: The XSLT stylesheet that keeps only the text content of input.
### getClassStylesheetResource

protected [StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) getClassStylesheetResource([Class](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Class.html) clazz, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourcePath)

Find the stylesheet resource in the class package with the given file name.
  Parameters: clazz - The class where to search for the stylesheet resource resourcePath - The resource to find. Returns: The stylesheet resource or a default stylesheet (that ignores everything) if it cannot be found.
### getFilterContentOfOutputStylesheet

protected [StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) getFilterContentOfOutputStylesheet()

Gets an XSLT stylesheet that can filter non text content from the output XML.
  Returns: The XSLT stylesheet that can filter non text content from the output XML.
### simpleTransform

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) simpleTransform([AuthorAccess](AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xml, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xsl)throws [TransformerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerException.html), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Transform the specified XML input with the specified XSLT stylesheet using Saxon HE processor.
  Parameters: authorAccess - helper object for creating the transformer xml - the input XML of the transformation xsl - the input XSLT of the transformation Returns: the result of the transformation Throws: [TransformerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerException.html) - thrown during transformation [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - thrown during writing the transform result to the output string
### simpleTransform

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) simpleTransform([AuthorAccess](AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xml, [StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) xsl)throws [TransformerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerException.html), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Transform the specified XML input with the specified XSLT stylesheet using Saxon HE processor.
  Parameters: authorAccess - helper object for creating the transformer xml - the input XML of the transformation xsl - the input XSLT of the transformation Returns: the result of the transformation Throws: [TransformerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerException.html) - thrown during transformation [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - thrown during writing the transform result to the output string
### setParametersToTransform

protected static void setParametersToTransform([Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) transformer, [AuthorAccess](AuthorAccess.md) authorAccess, boolean copyWordImageResources)

Set the parameters on the XSLT transform engine.
  Parameters: transformer - The XSLT transformer. authorAccess - The author access. copyWordImageResources - true to copy image resources from word document
### getContextPathNamesAndUris

protected static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getContextPathNamesAndUris([AuthorAccess](AuthorAccess.md) authorAccess)

Get the list of parent elements of insertion point in Author document.
  Parameters: authorAccess - The author access Returns: comma-separated list of parent elements of insertion point.
### createImporterStylesheetSource

protected [StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) createImporterStylesheetSource([AuthorAccess](AuthorAccess.md) authorAccess)

Create the [StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) for the main XSLT stylesheet which will do the importing (transforming from the XHTML content to content valid in the current framework). The main stylesheet will be applied in a pipeline after the preprocessing stylesheets and generates the markup of the current framework (DITA, DocBook, etc).
  Parameters: authorAccess - The Author access API. Returns: the stylesheet which will import from XHTML to this framework. If the main stylesheet of the current framework cannot be loaded from resources a default one will be returned which keeps only the text from the input. Since: 12.1
### getImporterStylesheetFileName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getImporterStylesheetFileName([AuthorAccess](AuthorAccess.md) authorAccess)

Get the file name of the main Author paste stylesheet. It will be resolved in the context of the current class loader.
  Parameters: authorAccess - The author access API. Returns: the file name of the main Author paste stylesheet. It will be resolved in the context of the current class loader. Since: 12.1
### getBaseURLAtCaretPosition

protected static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getBaseURLAtCaretPosition([AuthorAccess](AuthorAccess.md) authorAccess)

Get the base URL for the node located at caret position. Usually this is the URL of the opened editor but it can vary if nodes have xml:base defined on them.
  Parameters: authorAccess - The author access Returns: the base URL for the node located at caret position.
### checkImportedXHTMLContentIsPreservedEntirely

protected boolean checkImportedXHTMLContentIsPreservedEntirely()

Overwrite this method if you want to check the text data is preserved on paste after applying the conversion XSL stylesheet. If the data is not preserved the content will be copied without any styling and a warning will appear in the console.
  Returns: false by default.
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](Extension.md#getDescription()) in interface [Extension](Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
