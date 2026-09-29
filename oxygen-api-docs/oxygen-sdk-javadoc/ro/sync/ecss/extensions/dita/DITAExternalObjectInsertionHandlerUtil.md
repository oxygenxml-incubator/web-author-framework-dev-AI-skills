Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DITAExternalObjectInsertionHandlerUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.DITAExternalObjectInsertionHandlerUtil
   @API(type=INTERNAL, src=PUBLIC) public final class DITAExternalObjectInsertionHandlerUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Utility class for the DITA and DITA Map external object insertion handlers.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [clearInternalQueryParamsFromExtractedRefAttrVal](#clearInternalQueryParamsFromExtractedRefAttrVal(java.net.URL,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) base, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) refAttrValue)
Removes internal query from a relative URL.
  static ro.sync.ecss.dita.reference.keyref.KeyInfo [detectKeyInfo](#detectKeyInfo(java.net.URL,java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) urlToDrop, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
Extracts the KeyInfo (can be a fully qualified KeyInfo) from current URL and returns the appropriate key (can be the relative key).
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getMediaReferenceAttributeNameAndValue](#getMediaReferenceAttributeNameAndValue(ro.sync.ecss.dita.ContextKeyManagerProvider,java.net.URL,java.net.URL,java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode))([ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) keysManagerProvider, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) base, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [AuthorNode](../api/node/AuthorNode.md) contextNode)
Get the reference attribute name (href / keyref or data / datakeyref) and value.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getReferenceAttributeNameAndValue](#getReferenceAttributeNameAndValue(ro.sync.ecss.dita.ContextKeyManagerProvider,ro.sync.ecss.extensions.api.AuthorAccess,java.net.URL,java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode))([ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) keysManagerProvider, [AuthorAccess](../api/AuthorAccess.md) authorAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) base, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [AuthorNode](../api/node/AuthorNode.md) contextNode)
Get the reference attribute name (href or keyref) and value.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getReferenceAttributeNameAndValueInternal](#getReferenceAttributeNameAndValueInternal(ro.sync.ecss.dita.ContextKeyManagerProvider,java.net.URL,java.net.URL,java.net.URL,ro.sync.ecss.extensions.api.node.AuthorNode,boolean))([ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) keysManagerProvider, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) base, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [AuthorNode](../api/node/AuthorNode.md) contextNode, boolean isMediaElement)
Get the reference attribute name (href / keyref or data / datakeyref) and value.
  static void [insertContentReference](#insertContentReference(ro.sync.ecss.dita.ContextKeyManagerProvider,ro.sync.ecss.extensions.api.AuthorAccess,java.net.URL))([ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) keysManagerProvider, [AuthorAccess](../api/AuthorAccess.md) authorAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Inserts a content reference to the given URL.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### getReferenceAttributeNameAndValue

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getReferenceAttributeNameAndValue([ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) keysManagerProvider, [AuthorAccess](../api/AuthorAccess.md) authorAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) base, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [AuthorNode](../api/node/AuthorNode.md) contextNode)

Get the reference attribute name (href or keyref) and value.
  Parameters: keysManagerProvider - The keys manager provider. authorAccess - The Author access. base - The base URL. url - The current URL. contextNode - Context node Returns: An array of strings, containing the attribute name and the value.
### getMediaReferenceAttributeNameAndValue

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getMediaReferenceAttributeNameAndValue([ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) keysManagerProvider, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) base, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [AuthorNode](../api/node/AuthorNode.md) contextNode)

Get the reference attribute name (href / keyref or data / datakeyref) and value.
  Parameters: keysManagerProvider - The keys manager provider. editorLocation - The URL location of the current editor. base - The base URL. url - The current URL. contextNode - Context node, can be null Returns: An array of strings, containing the attribute name and the value.
### getReferenceAttributeNameAndValueInternal

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getReferenceAttributeNameAndValueInternal([ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) keysManagerProvider, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) base, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [AuthorNode](../api/node/AuthorNode.md) contextNode, boolean isMediaElement)

Get the reference attribute name (href / keyref or data / datakeyref) and value.
  Parameters: keysManagerProvider - The keys manager provider. editorLocation - The URL location of the current editor. base - The base URL. url - The current URL. contextNode - The context node, can be null isMediaElement - true to insert media objects. Returns: An array of strings, containing the attribute name and the value.
### insertContentReference

public static void insertContentReference([ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) keysManagerProvider, [AuthorAccess](../api/AuthorAccess.md) authorAccess, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)throws [AuthorOperationException](../api/AuthorOperationException.md)

Inserts a content reference to the given URL.
  Parameters: keysManagerProvider - The keys manager provider. authorAccess - Access to the current document. url - Target for the conref. Throws: [AuthorOperationException](../api/AuthorOperationException.md) - If it fails.
### clearInternalQueryParamsFromExtractedRefAttrVal

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) clearInternalQueryParamsFromExtractedRefAttrVal([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) base, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) refAttrValue)

Removes internal query from a relative URL.
  Parameters: base - The original base URL of the relative value. refAttrValue - The relative value. Returns: The relative value without internal query params or original value if no cleanup should be done.
### detectKeyInfo

public static ro.sync.ecss.dita.reference.keyref.KeyInfo detectKeyInfo([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) urlToDrop, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

Extracts the KeyInfo (can be a fully qualified KeyInfo) from current URL and returns the appropriate key (can be the relative key).
  Parameters: urlToDrop - The dropped URL originatorURL - The URL for which the keys are requested. Returns: The key extracted from URL (fully qualified or relative, context aware key) or null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
