Package [ro.sync.ecss.extensions.commons.table.support.errorscanner](package-summary.md)

# Enum Class TableLayoutProblem.Severity

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[TableLayoutProblem.Severity](TableLayoutProblem.Severity.md)>
        * ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutProblem.Severity
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[TableLayoutProblem.Severity](TableLayoutProblem.Severity.md)>, [Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html)   Enclosing interface: [TableLayoutProblem](TableLayoutProblem.md)   public static enum TableLayoutProblem.Severity extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[TableLayoutProblem.Severity](TableLayoutProblem.Severity.md)>
Problem severity

## Nested Class Summary

## Nested classes/interfaces inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [Enum.EnumDesc](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html) extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)>>
## Enum Constant Summary
 Enum Constants
Enum Constant

Description
 [ERROR](#ERROR)
Table layout error
  [INFO](#INFO)
Table layout information
  [WARN](#WARN)
Table layout warning

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md) [valueOf](#valueOf(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the enum constant of this class with the specified name.
  static [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md)[] [values](#values())()
Returns an array containing the constants of this enum class, in the order they are declared.

### Methods inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#clone()), [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#compareTo(E)), [describeConstable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#describeConstable()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#finalize()), [getDeclaringClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#getDeclaringClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#hashCode()), [name](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#name()), [ordinal](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#ordinal()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#toString()), [valueOf](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#valueOf(java.lang.Class,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Enum Constant Details

### ERROR

public static final [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md) ERROR

Table layout error

### WARN

public static final [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md) WARN

Table layout warning

### INFO

public static final [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md) INFO

Table layout information

## Method Details

### values

public static [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md)[] values()

Returns an array containing the constants of this enum class, in the order they are declared.
  Returns: an array containing the constants of this enum class, in the order they are declared
### valueOf

public static [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md) valueOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the enum constant of this class with the specified name. The string must match *exactly* an identifier used to declare an enum constant in this class. (Extraneous whitespace characters are not permitted.)
  Parameters: name - the name of the enum constant to be returned. Returns: the enum constant with the specified name Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if this enum class has no constant with the specified name [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the argument is null
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
