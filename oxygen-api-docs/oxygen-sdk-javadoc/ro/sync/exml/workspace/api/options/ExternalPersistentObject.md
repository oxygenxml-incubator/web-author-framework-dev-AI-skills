Package [ro.sync.exml.workspace.api.options](package-summary.md)

# Interface ExternalPersistentObject
    All Superinterfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), [PersistentObject](../../../../options/PersistentObject.md), [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)   All Known Implementing Classes: [SimpleListOfStringsExternalPersistentObject](SimpleListOfStringsExternalPersistentObject.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface ExternalPersistentObjectextends [PersistentObject](../../../../options/PersistentObject.md)
Marker interface for persistent objects which are implemented in plugins.

The implementation class should mostly contain simple fields (String, Integer, boolean).

If you want to use more complex structures, you can use the "ro.sync.options.SerializableList" and "ro.sync.options.SerializableLinkedHashMap" objects.

A sample implementation can be found in "ro.sync.exml.workspace.api.options.SimpleListOfStringsExternalPersistentObject".

The object can be serialized to XML using the API "ro.sync.exml.workspace.api.options.GlobalOptionsStorage.serializePersistentObject(Object)".

It can also be de-serialized using the "ro.sync.exml.workspace.api.options.GlobalOptionsStorage.deserializePersistentObject(String)" API.
  Since: 22
## Method Summary

### Methods inherited from interface ro.sync.options.[PersistentObject](../../../../options/PersistentObject.md)
 [checkValid](../../../../options/PersistentObject.md#checkValid()), [clone](../../../../options/PersistentObject.md#clone()), [getNotPersistentFieldNames](../../../../options/PersistentObject.md#getNotPersistentFieldNames())
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
