Package [ro.sync.ecss.conditions](package-summary.md)

# Class ProfilingAttributesPresentingColorsPO

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.conditions.ProfilingAttributesPresentingColorsPO
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), [PersistentObject](../../options/PersistentObject.md)   @API(type=EXTENDABLE, src=PRIVATE) public class ProfilingAttributesPresentingColorsPO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [PersistentObject](../../options/PersistentObject.md)
Persistent object containing information about the colors used when presenting the profiling attributes in the Author page.
  See Also:
* [Serialized Form](../../../../serialized-form.md#ro.sync.ecss.conditions.ProfilingAttributesPresentingColorsPO)

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [ProfilingAttributesPresentingColorsPO](ProfilingAttributesPresentingColorsPO.md) [DEFAULT_PROFILING_SHOW_ATTRIBUTES_COLORS](#DEFAULT_PROFILING_SHOW_ATTRIBUTES_COLORS)
Default colors used for profiling.

## Constructor Summary
 Constructors
Constructor

Description
 [ProfilingAttributesPresentingColorsPO](#%3Cinit%3E())()
Default constructor
  [ProfilingAttributesPresentingColorsPO](#%3Cinit%3E(int,int,int,int))(int backgroundColor, int nameForegroundColor, int valuesForegroundColor, int borderColor)
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
  int [getBackgroundColor](#getBackgroundColor())()

 int [getBorderColor](#getBorderColor())()

 int [getNameForegroundColor](#getNameForegroundColor())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getNotPersistentFieldNames](#getNotPersistentFieldNames())()

 int [getValuesForegroundColor](#getValuesForegroundColor())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### DEFAULT_PROFILING_SHOW_ATTRIBUTES_COLORS

public static final [ProfilingAttributesPresentingColorsPO](ProfilingAttributesPresentingColorsPO.md) DEFAULT_PROFILING_SHOW_ATTRIBUTES_COLORS

Default colors used for profiling.

## Constructor Details

### ProfilingAttributesPresentingColorsPO

public ProfilingAttributesPresentingColorsPO()

Default constructor

### ProfilingAttributesPresentingColorsPO

public ProfilingAttributesPresentingColorsPO(int backgroundColor, int nameForegroundColor, int valuesForegroundColor, int borderColor)

Constructor.
  Parameters: backgroundColor - Profiling background color. nameForegroundColor - Profiling attribute name foreground color. valuesForegroundColor - Profiling attribute values foreground color. borderColor - The color of the border that surrounds the profiled content.
## Method Details

### getNameForegroundColor

public int getNameForegroundColor()
  Returns: Returns the profiling attribute name foreground color.
### getValuesForegroundColor

public int getValuesForegroundColor()
  Returns: Returns the profiling attribute values foreground color.
### getBackgroundColor

public int getBackgroundColor()
  Returns: Returns the profiling background color.
### getBorderColor

public int getBorderColor()
  Returns: Returns the color of the border that surrounds the profiled content.
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

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
