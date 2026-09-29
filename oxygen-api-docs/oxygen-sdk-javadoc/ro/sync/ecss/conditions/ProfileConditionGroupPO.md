Package [ro.sync.ecss.conditions](package-summary.md)

# Class ProfileConditionGroupPO

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.conditions.ProfileConditionValuePO](ProfileConditionValuePO.md)
        * ro.sync.ecss.conditions.ProfileConditionGroupPO
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[ProfileConditionValuePO](ProfileConditionValuePO.md)>, [PersistentObject](../../options/PersistentObject.md)   @API(type=EXTENDABLE, src=PRIVATE) public class ProfileConditionGroupPO extends [ProfileConditionValuePO](ProfileConditionValuePO.md)
Profile condition group representation.
  See Also:
* [Serialized Form](../../../../serialized-form.md#ro.sync.ecss.conditions.ProfileConditionGroupPO)

## Constructor Summary
 Constructors
Constructor

Description
 [ProfileConditionGroupPO](#%3Cinit%3E())()
Default constructor.
  [ProfileConditionGroupPO](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) groupAttribute, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [compareTo](#compareTo(ro.sync.ecss.conditions.ProfileConditionValuePO))([ProfileConditionValuePO](ProfileConditionValuePO.md) other)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getComposeValue](#getComposeValue())()
Gets the composed value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getGroupAttribute](#getGroupAttribute())()

 void [setGroupAttribute](#setGroupAttribute(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) groupAttribute)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class ro.sync.ecss.conditions.[ProfileConditionValuePO](ProfileConditionValuePO.md)
 [checkValid](ProfileConditionValuePO.md#checkValid()), [clone](ProfileConditionValuePO.md#clone()), [getDescription](ProfileConditionValuePO.md#getDescription()), [getLevel](ProfileConditionValuePO.md#getLevel()), [getNotPersistentFieldNames](ProfileConditionValuePO.md#getNotPersistentFieldNames()), [getRenderName](ProfileConditionValuePO.md#getRenderName()), [getValue](ProfileConditionValuePO.md#getValue()), [getValueDisplayLabel](ProfileConditionValuePO.md#getValueDisplayLabel()), [setDescription](ProfileConditionValuePO.md#setDescription(java.lang.String)), [setLevel](ProfileConditionValuePO.md#setLevel(int)), [setRenderName](ProfileConditionValuePO.md#setRenderName(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ProfileConditionGroupPO

public ProfileConditionGroupPO()

Default constructor.

### ProfileConditionGroupPO

public ProfileConditionGroupPO([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) groupAttribute, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description)

Constructor.
  Parameters: groupAttribute - The group attribute. value - The group value. description - Condition group description.
## Method Details

### compareTo

public int compareTo([ProfileConditionValuePO](ProfileConditionValuePO.md) other)
  Specified by: [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html#compareTo(T)) in interface [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[ProfileConditionValuePO](ProfileConditionValuePO.md)> Overrides: [compareTo](ProfileConditionValuePO.md#compareTo(ro.sync.ecss.conditions.ProfileConditionValuePO)) in class [ProfileConditionValuePO](ProfileConditionValuePO.md) See Also:
        * [ProfileConditionValuePO.compareTo(ro.sync.ecss.conditions.ProfileConditionValuePO)](ProfileConditionValuePO.md#compareTo(ro.sync.ecss.conditions.ProfileConditionValuePO))

### getGroupAttribute

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getGroupAttribute()
  Returns: The group attribute.
### setGroupAttribute

public void setGroupAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) groupAttribute)
  Parameters: groupAttribute - The group attribute to be set.
### getComposeValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getComposeValue()
 Description copied from class: [ProfileConditionValuePO](ProfileConditionValuePO.md#getComposeValue())
Gets the composed value. If this value is part of a group, for example the value 'db1' from 'database(db1 db2)' then the composed value is 'database(db1)'.
  Overrides: [getComposeValue](ProfileConditionValuePO.md#getComposeValue()) in class [ProfileConditionValuePO](ProfileConditionValuePO.md) Returns: The composed value. See Also:
        * [ProfileConditionValuePO.getComposeValue()](ProfileConditionValuePO.md#getComposeValue())

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](ProfileConditionValuePO.md#toString()) in class [ProfileConditionValuePO](ProfileConditionValuePO.md) See Also:
        * [ProfileConditionValuePO.toString()](ProfileConditionValuePO.md#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
