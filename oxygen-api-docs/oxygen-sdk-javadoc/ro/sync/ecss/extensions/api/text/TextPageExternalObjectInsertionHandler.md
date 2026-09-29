Package [ro.sync.ecss.extensions.api.text](package-summary.md)

# Class TextPageExternalObjectInsertionHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.text.TextPageExternalObjectInsertionHandler
   All Implemented Interfaces: [Extension](../Extension.md), [ExternalObjectInsertionSources](../ExternalObjectInsertionSources.md)   Direct Known Subclasses: [DITATextPageExternalObjectInsertionHandler](../../dita/DITATextPageExternalObjectInsertionHandler.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class TextPageExternalObjectInsertionHandler extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ExternalObjectInsertionSources](../ExternalObjectInsertionSources.md), [Extension](../Extension.md)
This class is notified when URLs are dropped or pasted from a file explorer or from an Oxygen internal view to a Text Editor page. For the Eclipse Plugin the dropped files are handled by the platform and this API may not be called.
  Since: 19
## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[ExternalObjectInsertionSources](../ExternalObjectInsertionSources.md)
 [DND_DB_TREE](../ExternalObjectInsertionSources.md#DND_DB_TREE), [DND_DITA_COMPONENTS_TAB](../ExternalObjectInsertionSources.md#DND_DITA_COMPONENTS_TAB), [DND_DITA_KEYS_VIEW](../ExternalObjectInsertionSources.md#DND_DITA_KEYS_VIEW), [DND_DITA_MAPS_MANAGER](../ExternalObjectInsertionSources.md#DND_DITA_MAPS_MANAGER), [DND_DITA_MEDIA_TAB](../ExternalObjectInsertionSources.md#DND_DITA_MEDIA_TAB), [DND_EXTERNAL](../ExternalObjectInsertionSources.md#DND_EXTERNAL), [DND_IMAGE_PREVIEW](../ExternalObjectInsertionSources.md#DND_IMAGE_PREVIEW), [DND_PROJECT_TREE](../ExternalObjectInsertionSources.md#DND_PROJECT_TREE), [PASTE](../ExternalObjectInsertionSources.md#PASTE)
## Constructor Summary
 Constructors
Constructor

Description
 [TextPageExternalObjectInsertionHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [acceptsSource](#acceptsSource(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,int))([WSXMLTextEditorPage](../../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, int source)
Confirm that the source of URLs is interesting to this handler.
  boolean [acceptsURLs](#acceptsURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List,int))([WSXMLTextEditorPage](../../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, int source)
Confirm that the list of URLs is interesting to this handler.
  protected static boolean [containsOnlyBinaryResources](#containsOnlyBinaryResources(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List))([WSXMLTextEditorPage](../../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textPage, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urlList)
Verify if the provided URLs locate only binary resources.
  protected static boolean [containsOnlyImages](#containsOnlyImages(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List))([WSXMLTextEditorPage](../../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textPage, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urlList)
Verify if the provided URLs locate only images.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 void [insertURLs](#insertURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List,int))([WSXMLTextEditorPage](../../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, int source)
A list of URLs needs to be inserted at the caret position, probably as links.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TextPageExternalObjectInsertionHandler

public TextPageExternalObjectInsertionHandler()

## Method Details

### insertURLs

public void insertURLs([WSXMLTextEditorPage](../../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, int source)throws [TextPageOperationException](TextPageOperationException.md)

A list of URLs needs to be inserted at the caret position, probably as links. The source of the insertion can be a paste event or a drag and drop event. This call back is received if [acceptsURLs(WSXMLTextEditorPage, List, int)](#acceptsURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List,int))returned true for the same source and urls list. You can use it to link to those specific files/URLs.
  Parameters: textAccess - The text page access urls - The list of URLs. source - The source of the URLs, one of the [ExternalObjectInsertionSources](../ExternalObjectInsertionSources.md) constants. Throws: [TextPageOperationException](TextPageOperationException.md)
### acceptsURLs

public boolean acceptsURLs([WSXMLTextEditorPage](../../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, int source)

Confirm that the list of URLs is interesting to this handler. The source of the insertion can be a paste event or a drag and drop event. If the source is of drag and drop type and it is accepted, the caret will be moved to the drop position. By default all pasted URLs are accepted. Also all dropped images are accepted. For all other cases we accept by default URLs dropped from inside Oxygen (from views like Project and DITA Maps Manager).
  Parameters: textAccess - The text page access. urls - The list of URLs. source - The source of the URLs, one of the [ExternalObjectInsertionSources](../ExternalObjectInsertionSources.md) constants. Returns: true if the provided URLs are interesting. If false, the default behaviors for the text page will be done (usually this means inserting the URL at the caret position).
### acceptsSource

public boolean acceptsSource([WSXMLTextEditorPage](../../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, int source)

Confirm that the source of URLs is interesting to this handler. The source of the insertion can be a paste event or a drag and drop event. If the source is of drag and drop type and it is accepted, the caret will be moved to the drag position. By default accepts paste sources and drags from the Oxygen Project and DITA Maps Manager.
  Parameters: textAccess - The text page access. source - The source of the URLs, one of the [ExternalObjectInsertionSources](../ExternalObjectInsertionSources.md) constants (that represents a paste or a drag and drop event) Returns: true if the insert URLs are interesting.
### containsOnlyImages

protected static boolean containsOnlyImages([WSXMLTextEditorPage](../../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textPage, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urlList)

Verify if the provided URLs locate only images.
  Parameters: textPage - The text page access. urlList - The list of URLs. Returns: true if the URLs locate only images.
### containsOnlyBinaryResources

protected static boolean containsOnlyBinaryResources([WSXMLTextEditorPage](../../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textPage, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urlList)

Verify if the provided URLs locate only binary resources.
  Parameters: textPage - The text page access. urlList - The list of URLs. Returns: true if the URLs locate only binary resources.
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../Extension.md#getDescription()) in interface [Extension](../Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
