Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DITATextPageExternalObjectInsertionHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.text.TextPageExternalObjectInsertionHandler](../api/text/TextPageExternalObjectInsertionHandler.md)
        * ro.sync.ecss.extensions.dita.DITATextPageExternalObjectInsertionHandler
   All Implemented Interfaces: [Extension](../api/Extension.md), [ExternalObjectInsertionSources](../api/ExternalObjectInsertionSources.md)   Direct Known Subclasses: [DITAMapTextPageExternalObjectInsertionHandler](map/DITAMapTextPageExternalObjectInsertionHandler.md)   @API(type=INTERNAL, src=PUBLIC) public class DITATextPageExternalObjectInsertionHandler extends [TextPageExternalObjectInsertionHandler](../api/text/TextPageExternalObjectInsertionHandler.md)
The DITA text page external object insertion handler.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[ExternalObjectInsertionSources](../api/ExternalObjectInsertionSources.md)
 [DND_DB_TREE](../api/ExternalObjectInsertionSources.md#DND_DB_TREE), [DND_DITA_COMPONENTS_TAB](../api/ExternalObjectInsertionSources.md#DND_DITA_COMPONENTS_TAB), [DND_DITA_KEYS_VIEW](../api/ExternalObjectInsertionSources.md#DND_DITA_KEYS_VIEW), [DND_DITA_MAPS_MANAGER](../api/ExternalObjectInsertionSources.md#DND_DITA_MAPS_MANAGER), [DND_DITA_MEDIA_TAB](../api/ExternalObjectInsertionSources.md#DND_DITA_MEDIA_TAB), [DND_EXTERNAL](../api/ExternalObjectInsertionSources.md#DND_EXTERNAL), [DND_IMAGE_PREVIEW](../api/ExternalObjectInsertionSources.md#DND_IMAGE_PREVIEW), [DND_PROJECT_TREE](../api/ExternalObjectInsertionSources.md#DND_PROJECT_TREE), [PASTE](../api/ExternalObjectInsertionSources.md#PASTE)
## Constructor Summary
 Constructors
Constructor

Description
 [DITATextPageExternalObjectInsertionHandler](#%3Cinit%3E())()
Default constructor
  [DITATextPageExternalObjectInsertionHandler](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider))([ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) keyManagerProvider)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [acceptsURLs](#acceptsURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List,int))([WSXMLTextEditorPage](../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, int source)
Confirm that the list of URLs is interesting to this handler.
  void [insertURLs](#insertURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List,int))([WSXMLTextEditorPage](../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urlList, int source)
A list of URLs needs to be inserted at the caret position, probably as links.

### Methods inherited from class ro.sync.ecss.extensions.api.text.[TextPageExternalObjectInsertionHandler](../api/text/TextPageExternalObjectInsertionHandler.md)
 [acceptsSource](../api/text/TextPageExternalObjectInsertionHandler.md#acceptsSource(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,int)), [containsOnlyBinaryResources](../api/text/TextPageExternalObjectInsertionHandler.md#containsOnlyBinaryResources(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List)), [containsOnlyImages](../api/text/TextPageExternalObjectInsertionHandler.md#containsOnlyImages(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List)), [getDescription](../api/text/TextPageExternalObjectInsertionHandler.md#getDescription())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITATextPageExternalObjectInsertionHandler

public DITATextPageExternalObjectInsertionHandler()

Default constructor

### DITATextPageExternalObjectInsertionHandler

public DITATextPageExternalObjectInsertionHandler([ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) keyManagerProvider)

Constructor.
  Parameters: keyManagerProvider - The key manager provider
## Method Details

### acceptsURLs

public boolean acceptsURLs([WSXMLTextEditorPage](../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urls, int source)
 Description copied from class: [TextPageExternalObjectInsertionHandler](../api/text/TextPageExternalObjectInsertionHandler.md#acceptsURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List,int))
Confirm that the list of URLs is interesting to this handler. The source of the insertion can be a paste event or a drag and drop event. If the source is of drag and drop type and it is accepted, the caret will be moved to the drop position. By default all pasted URLs are accepted. Also all dropped images are accepted. For all other cases we accept by default URLs dropped from inside Oxygen (from views like Project and DITA Maps Manager).
  Overrides: [acceptsURLs](../api/text/TextPageExternalObjectInsertionHandler.md#acceptsURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List,int)) in class [TextPageExternalObjectInsertionHandler](../api/text/TextPageExternalObjectInsertionHandler.md) Parameters: textAccess - The text page access. urls - The list of URLs. source - The source of the URLs, one of the [ExternalObjectInsertionSources](../api/ExternalObjectInsertionSources.md) constants. Returns: true if the provided URLs are interesting. If false, the default behaviors for the text page will be done (usually this means inserting the URL at the caret position). See Also:
        * [TextPageExternalObjectInsertionHandler.acceptsURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage, java.util.List, int)](../api/text/TextPageExternalObjectInsertionHandler.md#acceptsURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List,int))

### insertURLs

public void insertURLs([WSXMLTextEditorPage](../../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> urlList, int source)throws [TextPageOperationException](../api/text/TextPageOperationException.md)
 Description copied from class: [TextPageExternalObjectInsertionHandler](../api/text/TextPageExternalObjectInsertionHandler.md#insertURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List,int))
A list of URLs needs to be inserted at the caret position, probably as links. The source of the insertion can be a paste event or a drag and drop event. This call back is received if [TextPageExternalObjectInsertionHandler.acceptsURLs(WSXMLTextEditorPage, List, int)](../api/text/TextPageExternalObjectInsertionHandler.md#acceptsURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List,int))returned true for the same source and urls list. You can use it to link to those specific files/URLs.
  Overrides: [insertURLs](../api/text/TextPageExternalObjectInsertionHandler.md#insertURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List,int)) in class [TextPageExternalObjectInsertionHandler](../api/text/TextPageExternalObjectInsertionHandler.md) Parameters: textAccess - The text page access urlList - The list of URLs. source - The source of the URLs, one of the [ExternalObjectInsertionSources](../api/ExternalObjectInsertionSources.md) constants. Throws: [TextPageOperationException](../api/text/TextPageOperationException.md) See Also:
        * [TextPageExternalObjectInsertionHandler.insertURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage, java.util.List, int)](../api/text/TextPageExternalObjectInsertionHandler.md#insertURLs(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.util.List,int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
