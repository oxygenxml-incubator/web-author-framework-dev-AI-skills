Package [ro.sync.ecss.extensions.api](package-summary.md)

# Enum Class WidthRepresentation.Unit

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[WidthRepresentation.Unit](WidthRepresentation.Unit.md)>
        * ro.sync.ecss.extensions.api.WidthRepresentation.Unit
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[WidthRepresentation.Unit](WidthRepresentation.Unit.md)>, [Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html)   Enclosing class: [WidthRepresentation](WidthRepresentation.md)   public static enum WidthRepresentation.Unit extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[WidthRepresentation.Unit](WidthRepresentation.Unit.md)>
The fixed width unit.

## Nested Class Summary

## Nested classes/interfaces inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [Enum.EnumDesc](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html) extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)>>
## Enum Constant Summary
 Enum Constants
Enum Constant

Description
 [CENTIMETER](#CENTIMETER)
Centimeters are converted to inches and then multiplied with the dots per inch.
  [EM](#EM)
The EM is relative to the font size.
  [EX](#EX)
The EX is relative the the height of the "x" character.
  [INCH](#INCH)
Value in inches are multiplied with the dots per inch value.
  [MILLIMETER](#MILLIMETER)
Value in millimeter is converted to inches and then to pixels.
  [PICA](#PICA)
Pica is a unit of measure equal to 12 points or one sixth of an inch.
  [PIXEL](#PIXEL)
Directly in pixels.
  [POINT](#POINT)
A point is approximately 1/72 inch.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

 static [WidthRepresentation.Unit](WidthRepresentation.Unit.md) [valueOf](#valueOf(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the enum constant of this class with the specified name.
  static [WidthRepresentation.Unit](WidthRepresentation.Unit.md)[] [values](#values())()
Returns an array containing the constants of this enum class, in the order they are declared.

### Methods inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#clone()), [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#compareTo(E)), [describeConstable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#describeConstable()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#finalize()), [getDeclaringClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#getDeclaringClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#hashCode()), [name](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#name()), [ordinal](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#ordinal()), [valueOf](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#valueOf(java.lang.Class,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Enum Constant Details

### CENTIMETER

public static final [WidthRepresentation.Unit](WidthRepresentation.Unit.md) CENTIMETER

Centimeters are converted to inches and then multiplied with the dots per inch. The value is cm.

### EM

public static final [WidthRepresentation.Unit](WidthRepresentation.Unit.md) EM

The EM is relative to the font size. 1 is the font size. The value is em.

### EX

public static final [WidthRepresentation.Unit](WidthRepresentation.Unit.md) EX

The EX is relative the the height of the "x" character. The value is ex.

### INCH

public static final [WidthRepresentation.Unit](WidthRepresentation.Unit.md) INCH

Value in inches are multiplied with the dots per inch value. The value is in.

### MILLIMETER

public static final [WidthRepresentation.Unit](WidthRepresentation.Unit.md) MILLIMETER

Value in millimeter is converted to inches and then to pixels. The value is mm.

### PICA

public static final [WidthRepresentation.Unit](WidthRepresentation.Unit.md) PICA

Pica is a unit of measure equal to 12 points or one sixth of an inch. The value is pc.

### PIXEL

public static final [WidthRepresentation.Unit](WidthRepresentation.Unit.md) PIXEL

Directly in pixels. No conversion needed. The value is px.

### POINT

public static final [WidthRepresentation.Unit](WidthRepresentation.Unit.md) POINT

A point is approximately 1/72 inch. The value is pt.

## Method Details

### values

public static [WidthRepresentation.Unit](WidthRepresentation.Unit.md)[] values()

Returns an array containing the constants of this enum class, in the order they are declared.
  Returns: an array containing the constants of this enum class, in the order they are declared
### valueOf

public static [WidthRepresentation.Unit](WidthRepresentation.Unit.md) valueOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the enum constant of this class with the specified name. The string must match *exactly* an identifier used to declare an enum constant in this class. (Extraneous whitespace characters are not permitted.)
  Parameters: name - the name of the enum constant to be returned. Returns: the enum constant with the specified name Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if this enum class has no constant with the specified name [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the argument is null
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#toString()) in class [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[WidthRepresentation.Unit](WidthRepresentation.Unit.md)> See Also:
        * [Enum.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
