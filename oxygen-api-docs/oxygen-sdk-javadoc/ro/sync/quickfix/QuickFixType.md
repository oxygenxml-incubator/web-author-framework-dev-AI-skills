Package [ro.sync.quickfix](package-summary.md)

# Enum Class QuickFixType

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[QuickFixType](QuickFixType.md)>
        * ro.sync.quickfix.QuickFixType
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[QuickFixType](QuickFixType.md)>, [Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html)   public enum QuickFixType extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[QuickFixType](QuickFixType.md)>
The type IDs for the quick fixes.

## Nested Class Summary

## Nested classes/interfaces inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [Enum.EnumDesc](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html) extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)>>
## Enum Constant Summary
 Enum Constants
Enum Constant

Description
 [ADD_QF](#ADD_QF)
Insert node quick fix id.
  [ATTRIBUTR_SET_QF](#ATTRIBUTR_SET_QF)
Create attribute set quick fix id.
  [CHANGE_REFERENCE_QF](#CHANGE_REFERENCE_QF)
Change component reference quick fix id.
  [CHARACTER_MAP_QF](#CHARACTER_MAP_QF)
Create character map quick fix id.
  [DELETE_QF](#DELETE_QF)
Delete component quick fix id.
  [ELEMENT_QF](#ELEMENT_QF)
Insert element quick fix id.
  [FUNCTION_PARAM_QF](#FUNCTION_PARAM_QF)
Create function parameter quick fix id.
  [FUNCTION_QF](#FUNCTION_QF)
Create functions quick fix id.
  [GLOBAL_PARAM_QF](#GLOBAL_PARAM_QF)
Create global parameter quick fix id.
  [GLOBAL_VARIABLE_QF](#GLOBAL_VARIABLE_QF)
Create global variable quick fix id.
  [IGNORE_QF](#IGNORE_QF)
Ignore problem quick fix id.
  [LOCAL_VARIABLE_QF](#LOCAL_VARIABLE_QF)
Create local variable quick fix id.
  [MIX_QF](#MIX_QF)
Insert node quick fix id.
  [REPLACE_QF](#REPLACE_QF)
Replace node quick fix id.
  [REPLACE_TEXT_QF](#REPLACE_TEXT_QF)
Change text node quick fix id.
  [TARGET_QF](#TARGET_QF)
Create target quick fix ID.
  [TEMPLATE_PARAM_QF](#TEMPLATE_PARAM_QF)
Create template parameter quick fix id.
  [TEMPLATE_QF](#TEMPLATE_QF)
Create template quick fix id.
  [UNIGNORE_QF](#UNIGNORE_QF)
Unignore problem quick fix id.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static [QuickFixType](QuickFixType.md) [forValue](#forValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Get the quick fix type for the given string value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toValue](#toValue())()

 static [QuickFixType](QuickFixType.md) [valueOf](#valueOf(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the enum constant of this class with the specified name.
  static [QuickFixType](QuickFixType.md)[] [values](#values())()
Returns an array containing the constants of this enum class, in the order they are declared.

### Methods inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#clone()), [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#compareTo(E)), [describeConstable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#describeConstable()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#finalize()), [getDeclaringClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#getDeclaringClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#hashCode()), [name](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#name()), [ordinal](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#ordinal()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#toString()), [valueOf](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#valueOf(java.lang.Class,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Enum Constant Details

### GLOBAL_VARIABLE_QF

public static final [QuickFixType](QuickFixType.md) GLOBAL_VARIABLE_QF

Create global variable quick fix id.

### LOCAL_VARIABLE_QF

public static final [QuickFixType](QuickFixType.md) LOCAL_VARIABLE_QF

Create local variable quick fix id.

### GLOBAL_PARAM_QF

public static final [QuickFixType](QuickFixType.md) GLOBAL_PARAM_QF

Create global parameter quick fix id.

### TEMPLATE_PARAM_QF

public static final [QuickFixType](QuickFixType.md) TEMPLATE_PARAM_QF

Create template parameter quick fix id.

### FUNCTION_PARAM_QF

public static final [QuickFixType](QuickFixType.md) FUNCTION_PARAM_QF

Create function parameter quick fix id.

### ATTRIBUTR_SET_QF

public static final [QuickFixType](QuickFixType.md) ATTRIBUTR_SET_QF

Create attribute set quick fix id.

### CHARACTER_MAP_QF

public static final [QuickFixType](QuickFixType.md) CHARACTER_MAP_QF

Create character map quick fix id.

### TEMPLATE_QF

public static final [QuickFixType](QuickFixType.md) TEMPLATE_QF

Create template quick fix id.

### FUNCTION_QF

public static final [QuickFixType](QuickFixType.md) FUNCTION_QF

Create functions quick fix id.

### TARGET_QF

public static final [QuickFixType](QuickFixType.md) TARGET_QF

Create target quick fix ID.

### CHANGE_REFERENCE_QF

public static final [QuickFixType](QuickFixType.md) CHANGE_REFERENCE_QF

Change component reference quick fix id.

### DELETE_QF

public static final [QuickFixType](QuickFixType.md) DELETE_QF

Delete component quick fix id.

### ELEMENT_QF

public static final [QuickFixType](QuickFixType.md) ELEMENT_QF

Insert element quick fix id.

### ADD_QF

public static final [QuickFixType](QuickFixType.md) ADD_QF

Insert node quick fix id.

### REPLACE_QF

public static final [QuickFixType](QuickFixType.md) REPLACE_QF

Replace node quick fix id.

### REPLACE_TEXT_QF

public static final [QuickFixType](QuickFixType.md) REPLACE_TEXT_QF

Change text node quick fix id.

### MIX_QF

public static final [QuickFixType](QuickFixType.md) MIX_QF

Insert node quick fix id.

### IGNORE_QF

public static final [QuickFixType](QuickFixType.md) IGNORE_QF

Ignore problem quick fix id.

### UNIGNORE_QF

public static final [QuickFixType](QuickFixType.md) UNIGNORE_QF

Unignore problem quick fix id.

## Method Details

### values

public static [QuickFixType](QuickFixType.md)[] values()

Returns an array containing the constants of this enum class, in the order they are declared.
  Returns: an array containing the constants of this enum class, in the order they are declared
### valueOf

public static [QuickFixType](QuickFixType.md) valueOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the enum constant of this class with the specified name. The string must match *exactly* an identifier used to declare an enum constant in this class. (Extraneous whitespace characters are not permitted.)
  Parameters: name - the name of the enum constant to be returned. Returns: the enum constant with the specified name Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if this enum class has no constant with the specified name [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the argument is null
### forValue

public static [QuickFixType](QuickFixType.md) forValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Get the quick fix type for the given string value.
  Parameters: value - The string value to get the constant for. Returns: The constant
### toValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toValue()
  Returns: The string representation of the current quick fix type.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
