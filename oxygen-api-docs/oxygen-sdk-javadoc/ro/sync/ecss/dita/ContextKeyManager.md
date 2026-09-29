Package [ro.sync.ecss.dita](package-summary.md)

# Class ContextKeyManager

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.dita.ContextKeyManager
   All Implemented Interfaces: [KeysManagerBase](KeysManagerBase.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public abstract class ContextKeyManager extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [KeysManagerBase](KeysManagerBase.md)
Context aware key manager. One can use the provided factory methods to create a key manager that uses the informations provided by the user to resolve the keys. It is an opaque class that can be passed to various [DITAAccess](DITAAccess.md) methods.
  Since: 15.2
## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [ContextKeyManager](ContextKeyManager.md) [createFromDitaMapUrl](#createFromDitaMapUrl(java.net.URL,ro.sync.ecss.dita.map.checker.ditaval.ConditionProcessor,ro.sync.ecss.dita.map.representation.DITAMapTreeModelCreatedListener))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) ditaMapUrl, ro.sync.ecss.dita.map.checker.ditaval.ConditionProcessor conditionProcessor, ro.sync.ecss.dita.map.representation.DITAMapTreeModelCreatedListener ditaMapTreeModelCreatedListener)
Creates a key manager that uses the DITA map with the given URL to resolve the keys.
  static [ContextKeyManager](ContextKeyManager.md) [createFromKeyDefinitionManager](#createFromKeyDefinitionManager(ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionManager))([KeyDefinitionManager](../../exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManager.md) keyDefinitionManager)
Creates a key manager that uses an user-provided [KeyDefinitionManager](../../exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManager.md)to resolve the keys.
  static [ContextKeyManager](ContextKeyManager.md) [getDefault](#getDefault())()
Returns the default key manager that uses the currently opened DITA map.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.dita.[KeysManagerBase](KeysManagerBase.md)
 [getCopyToMapping](KeysManagerBase.md#getCopyToMapping(java.net.URL)), [getEnumerationDefs](KeysManagerBase.md#getEnumerationDefs(java.net.URL)), [getKeyDefinitionForKeyName](KeysManagerBase.md#getKeyDefinitionForKeyName(java.net.URL,java.lang.String)), [getKeyDefinitionForTarget](KeysManagerBase.md#getKeyDefinitionForTarget(java.net.URL,java.net.URL)), [getKeys](KeysManagerBase.md#getKeys(java.net.URL)), [getReltableRelationships](KeysManagerBase.md#getReltableRelationships(java.net.URL)), [getURLKeyScopeContexts](KeysManagerBase.md#getURLKeyScopeContexts(java.net.URL))
## Method Details

### createFromDitaMapUrl

public static [ContextKeyManager](ContextKeyManager.md) createFromDitaMapUrl([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) ditaMapUrl, ro.sync.ecss.dita.map.checker.ditaval.ConditionProcessor conditionProcessor, ro.sync.ecss.dita.map.representation.DITAMapTreeModelCreatedListener ditaMapTreeModelCreatedListener)

Creates a key manager that uses the DITA map with the given URL to resolve the keys.
  Parameters: ditaMapUrl - The URL of the DITA map. conditionProcessor - A condition processor. ditaMapTreeModelCreatedListener - Listener to be notified when the DITA Map tree model is created. Returns: The key manager.
### createFromKeyDefinitionManager

public static [ContextKeyManager](ContextKeyManager.md) createFromKeyDefinitionManager([KeyDefinitionManager](../../exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManager.md) keyDefinitionManager)

Creates a key manager that uses an user-provided [KeyDefinitionManager](../../exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManager.md)to resolve the keys.
  Parameters: keyDefinitionManager - The key definition manager. Returns: The key manager.
### getDefault

public static [ContextKeyManager](ContextKeyManager.md) getDefault()

Returns the default key manager that uses the currently opened DITA map.
  Returns: The key manager.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
