Package [ro.sync.ecss.conditions](package-summary.md)

# Class ProfileConditionsSetInfoPO

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.conditions.ProfileConditionsSetInfoPO
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), [PersistentObject](../../options/PersistentObject.md)   @API(type=EXTENDABLE, src=PRIVATE) public class ProfileConditionsSetInfoPO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [PersistentObject](../../options/PersistentObject.md)
Contains information about a condition processing attribute name and possible values.
  See Also:
* [Serialized Form](../../../../serialized-form.md#ro.sync.ecss.conditions.ProfileConditionsSetInfoPO)

## Constructor Summary
 Constructors
Constructor

Description
 [ProfileConditionsSetInfoPO](#%3Cinit%3E())()
Constructor.
  [ProfileConditionsSetInfoPO](#%3Cinit%3E(ro.sync.options.SerializableLinkedHashMap,java.lang.String,java.lang.String))(ro.sync.options.SerializableLinkedHashMap<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[]> conditions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypePattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) conditionSetName)
Constructor.
  [ProfileConditionsSetInfoPO](#%3Cinit%3E(ro.sync.options.SerializableLinkedHashMap,java.lang.String,java.lang.String,java.lang.String,boolean))(ro.sync.options.SerializableLinkedHashMap<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[]> conditions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypePattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) conditionSetName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ditavalFile, boolean useDITAVAL)
Constructor.
  [ProfileConditionsSetInfoPO](#%3Cinit%3E(ro.sync.options.SerializableLinkedHashMap,java.lang.String,java.lang.String,java.lang.String,boolean,java.lang.String))(ro.sync.options.SerializableLinkedHashMap<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[]> conditions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypePattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) conditionSetName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ditavalFile, boolean useDITAVAL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) shortcut)
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
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[]> [getConditions](#getConditions())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getConditionSetName](#getConditionSetName())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDITAVALFile](#getDITAVALFile())()
Return the DITAVAL location.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentTypePattern](#getDocumentTypePattern())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getNotPersistentFieldNames](#getNotPersistentFieldNames())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getShortcut](#getShortcut())()
Get the condition set shortcut.
  int [hashCode](#hashCode())()

 void [setConditions](#setConditions(ro.sync.options.SerializableLinkedHashMap))(ro.sync.options.SerializableLinkedHashMap<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[]> conditions)

 void [setConditionSetName](#setConditionSetName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) conditionSetName)

 void [setDitavalFile](#setDitavalFile(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ditavalFile)
Set the DITAVAL location.
  void [setDocumentTypePattern](#setDocumentTypePattern(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypePattern)

 void [setShortcut](#setShortcut(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) shortcut)
Set the condition set shortcut.
  void [setUseDITAVAL](#setUseDITAVAL(boolean))(boolean useDITAVAL)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

 boolean [useDITAVAL](#useDITAVAL())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ProfileConditionsSetInfoPO

public ProfileConditionsSetInfoPO()

Constructor.

### ProfileConditionsSetInfoPO

public ProfileConditionsSetInfoPO(ro.sync.options.SerializableLinkedHashMap<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[]> conditions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypePattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) conditionSetName)

Constructor.
  Parameters: conditions - Map between attributes and profile values. documentTypePattern - Document type pattern (the conditions set will be used only for the document types that match it) conditionSetName - Condition set name.
### ProfileConditionsSetInfoPO

public ProfileConditionsSetInfoPO(ro.sync.options.SerializableLinkedHashMap<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[]> conditions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypePattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) conditionSetName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ditavalFile, boolean useDITAVAL)

Constructor.
  Parameters: conditions - Map between attributes and profile values. documentTypePattern - Document type pattern (the conditions set will be used only for the document types that match it) conditionSetName - Condition set name. ditavalFile - The DITAVAL file used for the condition set. A profiling consition set can be based either on a set of user defined consitions or a DITAVAL file. useDITAVAL - true if the DITAVAL file should be used instead of the consitions set.
### ProfileConditionsSetInfoPO

public ProfileConditionsSetInfoPO(ro.sync.options.SerializableLinkedHashMap<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[]> conditions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypePattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) conditionSetName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ditavalFile, boolean useDITAVAL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) shortcut)

Constructor.
  Parameters: conditions - Map between attributes and profile values. documentTypePattern - Document type pattern (the conditions set will be used only for the document types that match it) conditionSetName - Condition set name. ditavalFile - The DITAVAL file used for the condition set. A profiling consition set can be based either on a set of user defined consitions or a DITAVAL file. useDITAVAL - true if the DITAVAL file should be used instead of the consitions set. shortcut - The condition set shortcut.
## Method Details

### setConditions

public void setConditions(ro.sync.options.SerializableLinkedHashMap<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[]> conditions)
  Parameters: conditions - The conditions to set.
### getConditions

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[]> getConditions()
  Returns: Returns the conditions.
### setDocumentTypePattern

public void setDocumentTypePattern([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypePattern)
  Parameters: documentTypePattern - The documentTypePattern to set.
### getDocumentTypePattern

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentTypePattern()
  Returns: Returns the documentTypePattern.
### setConditionSetName

public void setConditionSetName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) conditionSetName)
  Parameters: conditionSetName - The conditionSetName to set.
### getConditionSetName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getConditionSetName()
  Returns: Returns the conditionSetName.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

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

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### getDITAVALFile

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDITAVALFile()

Return the DITAVAL location.
  Returns: The DITAVAL location. It can be null.
### setDitavalFile

public void setDitavalFile([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ditavalFile)

Set the DITAVAL location.
  Parameters: ditavalFile - The DITAVAL location to set.
### useDITAVAL

public boolean useDITAVAL()
  Returns: true if the DITAVAL file should be used instead of the conditions set.
### setUseDITAVAL

public void setUseDITAVAL(boolean useDITAVAL)
  Parameters: useDITAVAL - True if the condition set is using a DITAVAL file instead of the conditions set.
### getShortcut

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getShortcut()

Get the condition set shortcut.
  Returns: Returns the condition set shortcut.
### setShortcut

public void setShortcut([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) shortcut)

Set the condition set shortcut.
  Parameters: shortcut - The shortcut to set.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
