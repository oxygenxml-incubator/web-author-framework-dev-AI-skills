Package [ro.sync.exml.workspace.api.editor.page.ditamap.keys](package-summary.md)

# Class KeyDefinitionManager

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionManager
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class KeyDefinitionManager extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Provides information about all key definitions which are a context for all opened topics. This is implemented on the API side.
  Since: 14
## Constructor Summary
 Constructors
Constructor

Description
 [KeyDefinitionManager](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[KeyDefinitionInfo](KeyDefinitionInfo.md)> [getContextKeyDefinitions](#getContextKeyDefinitions())()  Deprecated.
For performance reasons, consider implementing the {[getContextKeyDefinitionsMap(URL)](#getContextKeyDefinitionsMap(java.net.URL)) method instead.
   [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[KeyDefinitionInfo](KeyDefinitionInfo.md)> [getContextKeyDefinitions](#getContextKeyDefinitions(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)  Deprecated.
For performance reasons, consider implementing the {[getContextKeyDefinitionsMap(URL)](#getContextKeyDefinitionsMap(java.net.URL)) method instead.
   [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[KeyDefinitionInfo](KeyDefinitionInfo.md)> [getContextKeyDefinitionsMap](#getContextKeyDefinitionsMap(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
Get the key definitions which will be used as a context for solving all conkeyref and keyref references in the opened DITA topics.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()
Gets a short description used to explain this resolving to the user.
  [LinkedHashSet](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashSet.html)<[EnumerationDefInfo](EnumerationDefInfo.md)> [getEnumerationDefinitions](#getEnumerationDefinitions(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
Get the list of enumeration defs (detected in a subject scheme referenced in the context DITA Map).
  [KeyDefinitionInfo](KeyDefinitionInfo.md) [getKeyDefinitionForKeyName](#getKeyDefinitionForKeyName(java.net.URL,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyName)
Get the key definition corresponding to the given key name.
  [KeyDefinitionInfo](KeyDefinitionInfo.md) [getKeyDefinitionForTarget](#getKeyDefinitionForTarget(java.net.URL,java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetURL)
Get the key definition corresponding to the target URL.
  [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> [getURLKeyScopeContexts](#getURLKeyScopeContexts(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
Retrieve a map between an URL and all the DITA 1.3 key scope contexts in the map where it appears.
  boolean [isPassKeyTargetReferencesThroughXMLCatalogMappings](#isPassKeyTargetReferencesThroughXMLCatalogMappings())()
Return true for the reference URL of each KeyDefinitionInfo to be passed through the application's XML Catalog URI mappings.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### KeyDefinitionManager

public KeyDefinitionManager()

## Method Details

### getContextKeyDefinitions

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[KeyDefinitionInfo](KeyDefinitionInfo.md)> getContextKeyDefinitions()
 Deprecated.
For performance reasons, consider implementing the {[getContextKeyDefinitionsMap(URL)](#getContextKeyDefinitionsMap(java.net.URL)) method instead.

Get the key definitions which will be used as a context for solving all conkeyref and keyref references in the opened DITA topics. This method might be asked quite often so it could be cached on the implementor's side.
  Returns: the key definitions which will be used as a context for solving all conkeyref and keyref references in the opened DITA topics.
### getContextKeyDefinitions

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[KeyDefinitionInfo](KeyDefinitionInfo.md)> getContextKeyDefinitions([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)
 Deprecated.
For performance reasons, consider implementing the {[getContextKeyDefinitionsMap(URL)](#getContextKeyDefinitionsMap(java.net.URL)) method instead.

Get the key definitions which will be used as a context for solving all conkeyref and keyref references in the opened DITA topics. This method might be asked quite often so it could be cached on the implementor's side.
  Parameters: originatorURL - The DITA topic or map for which the keys are requested to resolve something (either a clicked keyref or a conkeyref). Returns: the key definitions which will be used as a context for solving all conkeyref and keyref references in the opened DITA topics. Since: 14.2
### getContextKeyDefinitionsMap

public [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[KeyDefinitionInfo](KeyDefinitionInfo.md)> getContextKeyDefinitionsMap([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

Get the key definitions which will be used as a context for solving all conkeyref and keyref references in the opened DITA topics. This method might be asked quite often so it could be cached on the implementor's side.
  Parameters: originatorURL - The DITA topic or map for which the keys are requested to resolve something (either a clicked keyref or a conkeyref). Returns: the key definitions which will be used as a context for solving all conkeyref and keyref references in the opened DITA topics. Since: 22.1
### getEnumerationDefinitions

public [LinkedHashSet](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashSet.html)<[EnumerationDefInfo](EnumerationDefInfo.md)> getEnumerationDefinitions([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

Get the list of enumeration defs (detected in a subject scheme referenced in the context DITA Map). These are used to control the values allowed for certain attributes. The set can be null. This method might be asked quite often so it could be cached on the implementor's side.
  Parameters: originatorURL - The DITA topic or map for which the keys are requested to resolve something (when editing a keyref attribute or using the "Edit Profiling Attributes" dialog). Returns: the set of enumeration defs (detected in a subject scheme referenced in the context DITA Map). Since: 15
### getURLKeyScopeContexts

public [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>>>> getURLKeyScopeContexts([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL)

Retrieve a map between an URL and all the DITA 1.3 key scope contexts in the map where it appears. A key scope context is a stack of collected key scope values. As a key scope set on a topicref may have multiple values, the stack contains sets of keyscope values.
  Parameters: originatorURL - The context URL. Returns: a map between an URL and all the DITA 1.3 key scope contexts in the map where it appears. Since: 17.1
### getKeyDefinitionForTarget

public [KeyDefinitionInfo](KeyDefinitionInfo.md) getKeyDefinitionForTarget([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) targetURL)

Get the key definition corresponding to the target URL. This method may be asked when Oxygen's "Paste as content key reference" action is used or when dropping URLs in the editing area. If it returns null, Oxygen will ask for all keys using the "getContextKeyDefinitions" method and find the key itself.
  Parameters: originatorURL - The DITA topic or map for which the keys are requested to resolve something (either a clicked keyref or a conkeyref). targetURL - The URL for which we want to know the key which is bound to it. Returns: the key definition corresponding to the target URL Since: 21
### getKeyDefinitionForKeyName

public [KeyDefinitionInfo](KeyDefinitionInfo.md) getKeyDefinitionForKeyName([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) originatorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyName)

Get the key definition corresponding to the given key name. If it returns null, Oxygen will ask for all keys using the "getContextKeyDefinitions" method and find the key itself.
  Parameters: originatorURL - The current DITA topic or map. keyName - The key name for which we request the key definition. Returns: the key definition corresponding to the target URL Since: 21
### isPassKeyTargetReferencesThroughXMLCatalogMappings

public boolean isPassKeyTargetReferencesThroughXMLCatalogMappings()

Return true for the reference URL of each KeyDefinitionInfo to be passed through the application's XML Catalog URI mappings. The default implementation returns true.
  Returns: true to pass key reference URLs through XML Catalog URI mappings. Can be useful to provide additional indirections via the XML catalogs support in Oxygen, but this may induce delays when lots of keys are provided by the API. Since: 21.1
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()

Gets a short description used to explain this resolving to the user.
  Returns: A description used to explain this resolving to the user. Since: 15
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
