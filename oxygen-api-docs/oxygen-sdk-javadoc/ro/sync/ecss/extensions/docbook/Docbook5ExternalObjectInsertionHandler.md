Package [ro.sync.ecss.extensions.docbook](package-summary.md)

# Class Docbook5ExternalObjectInsertionHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md)
        * ro.sync.ecss.extensions.docbook.Docbook5ExternalObjectInsertionHandler
   All Implemented Interfaces: [Extension](../api/Extension.md), [ExternalObjectInsertionSources](../api/ExternalObjectInsertionSources.md)   @API(type=INTERNAL, src=PUBLIC) public class Docbook5ExternalObjectInsertionHandler extends [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md)
Dropped URLs handler

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[ExternalObjectInsertionSources](../api/ExternalObjectInsertionSources.md)
 [DND_DB_TREE](../api/ExternalObjectInsertionSources.md#DND_DB_TREE), [DND_DITA_COMPONENTS_TAB](../api/ExternalObjectInsertionSources.md#DND_DITA_COMPONENTS_TAB), [DND_DITA_KEYS_VIEW](../api/ExternalObjectInsertionSources.md#DND_DITA_KEYS_VIEW), [DND_DITA_MAPS_MANAGER](../api/ExternalObjectInsertionSources.md#DND_DITA_MAPS_MANAGER), [DND_DITA_MEDIA_TAB](../api/ExternalObjectInsertionSources.md#DND_DITA_MEDIA_TAB), [DND_EXTERNAL](../api/ExternalObjectInsertionSources.md#DND_EXTERNAL), [DND_IMAGE_PREVIEW](../api/ExternalObjectInsertionSources.md#DND_IMAGE_PREVIEW), [DND_PROJECT_TREE](../api/ExternalObjectInsertionSources.md#DND_PROJECT_TREE), [PASTE](../api/ExternalObjectInsertionSources.md#PASTE)
## Constructor Summary
 Constructors
Constructor

Description
 [Docbook5ExternalObjectInsertionHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getImporterStylesheetFileName](#getImporterStylesheetFileName(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../api/AuthorAccess.md) authorAccess)
Get the file name of the main Author paste stylesheet.
  void [insertURLs](#insertURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,int))([AuthorAccess](../api/AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, int source)
A list of URLs need to be inserted at the caret position, probably as links.
  void [insertURLs](#insertURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,java.util.List,int))([AuthorAccess](../api/AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ReferenceType](../api/ReferenceType.md)> types, int source)
A list of URLs need to be inserted at the caret position, probably as links.

### Methods inherited from class ro.sync.ecss.extensions.api.[AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md)
 [acceptSource](../api/AuthorExternalObjectInsertionHandler.md#acceptSource(ro.sync.ecss.extensions.api.AuthorAccess,int)), [acceptURLs](../api/AuthorExternalObjectInsertionHandler.md#acceptURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,int)), [checkImportedXHTMLContentIsPreservedEntirely](../api/AuthorExternalObjectInsertionHandler.md#checkImportedXHTMLContentIsPreservedEntirely()), [containOnlyBinaryResources](../api/AuthorExternalObjectInsertionHandler.md#containOnlyBinaryResources(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List)), [containOnlyImages](../api/AuthorExternalObjectInsertionHandler.md#containOnlyImages(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List)), [createImporterStylesheetSource](../api/AuthorExternalObjectInsertionHandler.md#createImporterStylesheetSource(ro.sync.ecss.extensions.api.AuthorAccess)), [getBaseURLAtCaretPosition](../api/AuthorExternalObjectInsertionHandler.md#getBaseURLAtCaretPosition(ro.sync.ecss.extensions.api.AuthorAccess)), [getClassStylesheetResource](../api/AuthorExternalObjectInsertionHandler.md#getClassStylesheetResource(java.lang.Class,java.lang.String)), [getContextPathNamesAndUris](../api/AuthorExternalObjectInsertionHandler.md#getContextPathNamesAndUris(ro.sync.ecss.extensions.api.AuthorAccess)), [getDescription](../api/AuthorExternalObjectInsertionHandler.md#getDescription()), [getFilterContentOfOutputStylesheet](../api/AuthorExternalObjectInsertionHandler.md#getFilterContentOfOutputStylesheet()), [getOnlyTextContentStylesheet](../api/AuthorExternalObjectInsertionHandler.md#getOnlyTextContentStylesheet(ro.sync.ecss.extensions.api.AuthorAccess)), [insertImportedContent](../api/AuthorExternalObjectInsertionHandler.md#insertImportedContent(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String)), [insertXHTMLFragment](../api/AuthorExternalObjectInsertionHandler.md#insertXHTMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,java.io.Reader)), [setParametersToTransform](../api/AuthorExternalObjectInsertionHandler.md#setParametersToTransform(javax.xml.transform.Transformer,ro.sync.ecss.extensions.api.AuthorAccess,boolean)), [simpleTransform](../api/AuthorExternalObjectInsertionHandler.md#simpleTransform(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String)), [simpleTransform](../api/AuthorExternalObjectInsertionHandler.md#simpleTransform(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,javax.xml.transform.stream.StreamSource))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### Docbook5ExternalObjectInsertionHandler

public Docbook5ExternalObjectInsertionHandler()

## Method Details

### insertURLs

public void insertURLs([AuthorAccess](../api/AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ReferenceType](../api/ReferenceType.md)> types, int source)throws [AuthorOperationException](../api/AuthorOperationException.md)
 Description copied from class: [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md#insertURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,java.util.List,int))
A list of URLs need to be inserted at the caret position, probably as links. The source of the insertion can be a paste event or a drag and drop event. This call back is received if [AuthorExternalObjectInsertionHandler.acceptURLs(AuthorAccess, List, int)](../api/AuthorExternalObjectInsertionHandler.md#acceptURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,int))returned true for the same source and urls list. You can use it to link to those specific files/URLs.
  Overrides: [insertURLs](../api/AuthorExternalObjectInsertionHandler.md#insertURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,java.util.List,int)) in class [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) Parameters: authorAccess - The author access urls - The list of URLs. types - The type of the URL reference - if null, the type will be inferred. source - The source of the URLs, one of the [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) constants. Throws: [AuthorOperationException](../api/AuthorOperationException.md) See Also:
        * [AuthorExternalObjectInsertionHandler.insertURLs(ro.sync.ecss.extensions.api.AuthorAccess, java.util.List, java.util.List, int)](../api/AuthorExternalObjectInsertionHandler.md#insertURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,java.util.List,int))

### insertURLs

public void insertURLs([AuthorAccess](../api/AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, int source)throws [AuthorOperationException](../api/AuthorOperationException.md)
 Description copied from class: [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md#insertURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,int))
A list of URLs need to be inserted at the caret position, probably as links. The source of the insertion can be a paste event or a drag and drop event. This call back is received if [AuthorExternalObjectInsertionHandler.acceptURLs(AuthorAccess, List, int)](../api/AuthorExternalObjectInsertionHandler.md#acceptURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,int))returned true for the same source and urls list. You can use it to link to those specific files/URLs.
  Overrides: [insertURLs](../api/AuthorExternalObjectInsertionHandler.md#insertURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,int)) in class [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) Parameters: authorAccess - The author access urls - The list of URLs. source - The source of the URLs, one of the [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) constants. Throws: [AuthorOperationException](../api/AuthorOperationException.md) See Also:
        * [AuthorExternalObjectInsertionHandler.insertURLs(ro.sync.ecss.extensions.api.AuthorAccess, java.util.List, int)](../api/AuthorExternalObjectInsertionHandler.md#insertURLs(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,int))

### getImporterStylesheetFileName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getImporterStylesheetFileName([AuthorAccess](../api/AuthorAccess.md) authorAccess)
 Description copied from class: [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md#getImporterStylesheetFileName(ro.sync.ecss.extensions.api.AuthorAccess))
Get the file name of the main Author paste stylesheet. It will be resolved in the context of the current class loader.
  Overrides: [getImporterStylesheetFileName](../api/AuthorExternalObjectInsertionHandler.md#getImporterStylesheetFileName(ro.sync.ecss.extensions.api.AuthorAccess)) in class [AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) Parameters: authorAccess - The author access API. Returns: the file name of the main Author paste stylesheet. It will be resolved in the context of the current class loader. See Also:
        * [AuthorExternalObjectInsertionHandler.getImporterStylesheetFileName(ro.sync.ecss.extensions.api.AuthorAccess)](../api/AuthorExternalObjectInsertionHandler.md#getImporterStylesheetFileName(ro.sync.ecss.extensions.api.AuthorAccess))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
