Package [ro.sync.ecss.conditions](package-summary.md)

# Class ProfileConditionInfoPO

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.conditions.ProfileConditionInfoPO
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), [PersistentObject](../../options/PersistentObject.md)   @API(type=EXTENDABLE, src=PRIVATE) public class ProfileConditionInfoPO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [PersistentObject](../../options/PersistentObject.md)
Contains information about a condition processing attribute name and possible values.
  See Also:
* [Serialized Form](../../../../serialized-form.md#ro.sync.ecss.conditions.ProfileConditionInfoPO)

## Constructor Summary
 Constructors
Constructor

Description
 [ProfileConditionInfoPO](#%3Cinit%3E())()
Constructor.
  [ProfileConditionInfoPO](#%3Cinit%3E(java.lang.String,java.lang.String,boolean,ro.sync.ecss.conditions.ProfileConditionValuePO%5B%5D,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeRenderName, boolean allowsMultipleValues, [ProfileConditionValuePO](ProfileConditionValuePO.md)[] allowedValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) valuesSeparator, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypePattern)
Constructor used only by default values.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [checkValid](#checkValid())()
Check if object is valid to be used.
  [ProfileConditionInfoPO](ProfileConditionInfoPO.md) [clone](#clone())()
Forces all the persistent objects to be cloneable.
  boolean [containsGroup](#containsGroup(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attribute, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Check if a specific group with the given attribute and value is allowed.
  boolean [containsValue](#containsValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Check if a specific value is allowed.
  static [ProfileConditionInfoPO](ProfileConditionInfoPO.md) [createDefaultProfileConditionInfoPO](#createDefaultProfileConditionInfoPO(java.lang.String,java.lang.String,boolean,java.lang.String%5B%5D,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeRenderName, boolean allowsMultipleValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) valuesSeparator, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypePattern)
Creates a default Profile Condition Info.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [ProfileConditionValuePO](ProfileConditionValuePO.md)[] [getAllowedValues](#getAllowedValues())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAllowedValuesDescription](#getAllowedValuesDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeName](#getAttributeName())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeRenderName](#getAttributeRenderName())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentTypePattern](#getDocumentTypePattern())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getNotPersistentFieldNames](#getNotPersistentFieldNames())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRenderValueName](#getRenderValueName(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) groupAttribute, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Get the render name for the given value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getValuesSeparator](#getValuesSeparator())()

 int [hashCode](#hashCode())()

 boolean [isAllowsMultipleValues](#isAllowsMultipleValues())()

 void [setAllowedValues](#setAllowedValues(ro.sync.ecss.conditions.ProfileConditionValuePO%5B%5D,boolean))([ProfileConditionValuePO](ProfileConditionValuePO.md)[] allowedValues, boolean sort)
Set the list of allowed values.
  void [setAllowsMultipleValues](#setAllowsMultipleValues(boolean))(boolean allowsMultipleValues)
true if allows or not multiple values.
  void [setAttributeRenderName](#setAttributeRenderName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeRenderName)
Set the attribute render name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ProfileConditionInfoPO

public ProfileConditionInfoPO()

Constructor.

### ProfileConditionInfoPO

public ProfileConditionInfoPO([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeRenderName, boolean allowsMultipleValues, [ProfileConditionValuePO](ProfileConditionValuePO.md)[] allowedValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) valuesSeparator, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypePattern)

Constructor used only by default values.
  Parameters: attributeName - The conditional attribute name. attributeRenderName - Attribute render name. allowsMultipleValues - True if multiple values are allowed for this attribute allowedValues - Allowed values for this attribute. valuesSeparator - The condition values separator. documentTypePattern - Document type pattern. If specified, the condition will be used only for the document types that match it.
## Method Details

### createDefaultProfileConditionInfoPO

public static [ProfileConditionInfoPO](ProfileConditionInfoPO.md) createDefaultProfileConditionInfoPO([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeRenderName, boolean allowsMultipleValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) valuesSeparator, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypePattern)

Creates a default Profile Condition Info.
  Parameters: attributeName - The conditional attribute name. attributeRenderName - Attribute render name. allowsMultipleValues - True if multiple values are allowed for this attribute allowedValues - Allowed values for this attribute. valuesSeparator - The condition values separator. documentTypePattern - Document type pattern. If specified, the condition will be used only for the document types that match it. Returns: A default Profile Condition Info.
### setAttributeRenderName

public void setAttributeRenderName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeRenderName)

Set the attribute render name.
  Parameters: attributeRenderName - The attribute Render Name.
### getAttributeName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeName()
  Returns: Returns the attribute name.
### getAttributeRenderName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeRenderName()
  Returns: Returns the attributeRenderName.
### isAllowsMultipleValues

public boolean isAllowsMultipleValues()
  Returns: Returns true if multiple values are allowed for this attribute
### getAllowedValues

public [ProfileConditionValuePO](ProfileConditionValuePO.md)[] getAllowedValues()
  Returns: Returns the allowed values for this attribute.
### getValuesSeparator

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getValuesSeparator()
  Returns: Returns the conditional values separator.
### getDocumentTypePattern

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentTypePattern()
  Returns: Returns the document type pattern.  If specified, the condition will be used only for the document types that match it.
### containsValue

public boolean containsValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Check if a specific value is allowed.
  Parameters: value - The value to be checked. Returns: True if the value is allowed
### containsGroup

public boolean containsGroup([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attribute, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Check if a specific group with the given attribute and value is allowed.
  Parameters: attribute - The attribute of the group to be checked. value - The value of the group attribute to be checked. Returns: True if the group is allowed.
### getAllowedValuesDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAllowedValuesDescription()
  Returns: the values composed with the separator
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

public [ProfileConditionInfoPO](ProfileConditionInfoPO.md) clone()
 Description copied from interface: [PersistentObject](../../options/PersistentObject.md#clone())
Forces all the persistent objects to be cloneable.
  Specified by: [clone](../../options/PersistentObject.md#clone()) in interface [PersistentObject](../../options/PersistentObject.md) Overrides: [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Returns: A clone of this object. The clone and the original are disjunct. They share only immutable objects, like Strings, Integers, etc. See Also:
        * [Object.clone()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone())

### setAllowedValues

public void setAllowedValues([ProfileConditionValuePO](ProfileConditionValuePO.md)[] allowedValues, boolean sort)

Set the list of allowed values.
  Parameters: allowedValues - The allowedValues to set. sort - true to sort the allowed values.
### setAllowsMultipleValues

public void setAllowsMultipleValues(boolean allowsMultipleValues)

true if allows or not multiple values.
  Parameters: allowsMultipleValues - true if allows or not multiple values.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### getRenderValueName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRenderValueName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) groupAttribute, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Get the render name for the given value.
  Parameters: groupAttribute - The group attribute name. It can be null if the value is simple. value - The value to search. Returns: The render name for the given value or null if wasn't found a render for value.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
