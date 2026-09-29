Package [ro.sync.ecss.dita](package-summary.md)

# Class DITAAccess

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.dita.DITAAccess
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public final class DITAAccess extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Utility methods for DITA interaction.

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static interface  [DITAAccess.InsertLinkReferenceShortcut](DITAAccess.InsertLinkReferenceShortcut.md)
Short cut for the insert link operation.
  static enum  [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md)
Paste type of clipboard fragments.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [CONKEYREF_TYPE](#CONKEYREF_TYPE)
Conkeyref
  static final int [CONREF_TYPE](#CONREF_TYPE)
Conref
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DEFAULT_CONKEYREF_CONREFEND](#DEFAULT_CONKEYREF_CONREFEND)
Value for conrefend attribute value when a conkeyref is used.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_ROOT_MAP_KEYS_MANAGER_ATTRIBUTE](#DITA_ROOT_MAP_KEYS_MANAGER_ATTRIBUTE)
The attribute name for the keys manager.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_ROOT_MAP_URL_ATTRIBUTE](#DITA_ROOT_MAP_URL_ATTRIBUTE)
The attribute name for the dita root map url.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_VAL_URL_ATTRIBUTE](#DITA_VAL_URL_ATTRIBUTE)
The attribute name for the ditaval url.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FULLY_QUALIFIED_KEYNAME_URL_PARAM](#FULLY_QUALIFIED_KEYNAME_URL_PARAM)
Can be sent as an URL parameter to give more information about the keyref fully qualified value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ID_ANY](#ID_ANY)  Deprecated.
Use [ID_FIRST_TOPIC_ID](#ID_FIRST_TOPIC_ID) instead which has a clearer meaning.
   static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ID_FIRST_TOPIC_ID](#ID_FIRST_TOPIC_ID)
Identifier used in references path, representing that the topic id is the first topic ID in the file.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [IMPOSED_INSERTION_TYPE](#IMPOSED_INSERTION_TYPE)
Query parameter that imposes how a reference will be inserted in DITA
  static final int [INHERITANCE_GENERALIZATION](#INHERITANCE_GENERALIZATION)
If the source is a generalization of the target
  static final int [INHERITANCE_NONE](#INHERITANCE_NONE)
No match between the two classes..
  static final int [INHERITANCE_SAME](#INHERITANCE_SAME)
If the source class is the same as the target class.
  static final int [INHERITANCE_SPECIALIZATION](#INHERITANCE_SPECIALIZATION)
If the source is a specialization of the target
  static final int [KEYREF_TYPE](#KEYREF_TYPE)
Keyref
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LINK_TYPE_DITA_TOPIC](#LINK_TYPE_DITA_TOPIC)
The 'href' attribute type DITA topic.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LINK_TYPE_NON_DITA_RESOURCE](#LINK_TYPE_NON_DITA_RESOURCE)
The 'href' attribute type non DITA resource.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LINK_TYPE_WEB_PAGE](#LINK_TYPE_WEB_PAGE)
The 'href' attribute type web page.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [REF_ATTRIBUTES](#REF_ATTRIBUTES)
DITA reference attributes.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [REUSABLE_COMPONENT_ELEMENT_CLASS_PARAM](#REUSABLE_COMPONENT_ELEMENT_CLASS_PARAM)
Can be sent as an URL parameter to specify the class of the element that will be inserted as conref/conkeyref.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [REUSABLE_COMPONENT_TARGET_PATH_PARAM](#REUSABLE_COMPONENT_TARGET_PATH_PARAM)
Can be sent as an URL parameter to give more information about the element that will be inserted - path to the element ID (topicID/elementID).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [REUSABLE_COMPONENT_TARGET_QNAME_PARAM](#REUSABLE_COMPONENT_TARGET_QNAME_PARAM)
Can be sent as an URL parameter to specify the qname of the element that will be inserted as conref/conkeyref.

## Method Summary
  All MethodsStatic MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 static void [addEditReference](#addEditReference(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Add a new conref to the current element or edit the existing one.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../contentcompletion/xml/CIAttribute.md)> [annotateAttributes](#annotateAttributes(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../contentcompletion/xml/CIAttribute.md)> attributes)  Deprecated.
This method does not do anything anynmore, the attribute annotations are gathered from the framework folder.
   static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [attachKeyScopeInformation](#attachKeyScopeInformation(java.net.URL,java.lang.String,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextMapURL)  Deprecated.  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [attachKeyScopeInformation](#attachKeyScopeInformation(java.net.URL,java.lang.String,java.lang.String,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextMapURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) originalKeyName)
Attach key scope information to the target URL.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [attachKeyScopeInformation](#attachKeyScopeInformation(java.net.URL,java.util.Stack,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetURL, [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextMapURL)
Attach key scope information to the target URL.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [buildFigureHrefImageXMLToInsert](#buildFigureHrefImageXMLToInsert(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) figTitle, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) refAttrValue)
Creates a figure with title and image with href XML element.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [buildFigureKeyrefImageXMLToInsert](#buildFigureKeyrefImageXMLToInsert(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) figTitle, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyName)
Creates a figure with title and image with keyref XML element.
  protected static int [checkConsecutiveInsertionWarning](#checkConsecutiveInsertionWarning(int,int,int,ro.sync.ecss.dita.reference.ReferenceInfo,ro.sync.ecss.dita.reference.ReferenceInfo))(int previousOperationOffset, int selectionStart, int selectionEnd, ro.sync.ecss.dita.reference.ReferenceInfo previousReferenceInfo, ro.sync.ecss.dita.reference.ReferenceInfo currentReferenceInfo)
Show a warning message when consecutive insertion of the same references are performed.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [checkValidKeyName](#checkValidKeyName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyName)
Check if a keyref has a valid key name.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [checkValidKeyRef](#checkValidKeyRef(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref)
Check if a keyref has a valid key name.
  static ro.sync.ecss.dita.ImageInfo [chooseImageReference](#chooseImageReference(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Allows the user to choose an image reference, which will be inserted inside the document.
  static ro.sync.ecss.dita.MediaInfo [chooseMediaReference](#chooseMediaReference(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Allows the user to choose an media file reference, which will be inserted inside the document.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeElementClazz](#computeElementClazz(ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))([WhatPossibleValuesHasAttributeContext](../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context)
Compute the element's clazz
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeFormatForURLPasteAndDnD](#computeFormatForURLPasteAndDnD(ro.sync.exml.workspace.api.util.UtilAccess,java.net.URL,ro.sync.ecss.extensions.api.ReferenceType))([UtilAccess](../../exml/workspace/api/util/UtilAccess.md) utilAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [ReferenceType](../extensions/api/ReferenceType.md) refType)
Computes the format of the xref.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeImageReferenceXMLToInsert](#computeImageReferenceXMLToInsert(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) refAttrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) refValue)
Compute the image reference XML fragment to insert.
  static [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> [computeKeyScopeStack](#computeKeyScopeStack(ro.sync.ecss.extensions.api.node.AuthorNode,java.util.LinkedHashMap))([AuthorNode](../extensions/api/node/AuthorNode.md) contextNode, [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> urlKeyScopesMapping)
Compute the entire key scope stack.
  static [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> [computeKeyScopeStack](#computeKeyScopeStack(ro.sync.ecss.extensions.api.node.AuthorNode,java.util.LinkedHashMap,java.util.Map))([AuthorNode](../extensions/api/node/AuthorNode.md) contextNode, [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> urlKeyScopesMapping, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorNode](../extensions/api/node/AuthorNode.md),[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> stackCache)
Compute the entire key scope stack.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeLinkScope](#computeLinkScope(java.net.URL,java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) hrefURL)
Compute the scope attribute.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeLinkText](#computeLinkText(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseSystemID)  Deprecated.
Use [computeLinkText(AuthorNode, String, String, String, KeysManagerBase)](#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.dita.KeysManagerBase)) instead.
   static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeLinkText](#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String))([AuthorNode](../extensions/api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseSystemID)  Deprecated.
Use [computeLinkText(AuthorNode, String, String, String, KeysManagerBase)](#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.dita.KeysManagerBase)) instead.
   static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeLinkText](#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String))([AuthorNode](../extensions/api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseSystemID)  Deprecated.
Use [computeLinkText(AuthorNode, String, String, String, KeysManagerBase)](#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.dita.KeysManagerBase)) instead.
   static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeLinkText](#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.dita.KeysManagerBase))([AuthorNode](../extensions/api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseSystemID, [KeysManagerBase](KeysManagerBase.md) keysManager)
Obtains information about the referred target.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeMediaReferenceXMLToInsert](#computeMediaReferenceXMLToInsert(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.dita.MediaInfo))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, ro.sync.ecss.dita.MediaInfo reference)
Compute the media reference XML fragment to insert.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [computeQualifiedKeyNames](#computeQualifiedKeyNames(java.lang.String,java.util.Stack))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyToken, [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> keyScopeStack)
Compute key names qualified with key scope stack prefix.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeVariableKeyrefElementName](#computeVariableKeyrefElementName(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Compute the elements name.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeVariableKeyrefElementName](#computeVariableKeyrefElementName(ro.sync.ecss.extensions.api.AuthorAccess,boolean))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, boolean preferImageElement)
Compute the elements name.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [convertDitaCompatibleResource](#convertDitaCompatibleResource(java.io.Reader,java.lang.String,java.lang.String))([Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) toConvert, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) format)
Get the DITA-translated content for the given compatible resource
  static void [createNewTopicReference](#createNewTopicReference(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Create a new DITA topic and link to it as a reference.
  static [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [createReferencesGraph](#createReferencesGraph())()
Create a references graph, will make subsequent searches much faster and it can be reused among multiple searches with the method ro.sync.ecss.dita.DITAAccess.searchReferences(URL, Object).
  static void [createReusableComponent](#createReusableComponent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.DITAUniqueIDAssigner))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, ro.sync.ecss.extensions.api.DITAUniqueIDAssigner idsAssigner)
Reuse the selected content.
  static [DITAImposedReferenceType](DITAImposedReferenceType.md) [detectInsertionType](#detectInsertionType(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Looks at the provided URL and detects if the referred resource should be inserted as a specific XML element.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [detectMediaObjectOutputclass](#detectMediaObjectOutputclass(ro.sync.ecss.dita.reference.keyref.KeyInfo))(ro.sync.ecss.dita.reference.keyref.KeyInfo key)
Detects the output class of a key.
  static void [editProperties](#editProperties(java.net.URL,ro.sync.ecss.contentcompletion.AuthorCCManager,ro.sync.ecss.ue.AuthorDocumentControllerImpl,ro.sync.ecss.extensions.api.node.AuthorElement%5B%5D,ro.sync.ecss.dita.topic.ref.TopicRefInserter,java.lang.Object,boolean))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) location, ro.sync.ecss.contentcompletion.AuthorCCManager ccM, ro.sync.ecss.ue.AuthorDocumentControllerImpl ctrl, [AuthorElement](../extensions/api/node/AuthorElement.md)[] elementsToEdit, ro.sync.ecss.dita.topic.ref.TopicRefInserter topicRefInserter, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, boolean displayReferenceUrl)
Edit properties for the given reference elements.
  static void [editProperties](#editProperties(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Edit properties for the given reference elements.
  static void [editTopicref](#editTopicref(ro.sync.ecss.extensions.api.node.AuthorElement%5B%5D,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorElement](../extensions/api/node/AuthorElement.md)[] topicrefNodes, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Edits one or more topicref elements inside a specialized dialog.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../document/DocumentPositionedInfo.md)> [expandAllKeyrefs](#expandAllKeyrefs(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.link.LinkTextResolver))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [LinkTextResolver](../extensions/api/link/LinkTextResolver.md) linkTextResolver)
Expand all keyrefs from the current document.
  static void [exportDITAMap](#exportDITAMap(java.net.URL,java.io.File,boolean,java.lang.String,ro.sync.ecss.dita.mapeditor.actions.export.helper.ExportProgressUpdater))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) ditamapURL, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) exportDirectory, boolean exportAsZip, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) zipFileName, [ExportProgressUpdater](mapeditor/actions/export/helper/ExportProgressUpdater.md) progressUpdater)
Export DITA Map as zip.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> [filterAttributeValues](#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext,java.lang.String))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypeName)  Deprecated.
Please use the equivalent method which also receives the URL of the requestor.
   static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> [filterAttributeValues](#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypeName, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Propose additional attribute values.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> [filterAttributeValues](#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext,ro.sync.ecss.dita.ContextKeyManager,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context, [ContextKeyManager](ContextKeyManager.md) keyManager, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypeName, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Propose additional attribute values.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> [filterDITAVALAttributeValues](#filterDITAVALAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context)
Filter DITAVAL Attribute values.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../contentcompletion/xml/CIElement.md)> [filterElements](#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../contentcompletion/xml/CIElement.md)> elements, [WhatElementsCanGoHereContext](../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context)
Filter the given elements according to the given context.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../contentcompletion/xml/CIElement.md)> [filterElements](#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext,java.lang.String))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../contentcompletion/xml/CIElement.md)> elements, [WhatElementsCanGoHereContext](../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) authorName)
Filter the given elements according to the given context.
  static void [findSimilarTopics](#findSimilarTopics(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Find similar topics based on words found in title, shortdesc, keyword, and indexterm elements.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAPIKeysManagerDescription](#getAPIKeysManagerDescription())()

 static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAutoInsertImageRefElementName](#getAutoInsertImageRefElementName(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int caretPosition)
Get the name of the image element to insert.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAutoInsertRefElementName](#getAutoInsertRefElementName(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int caretPosition)
Get the name of the topic ref element to insert
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAutoInsertTopicRefElementName](#getAutoInsertTopicRefElementName(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int caretPosition)
Get the name of the topic ref element to insert
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAutoInsertTopicRefElementName](#getAutoInsertTopicRefElementName(ro.sync.ecss.extensions.api.AuthorDocumentController,int))([AuthorDocumentController](../extensions/api/AuthorDocumentController.md) authorDocumentController, int caretPosition)
Get the name of the topic ref element to insert
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getConverterFormatForDITACompatibleResource](#getConverterFormatForDITACompatibleResource(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourceExtension)
Get the converter format that corresponds with the given file extension of the DITA Compatible resource
  static ro.sync.ecss.dita.DITAAccessCustomizer [getDitaAccessCustomizer](#getDitaAccessCustomizer())()

 static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DitaReferenceTargetDescriptor](DitaReferenceTargetDescriptor.md)> [getDitaReferenceTargets](#getDitaReferenceTargets(java.net.URL,java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseUrl, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) topicUrl)
Returns the DITA reference targets in the given topic.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DitaReferenceTargetDescriptor](DitaReferenceTargetDescriptor.md)> [getDitaReferenceTargets](#getDitaReferenceTargets(ro.sync.ecss.extensions.api.AuthorAccess,java.net.URL))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetURL)
Returns the DITA reference targets in the given topic.
  static [CIElement](../../contentcompletion/xml/CIElement.md) [getEquivalentChildCIElement](#getEquivalentChildCIElement(ro.sync.ecss.extensions.api.AuthorAccess,int,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int caretOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tagName)
Get the equivalent child CIElement
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFormat](#getFormat(java.lang.String,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, boolean fillFormatAttr)  Deprecated.
Use [getFormatForLinkCreatedFromGUI(String, String, boolean)](#getFormatForLinkCreatedFromGUI(java.lang.String,java.lang.String,boolean))
   static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFormatForLinkCreatedFromGUI](#getFormatForLinkCreatedFromGUI(java.lang.String,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, boolean fillFormatAttr)
Get the format for the specified resource.
  static [AuthorDocumentFragment](../extensions/api/node/AuthorDocumentFragment.md) [getFragWithMostSuitableTopicrefs](#getFragWithMostSuitableTopicrefs(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment,int))([AuthorDocumentController](../extensions/api/AuthorDocumentController.md) controller, [AuthorDocumentFragment](../extensions/api/node/AuthorDocumentFragment.md) frag, int insertOffset)
When moving/copying topic references, maybe they are not allowed at the new position.
  static [AuthorDocumentFragment](../extensions/api/node/AuthorDocumentFragment.md) [getFragWithMostSuitableTopicrefs](#getFragWithMostSuitableTopicrefs(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorNode,int))([AuthorDocumentController](../extensions/api/AuthorDocumentController.md) controller, [AuthorNode](../extensions/api/node/AuthorNode.md) selectedElem, int insertOffset)
When moving/copying topic references, maybe they are not allowed at the new position.
  static [HrefInfo](HrefInfo.md) [getHrefInformation](#getHrefInformation(ro.sync.ecss.dita.KeysManagerBase,ro.sync.ecss.extensions.api.node.AuthorNode))([KeysManagerBase](KeysManagerBase.md) keyManager, [AuthorNode](../extensions/api/node/AuthorNode.md) node)
Get the reference information (by analizing attributes like keyref, href, mapref, ...) of a node.
  static [HrefInfo](HrefInfo.md) [getHrefInformation](#getHrefInformation(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../extensions/api/node/AuthorNode.md) node)
Get the reference information (by analizing attributes like keyref, href, mapref, ...) of a node.
  static int [getInheritanceType](#getInheritanceType(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sourceClass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetClass)
Check what inheritance is between the two classes.
  static void [getInsertTopicref](#getInsertTopicref(java.net.URL,java.lang.Object,ro.sync.ecss.contentcompletion.AuthorCCManager,ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String,ro.sync.ecss.dita.topic.ref.TopicRefInserter,java.lang.String,boolean))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, ro.sync.ecss.contentcompletion.AuthorCCManager ccM, [AuthorDocumentController](../extensions/api/AuthorDocumentController.md) ctrl, int caretOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialTopicRefLocation, ro.sync.ecss.dita.topic.ref.TopicRefInserter inserter, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) preferredElementName, boolean displayReferenceUrl)
Insert a topic reference.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getKeyForUrl](#getKeyForUrl(java.net.URL,java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
Get the key corresponding to the given URL.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getKeyForUrl](#getKeyForUrl(ro.sync.ecss.dita.KeysManagerBase,java.net.URL,java.net.URL))([KeysManagerBase](KeysManagerBase.md) keyManager, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
Get the key corresponding to the given URL.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getKeyForUrl](#getKeyForUrl(ro.sync.ecss.dita.KeysManagerBase,java.net.URL,java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode))([KeysManagerBase](KeysManagerBase.md) keyManager, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation, [AuthorNode](../extensions/api/node/AuthorNode.md) contextNode)
Get the key corresponding to the given URL.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getKeyRefValueForUrl](#getKeyRefValueForUrl(ro.sync.ecss.dita.KeysManagerBase,java.net.URL,java.net.URL))([KeysManagerBase](KeysManagerBase.md) keysManager, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) referenceUrl, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
Get the key reference corresponding to the given URL.
  static [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.dita.reference.keyref.KeyInfo> [getKeys](#getKeys())()  Deprecated.
Please use the equivalent method which also receives the URL of the requestor.
   static [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.dita.reference.keyref.KeyInfo> [getKeys](#getKeys(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

 static [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.dita.reference.keyref.KeyInfo> [getKeys](#getKeys(java.net.URL,ro.sync.ecss.dita.ContextKeyManager))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [ContextKeyManager](ContextKeyManager.md) keysManager)
Returns the mapped DITA 1.2 keys
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getKeysAttributeValueBasedOnFilename](#getKeysAttributeValueBasedOnFilename(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Get the value of the "keys" attribute based on the current filename.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.ecss.dita.reference.keyref.KeyInfo> [getKeysForInsertion](#getKeysForInsertion(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
Get the list of keys which can be inserted in the topic identified by the "originatorURL" field.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPossibleElementQName](#getPossibleElementQName(ro.sync.ecss.extensions.api.AuthorDocumentController,java.lang.String,java.lang.String))([AuthorDocumentController](../extensions/api/AuthorDocumentController.md) ctrl, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) clazzFrag, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mostUsed)
Obtain the qualified name of the element with the given class, which will be inserted in the document.
  static [CIElement](../../contentcompletion/xml/CIElement.md)[] [getPossibleElements](#getPossibleElements(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String,java.lang.String...))([AuthorDocumentController](../extensions/api/AuthorDocumentController.md) ctrl, int offset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reqAttr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... classFrag)
Get the possible elements that can be inserted at a given offset and have the class 'classFrag' and a 'reqAttr' attribute.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[RelLink](reference/reltable/RelLink.md)> [getRelatedLinksFromReltable](#getRelatedLinksFromReltable(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
Get the list of related links from all the relationship tables defined in the DITA Maps.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getRootMapURL](#getRootMapURL())()
Get DITA root map URL.
  static void [getTopicRefInfo](#getTopicRefInfo(java.net.URL,java.lang.Object,ro.sync.ecss.contentcompletion.AuthorCCManager,ro.sync.ecss.ue.AuthorDocumentControllerImpl,int,ro.sync.ecss.dita.topic.ref.TopicrefInfo,ro.sync.ecss.dita.topic.ref.TopicRefInserter))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) location, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, ro.sync.ecss.contentcompletion.AuthorCCManager ccM, ro.sync.ecss.ue.AuthorDocumentControllerImpl ctrl, int caretOffset, ro.sync.ecss.dita.topic.ref.TopicrefInfo initialTopicrefInfo, ro.sync.ecss.dita.topic.ref.TopicRefInserter inserter)  Deprecated.
This method is not used anymore from oXygen to insert topic reference elements and it will be removed in a future release.
   static [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> [getURLKeyScopeContexts](#getURLKeyScopeContexts(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
Get the URL to key scopes context for the default keys manager.
  static [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> [getURLKeyScopeContexts](#getURLKeyScopeContexts(java.net.URL,ro.sync.ecss.dita.ContextKeyManager))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [ContextKeyManager](ContextKeyManager.md) keysManager)
Returns a mapping between topic URLs and DITA 1.3 key scopes where the URLs are referenced.
  static void [handleTopicRefInsertUrl](#handleTopicRefInsertUrl(ro.sync.ecss.extensions.api.AuthorAccess,java.net.URL))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) topicUrl)
Insert a topic ref with the given URL.
  static boolean [hasAPIKeysManager](#hasAPIKeysManager())()

 static void [insertContentKeyReference](#insertContentKeyReference(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialKeyName)
Shows a dialog that allows inserting a content key reference and setting the original key to select in the Keys combo box.
  static void [insertContentReference](#insertContentReference(ro.sync.ecss.extensions.api.AuthorAccess,java.net.URL,boolean))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl)
Shows a dialog that allows inserting a content reference (conref).
  static void [insertHref](#insertHref(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,java.lang.String,boolean,boolean))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, boolean isHrefTypeDitaTopic)
Insert a Xref.
  static void [insertHref](#insertHref(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,java.lang.String,boolean,boolean,java.net.URL,boolean))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, boolean isHrefTypeDitaTopic, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl)
Insert a Xref or link element.
  static void [insertImage](#insertImage(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ref)
Insert a DITA Image
  static void [insertImage](#insertImage(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.dita.ImageInfo))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, ro.sync.ecss.dita.ImageInfo ref)
Insert a DITA Image.
  static [SchemaAwareHandlerResult](../extensions/api/schemaaware/SchemaAwareHandlerResult.md) [insertImageSchemaAware](#insertImageSchemaAware(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ref)
Insert a DITA Image
  static [SchemaAwareHandlerResult](../extensions/api/schemaaware/SchemaAwareHandlerResult.md) [insertImageSchemaAware](#insertImageSchemaAware(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) refAttrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) refValue)
Insert a DITA Image
  static [SchemaAwareHandlerResult](../extensions/api/schemaaware/SchemaAwareHandlerResult.md) [insertImageSchemaAware](#insertImageSchemaAware(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.dita.ImageInfo))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, ro.sync.ecss.dita.ImageInfo reference)
Insert a DITA image.
  static void [insertKeydefWithKeyword](#insertKeydefWithKeyword(java.lang.Object,ro.sync.ecss.contentcompletion.AuthorCCManager,ro.sync.ecss.extensions.api.AuthorDocumentController,int,ro.sync.ecss.dita.topic.ref.TopicRefInserter,boolean))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, ro.sync.ecss.contentcompletion.AuthorCCManager ccM, [AuthorDocumentController](../extensions/api/AuthorDocumentController.md) ctrl, int caretOffset, ro.sync.ecss.dita.topic.ref.TopicRefInserter inserter, boolean append)
Insert a key definition with keyword.
  static void [insertKeydefWithKeyword](#insertKeydefWithKeyword(java.lang.Object,ro.sync.ecss.contentcompletion.AuthorCCManager,ro.sync.ecss.extensions.api.AuthorDocumentController,int,ro.sync.ecss.dita.topic.ref.TopicRefInserter,ro.sync.ecss.dita.DITATopicInsertionPosition))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, ro.sync.ecss.contentcompletion.AuthorCCManager ccM, [AuthorDocumentController](../extensions/api/AuthorDocumentController.md) ctrl, int caretOffset, ro.sync.ecss.dita.topic.ref.TopicRefInserter inserter, [DITATopicInsertionPosition](DITATopicInsertionPosition.md) insertPos)
Insert a key definition with keyword.
  static void [insertKeydefWithKeyword](#insertKeydefWithKeyword(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Insert a key definition with keyword.
  static void [insertLinkReference](#insertLinkReference(java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,java.lang.String,boolean,boolean,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetElementClass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetElementQName, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, boolean useKeyRef, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefType)
Insert a Xref or link element.
  static void [insertLinkReference](#insertLinkReference(java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,java.lang.String,boolean,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetElementClass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetElementQName, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefType)
Insert a Xref or link element.
  static void [insertLinkReference](#insertLinkReference(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,java.lang.String,boolean,java.lang.String,java.lang.String,java.net.URL,boolean))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) preferredElName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefType, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl)
Insert a Xref or link element.
  static void [insertLinkReference](#insertLinkReference(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,java.lang.String,boolean,java.lang.String,java.lang.String,java.net.URL,boolean,ro.sync.ecss.dita.DITAAccess.InsertLinkReferenceShortcut))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) preferredElName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefType, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl, [DITAAccess.InsertLinkReferenceShortcut](DITAAccess.InsertLinkReferenceShortcut.md) insertLinkReferenceShortcut)
Insert a Xref or link element.
  static void [insertLinkReference](#insertLinkReference(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,java.lang.String,boolean,java.lang.String,java.net.URL,boolean))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefType, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl)
Insert a Xref or link element.
  static void [insertLinkReference](#insertLinkReference(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,java.lang.String,boolean,java.lang.String,java.net.URL,boolean,ro.sync.ecss.dita.DITAAccess.InsertLinkReferenceShortcut))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefType, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl, [DITAAccess.InsertLinkReferenceShortcut](DITAAccess.InsertLinkReferenceShortcut.md) insertLinkReferenceShortcut)
Insert a Xref or link element.
  static void [insertMedia](#insertMedia(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.dita.MediaInfo))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, ro.sync.ecss.dita.MediaInfo ref)
Insert a media object.
  static [SchemaAwareHandlerResult](../extensions/api/schemaaware/SchemaAwareHandlerResult.md) [insertMediaSchemaAware](#insertMediaSchemaAware(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.dita.MediaInfo))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, ro.sync.ecss.dita.MediaInfo reference)
Insert a DITA media object.
  static void [insertReference](#insertReference(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int refType)
Insert a keyref or a conkeyref.
  static int [insertReference](#insertReference(ro.sync.ecss.extensions.api.AuthorAccess,int,ro.sync.ecss.component.HeadlessViewport,ro.sync.ecss.contentcompletion.AuthorCCManager,ro.sync.ecss.dita.reference.ReferenceInfo))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int refType, ro.sync.ecss.component.HeadlessViewport viewport, ro.sync.ecss.contentcompletion.AuthorCCManager ccManager, ro.sync.ecss.dita.reference.ReferenceInfo refInfo)
Insert the given reference information with the given type.
  static void [insertReference](#insertReference(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,int,java.lang.String,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceValue, int refType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetElementQName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementClass)
Inserts a reference from the information passed in the ArgumentsMap.
  static void [insertReference](#insertReference(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetElementQName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementClass)
Inserts a reference from the information passed in the ArgumentsMap.
  static void [insertReusableComponent](#insertReusableComponent(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Insert a reusable component
  static void [insertTopicgroup](#insertTopicgroup(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Insert a topic group.
  static void [insertTopichead](#insertTopichead(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Insert a topic head.
  static void [insertTopicref](#insertTopicref(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Insert a topic ref.
  static void [insertTopicref](#insertTopicref(ro.sync.ecss.extensions.api.AuthorAccess,java.net.URL,boolean))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl)
Insert a topic reference.
  static void [insertTopicref](#insertTopicref(ro.sync.exml.workspace.api.editor.page.ditamap.WSDITAMapEditorPage,java.net.URL,java.lang.String,boolean,boolean))([WSDITAMapEditorPage](../../exml/workspace/api/editor/page/ditamap/WSDITAMapEditorPage.md) ditaPageAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) preferredElementName, boolean asChild, boolean displayReferenceUrl)
Insert a topic reference in the DITA Map tree.
  static void [insertTopicref](#insertTopicref(ro.sync.exml.workspace.api.editor.page.ditamap.WSDITAMapEditorPage,java.net.URL,java.lang.String,ro.sync.ecss.dita.DITATopicInsertionPosition,boolean))([WSDITAMapEditorPage](../../exml/workspace/api/editor/page/ditamap/WSDITAMapEditorPage.md) ditaPageAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) preferredElementName, [DITATopicInsertionPosition](DITATopicInsertionPosition.md) insertPos, boolean displayReferenceUrl)
Insert a topic reference in the DITA Map tree.
  static boolean [isDITA](#isDITA(org.xml.sax.Attributes))([Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) atts)
Check if the resource is DITA.
  static boolean [isDITA1_3OrNewer](#isDITA1_3OrNewer(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) archVersion)
Check if the topic or map with a certain architecture version is DITA 1.3 or newer,
  static boolean [isDITA1_3OrNewer](#isDITA1_3OrNewer(org.xml.sax.Attributes))([Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) atts)
Check if the topic or map with a certain architecture version is DITA 1.3 or newer,
  static boolean [isDITACompatileFormat](#isDITACompatileFormat(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) format)
Check if the given format is compatible to be converted to DITA XML.
  static boolean [isGeneralizationOf](#isGeneralizationOf(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sourceClass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetClass)  Deprecated.
use getInheritanceType instead.
   static boolean [isGenericMediaContent](#isGenericMediaContent(ro.sync.ecss.dita.reference.keyref.KeyInfo))(ro.sync.ecss.dita.reference.keyref.KeyInfo selectedKey)
Checks if the selected key refers resources that can be wrapped in a media object.s
  static boolean [isKeyDefToDITAResource](#isKeyDefToDITAResource(ro.sync.ecss.dita.reference.keyref.KeyInfo))(ro.sync.ecss.dita.reference.keyref.KeyInfo keyInfo)
Check if this key definition points to a DITA topic, map or variable text.
  static boolean [isKeyReferenceToImage](#isKeyReferenceToImage(ro.sync.ecss.dita.reference.keyref.KeyInfo))(ro.sync.ecss.dita.reference.keyref.KeyInfo key)
Checks if the current key is a reference to an image.
  static boolean [isReferenceToDITACompatibleResource](#isReferenceToDITACompatibleResource(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.dita.reference.keyref.KeyInfo))([AuthorNode](../extensions/api/node/AuthorNode.md) node, ro.sync.ecss.dita.reference.keyref.KeyInfo keyInfo)
Check if this reference points to a DITA compatible resource (that can be converted to DITA using dynamic converter DITA-OT plugin).
  static boolean [isReferenceToDITAResource](#isReferenceToDITAResource(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.dita.reference.keyref.KeyInfo))([AuthorNode](../extensions/api/node/AuthorNode.md) node, ro.sync.ecss.dita.reference.keyref.KeyInfo keyInfo)
Check if this reference points to a DITA topic, map or variable text.
  static [Reference](Reference.md) [parseDITAHref](#parseDITAHref(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseUrl, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue)
Parse the href attribute and returns the absolute URL and the id.
  static [Reference](Reference.md) [parseDITAHref](#parseDITAHref(java.lang.String,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseUrl, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, boolean isHrefToDITAResource)
Parse the href attribute and returns the absolute URL and the id.
  static [Reference](Reference.md) [parseDITAKeyRef](#parseDITAKeyRef(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref)  Deprecated.
Please use the equivalent method which also receives the URL of the requestor.
   static [Reference](Reference.md) [parseDITAKeyRef](#parseDITAKeyRef(java.lang.String,ro.sync.ecss.dita.reference.keyref.KeyResolver))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref, ro.sync.ecss.dita.reference.keyref.KeyResolver kr)
Parse the DITA conkeyref value
  static [Reference](Reference.md) [parseDITAKeyRef](#parseDITAKeyRef(java.net.URL,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref)
Parse the DITA conkeyref value
  static [Reference](Reference.md) [parseDITAKeyRef](#parseDITAKeyRef(java.net.URL,ro.sync.ecss.dita.ContextKeyManager,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [ContextKeyManager](ContextKeyManager.md) keyManager, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref)
Parse the DITA conkeyref value
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [pasteAsReference](#pasteAsReference(ro.sync.ecss.extensions.api.AuthorAccess,boolean))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, boolean asConref)
Paste as reference
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [pasteAsReference](#pasteAsReference(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.dita.DITAAccess.PasteInfo))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md) pasteInfo)
Paste as reference
  static boolean [pasteClipboardFragmentsAsReference](#pasteClipboardFragmentsAsReference(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.dita.DITAAccess.PasteInfo,ro.sync.ecss.component.AuthorDocumentFragmentClipboardObject%5B%5D))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md) pasteInfo, ro.sync.ecss.component.AuthorDocumentFragmentClipboardObject[] fragments)
Paste the fragments from clipboard as reference.
  static boolean [pasteClipboardFragmentsAsReference](#pasteClipboardFragmentsAsReference(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.dita.DITAAccess.PasteInfo,ro.sync.ecss.component.AuthorDocumentFragmentClipboardObject%5B%5D,ro.sync.ecss.extensions.api.SelectionInterpretationMode))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md) pasteInfo, ro.sync.ecss.component.AuthorDocumentFragmentClipboardObject[] fragments, [SelectionInterpretationMode](../extensions/api/SelectionInterpretationMode.md) selectionInterpretationMode)
Paste the fragments from clipboard as reference.
  static boolean [preferAddingKeyrefToAlreadyReferencedResource](#preferAddingKeyrefToAlreadyReferencedResource(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorURL)
Check if a keyref is preferred to be added when inserting a resource (that is already referred) in the editor .
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [proposeFolderUrlForChildTopicref](#proposeFolderUrlForChildTopicref(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../extensions/api/node/AuthorElement.md) parent)
Propose a folder URL where to save a new topicref that is added in a DITA Map as a child of the given node.
  static void [pushElement](#pushElement(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Shows a dialog that allows the user to push an element.
  static void [removeReference](#removeReference(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Remove a content reference from a DITA document.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../document/DocumentPositionedInfo.md)> [replaceAllConrefs](#replaceAllConrefs(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Expand all conrefs and conkeyrefs from the current document.
  static void [replaceConref](#replaceConref(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Replace the conref at caret position
  static void [resolveKeyNotFoundError](#resolveKeyNotFoundError(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref)
The give key was not found.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolveKeyRef](#resolveKeyRef(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRef)  Deprecated.
Please use the equivalent method which also receives the URL of the requestor.
   static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolveKeyRef](#resolveKeyRef(java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRef, boolean addANYIdentifierForKeys)  Deprecated.
Please use the equivalent method which also receives the URL of the requestor.
   static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolveKeyRef](#resolveKeyRef(java.net.URL,java.lang.String,boolean))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRef, boolean addANYIdentifierForKeys)
Resolve a keyref.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolveKeyRef](#resolveKeyRef(java.net.URL,java.lang.String,ro.sync.ecss.dita.ContextKeyManager,boolean))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRef, [ContextKeyManager](ContextKeyManager.md) keysManager, boolean addANYIdentifierForKeys)
Resolve a keyref.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [resolveKeyRefToHref](#resolveKeyRefToHref(java.net.URL,java.lang.String,ro.sync.ecss.dita.ContextKeyManager,boolean))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRef, [ContextKeyManager](ContextKeyManager.md) keysManager, boolean addANYIdentifierForKeys)
Resolve a keyref to a plain href which may or may not be an URL.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [rewriteKeyref](#rewriteKeyref(java.util.LinkedHashMap,java.util.LinkedHashMap,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> urlKeyScopesMapping, [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.dita.reference.keyref.KeyInfo> keys, [AuthorNode](../extensions/api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref)
Rewrite a keyref looking also at key scopes..
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../document/DocumentPositionedInfo.md)> [searchReferences](#searchReferences(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetTopicURL)
Search the references to this topic.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../document/DocumentPositionedInfo.md)> [searchReferences](#searchReferences(java.net.URL,java.lang.Object))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetTopicURL, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) referencesGraph)
Search the references to this topic.
  static void [searchReferences](#searchReferences(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Search references to a certain element at the caret position.
  static void [setDitaAccessCustomizer](#setDitaAccessCustomizer(ro.sync.ecss.dita.DITAAccessCustomizer))(ro.sync.ecss.dita.DITAAccessCustomizer ditaAccessCustomizer)
Set the DITA access customizer from SA or EC.
  static void [setExtraMainFileURLs](#setExtraMainFileURLs(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> mainFileURLs)
Set extra main file URLs
  static void [setKeyNameGenerator](#setKeyNameGenerator(ro.sync.ecss.dita.DITAKeyNameGenerator))([DITAKeyNameGenerator](DITAKeyNameGenerator.md) ditaKeyNameGenerator)
Set a key name generator for when the "keys" attribute is automatically generated and set to topicrefs based on the names of the referenced files.
  static void [showInsertReferenceDialog](#showInsertReferenceDialog(ro.sync.ecss.contentcompletion.AuthorCCManager,ro.sync.ecss.ue.AuthorDocumentControllerImpl,int,java.lang.Object,int,boolean,ro.sync.ecss.dita.topic.ref.ReferenceInserter))(ro.sync.ecss.contentcompletion.AuthorCCManager ccManager, ro.sync.ecss.ue.AuthorDocumentControllerImpl controller, int caretOffset, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, int refType, boolean showOnlyKeysList, ro.sync.ecss.dita.topic.ref.ReferenceInserter referenceInserter)
Shows the keyref/conkeyref insert dialog and returns the chosen reference information.
  static void [showInsertReferenceDialog](#showInsertReferenceDialog(ro.sync.ecss.contentcompletion.AuthorCCManager,ro.sync.ecss.ue.AuthorDocumentControllerImpl,int,java.lang.Object,int,boolean,ro.sync.ecss.dita.topic.ref.ReferenceInserter,ro.sync.ecss.dita.IKeyInfoFilter,boolean))(ro.sync.ecss.contentcompletion.AuthorCCManager ccManager, ro.sync.ecss.ue.AuthorDocumentControllerImpl controller, int caretOffset, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, int refType, boolean showOnlyKeysList, ro.sync.ecss.dita.topic.ref.ReferenceInserter referenceInserter, ro.sync.ecss.dita.IKeyInfoFilter keysFilter, boolean useModalDialog)
Shows the keyref/conkeyref insert dialog and returns the chosen reference information.
  static void [showKeysAndReusableComponents](#showKeysAndReusableComponents(ro.sync.ecss.extensions.api.AuthorAccess,boolean,boolean))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, boolean showKeys, boolean showComps)
Show a content completion window with keys and components.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [showNewFileDialog](#showNewFileDialog(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) proposedTitle)
Shows the New File wizard to allow creating new documents.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### IMPOSED_INSERTION_TYPE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) IMPOSED_INSERTION_TYPE

Query parameter that imposes how a reference will be inserted in DITA
  Since: 25 See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.IMPOSED_INSERTION_TYPE)

### FULLY_QUALIFIED_KEYNAME_URL_PARAM

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FULLY_QUALIFIED_KEYNAME_URL_PARAM

Can be sent as an URL parameter to give more information about the keyref fully qualified value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.FULLY_QUALIFIED_KEYNAME_URL_PARAM)

### REUSABLE_COMPONENT_TARGET_PATH_PARAM

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) REUSABLE_COMPONENT_TARGET_PATH_PARAM

Can be sent as an URL parameter to give more information about the element that will be inserted - path to the element ID (topicID/elementID).
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.REUSABLE_COMPONENT_TARGET_PATH_PARAM)

### REUSABLE_COMPONENT_TARGET_QNAME_PARAM

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) REUSABLE_COMPONENT_TARGET_QNAME_PARAM

Can be sent as an URL parameter to specify the qname of the element that will be inserted as conref/conkeyref.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.REUSABLE_COMPONENT_TARGET_QNAME_PARAM)

### REUSABLE_COMPONENT_ELEMENT_CLASS_PARAM

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) REUSABLE_COMPONENT_ELEMENT_CLASS_PARAM

Can be sent as an URL parameter to specify the class of the element that will be inserted as conref/conkeyref.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.REUSABLE_COMPONENT_ELEMENT_CLASS_PARAM)

### LINK_TYPE_WEB_PAGE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LINK_TYPE_WEB_PAGE

The 'href' attribute type web page.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.LINK_TYPE_WEB_PAGE)

### LINK_TYPE_NON_DITA_RESOURCE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LINK_TYPE_NON_DITA_RESOURCE

The 'href' attribute type non DITA resource.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.LINK_TYPE_NON_DITA_RESOURCE)

### LINK_TYPE_DITA_TOPIC

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LINK_TYPE_DITA_TOPIC

The 'href' attribute type DITA topic.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.LINK_TYPE_DITA_TOPIC)

### DITA_ROOT_MAP_URL_ATTRIBUTE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_ROOT_MAP_URL_ATTRIBUTE

The attribute name for the dita root map url. The attribute is given as string.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.DITA_ROOT_MAP_URL_ATTRIBUTE)

### DITA_VAL_URL_ATTRIBUTE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_VAL_URL_ATTRIBUTE

The attribute name for the ditaval url. The attribute is given as string.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.DITA_VAL_URL_ATTRIBUTE)

### DITA_ROOT_MAP_KEYS_MANAGER_ATTRIBUTE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_ROOT_MAP_KEYS_MANAGER_ATTRIBUTE

The attribute name for the keys manager. If set it has priority over [DITA_ROOT_MAP_URL_ATTRIBUTE](#DITA_ROOT_MAP_URL_ATTRIBUTE). The attribute class is [ContextKeyManager](ContextKeyManager.md).
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.DITA_ROOT_MAP_KEYS_MANAGER_ATTRIBUTE)

### REF_ATTRIBUTES

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] REF_ATTRIBUTES

DITA reference attributes.

### DEFAULT_CONKEYREF_CONREFEND

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DEFAULT_CONKEYREF_CONREFEND

Value for conrefend attribute value when a conkeyref is used.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.DEFAULT_CONKEYREF_CONREFEND)

### KEYREF_TYPE

public static final int KEYREF_TYPE

Keyref
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.KEYREF_TYPE)

### CONREF_TYPE

public static final int CONREF_TYPE

Conref
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.CONREF_TYPE)

### CONKEYREF_TYPE

public static final int CONKEYREF_TYPE

Conkeyref
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.CONKEYREF_TYPE)

### ID_FIRST_TOPIC_ID

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ID_FIRST_TOPIC_ID

Identifier used in references path, representing that the topic id is the first topic ID in the file.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.ID_FIRST_TOPIC_ID)

### ID_ANY

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ID_ANY
 Deprecated.
Use [ID_FIRST_TOPIC_ID](#ID_FIRST_TOPIC_ID) instead which has a clearer meaning. Identifier used in references path, representing that the topic id can be excluded from the reference.
   See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.ID_ANY)

### INHERITANCE_GENERALIZATION

public static final int INHERITANCE_GENERALIZATION

If the source is a generalization of the target
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.INHERITANCE_GENERALIZATION)

### INHERITANCE_SPECIALIZATION

public static final int INHERITANCE_SPECIALIZATION

If the source is a specialization of the target
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.INHERITANCE_SPECIALIZATION)

### INHERITANCE_SAME

public static final int INHERITANCE_SAME

If the source class is the same as the target class.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.INHERITANCE_SAME)

### INHERITANCE_NONE

public static final int INHERITANCE_NONE

No match between the two classes..
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.dita.DITAAccess.INHERITANCE_NONE)

## Method Details

### setKeyNameGenerator

public static void setKeyNameGenerator([DITAKeyNameGenerator](DITAKeyNameGenerator.md) ditaKeyNameGenerator)

Set a key name generator for when the "keys" attribute is automatically generated and set to topicrefs based on the names of the referenced files.
  Parameters: ditaKeyNameGenerator - The dita key name generator to set. null to remove the previous one. Since: 23
### getKeysAttributeValueBasedOnFilename

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getKeysAttributeValueBasedOnFilename([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Get the value of the "keys" attribute based on the current filename.
  Parameters: url - The URL of the current file. Returns: the value.
### createReferencesGraph

public static [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) createReferencesGraph()

Create a references graph, will make subsequent searches much faster and it can be reused among multiple searches with the method ro.sync.ecss.dita.DITAAccess.searchReferences(URL, Object).
  Returns: the references graph. Can be null is something went wrong. Since: 23
### searchReferences

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../document/DocumentPositionedInfo.md)> searchReferences([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetTopicURL)

Search the references to this topic.
  Parameters: targetTopicURL - The URL of the target topic (i.e. the topic that is referenced). Returns: the references or an empty list. Never null;
### searchReferences

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../document/DocumentPositionedInfo.md)> searchReferences([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetTopicURL, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) referencesGraph)

Search the references to this topic.
  Parameters: targetTopicURL - The URL of the target topic (i.e. the topic that is referenced). referencesGraph - The already created graph, if not null the search will be much faster. Returns: the references or an empty list. Never null; Since: 23
### insertTopicref

public static void insertTopicref([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a topic ref.
  Parameters: authorAccess - The author access. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### handleTopicRefInsertUrl

public static void handleTopicRefInsertUrl([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) topicUrl)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a topic ref with the given URL. No dialog is displayed.
  Parameters: authorAccess - The author access. topicUrl - The URL of the topic to be inserted. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### insertTopicgroup

public static void insertTopicgroup([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a topic group.
  Parameters: authorAccess - The author access. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### getTopicRefInfo

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static void getTopicRefInfo([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) location, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, ro.sync.ecss.contentcompletion.AuthorCCManager ccM, ro.sync.ecss.ue.AuthorDocumentControllerImpl ctrl, int caretOffset, ro.sync.ecss.dita.topic.ref.TopicrefInfo initialTopicrefInfo, ro.sync.ecss.dita.topic.ref.TopicRefInserter inserter)
 Deprecated.
This method is not used anymore from oXygen to insert topic reference elements and it will be removed in a future release. All topic reference elements are inserted using the same method: [editProperties(URL, AuthorCCManager, AuthorDocumentControllerImpl, AuthorElement[], TopicRefInserter, Object, boolean)](#editProperties(java.net.URL,ro.sync.ecss.contentcompletion.AuthorCCManager,ro.sync.ecss.ue.AuthorDocumentControllerImpl,ro.sync.ecss.extensions.api.node.AuthorElement%5B%5D,ro.sync.ecss.dita.topic.ref.TopicRefInserter,java.lang.Object,boolean))

Show the topic reference info dialog with some initial content
  Parameters: location - The DITA map location parentFrame - The parent frame. ccM - The CC Manager. ctrl - The document controller. caretOffset - The caret offset. initialTopicrefInfo - Initial topic ref info. inserter - Callback when the dialog is used.
### getInsertTopicref

public static void getInsertTopicref([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, ro.sync.ecss.contentcompletion.AuthorCCManager ccM, [AuthorDocumentController](../extensions/api/AuthorDocumentController.md) ctrl, int caretOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialTopicRefLocation, ro.sync.ecss.dita.topic.ref.TopicRefInserter inserter, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) preferredElementName, boolean displayReferenceUrl)

Insert a topic reference.
  Parameters: editorLocation - The editor location. parentFrame - The parent frame. ccM - The CC Manager. ctrl - The document controller. caretOffset - The caret offset. initialTopicRefLocation - The initial location (relative or absolute) to set to the topic ref insert dialog. inserter - Topic ref inserter preferredElementName - Preferred name or class of the element to insert displayReferenceUrl - If true the URL input will be displayed in the insert topic reference dialog (the user will have the possibility to change the reference URL). This parameter can be set to false when an initialReferenceURL is provided, and the user must not have the possibility to change it (the reference URL must be fixed).  **Note:**  this parameter is not used on Eclipse plugin implementation.
### insertKeydefWithKeyword

public static void insertKeydefWithKeyword([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, ro.sync.ecss.contentcompletion.AuthorCCManager ccM, [AuthorDocumentController](../extensions/api/AuthorDocumentController.md) ctrl, int caretOffset, ro.sync.ecss.dita.topic.ref.TopicRefInserter inserter, boolean append)

Insert a key definition with keyword.
  Parameters: parentFrame - The parent frame. ccM - The CC Manager. ctrl - The document controller. caretOffset - The caret offset. inserter - Topic reference inserter  **Note:**  the preferredElementName parameter is not used on Eclipse plugin implementation. append - true to append child, false to insert after.
### insertKeydefWithKeyword

public static void insertKeydefWithKeyword([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, ro.sync.ecss.contentcompletion.AuthorCCManager ccM, [AuthorDocumentController](../extensions/api/AuthorDocumentController.md) ctrl, int caretOffset, ro.sync.ecss.dita.topic.ref.TopicRefInserter inserter, [DITATopicInsertionPosition](DITATopicInsertionPosition.md) insertPos)

Insert a key definition with keyword.
  Parameters: parentFrame - The parent frame. ccM - The CC Manager. ctrl - The document controller. caretOffset - The caret offset. inserter - Topic reference inserter  **Note:**  the preferredElementName parameter is not used on Eclipse plugin implementation. insertPos - one of the values defined in [DITATopicInsertionPosition](DITATopicInsertionPosition.md).
### insertKeydefWithKeyword

public static void insertKeydefWithKeyword([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)

Insert a key definition with keyword.
  Parameters: authorAccess - Author access.
### insertTopichead

public static void insertTopichead([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a topic head.
  Parameters: authorAccess - The author access. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### setDitaAccessCustomizer

public static void setDitaAccessCustomizer(ro.sync.ecss.dita.DITAAccessCustomizer ditaAccessCustomizer)

Set the DITA access customizer from SA or EC.
  Parameters: ditaAccessCustomizer - The DITA access customizer.
### getDitaAccessCustomizer

public static ro.sync.ecss.dita.DITAAccessCustomizer getDitaAccessCustomizer()
  Returns: Returns the ditaAccessCustomizer.
### hasAPIKeysManager

public static boolean hasAPIKeysManager()
  Returns: true if we have a keys manager provided through the API.
### getAPIKeysManagerDescription

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAPIKeysManagerDescription()
  Returns: A description for the API Keys manager.
### editProperties

public static void editProperties([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) location, ro.sync.ecss.contentcompletion.AuthorCCManager ccM, ro.sync.ecss.ue.AuthorDocumentControllerImpl ctrl, [AuthorElement](../extensions/api/node/AuthorElement.md)[] elementsToEdit, ro.sync.ecss.dita.topic.ref.TopicRefInserter topicRefInserter, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, boolean displayReferenceUrl)

Edit properties for the given reference elements.
  Parameters: location - DITA Map editor location. ccM - The CC Manager ctrl - The Author document controller. elementsToEdit - The elements that must be edited. topicRefInserter - Callback to insert/edit a topic ref parentFrame - Parent frame. displayReferenceUrl - If true the URL input will be displayed in the edit reference dialog (the user will have the possibility to change the reference URL). Since: 17.1
### editProperties

public static void editProperties([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Edit properties for the given reference elements.
  Parameters: authorAccess - the author access. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### insertHref

public static void insertHref([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, boolean isHrefTypeDitaTopic, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a Xref or link element.
  Parameters: authorAccess - The author access. typeValue - The type attribute value. If not null, the generated reference will have the 'type="typeValue"' attribute set to it. formatValue - The format attribute value. If not null and the reference points to a non-DITA resource, the generated reference will have the 'format="formatValue"' attribute set to it. scopeValue - The scope attribute value. If not null, the generated reference will have the 'scope="scopeValue"' attribute set to it. isXref - true if we need to insert an <xref> element, false for the <link> element. isHrefTypeDitaTopic - If true the user wants to insert a reference to a DITA resource (Insert Cross Reference action) If false the user wants to a reference to an external non-dita resource (Web Link action or File Reference action). initialReferenceURL - The default URL that will be displayed in the URL field of the insert reference dialog.  **Note:**  this parameter is not used on Eclipse plugin implementation. displayReferenceUrl - If true the URL input will be displayed in the insert reference dialog (the user will have the possibility to change the reference URL). This parameter can be set to false when an initialReferenceURL is provided, and the user must not have the possibility to change it (the reference URL must be fixed).  **Note:**  this parameter is not used on Eclipse plugin implementation. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) Since: 14.2
### insertHref

public static void insertHref([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, boolean isHrefTypeDitaTopic)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a Xref.
  Parameters: authorAccess - The author access. typeValue - The the attribute value. formatValue - The format attribute value. scopeValue - The scope attribute value. isXref - true if we need to insert a xref element, false for link element. isHrefTypeDitaTopic - if true a dita topic chooser will be shown otherwise a input url dialog will be show for the href attribute value. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### insertContentKeyReference

public static void insertContentKeyReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialKeyName)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Shows a dialog that allows inserting a content key reference and setting the original key to select in the Keys combo box.
  Parameters: authorAccess - The Author access. initialKeyName - The key that will be displayed in the Key field of the insert reference dialog. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) Since: 21  **Note:**  this API method is implemented only for Eclipse plugin.
### insertContentReference

public static void insertContentReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Shows a dialog that allows inserting a content reference (conref).
  Parameters: authorAccess - The Author access. initialReferenceURL - The default URL that will be displayed in the URL field of the insert reference dialog.  **Note:**  this parameter is not used on Eclipse plugin implementation. displayReferenceUrl - If true the URL input will be displayed in the insert reference dialog (the user will have the possibility to change the reference URL). This parameter can be set to false when an initialReferenceURL is provided, and the user must not have the possibility to change it (the reference URL must be fixed).  **Note:**  this parameter is not used on Eclipse plugin implementation. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) Since: 14.2
### insertTopicref

public static void insertTopicref([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a topic reference.
  Parameters: authorAccess - The Author access. initialReferenceURL - The default URL that will be displayed in the URL field of the insert reference dialog.  **Note:**  this parameter is not used on Eclipse plugin implementation. displayReferenceUrl - If true the URL input will be displayed in the insert reference dialog (the user will have the possibility to change the reference URL). This parameter can be set to false when an initialReferenceURL is provided, and the user must not have the possibility to change it (the reference URL must be fixed).  **Note:**  this parameter is not used on Eclipse plugin implementation. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) Since: 14.2
### insertTopicref

public static void insertTopicref([WSDITAMapEditorPage](../../exml/workspace/api/editor/page/ditamap/WSDITAMapEditorPage.md) ditaPageAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) preferredElementName, boolean asChild, boolean displayReferenceUrl)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a topic reference in the DITA Map tree.
  Parameters: ditaPageAccess - The DITA Page access. initialReferenceURL - The default URL that will be displayed in the URL field of the insert reference dialog.  **Note:**  this parameter is not used on Eclipse plugin implementation. preferredElementName - The preferred name of the element to insert. asChild - true to insert as a child of the selected item, false to insert as a next sibling. displayReferenceUrl - If true the URL input will be displayed in the insert reference dialog (the user will have the possibility to change the reference URL). This parameter can be set to false when an initialReferenceURL is provided, and the user must not have the possibility to change it (the reference URL must be fixed).  **Note:**  this parameter is not used on Eclipse plugin implementation. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) Since: 15
### insertTopicref

public static void insertTopicref([WSDITAMapEditorPage](../../exml/workspace/api/editor/page/ditamap/WSDITAMapEditorPage.md) ditaPageAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) preferredElementName, [DITATopicInsertionPosition](DITATopicInsertionPosition.md) insertPos, boolean displayReferenceUrl)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a topic reference in the DITA Map tree.
  Parameters: ditaPageAccess - The DITA Page access. initialReferenceURL - The default URL that will be displayed in the URL field of the insert reference dialog.  **Note:**  this parameter is not used on Eclipse plugin implementation. preferredElementName - The preferred name of the element to insert. insertPos - one of the values defined in [DITATopicInsertionPosition](DITATopicInsertionPosition.md). displayReferenceUrl - If true the URL input will be displayed in the insert reference dialog (the user will have the possibility to change the reference URL). This parameter can be set to false when an initialReferenceURL is provided, and the user must not have the possibility to change it (the reference URL must be fixed).  **Note:**  this parameter is not used on Eclipse plugin implementation. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) Since: 15
### insertReference

public static void insertReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int refType)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a keyref or a conkeyref.
  Parameters: authorAccess - The author access. refType - Reference type. Can be one of the following constants:
        * [CONKEYREF_TYPE](#CONKEYREF_TYPE),
        * [CONREF_TYPE](#CONREF_TYPE),
        * [KEYREF_TYPE](#KEYREF_TYPE),
 Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### showInsertReferenceDialog

public static void showInsertReferenceDialog(ro.sync.ecss.contentcompletion.AuthorCCManager ccManager, ro.sync.ecss.ue.AuthorDocumentControllerImpl controller, int caretOffset, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, int refType, boolean showOnlyKeysList, ro.sync.ecss.dita.topic.ref.ReferenceInserter referenceInserter)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Shows the keyref/conkeyref insert dialog and returns the chosen reference information.
  Parameters: ccManager - CC manager. controller - Author document controller. caretOffset - Caret offset. parentFrame - Parent frame. refType - One of: [KEYREF_TYPE](#KEYREF_TYPE), [CONREF_TYPE](#CONREF_TYPE), [CONKEYREF_TYPE](#CONKEYREF_TYPE) showOnlyKeysList - true to show only keys list in the insert reference dialog. referenceInserter - The reference inserter. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - When the insertion fails.
### showInsertReferenceDialog

public static void showInsertReferenceDialog(ro.sync.ecss.contentcompletion.AuthorCCManager ccManager, ro.sync.ecss.ue.AuthorDocumentControllerImpl controller, int caretOffset, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, int refType, boolean showOnlyKeysList, ro.sync.ecss.dita.topic.ref.ReferenceInserter referenceInserter, ro.sync.ecss.dita.IKeyInfoFilter keysFilter, boolean useModalDialog)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Shows the keyref/conkeyref insert dialog and returns the chosen reference information.
  Parameters: ccManager - CC manager. controller - Author document controller. caretOffset - Caret offset. parentFrame - Parent frame. refType - One of: [KEYREF_TYPE](#KEYREF_TYPE), [CONREF_TYPE](#CONREF_TYPE), [CONKEYREF_TYPE](#CONKEYREF_TYPE) showOnlyKeysList - true to show only keys list in the insert reference dialog. referenceInserter - The reference inserter. keysFilter - Filters the keys. useModalDialog - true if the dialog should be modal. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - When the insertion fails.
### insertReference

public static void insertReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetElementQName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementClass)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Inserts a reference from the information passed in the ArgumentsMap.
  Parameters: authorAccess - the AuthorAccess referenceValue - the reference value. targetElementQName - the target element qualified name. elementClass - the element class. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - if the operation fails.
### insertReference

public static void insertReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceValue, int refType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetElementQName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementClass)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Inserts a reference from the information passed in the ArgumentsMap.
  Parameters: authorAccess - The AuthorAccess referenceValue - The reference value. refType - The reference type targetElementQName - The target element qualified name. elementClass - The element class. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - if the operation fails.
### insertReference

public static int insertReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int refType, ro.sync.ecss.component.HeadlessViewport viewport, ro.sync.ecss.contentcompletion.AuthorCCManager ccManager, ro.sync.ecss.dita.reference.ReferenceInfo refInfo)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert the given reference information with the given type.
  Parameters: authorAccess - The author access refType - The reference type viewport - The viewport ccManager - The CC Manager refInfo - The reference info. Returns: The offset where the insertion took place. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - When a problem occurs.
### getRootMapURL

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getRootMapURL()

Get DITA root map URL.
  Returns: DITA root map URL.
### resolveKeyRef

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolveKeyRef([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRef)
 Deprecated.
Please use the equivalent method which also receives the URL of the requestor.

Deprecated method for resolving a keyref. Preserved for backward compatibility.
  Parameters: keyRef - The keyref value Returns: The absolute value of the key ref target.
### resolveKeyRef

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolveKeyRef([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRef, boolean addANYIdentifierForKeys)
 Deprecated.
Please use the equivalent method which also receives the URL of the requestor.

Resolve a keyref.
  Parameters: keyRef - The keyref value addANYIdentifierForKeys - If true then reference keys will be prefixed by 'ANY/'. in a element_keyref function. Returns: The absolute value of the key ref target.
### resolveKeyRef

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolveKeyRef([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRef, boolean addANYIdentifierForKeys)

Resolve a keyref.
  Parameters: originatorURL - The originator URL. keyRef - The keyref value addANYIdentifierForKeys - If true then reference keys will be prefixed by 'ANY/'. in a element_keyref function. Returns: The absolute value of the key ref target.
### checkValidKeyRef

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) checkValidKeyRef([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref)

Check if a keyref has a valid key name.
  Parameters: keyref - The keyref (may also contain the "/"). Returns: an error message if the key name is not valid or null if the key name is valid.
### resolveKeyRef

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolveKeyRef([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRef, [ContextKeyManager](ContextKeyManager.md) keysManager, boolean addANYIdentifierForKeys)

Resolve a keyref.
  Parameters: originatorURL - The url that contains the key. keyRef - The keyref value keysManager - The key manager. addANYIdentifierForKeys - If true then reference keys will be prefixed by 'ANY/'. in a element_keyref function. Returns: The absolute value of the key ref target.
### resolveKeyRefToHref

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resolveKeyRefToHref([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRef, [ContextKeyManager](ContextKeyManager.md) keysManager, boolean addANYIdentifierForKeys)

Resolve a keyref to a plain href which may or may not be an URL.
  Parameters: originatorURL - The url that contains the key. keyRef - The keyref value keysManager - The key manager. addANYIdentifierForKeys - If true then reference keys will be prefixed by 'ANY/'. in a element_keyref function. Returns: The absolute value of the key ref target. Since: 27.1
### createReusableComponent

public static void createReusableComponent([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, ro.sync.ecss.extensions.api.DITAUniqueIDAssigner idsAssigner)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Reuse the selected content.
  Parameters: authorAccess - The author access idsAssigner - The IDs assigner Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - If fails
### insertReusableComponent

public static void insertReusableComponent([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a reusable component
  Parameters: authorAccess - The author access Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### replaceAllConrefs

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../document/DocumentPositionedInfo.md)> replaceAllConrefs([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Expand all conrefs and conkeyrefs from the current document.
  Parameters: authorAccess - The access in author page. Returns: A list with problems from this process. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - If failed to find conrefs or conkeyrefs.
### replaceConref

public static void replaceConref([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Replace the conref at caret position
  Parameters: authorAccess -  Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### expandAllKeyrefs

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../document/DocumentPositionedInfo.md)> expandAllKeyrefs([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [LinkTextResolver](../extensions/api/link/LinkTextResolver.md) linkTextResolver)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Expand all keyrefs from the current document. The keyrefs from xrefs and links are changed with hrefs.
  Parameters: authorAccess - Access class to the author functions. linkTextResolver - Resolves a link and obtains a text representation. Returns: A list with problems from this process. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - If failed to find keyrefs.
### removeReference

public static void removeReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Remove a content reference from a DITA document.
  Parameters: authorAccess - The author access. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### addEditReference

public static void addEditReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Add a new conref to the current element or edit the existing one.
  Parameters: authorAccess - The author access Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### isGeneralizationOf

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static boolean isGeneralizationOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sourceClass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetClass)
 Deprecated.
use getInheritanceType instead.

True if the first class value is a generalization or the same as the second class value.
  Parameters: sourceClass - The source class value targetClass - The target class value Returns: True if the first class value is a generalization of the second
### getInheritanceType

public static int getInheritanceType([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sourceClass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetClass)

Check what inheritance is between the two classes.
  Parameters: sourceClass - The source class value targetClass - The target class value Returns: the inheritance type between the source and target class
### parseDITAHref

public static [Reference](Reference.md) parseDITAHref([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseUrl, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Parse the href attribute and returns the absolute URL and the id.
  Parameters: baseUrl - The base document URL. hrefValue - The href attribute value. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility Returns: A container object with the content reference URI and topicID or null. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - Can't create the URL.
### parseDITAHref

public static [Reference](Reference.md) parseDITAHref([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseUrl, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, boolean isHrefToDITAResource)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Parse the href attribute and returns the absolute URL and the id.
  Parameters: baseUrl - The base document URL. hrefValue - The href attribute value. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility isHrefToDITAResource - true if this is an href to a DITA resource Returns: A container object with the content reference URI and topicID or null. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - Can't create the URL.
### parseDITAKeyRef

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static [Reference](Reference.md) parseDITAKeyRef([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)
 Deprecated.
Please use the equivalent method which also receives the URL of the requestor.

Parse the DITA conkeyref value
  Parameters: keyref - The attribute 'conkeyref' value Returns: The DITA Conref object Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)
### parseDITAKeyRef

public static [Reference](Reference.md) parseDITAKeyRef([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Parse the DITA conkeyref value
  Parameters: originatorURL - The originator URL. keyref - The attribute 'conkeyref' value Returns: The DITA Conref object Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)
### parseDITAKeyRef

public static [Reference](Reference.md) parseDITAKeyRef([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [ContextKeyManager](ContextKeyManager.md) keyManager, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Parse the DITA conkeyref value
  Parameters: originatorURL - The originator URL. keyManager - The key manager used to resolve the keyref. keyref - The attribute 'conkeyref' value Returns: The DITA Conref object Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)
### parseDITAKeyRef

public static [Reference](Reference.md) parseDITAKeyRef([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref, ro.sync.ecss.dita.reference.keyref.KeyResolver kr)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Parse the DITA conkeyref value
  Parameters: keyref - The attribute 'conkeyref' value kr - The keys resolver Returns: The DITA Conref object Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)
### getAutoInsertTopicRefElementName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAutoInsertTopicRefElementName([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int caretPosition)

Get the name of the topic ref element to insert
  Parameters: authorAccess - The author access caretPosition - Caret position Returns: A name for the topic ref to insert
### getAutoInsertTopicRefElementName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAutoInsertTopicRefElementName([AuthorDocumentController](../extensions/api/AuthorDocumentController.md) authorDocumentController, int caretPosition)

Get the name of the topic ref element to insert
  Parameters: authorDocumentController - The author document controller. caretPosition - Caret position Returns: A name for the topic ref to insert Since: 23.1
### getAutoInsertRefElementName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAutoInsertRefElementName([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int caretPosition)

Get the name of the topic ref element to insert
  Parameters: authorAccess - The author access caretPosition - Caret position Returns: A name for the topic ref to insert
### getAutoInsertImageRefElementName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAutoInsertImageRefElementName([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int caretPosition)

Get the name of the image element to insert.
  Parameters: authorAccess - The author access caretPosition - Caret position Returns: A name for the topic ref to insert
### getPossibleElements

public static [CIElement](../../contentcompletion/xml/CIElement.md)[] getPossibleElements([AuthorDocumentController](../extensions/api/AuthorDocumentController.md) ctrl, int offset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reqAttr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... classFrag)

Get the possible elements that can be inserted at a given offset and have the class 'classFrag' and a 'reqAttr' attribute.
  Parameters: ctrl - the author document controller. offset - the offset. reqAttr - the required attribute that needs to be on the element. classFrag - the class fragments to search for in the element. Returns: the possible elements that can be inserted at a given offset and have the class 'classFrag' and a 'reqAttr' attribute.
### getEquivalentChildCIElement

public static [CIElement](../../contentcompletion/xml/CIElement.md) getEquivalentChildCIElement([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int caretOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tagName)

Get the equivalent child CIElement
  Parameters: authorAccess - Author access caretOffset - The caret offset tagName - The tag name Returns: the equivalent child CIElement
### getKeys

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.dita.reference.keyref.KeyInfo> getKeys()
 Deprecated.
Please use the equivalent method which also receives the URL of the requestor.
   Returns: The mapped DITA 1.2 keys
### getKeys

public static [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.dita.reference.keyref.KeyInfo> getKeys([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
  Parameters: originatorURL - The URL for which the keys are requested Returns: The mapped DITA 1.2 keys
### getKeysForInsertion

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.ecss.dita.reference.keyref.KeyInfo> getKeysForInsertion([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

Get the list of keys which can be inserted in the topic identified by the "originatorURL" field. Depending on the places where the topic is referenced in the DITA Map, if there are key scopes defined the list of keys may contain the same key present multiple number of times but with different key scope prefixed names.
  Parameters: originatorURL - The URL for which the keys are requested Returns: The list of keys depends on the current editing context.
### getKeys

public static [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.dita.reference.keyref.KeyInfo> getKeys([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [ContextKeyManager](ContextKeyManager.md) keysManager)

Returns the mapped DITA 1.2 keys
  Parameters: originatorURL - The URL of the document which contains the keys. keysManager - The key manager that is aware of the context of the document. Returns: The mapped DITA 1.2 keys
### getURLKeyScopeContexts

public static [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> getURLKeyScopeContexts([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [ContextKeyManager](ContextKeyManager.md) keysManager)

Returns a mapping between topic URLs and DITA 1.3 key scopes where the URLs are referenced.
  Parameters: originatorURL - The URL of the document which contains the keys. keysManager - The key manager that is aware of the context of the document. Returns: The mapped DITA 1.2 keys
### computeFormatForURLPasteAndDnD

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeFormatForURLPasteAndDnD([UtilAccess](../../exml/workspace/api/util/UtilAccess.md) utilAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [ReferenceType](../extensions/api/ReferenceType.md) refType)

Computes the format of the xref.
  Parameters: utilAccess - The util access API. Never null. url - The URL to paste. refType - The reference type. Returns: The format.
### computeLinkScope

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeLinkScope([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) hrefURL)

Compute the scope attribute.
  Parameters: editorLocation - Editor location hrefURL - Href location. Returns: the computed scope attribute construction. Never null.
### pasteAsReference

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pasteAsReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, boolean asConref)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Paste as reference
  Parameters: authorAccess - The author access. asConref - True if paste as conref, false as link Returns: information about how this action should be used. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### pasteAsReference

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pasteAsReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md) pasteInfo)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Paste as reference
  Parameters: authorAccess - The author access. pasteInfo - Paste type of clipboard fragments. Returns: information about how this action should be used. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### pasteClipboardFragmentsAsReference

public static boolean pasteClipboardFragmentsAsReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md) pasteInfo, ro.sync.ecss.component.AuthorDocumentFragmentClipboardObject[] fragments)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Paste the fragments from clipboard as reference.
  Parameters: authorAccess - The author access. pasteInfo - Paste type of clipboard fragments. fragments - The fragments to paste with. Returns: true if the paste was valid. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### pasteClipboardFragmentsAsReference

public static boolean pasteClipboardFragmentsAsReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md) pasteInfo, ro.sync.ecss.component.AuthorDocumentFragmentClipboardObject[] fragments, [SelectionInterpretationMode](../extensions/api/SelectionInterpretationMode.md) selectionInterpretationMode)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Paste the fragments from clipboard as reference.
  Parameters: authorAccess - The author access. pasteInfo - Paste type of clipboard fragments. fragments - The fragments to paste with. selectionInterpretationMode - Selection interpretation mode Returns: true if the paste was valid. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### filterAttributeValues

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> filterAttributeValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypeName)
 Deprecated.
Please use the equivalent method which also receives the URL of the requestor.

Propose additional attribute values.
  Parameters: attributeValues - The attribute values. context - The context. documentTypeName - The document type name. Returns: The enriched list.
### filterAttributeValues

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> filterAttributeValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypeName, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)

Propose additional attribute values.
  Parameters: attributeValues - The attribute values. context - The context. documentTypeName - The document type name. authorAccess - The Author Access. Returns: The enriched list.
### filterAttributeValues

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> filterAttributeValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context, [ContextKeyManager](ContextKeyManager.md) keyManager, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypeName, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)

Propose additional attribute values.
  Parameters: attributeValues - The attribute values. context - The context. keyManager - The key manager to use to propose values for attributes like keyref. documentTypeName - The document type name. authorAccess - The Author Access. Can be null Returns: The enriched list.
### computeElementClazz

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeElementClazz([WhatPossibleValuesHasAttributeContext](../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context)

Compute the element's clazz
  Parameters: context - The attributes editing context. Returns: The element clazz or null.
### insertImage

public static void insertImage([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ref)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a DITA Image
  Parameters: authorAccess - The author access ref - The reference. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### insertMedia

public static void insertMedia([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, ro.sync.ecss.dita.MediaInfo ref)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a media object.
  Parameters: authorAccess - The author access. ref - Media reference. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - When fail.
### chooseMediaReference

public static ro.sync.ecss.dita.MediaInfo chooseMediaReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Allows the user to choose an media file reference, which will be inserted inside the document.
  Parameters: authorAccess - The author access. Returns: A MediaInfo object containing all the properties for the file which will be inserted. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - On fail.
### insertMediaSchemaAware

public static [SchemaAwareHandlerResult](../extensions/api/schemaaware/SchemaAwareHandlerResult.md) insertMediaSchemaAware([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, ro.sync.ecss.dita.MediaInfo reference)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a DITA media object.
  Parameters: authorAccess - The author access reference - The reference value. Returns: The insertion result Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - On fail.
### computeMediaReferenceXMLToInsert

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeMediaReferenceXMLToInsert([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, ro.sync.ecss.dita.MediaInfo reference)

Compute the media reference XML fragment to insert.
  Parameters: authorAccess - The author access. reference - The reference information . Returns: the image reference XML fragment to insert.
### insertImage

public static void insertImage([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, ro.sync.ecss.dita.ImageInfo ref)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a DITA Image.
  Parameters: authorAccess - The author access ref - The information reference. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - If the image could not be inserted.
### chooseImageReference

public static ro.sync.ecss.dita.ImageInfo chooseImageReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Allows the user to choose an image reference, which will be inserted inside the document.
  Parameters: authorAccess - The author access. Returns: A ImageInfo object containing all the properties for the image, which will be inserted. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### insertImageSchemaAware

public static [SchemaAwareHandlerResult](../extensions/api/schemaaware/SchemaAwareHandlerResult.md) insertImageSchemaAware([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ref)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a DITA Image
  Parameters: authorAccess - The author access ref - The reference. Returns: The insertion result Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### insertImageSchemaAware

public static [SchemaAwareHandlerResult](../extensions/api/schemaaware/SchemaAwareHandlerResult.md) insertImageSchemaAware([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) refAttrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) refValue)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a DITA Image
  Parameters: authorAccess - The author access refAttrName - The reference attribute name. refValue - The reference value. Returns: The insertion result Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### insertImageSchemaAware

public static [SchemaAwareHandlerResult](../extensions/api/schemaaware/SchemaAwareHandlerResult.md) insertImageSchemaAware([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, ro.sync.ecss.dita.ImageInfo reference)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a DITA image.
  Parameters: authorAccess - The author access reference - The reference value. Returns: The insertion result Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### computeImageReferenceXMLToInsert

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeImageReferenceXMLToInsert([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) refAttrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) refValue)

Compute the image reference XML fragment to insert.
  Parameters: authorAccess - The author access. refAttrName - The reference attribute name refValue - The reference value name Returns: the image reference XML fragment to insert.
### buildFigureHrefImageXMLToInsert

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) buildFigureHrefImageXMLToInsert([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) figTitle, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) refAttrValue)

Creates a figure with title and image with href XML element.
  Parameters: authorAccess - Offers access to Author page API. figTitle - The title of the figure. refAttrValue - The value of the href attribute. Returns: a figure with title and image XML element. Since: 25.0
### buildFigureKeyrefImageXMLToInsert

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) buildFigureKeyrefImageXMLToInsert([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) figTitle, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyName)

Creates a figure with title and image with keyref XML element.
  Parameters: authorAccess - Offers access to Author page API. figTitle - The title of the figure. keyName - The name of the key. Returns: a figure with title and image with keyref XML element. Since: 25.0
### getPossibleElementQName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPossibleElementQName([AuthorDocumentController](../extensions/api/AuthorDocumentController.md) ctrl, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) clazzFrag, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mostUsed)

Obtain the qualified name of the element with the given class, which will be inserted in the document.
  Parameters: ctrl - The author document controller. clazzFrag - The class of the element, whose name is searched. mostUsed - The most used name of the element with the given class. Returns: The qualified name of the element with the given class.
### searchReferences

public static void searchReferences([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)

Search references to a certain element at the caret position.
  Parameters: authorAccess - The author access.
### computeLinkText

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeLinkText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseSystemID)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html), [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html), [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
 Deprecated.
Use [computeLinkText(AuthorNode, String, String, String, KeysManagerBase)](#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.dita.KeysManagerBase)) instead.

Obtains information about the referred target.
  Parameters: hrefValue - The relative location of the target. baseSystemID - base system ID. Returns: The computed title information. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html) [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
### computeLinkText

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeLinkText([AuthorNode](../extensions/api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseSystemID)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html), [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html), [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
 Deprecated.
Use [computeLinkText(AuthorNode, String, String, String, KeysManagerBase)](#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.dita.KeysManagerBase)) instead.

Obtains information about the referred target.
  Parameters: contextNode - The context node. hrefValue - The relative location of the target. baseSystemID - base system ID. Returns: The computed title information. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html) [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
### computeLinkText

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeLinkText([AuthorNode](../extensions/api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseSystemID)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html), [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html), [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
 Deprecated.
Use [computeLinkText(AuthorNode, String, String, String, KeysManagerBase)](#computeLinkText(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.dita.KeysManagerBase)) instead.

Obtains information about the referred target.
  Parameters: contextNode - The context node. keyRefValue - The fully prefixed key scope value hrefValue - The relative location of the target. baseSystemID - base system ID. Returns: The computed title information. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html) [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
### computeLinkText

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeLinkText([AuthorNode](../extensions/api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseSystemID, [KeysManagerBase](KeysManagerBase.md) keysManager)throws [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

Obtains information about the referred target.
  Parameters: contextNode - The context node. keyRefValue - The fully prefixed key scope value hrefValue - The relative location of the target. baseSystemID - base system ID. keysManager - The key manager. Returns: The computed title information. Throws: [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) Since: 21
### filterElements

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../contentcompletion/xml/CIElement.md)> filterElements([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../contentcompletion/xml/CIElement.md)> elements, [WhatElementsCanGoHereContext](../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context)

Filter the given elements according to the given context.
  Parameters: elements - The list of CIElement elements. context - The context. Returns: The filtered CIElements.
### filterElements

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../contentcompletion/xml/CIElement.md)> filterElements([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../contentcompletion/xml/CIElement.md)> elements, [WhatElementsCanGoHereContext](../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) authorName)

Filter the given elements according to the given context.
  Parameters: elements - The list of CIElement elements. context - The context. authorName - the name of the author to be used for draft comment author attribute. If null, the user from the current editor is used. Returns: The filtered CIElements.
### resolveKeyNotFoundError

public static void resolveKeyNotFoundError([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref)

The give key was not found. We will present a warning dialog to the user and we will offer the user as a possible solution to change the root map.
  Parameters: authorAccess - Interface to the author context. keyref - The key that wasn't found in the current root map context.
### filterDITAVALAttributeValues

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> filterDITAVALAttributeValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context)

Filter DITAVAL Attribute values.
  Parameters: attributeValues - The current list of attribute values. context - The what attribute values context. Returns: The modified list of values.
### createNewTopicReference

public static void createNewTopicReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

Create a new DITA topic and link to it as a reference.
  Parameters: authorAccess - The Author Access Throws: [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) - if it fails.
### pushElement

public static void pushElement([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Shows a dialog that allows the user to push an element.
  Parameters: authorAccess - The Author access. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - When the operation could not be completed. Since: 17.1
### isDITA

public static boolean isDITA([Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) atts)

Check if the resource is DITA.
  Parameters: atts - The SAX attributes from the root element. Returns: true if the topic or map with a certain architecture version is DITA, Since: 20.1
### isDITA1_3OrNewer

public static boolean isDITA1_3OrNewer([Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) atts)

Check if the topic or map with a certain architecture version is DITA 1.3 or newer,
  Parameters: atts - The SAX attributes from the root element. Returns: true if the topic or map with a certain architecture version is DITA 1.3 or newer, Since: 20.1
### isDITA1_3OrNewer

public static boolean isDITA1_3OrNewer([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) archVersion)

Check if the topic or map with a certain architecture version is DITA 1.3 or newer,
  Parameters: archVersion - The architecture version taken from the root element. Returns: true if the topic or map with a certain architecture version is DITA 1.3 or newer,
### insertLinkReference

public static void insertLinkReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefType, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a Xref or link element.
  Parameters: authorAccess - The author access. typeValue - The type attribute value. If not null, the generated reference will have the 'type="typeValue"' attribute set to it. formatValue - The format attribute value. If not null and the reference points to a non-DITA resource, the generated reference will have the 'format="formatValue"' attribute set to it. scopeValue - The scope attribute value. If not null, the generated reference will have the 'scope="scopeValue"' attribute set to it. isXref - true if we need to insert an <xref> element, false for the <link> element. hrefType - The type of the link. If [LINK_TYPE_DITA_TOPIC](#LINK_TYPE_DITA_TOPIC), the user wants to insert a reference to a DITA resource (Insert Cross Reference action). If [LINK_TYPE_NON_DITA_RESOURCE](#LINK_TYPE_NON_DITA_RESOURCE), wants to a reference to an external non-dita resource (Web Link action or File Reference action). initialReferenceURL - The default URL that will be displayed in the URL field of the insert reference dialog.  **Note:**  this parameter is not used on Eclipse plugin implementation. displayReferenceUrl - If true the URL input will be displayed in the insert reference dialog (the user will have the possibility to change the reference URL). This parameter can be set to false when an initialReferenceURL is provided, and the user must not have the possibility to change it (the reference URL must be fixed).  **Note:**  this parameter is not used on Eclipse plugin implementation. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### insertLinkReference

public static void insertLinkReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) preferredElName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefType, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a Xref or link element.
  Parameters: authorAccess - The author access. typeValue - The type attribute value. If not null, the generated reference will have the 'type="typeValue"' attribute set to it. formatValue - The format attribute value. If not null and the reference points to a non-DITA resource, the generated reference will have the 'format="formatValue"' attribute set to it. scopeValue - The scope attribute value. If not null, the generated reference will have the 'scope="scopeValue"' attribute set to it. isXref - true if we need to insert an <xref> element, false for the <link> element. preferredElName - The preferred name of the reference element. hrefType - The type of the link. If [LINK_TYPE_DITA_TOPIC](#LINK_TYPE_DITA_TOPIC), the user wants to insert a reference to a DITA resource (Insert Cross Reference action). If [LINK_TYPE_NON_DITA_RESOURCE](#LINK_TYPE_NON_DITA_RESOURCE), wants to a reference to an external non-dita resource (Web Link action or File Reference action). initialReferenceURL - The default URL that will be displayed in the URL field of the insert reference dialog.  **Note:**  this parameter is not used on Eclipse plugin implementation. displayReferenceUrl - If true the URL input will be displayed in the insert reference dialog (the user will have the possibility to change the reference URL). This parameter can be set to false when an initialReferenceURL is provided, and the user must not have the possibility to change it (the reference URL must be fixed).  **Note:**  this parameter is not used on Eclipse plugin implementation. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### insertLinkReference

public static void insertLinkReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefType, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl, [DITAAccess.InsertLinkReferenceShortcut](DITAAccess.InsertLinkReferenceShortcut.md) insertLinkReferenceShortcut)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a Xref or link element.
  Parameters: authorAccess - The author access. typeValue - The type attribute value. If not null, the generated reference will have the 'type="typeValue"' attribute set to it. formatValue - The format attribute value. If not null and the reference points to a non-DITA resource, the generated reference will have the 'format="formatValue"' attribute set to it. scopeValue - The scope attribute value. If not null, the generated reference will have the 'scope="scopeValue"' attribute set to it. isXref - true if we need to insert an <xref> element, false for the <link> element. hrefType - The type of the link. If [LINK_TYPE_DITA_TOPIC](#LINK_TYPE_DITA_TOPIC), the user wants to insert a reference to a DITA resource (Insert Cross Reference action). If [LINK_TYPE_NON_DITA_RESOURCE](#LINK_TYPE_NON_DITA_RESOURCE), wants to a reference to an external non-dita resource (Web Link action or File Reference action). initialReferenceURL - The default URL that will be displayed in the URL field of the insert reference dialog.  **Note:**  this parameter is not used on Eclipse plugin implementation. displayReferenceUrl - If true the URL input will be displayed in the insert reference dialog (the user will have the possibility to change the reference URL). This parameter can be set to false when an initialReferenceURL is provided, and the user must not have the possibility to change it (the reference URL must be fixed).  **Note:**  this parameter is not used on Eclipse plugin implementation. insertLinkReferenceShortcut - A shortcut class that allows us to collectthe references before inserting them into document. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) Since: 18
### insertLinkReference

public static void insertLinkReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) preferredElName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefType, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) initialReferenceURL, boolean displayReferenceUrl, [DITAAccess.InsertLinkReferenceShortcut](DITAAccess.InsertLinkReferenceShortcut.md) insertLinkReferenceShortcut)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a Xref or link element.
  Parameters: authorAccess - The author access. typeValue - The type attribute value. If not null, the generated reference will have the type="typeValue" attribute set to it. formatValue - The format attribute value. If not null and the reference points to a non-DITA resource, the generated reference will have the format="formatValue" attribute set to it. scopeValue - The scope attribute value. If not null, the generated reference will have the scope="scopeValue" attribute set to it. isXref - true if we need to insert an <xref> element, false for the <link> element. preferredElName - The preferred name of the reference element. hrefType - The type of the link. If [LINK_TYPE_DITA_TOPIC](#LINK_TYPE_DITA_TOPIC), the user wants to insert a reference to a DITA resource (Insert Cross Reference action). If [LINK_TYPE_NON_DITA_RESOURCE](#LINK_TYPE_NON_DITA_RESOURCE), wants to a reference to an external non-dita resource (Web Link action or File Reference action). initialReferenceURL - The default URL that will be displayed in the URL field of the insert reference dialog. **Note:**  this parameter is not used on Eclipse plugin implementation. displayReferenceUrl - If true the URL input will be displayed in the insert reference dialog (the user will have the possibility to change the reference URL). This parameter can be set to false when an initialReferenceURLis provided, and the user must not have the possibility to change it (the reference URL must be fixed). **Note:**  this parameter is not used on Eclipse plugin implementation. insertLinkReferenceShortcut - A shortcut class that allows us to collectthe references before inserting them into document. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) Since: 18
### insertLinkReference

public static void insertLinkReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetElementClass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetElementQName, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefType)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a Xref or link element.
  Parameters: referenceValue - The class of the target element. targetElementClass - The class of the target element. targetElementQName - The qualified name of the target element. authorAccess - The author access. typeValue - The type attribute value. If not null, the generated reference will have the 'type="typeValue"' attribute set to it. formatValue - The format attribute value. If not null and the reference points to a non-DITA resource, the generated reference will have the 'format="formatValue"' attribute set to it. scopeValue - The scope attribute value. If not null, the generated reference will have the 'scope="scopeValue"' attribute set to it. isXref - true if we need to insert an <xref> element, false for the <link> element. hrefType - The type of the link. If [LINK_TYPE_DITA_TOPIC](#LINK_TYPE_DITA_TOPIC), the user wants to insert a reference to a DITA resource (Insert Cross Reference action). If [LINK_TYPE_NON_DITA_RESOURCE](#LINK_TYPE_NON_DITA_RESOURCE), wants to a reference to an external non-dita resource (Web Link action or File Reference action). Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) Since: 18
### insertLinkReference

public static void insertLinkReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetElementClass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetElementQName, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scopeValue, boolean isXref, boolean useKeyRef, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefType)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a Xref or link element.
  Parameters: referenceValue - The class of the target element. targetElementClass - The class of the target element. targetElementQName - The qualified name of the target element. authorAccess - The author access. typeValue - The type attribute value. If not null, the generated reference will have the 'type="typeValue"' attribute set to it. formatValue - The format attribute value. If not null and the reference points to a non-DITA resource, the generated reference will have the 'format="formatValue"' attribute set to it. scopeValue - The scope attribute value. If not null, the generated reference will have the 'scope="scopeValue"' attribute set to it. isXref - true if we need to insert an <xref> element, false for the <link> element. useKeyRef - true if the reference is a keyref. hrefType - The type of the link. If [LINK_TYPE_DITA_TOPIC](#LINK_TYPE_DITA_TOPIC), the user wants to insert a reference to a DITA resource (Insert Cross Reference action). If [LINK_TYPE_NON_DITA_RESOURCE](#LINK_TYPE_NON_DITA_RESOURCE), wants to a reference to an external non-dita resource (Web Link action or File Reference action). Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) Since: 21
### rewriteKeyref

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rewriteKeyref([LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> urlKeyScopesMapping, [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.dita.reference.keyref.KeyInfo> keys, [AuthorNode](../extensions/api/node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref)

Rewrite a keyref looking also at key scopes..
  Parameters: urlKeyScopesMapping - Global URL to key scopes mapping. keys - Map of keys. contextNode - The context node. keyref - The original keyref. Returns: The rewritten reference.
### getURLKeyScopeContexts

public static [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> getURLKeyScopeContexts([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

Get the URL to key scopes context for the default keys manager.
  Parameters: originatorURL - The originator URL. Returns: the URL to key scopes context mapping for the default keys manager.
### editTopicref

public static void editTopicref([AuthorElement](../extensions/api/node/AuthorElement.md)[] topicrefNodes, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)

Edits one or more topicref elements inside a specialized dialog.
  Parameters: topicrefNodes - The topicref elements. authorAccess - Author access.
### getDitaReferenceTargets

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DitaReferenceTargetDescriptor](DitaReferenceTargetDescriptor.md)> getDitaReferenceTargets([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetURL)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Returns the DITA reference targets in the given topic.
  Parameters: authorAccess - The author access of the currently opened document. targetURL - The URL of the topic. Returns: the DITA reference targets in the given topic. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If an error occured while reading the URL. Since: 18.0
### getDitaReferenceTargets

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DitaReferenceTargetDescriptor](DitaReferenceTargetDescriptor.md)> getDitaReferenceTargets([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseUrl, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) topicUrl)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Returns the DITA reference targets in the given topic.
  Parameters: baseUrl - the target URL. topicUrl - the URL of the source topic. Returns: the DITA reference targets in the given topic. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) Since: 23.0
### getFormat

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFormat([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, boolean fillFormatAttr)
 Deprecated.
Use [getFormatForLinkCreatedFromGUI(String, String, boolean)](#getFormatForLinkCreatedFromGUI(java.lang.String,java.lang.String,boolean))

Get the format for the specified resource.
  Parameters: hrefValue - The HREF of the resource. formatValue - The default format value. fillFormatAttr - true if the attribute should be filled when serializing. Returns: The format for the resource.
### getFormatForLinkCreatedFromGUI

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFormatForLinkCreatedFromGUI([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) formatValue, boolean fillFormatAttr)

Get the format for the specified resource.
  Parameters: hrefValue - The HREF of the resource. formatValue - The default format value. fillFormatAttr - true if the attribute should be filled when serializing. Returns: The format for the resource.
### checkValidKeyName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) checkValidKeyName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyName)

Check if a keyref has a valid key name.
  Parameters: keyName - The key name. Returns: an error message if the key name is not valid or null if the key name is valid.
### getHrefInformation

public static [HrefInfo](HrefInfo.md) getHrefInformation([AuthorNode](../extensions/api/node/AuthorNode.md) node)

Get the reference information (by analizing attributes like keyref, href, mapref, ...) of a node.
  Parameters: node - The author node to get the reference information for. Returns: The information about what the given node references. Since: 18.1
### getHrefInformation

public static [HrefInfo](HrefInfo.md) getHrefInformation([KeysManagerBase](KeysManagerBase.md) keyManager, [AuthorNode](../extensions/api/node/AuthorNode.md) node)

Get the reference information (by analizing attributes like keyref, href, mapref, ...) of a node.
  Parameters: keyManager - The key manager to use to resolve keys. node - The author node to get the reference information for. Returns: The information about what the given node references. Since: 22
### exportDITAMap

public static void exportDITAMap([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) ditamapURL, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) exportDirectory, boolean exportAsZip, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) zipFileName, [ExportProgressUpdater](mapeditor/actions/export/helper/ExportProgressUpdater.md) progressUpdater)

Export DITA Map as zip.
  Parameters: ditamapURL - The DITA Map URL. exportDirectory - The export directory. exportAsZip - true to export as ZIP zipFileName - Zip file name. progressUpdater - The progress updater. Since: 18.1
### attachKeyScopeInformation

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) attachKeyScopeInformation([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextMapURL)
 Deprecated.
Attach key scope information to the target URL.
  Parameters: targetURL - The URL which needs to be opened, referenced via a keyref. keyref - The fully qualified keyref. contextMapURL - The URL of the context map. Since: 19
### attachKeyScopeInformation

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) attachKeyScopeInformation([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextMapURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) originalKeyName)

Attach key scope information to the target URL.
  Parameters: targetURL - The URL which needs to be opened, referenced via a keyref. keyref - The fully qualified keyref. contextMapURL - The URL of the context map. originalKeyName - The original key name without key scopes. Returns: The URL with key scope information attached, so that we know from what key scope the URL was opened. Since: 25.1
### attachKeyScopeInformation

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) attachKeyScopeInformation([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetURL, [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextMapURL)

Attach key scope information to the target URL.
  Parameters: targetURL - The URL which needs to be opened, referenced via a keyref. context - The key scope context.  As an example, for a DITA map looking like this:
```
<map><topicref keyscope="a b c"><topicref keyscope="d e f"/></topicref></map>
```
the stack consists of two sets, the first containing [a, b, c] and the second containing [d, e, f]. contextMapURL - The URL of the context map. Returns: The URL with key scope information attached, so that we know from what key scope the URL was opened. Since: 19
### computeVariableKeyrefElementName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeVariableKeyrefElementName([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)

Compute the elements name.
  Parameters: authorAccess - The author access. Returns: Returns the name of an element, that allows
### computeVariableKeyrefElementName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeVariableKeyrefElementName([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, boolean preferImageElement)

Compute the elements name.
  Parameters: authorAccess - The author access. preferImageElement - true if an image should be inserted. Returns: Returns the name of an element, that allows
### computeKeyScopeStack

public static [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> computeKeyScopeStack([AuthorNode](../extensions/api/node/AuthorNode.md) contextNode, [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> urlKeyScopesMapping)

Compute the entire key scope stack.
  Parameters: contextNode - The context node. urlKeyScopesMapping - The URL to key scopes mapping. Returns: the entire key scope stack. Since: 19
### computeKeyScopeStack

public static [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> computeKeyScopeStack([AuthorNode](../extensions/api/node/AuthorNode.md) contextNode, [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> urlKeyScopesMapping, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorNode](../extensions/api/node/AuthorNode.md),[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> stackCache)

Compute the entire key scope stack.
  Parameters: contextNode - The context node. urlKeyScopesMapping - The URL to key scopes mapping. stackCache - Key scopes stack cache. Can be null. Returns: the entire key scope stack. Since: 23
### getKeyForUrl

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getKeyForUrl([KeysManagerBase](KeysManagerBase.md) keyManager, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

Get the key corresponding to the given URL.
  Parameters: keyManager - The key manager url - The URL for which the search for a key is performed. editorLocation - The URL which is edited. Returns: The name of the corresponding key, if existing, or null. Since: 21
### getKeyForUrl

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getKeyForUrl([KeysManagerBase](KeysManagerBase.md) keyManager, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation, [AuthorNode](../extensions/api/node/AuthorNode.md) contextNode)

Get the key corresponding to the given URL.
  Parameters: keyManager - The key manager url - The URL for which the search for a key is performed. editorLocation - The URL which is edited. contextNode - The context node. Can be null Returns: The name of the corresponding key, if existing, or null. Since: 24
### getKeyForUrl

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getKeyForUrl([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

Get the key corresponding to the given URL.
  Parameters: url - The URL for which the search for a key is performed. editorLocation - The URL which is edited. Returns: The name of the corresponding key, if existing, or null.
### getKeyRefValueForUrl

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getKeyRefValueForUrl([KeysManagerBase](KeysManagerBase.md) keysManager, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) referenceUrl, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

Get the key reference corresponding to the given URL.
  Parameters: referenceUrl - The URL for which the search for a key is performed. editorLocation - The URL which is edited. keysManager - The context keys manager. Returns: The name of the corresponding key, if existing, or null. Since: 21
### checkConsecutiveInsertionWarning

protected static int checkConsecutiveInsertionWarning(int previousOperationOffset, int selectionStart, int selectionEnd, ro.sync.ecss.dita.reference.ReferenceInfo previousReferenceInfo, ro.sync.ecss.dita.reference.ReferenceInfo currentReferenceInfo)

Show a warning message when consecutive insertion of the same references are performed.
  Parameters: previousOperationOffset - The previous operation offset, usually where the caret is positioned. selectionStart - The current selection start. selectionEnd - The current selection end. previousReferenceInfo - The previous inserted reference. currentReferenceInfo - The current inserted reference. !!! OBS: Do not delete. Internal API. !!!
### isKeyReferenceToImage

public static boolean isKeyReferenceToImage(ro.sync.ecss.dita.reference.keyref.KeyInfo key)

Checks if the current key is a reference to an image.
  Parameters: key - Current key to check. Returns: true if we should treat the key as a reference to an image.
### isGenericMediaContent

public static boolean isGenericMediaContent(ro.sync.ecss.dita.reference.keyref.KeyInfo selectedKey)

Checks if the selected key refers resources that can be wrapped in a media object.s
  Parameters: selectedKey - Current key to check. Returns: true if the current key has a reference to content that can be embedded in a media object.
### detectMediaObjectOutputclass

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) detectMediaObjectOutputclass(ro.sync.ecss.dita.reference.keyref.KeyInfo key)

Detects the output class of a key.
  Parameters: key - The key info. Returns: the output class that should be used when the key is inserted as a media object.
### isReferenceToDITAResource

public static boolean isReferenceToDITAResource([AuthorNode](../extensions/api/node/AuthorNode.md) node, ro.sync.ecss.dita.reference.keyref.KeyInfo keyInfo)

Check if this reference points to a DITA topic, map or variable text.
  Parameters: node - The node. keyInfo - The referenced key definition, can be null Returns: true if this reference points to a DITA topic, map or variable text. Since: 21
### isReferenceToDITACompatibleResource

public static boolean isReferenceToDITACompatibleResource([AuthorNode](../extensions/api/node/AuthorNode.md) node, ro.sync.ecss.dita.reference.keyref.KeyInfo keyInfo)

Check if this reference points to a DITA compatible resource (that can be converted to DITA using dynamic converter DITA-OT plugin).
  Parameters: node - The node. keyInfo - The referenced key definition, can be null Returns: true if this reference points to a DITA topic, map or variable text. Since: 25
### getConverterFormatForDITACompatibleResource

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getConverterFormatForDITACompatibleResource([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourceExtension)

Get the converter format that corresponds with the given file extension of the DITA Compatible resource
  Parameters: resourceExtension - The file extension. Returns: The converter format, or null when resource is not DITA-compatible or it's DITA. Since: 25
### isDITACompatileFormat

public static boolean isDITACompatileFormat([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) format)

Check if the given format is compatible to be converted to DITA XML.
  Parameters: format - The format to check. Returns: true when the format is compatible with DITA XML. Since: 28
### convertDitaCompatibleResource

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) convertDitaCompatibleResource([Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) toConvert, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) format)throws ro.sync.exml.editor.xmleditor.ErrorListException

Get the DITA-translated content for the given compatible resource
  Parameters: toConvert - The content to convert. systemId - The system id of the content. format - The compatible resource conversion format. Returns: The DITA content. Throws: ro.sync.exml.editor.xmleditor.ErrorListException - if something goes wrong. Since: 25
### isKeyDefToDITAResource

public static boolean isKeyDefToDITAResource(ro.sync.ecss.dita.reference.keyref.KeyInfo keyInfo)

Check if this key definition points to a DITA topic, map or variable text.
  Parameters: keyInfo - The key info. Returns: true if this key definition points to a DITA topic, map or variable text. Since: 21
### annotateAttributes

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../contentcompletion/xml/CIAttribute.md)> annotateAttributes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../contentcompletion/xml/CIAttribute.md)> attributes)
 Deprecated.
This method does not do anything anynmore, the attribute annotations are gathered from the framework folder.

Annotate a list of attributes.
  Parameters: attributes - The attributes list. Returns: The list of attributes with annotations.
### getFragWithMostSuitableTopicrefs

public static [AuthorDocumentFragment](../extensions/api/node/AuthorDocumentFragment.md) getFragWithMostSuitableTopicrefs([AuthorDocumentController](../extensions/api/AuthorDocumentController.md) controller, [AuthorDocumentFragment](../extensions/api/node/AuthorDocumentFragment.md) frag, int insertOffset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

When moving/copying topic references, maybe they are not allowed at the new position. Try with other topic reference elements.
  Parameters: controller - Document controller frag - The fragment to move insertOffset - The offset position Returns: the created fragment Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### getFragWithMostSuitableTopicrefs

public static [AuthorDocumentFragment](../extensions/api/node/AuthorDocumentFragment.md) getFragWithMostSuitableTopicrefs([AuthorDocumentController](../extensions/api/AuthorDocumentController.md) controller, [AuthorNode](../extensions/api/node/AuthorNode.md) selectedElem, int insertOffset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

When moving/copying topic references, maybe they are not allowed at the new position. Try with other topic reference elements.
  Parameters: controller - document controller selectedElem - the node to move insertOffset - the offset position Returns: the created fragment Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### findSimilarTopics

public static void findSimilarTopics([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)

Find similar topics based on words found in title, shortdesc, keyword, and indexterm elements.
  Parameters: authorAccess - The author access.
### getRelatedLinksFromReltable

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[RelLink](reference/reltable/RelLink.md)> getRelatedLinksFromReltable([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

Get the list of related links from all the relationship tables defined in the DITA Maps.
  Parameters: originatorURL - The topic for which we are searching for outgoing links. Returns: The list of related links from all the relationship tables defined in the DITA Maps. Since: 22
### proposeFolderUrlForChildTopicref

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) proposeFolderUrlForChildTopicref([AuthorElement](../extensions/api/node/AuthorElement.md) parent)

Propose a folder URL where to save a new topicref that is added in a DITA Map as a child of the given node.
  Parameters: parent - The parent node in the DITA Map of the new topicref element. Returns: the folder URL where this topicref should be saved. Since: 25.0
### detectInsertionType

public static [DITAImposedReferenceType](DITAImposedReferenceType.md) detectInsertionType([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Looks at the provided URL and detects if the referred resource should be inserted as a specific XML element.
  Parameters: url - The url. Returns: the type the resource should be inserted. Since: 25.0
### computeQualifiedKeyNames

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> computeQualifiedKeyNames([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyToken, [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> keyScopeStack)

Compute key names qualified with key scope stack prefix.
  Parameters: keyToken - The key token. keyScopeStack - The current key scope stack. Returns: key names qualified with key scope stack prefix. Since: 25.1
### preferAddingKeyrefToAlreadyReferencedResource

public static boolean preferAddingKeyrefToAlreadyReferencedResource([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorURL)

Check if a keyref is preferred to be added when inserting a resource (that is already referred) in the editor .
  Parameters: editorURL - The URL location of the editor in which an already referenced resource needs to be inserted Returns: true if a keyref should be added to the resource that needs to be inserted Since: 25.1
### showNewFileDialog

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) showNewFileDialog([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) proposedTitle)

Shows the New File wizard to allow creating new documents.
  Parameters: authorAccess - The author access of the current opened document in Author page. proposedTitle - The title that will be presented in the New Document wizard. If null no proposal will be presented. Returns: the URL of the newly created document or null. Since: 26.0
### showKeysAndReusableComponents

public static void showKeysAndReusableComponents([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, boolean showKeys, boolean showComps)

Show a content completion window with keys and components. Implemented only in the Oxygen desktop application.
  Parameters: authorAccess - The author access showKeys - true to show keys. showComps - true to show components Since: 26.1
### setExtraMainFileURLs

public static void setExtraMainFileURLs([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> mainFileURLs)

Set extra main file URLs
  Parameters: mainFileURLs - Main file URLs Since: 28.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
