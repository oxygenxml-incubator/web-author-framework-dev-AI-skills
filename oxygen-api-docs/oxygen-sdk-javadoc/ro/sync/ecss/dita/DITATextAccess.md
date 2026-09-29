Package [ro.sync.ecss.dita](package-summary.md)

# Class DITATextAccess

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.dita.DITATextAccess
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public final class DITATextAccess extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Access utility methods to work with DITA in the text editing mode.

## Method Summary
  All MethodsStatic MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [buildFigureHrefImageXMLToInsert](#buildFigureHrefImageXMLToInsert(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.net.URL,java.lang.String,java.lang.String%5B%5D))([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) nodeBaseUrl, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] referenceAttributeNameAndValue)
Creates a figure with title and image XML element.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [buildFigureKeyrefImageXMLToInsert](#buildFigureKeyrefImageXMLToInsert(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.lang.String,java.lang.String))([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) figTitle, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyName)
Creates a figure with title and image XML element with a keyref.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [buildNonMediaFragment](#buildNonMediaFragment(java.lang.String%5B%5D,java.lang.String,java.net.URL))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] referenceAttributeNameAndValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementName, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) nodeBaseUrl)
Creates the xml fragment to insert for non media objects.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [collectPossibleElements](#collectPossibleElements(java.lang.String,java.lang.String,ro.sync.exml.workspace.api.editor.page.text.WSTextXMLSchemaManager,int,java.lang.String...))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reqAttr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultElementName, [WSTextXMLSchemaManager](../../exml/workspace/api/editor/page/text/WSTextXMLSchemaManager.md) schemaManager, int caretOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... classFrag)
Get all the element names that can be inserted at the current caret position and have the class 'classFrag' and a 'reqAttr' attribute.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeKeyReferenceElementName](#computeKeyReferenceElementName(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,ro.sync.ecss.dita.reference.keyref.KeyInfo,boolean,boolean,boolean))([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, ro.sync.ecss.dita.reference.keyref.KeyInfo key, boolean isImage, boolean forceInsertAsVariableKeyref, boolean preferRelatedLinks)
Calculates a suitable reference element to be later inserted for the dropped key.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getCurrentNodeBaseURL](#getCurrentNodeBaseURL(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage))([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess)

 static ro.sync.ecss.dita.reference.keyref.KeyInfo [getKeyInfo](#getKeyInfo(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,java.lang.String))([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fullyQualifiedKeyName)
Get the key info for the fully qualified key name.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPossibleElementQName](#getPossibleElementQName(ro.sync.exml.workspace.api.editor.page.text.WSTextXMLSchemaManager,java.lang.String,java.lang.String))([WSTextXMLSchemaManager](../../exml/workspace/api/editor/page/text/WSTextXMLSchemaManager.md) schemaManager, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) clazzFrag, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mostUsed)
Obtain the qualified name of the element with the given class, which will be inserted in the document.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPreferredKeyRefElementName](#getPreferredKeyRefElementName(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,boolean,boolean))([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textPage, boolean insertImg, boolean insertVariable)
Get the preferred key ref element name.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPreferredKeyRefElementName](#getPreferredKeyRefElementName(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,ro.sync.ecss.dita.reference.keyref.KeyInfo))([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textPage, ro.sync.ecss.dita.reference.keyref.KeyInfo key)
Get the preferred key ref element name.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPreferredKeyRefElementName](#getPreferredKeyRefElementName(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,ro.sync.ecss.dita.reference.keyref.KeyInfo,boolean))([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textPage, ro.sync.ecss.dita.reference.keyref.KeyInfo key, boolean insertImg)
Deprecated.
  static [UtilAccess](../../exml/workspace/api/util/UtilAccess.md) [getUtilAccess](#getUtilAccess())()
Provides access to generic utility methods.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### getKeyInfo

public static ro.sync.ecss.dita.reference.keyref.KeyInfo getKeyInfo([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fullyQualifiedKeyName)

Get the key info for the fully qualified key name.
  Parameters: textPage - The text page access. fullyQualifiedKeyName - The fully qualified name. Returns: The key info. Can be null.
### getPreferredKeyRefElementName

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPreferredKeyRefElementName([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textPage, ro.sync.ecss.dita.reference.keyref.KeyInfo key, boolean insertImg)
 Deprecated.
Get the preferred key ref element name. If the key is reference to an image and the insertImg param is set to true, the returned element will be an image element. Please use [getPreferredKeyRefElementName(WSXMLTextEditorPage, boolean, boolean)](#getPreferredKeyRefElementName(ro.sync.exml.workspace.api.editor.page.text.xml.WSXMLTextEditorPage,boolean,boolean))}
  Parameters: textPage - The text page. key - The key insertImg - true if the keyref should be an image element. Returns: the preferred key ref element name.
### getPreferredKeyRefElementName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPreferredKeyRefElementName([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textPage, ro.sync.ecss.dita.reference.keyref.KeyInfo key)

Get the preferred key ref element name. If the key has reference to an image, won't insert an image element.
  Parameters: textPage - The text page. key - The key Returns: the preferred key ref element name.
### getPreferredKeyRefElementName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPreferredKeyRefElementName([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textPage, boolean insertImg, boolean insertVariable)

Get the preferred key ref element name. If the key is reference to an image and the insertImg param is set to true, the returned element will be an image element.
  Parameters: textPage - The text page. insertImg - true if the keyref should be an image element. insertVariable - true to insert a variable (ph with keyref). Returns: the preferred key ref element name.
### collectPossibleElements

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] collectPossibleElements([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reqAttr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultElementName, [WSTextXMLSchemaManager](../../exml/workspace/api/editor/page/text/WSTextXMLSchemaManager.md) schemaManager, int caretOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... classFrag)

Get all the element names that can be inserted at the current caret position and have the class 'classFrag' and a 'reqAttr' attribute.
  Parameters: reqAttr - The required attribute that needs to be on the element defaultElementName - The default element name, returned if no matching element found. schemaManager - Text page XML schema manager. Provides support for obtaining information about what elements, attributes can be inserted in a given context. caretOffset - The caret offset. classFrag - The class fragment to search for in the element. Returns: All the element names that can be inserted at the current caret position and have the class 'classFrag' and a 'reqAttr' attribute
### getPossibleElementQName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPossibleElementQName([WSTextXMLSchemaManager](../../exml/workspace/api/editor/page/text/WSTextXMLSchemaManager.md) schemaManager, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) clazzFrag, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mostUsed)

Obtain the qualified name of the element with the given class, which will be inserted in the document.
  Parameters: schemaManager - Current schema manager. clazzFrag - The class of the element, whose name is searched. mostUsed - The most used name of the element with the given class. Returns: The qualified name of the element with the given class.
### getCurrentNodeBaseURL

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getCurrentNodeBaseURL([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess)
  Parameters: textAccess - Contains methods specific to XML editors. Returns: The base url of the node at caret position or null.
### computeKeyReferenceElementName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeKeyReferenceElementName([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, ro.sync.ecss.dita.reference.keyref.KeyInfo key, boolean isImage, boolean forceInsertAsVariableKeyref, boolean preferRelatedLinks)

Calculates a suitable reference element to be later inserted for the dropped key.
  Parameters: textAccess - Contains methods specific to XML editors. key - The key to insert. isImage - true if the key is an image reference. forceInsertAsVariableKeyref - true to force insert a variable (ph with keyref). preferRelatedLinks - true to prefer insertion as related links. Returns: Reference element qName to insert or at least a fallback element, never null.
### buildFigureHrefImageXMLToInsert

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) buildFigureHrefImageXMLToInsert([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) nodeBaseUrl, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] referenceAttributeNameAndValue)

Creates a figure with title and image XML element.
  Parameters: textAccess - Offers access to Text page API. nodeBaseUrl - The base url of the document. title - The title of the fig. referenceAttributeNameAndValue - Pair attribute name and value; For example: href, file://filename.pdf. Returns: a figure with title and image XML element.
### buildFigureKeyrefImageXMLToInsert

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) buildFigureKeyrefImageXMLToInsert([WSXMLTextEditorPage](../../exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md) textAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) figTitle, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyName)

Creates a figure with title and image XML element with a keyref.
  Parameters: textAccess - Offers access to Text page API. figTitle - The title of the fig. keyName - The name of the key. Returns: a figure with title and image XML element with a keyref.
### buildNonMediaFragment

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) buildNonMediaFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] referenceAttributeNameAndValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementName, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) nodeBaseUrl)

Creates the xml fragment to insert for non media objects.
  Parameters: referenceAttributeNameAndValue - Pair attribute name and value; For example: href, file://filename.pdf. elementName - The name of the element to be inserted. nodeBaseUrl - The value of the base-uri() attribute of the current node. Returns: The XML fragment to insert.
### getUtilAccess

public static [UtilAccess](../../exml/workspace/api/util/UtilAccess.md) getUtilAccess()

Provides access to generic utility methods.
  Returns: Access to generic utility methods. or null from tests.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
