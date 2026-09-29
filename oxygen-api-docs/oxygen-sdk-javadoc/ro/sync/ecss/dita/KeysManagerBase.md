Package [ro.sync.ecss.dita](package-summary.md)

# Interface KeysManagerBase
    All Known Implementing Classes: [ContextKeyManager](ContextKeyManager.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public interface KeysManagerBase
Common keys manager methods

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> [getCopyToMapping](#getCopyToMapping(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
Get mappings between URLs referenced with copy-to and actual URL.
  [LinkedHashSet](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashSet.html)<[EnumerationDefInfo](../../exml/workspace/api/editor/page/ditamap/keys/EnumerationDefInfo.md)> [getEnumerationDefs](#getEnumerationDefs(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
Gets all enumeration defs found in the subject scheme mapping starting from the currently opened DITA Map.
  ro.sync.ecss.dita.reference.keyref.KeyInfo [getKeyDefinitionForKeyName](#getKeyDefinitionForKeyName(java.net.URL,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyName)
Get the key definition corresponding to the given key name.
  ro.sync.ecss.dita.reference.keyref.KeyInfo [getKeyDefinitionForTarget](#getKeyDefinitionForTarget(java.net.URL,java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetURL)
Get the key definition corresponding to the target URL.
  [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.dita.reference.keyref.KeyInfo> [getKeys](#getKeys(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
Gets all keys in the currently opened DITA Map.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[RelLink](reference/reltable/RelLink.md)> [getReltableRelationships](#getReltableRelationships(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
Get a list with relationships between topics established in the reltable.
  [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> [getURLKeyScopeContexts](#getURLKeyScopeContexts(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
Get mapping between URLs and list of key scope contexts where they appeared in the map.

## Method Details

### getKeys

[LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.dita.reference.keyref.KeyInfo> getKeys([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

Gets all keys in the currently opened DITA Map.
  Parameters: originatorURL - The URL of the topic which needs to resolve keys. Can be null in rare cases when the keys are asked for nodes which part of an AuthorDocumentFragment, in which case usually the callback can be ignored. Returns: All keys found in the currently opened DITA Map.
### getEnumerationDefs

[LinkedHashSet](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashSet.html)<[EnumerationDefInfo](../../exml/workspace/api/editor/page/ditamap/keys/EnumerationDefInfo.md)> getEnumerationDefs([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

Gets all enumeration defs found in the subject scheme mapping starting from the currently opened DITA Map. Can be null.
  Parameters: originatorURL - The URL of the topic which needs to resolve the enumeration defs. Can be null in rare cases when the keys are asked for nodes which part of an AuthorDocumentFragment, case in which usually the callback can be ignored. Returns: All enumeration defs in the currently opened DITA Map.
### getURLKeyScopeContexts

[LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> getURLKeyScopeContexts([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

Get mapping between URLs and list of key scope contexts where they appeared in the map.
  Parameters: originatorURL - The URL of the topic which needs to resolve the enumeration defs. Can be null in rare cases when the keys are asked for nodes which part of an AuthorDocumentFragment, case in which usually the callback can be ignored. Returns: Returns the mapping between URLs and list of key scope contexts where they appeared in the map. Can be null
### getKeyDefinitionForTarget

ro.sync.ecss.dita.reference.keyref.KeyInfo getKeyDefinitionForTarget([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetURL)

Get the key definition corresponding to the target URL. This method may be asked when Oxygen's "Paste as content key reference" action is used. If it returns null, Oxygen will ask for all keys and find the key itself.
  Parameters: originatorURL - The DITA topic or map for which the keys are requested to resolve something (either a clicked keyref or a conkeyref). targetURL - The URL for which we want to know the key which is bound to it. Returns: the key definition corresponding to the target URL
### getKeyDefinitionForKeyName

ro.sync.ecss.dita.reference.keyref.KeyInfo getKeyDefinitionForKeyName([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyName)

Get the key definition corresponding to the given key name. If it returns null, Oxygen will ask for all keys using the "getContextKeyDefinitions" method and find the key itself.
  Parameters: originatorURL - The current DITA topic or map. keyName - The key name for which we request the key definition. Returns: the key definition corresponding to the target URL
### getCopyToMapping

[LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> getCopyToMapping([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

Get mappings between URLs referenced with copy-to and actual URL.
  Parameters: originatorURL - The originator URL. Can be null in rare cases when the keys are asked for nodes which part of an AuthorDocumentFragment, case in which usually the callback can be ignored. Returns: Returns the mappings between URLs referenced with copy-to and actual URL..
### getReltableRelationships

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[RelLink](reference/reltable/RelLink.md)> getReltableRelationships([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

Get a list with relationships between topics established in the reltable.
  Parameters: originatorURL - The originator URL. Returns: a list with relationships between topics established in the reltable.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
