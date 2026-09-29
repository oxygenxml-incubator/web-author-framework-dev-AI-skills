Package [ro.sync.exml.workspace.api.options](package-summary.md)

# Class SimpleListOfStringsExternalPersistentObject

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.options.SimpleListOfStringsExternalPersistentObject
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), [ExternalPersistentObject](ExternalPersistentObject.md), [PersistentObject](../../../../options/PersistentObject.md)   @API(type=EXTENDABLE, src=PUBLIC) public class SimpleListOfStringsExternalPersistentObject extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ExternalPersistentObject](ExternalPersistentObject.md)
A persistent object which holds a list of strings. Used as an example and for tests.
  See Also:
* [Serialized Form](../../../../../../serialized-form.md#ro.sync.exml.workspace.api.options.SimpleListOfStringsExternalPersistentObject)

## Constructor Summary
 Constructors
Constructor

Description
 [SimpleListOfStringsExternalPersistentObject](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addItem](#addItem(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) item)
Add an item.
  void [checkValid](#checkValid())()
Check if object is valid to be used.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()
Forces all the persistent objects to be cloneable.
  ro.sync.options.SerializableList<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getItems](#getItems())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getNotPersistentFieldNames](#getNotPersistentFieldNames())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SimpleListOfStringsExternalPersistentObject

public SimpleListOfStringsExternalPersistentObject()

## Method Details

### getItems

public ro.sync.options.SerializableList<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getItems()
  Returns: Returns the items list.
### addItem

public void addItem([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) item)

Add an item.
  Parameters: item - The item to add.
### checkValid

public void checkValid() throws [InvalidPersistentObjException](../../../../options/InvalidPersistentObjException.md)
 Description copied from interface: [PersistentObject](../../../../options/PersistentObject.md#checkValid())
Check if object is valid to be used. Method is called after it is deserialized from options. If not then throw an InvalidPersistentObjException exception.
  Specified by: [checkValid](../../../../options/PersistentObject.md#checkValid()) in interface [PersistentObject](../../../../options/PersistentObject.md) Throws: [InvalidPersistentObjException](../../../../options/InvalidPersistentObjException.md) - Thrown when instance is not valid. See Also:
        * [PersistentObject.checkValid()](../../../../options/PersistentObject.md#checkValid())

### getNotPersistentFieldNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getNotPersistentFieldNames()
  Specified by: [getNotPersistentFieldNames](../../../../options/PersistentObject.md#getNotPersistentFieldNames()) in interface [PersistentObject](../../../../options/PersistentObject.md) Returns: The names of the field from this object which should not be serialized. See Also:
        * [PersistentObject.getNotPersistentFieldNames()](../../../../options/PersistentObject.md#getNotPersistentFieldNames())

### clone

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone()
 Description copied from interface: [PersistentObject](../../../../options/PersistentObject.md#clone())
Forces all the persistent objects to be cloneable.
  Specified by: [clone](../../../../options/PersistentObject.md#clone()) in interface [PersistentObject](../../../../options/PersistentObject.md) Overrides: [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Returns: A clone of this object. The clone and the original are disjunct. They share only immutable objects, like Strings, Integers, etc. See Also:
        * [Object.clone()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone())

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
