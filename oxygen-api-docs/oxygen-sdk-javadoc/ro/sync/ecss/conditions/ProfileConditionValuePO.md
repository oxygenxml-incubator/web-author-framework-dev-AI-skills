Package [ro.sync.ecss.conditions](package-summary.md)

# Class ProfileConditionValuePO

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.conditions.ProfileConditionValuePO
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[ProfileConditionValuePO](ProfileConditionValuePO.md)>, [PersistentObject](../../options/PersistentObject.md)   Direct Known Subclasses: [ProfileConditionGroupPO](ProfileConditionGroupPO.md)   @API(type=EXTENDABLE, src=PRIVATE) public class ProfileConditionValuePO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [PersistentObject](../../options/PersistentObject.md), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[ProfileConditionValuePO](ProfileConditionValuePO.md)>
Profile condition attribute value representation.
  See Also:
* [Serialized Form](../../../../serialized-form.md#ro.sync.ecss.conditions.ProfileConditionValuePO)

## Constructor Summary
 Constructors
Constructor

Description
 [ProfileConditionValuePO](#%3Cinit%3E())()
Constructor.
  [ProfileConditionValuePO](#%3Cinit%3E(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [checkValid](#checkValid())()
Check if object is valid to be used.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()
Forces all the persistent objects to be cloneable.
  int [compareTo](#compareTo(ro.sync.ecss.conditions.ProfileConditionValuePO))([ProfileConditionValuePO](ProfileConditionValuePO.md) other)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getComposeValue](#getComposeValue())()
Gets the composed value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 int [getLevel](#getLevel())()
Get the level in the hierarchy of Subject Scheme values this condition is located on.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getNotPersistentFieldNames](#getNotPersistentFieldNames())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRenderName](#getRenderName())()
Get the render name for the profiling condition.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getValue](#getValue())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getValueDisplayLabel](#getValueDisplayLabel())()
Get the display label for the attribute's value.
  void [setDescription](#setDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description)

 void [setLevel](#setLevel(int))(int level)
Set the level in the hierarchy of Subject Scheme values this condition is located on.
  void [setRenderName](#setRenderName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) renderName)
Set the render name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ProfileConditionValuePO

public ProfileConditionValuePO()

Constructor.

### ProfileConditionValuePO

public ProfileConditionValuePO([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description)

Constructor.
  Parameters: value - Condition value. description - Condition value description.
## Method Details

### getValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getValue()
  Returns: Returns the value.
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: Returns the description.
### setDescription

public void setDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description)
  Parameters: description - The description to set.
### checkValid

public void checkValid() throws [InvalidPersistentObjException](../../options/InvalidPersistentObjException.md)
 Description copied from interface: [PersistentObject](../../options/PersistentObject.md#checkValid())
Check if object is valid to be used. Method is called after it is deserialized from options. If not then throw an InvalidPersistentObjException exception.
  Specified by: [checkValid](../../options/PersistentObject.md#checkValid()) in interface [PersistentObject](../../options/PersistentObject.md) Throws: [InvalidPersistentObjException](../../options/InvalidPersistentObjException.md) - Thrown when instance is not valid. See Also:
        * [PersistentObject.checkValid()](../../options/PersistentObject.md#checkValid())

### getNotPersistentFieldNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getNotPersistentFieldNames()
  Specified by: [getNotPersistentFieldNames](../../options/PersistentObject.md#getNotPersistentFieldNames()) in interface [PersistentObject](../../options/PersistentObject.md) Returns: The names of the field from this object which should not be serialized. See Also:
        * [PersistentObject.getNotPersistentFieldNames()](../../options/PersistentObject.md#getNotPersistentFieldNames())

### clone

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone()
 Description copied from interface: [PersistentObject](../../options/PersistentObject.md#clone())
Forces all the persistent objects to be cloneable.
  Specified by: [clone](../../options/PersistentObject.md#clone()) in interface [PersistentObject](../../options/PersistentObject.md) Overrides: [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Returns: A clone of this object. The clone and the original are disjunct. They share only immutable objects, like Strings, Integers, etc. See Also:
        * [Object.clone()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone())

### compareTo

public int compareTo([ProfileConditionValuePO](ProfileConditionValuePO.md) other)
  Specified by: [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html#compareTo(T)) in interface [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[ProfileConditionValuePO](ProfileConditionValuePO.md)> See Also:
        * [Comparable.compareTo(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html#compareTo(T))

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### setLevel

public void setLevel(int level)

Set the level in the hierarchy of Subject Scheme values this condition is located on.
  Parameters: level - the level in the hierarchy of Subject Scheme values this condition is located on.
### getLevel

public int getLevel()

Get the level in the hierarchy of Subject Scheme values this condition is located on.
  Returns: Returns the level in the hierarchy of Subject Scheme values this condition is located on.
### getComposeValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getComposeValue()

Gets the composed value. If this value is part of a group, for example the value 'db1' from 'database(db1 db2)' then the composed value is 'database(db1)'.
  Returns: The composed value.
### getRenderName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRenderName()

Get the render name for the profiling condition. May be null.
  Returns: Returns the render name.
### setRenderName

public void setRenderName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) renderName)

Set the render name.
  Parameters: renderName - The render name to be set in the dialog used to edit the profile condition value.
### getValueDisplayLabel

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getValueDisplayLabel()

Get the display label for the attribute's value.
  Returns: the display label if the render name is not null, empty otherwise.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
