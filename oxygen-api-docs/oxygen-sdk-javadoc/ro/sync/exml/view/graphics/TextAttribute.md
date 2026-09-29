Package [ro.sync.exml.view.graphics](package-summary.md)

# Enum Class TextAttribute

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[TextAttribute](TextAttribute.md)>
        * ro.sync.exml.view.graphics.TextAttribute
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[TextAttribute](TextAttribute.md)>, [Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html)   @API(type=EXTENDABLE, src=PRIVATE) public enum TextAttribute extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[TextAttribute](TextAttribute.md)>
Constants for the [AttributedString](AttributedString.md) attributes. Similar to the [TextAttribute](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/font/TextAttribute.html) class.

## Nested Class Summary

## Nested classes/interfaces inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [Enum.EnumDesc](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html) extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)>>
## Enum Constant Summary
 Enum Constants
Enum Constant

Description
 [FONT](#FONT)
Specifies a font for a text interval.
  [FOREGROUND](#FOREGROUND)
The foreground color for a piece of [AttributedString](AttributedString.md).
  [POSTURE](#POSTURE)
The font posture (like italic, regular)
  [POSTURE_OBLIQUE](#POSTURE_OBLIQUE)
The standard italic posture value.
  [POSTURE_REGULAR](#POSTURE_REGULAR)
The standard posture value, upright.
  [RELATIVE_SIZE](#RELATIVE_SIZE)
The relative size of the font
  [RELATIVE_SIZE_SMALL](#RELATIVE_SIZE_SMALL)
A value for the relative size.
  [RUN_DIRECTION](#RUN_DIRECTION)
Attribute key for the run direction of the line.
  [RUN_DIRECTION_LTR](#RUN_DIRECTION_LTR)
Left-to-right run direction.
  [RUN_DIRECTION_RTL](#RUN_DIRECTION_RTL)
Right-to-left run direction.
  [STRIKETHROUGH](#STRIKETHROUGH)
Strike through
  [UNDERLINE](#UNDERLINE)
Underline.
  [WEIGHT](#WEIGHT)
The font weight of [AttributedString](AttributedString.md).
  [WEIGHT_BOLD](#WEIGHT_BOLD)
Value for the weight.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [TextAttribute](TextAttribute.md) [valueOf](#valueOf(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the enum constant of this class with the specified name.
  static [TextAttribute](TextAttribute.md)[] [values](#values())()
Returns an array containing the constants of this enum class, in the order they are declared.

### Methods inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#clone()), [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#compareTo(E)), [describeConstable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#describeConstable()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#finalize()), [getDeclaringClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#getDeclaringClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#hashCode()), [name](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#name()), [ordinal](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#ordinal()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#toString()), [valueOf](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#valueOf(java.lang.Class,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Enum Constant Details

### FOREGROUND

public static final [TextAttribute](TextAttribute.md) FOREGROUND

The foreground color for a piece of [AttributedString](AttributedString.md).

### WEIGHT

public static final [TextAttribute](TextAttribute.md) WEIGHT

The font weight of [AttributedString](AttributedString.md).

### WEIGHT_BOLD

public static final [TextAttribute](TextAttribute.md) WEIGHT_BOLD

Value for the weight.

### POSTURE

public static final [TextAttribute](TextAttribute.md) POSTURE

The font posture (like italic, regular)

### POSTURE_REGULAR

public static final [TextAttribute](TextAttribute.md) POSTURE_REGULAR

The standard posture value, upright. This is the default value for POSTURE.
  See Also:
        * [POSTURE](#POSTURE)

### POSTURE_OBLIQUE

public static final [TextAttribute](TextAttribute.md) POSTURE_OBLIQUE

The standard italic posture value.
  See Also:
        * [POSTURE](#POSTURE)

### RELATIVE_SIZE

public static final [TextAttribute](TextAttribute.md) RELATIVE_SIZE

The relative size of the font

### RELATIVE_SIZE_SMALL

public static final [TextAttribute](TextAttribute.md) RELATIVE_SIZE_SMALL

A value for the relative size. Imposes a smaller size for the font.
  See Also:
        * [RELATIVE_SIZE](#RELATIVE_SIZE)

### RUN_DIRECTION

public static final [TextAttribute](TextAttribute.md) RUN_DIRECTION

Attribute key for the run direction of the line. Values are instances of **Boolean**. The default value is null, which indicates that the standard Bidi algorithm for determining run direction should be used with the value [Bidi.DIRECTION_DEFAULT_LEFT_TO_RIGHT](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/text/Bidi.html#DIRECTION_DEFAULT_LEFT_TO_RIGHT).
The constants [RUN_DIRECTION_RTL](#RUN_DIRECTION_RTL) and [RUN_DIRECTION_LTR](#RUN_DIRECTION_LTR) are provided.

This determines the value passed to the [Bidi](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/text/Bidi.html) constructor to select the primary direction of the text in the paragraph.

Note: This attribute should have the same value for all the text in a paragraph, otherwise the behavior is undetermined.

  See Also:
        * [Bidi](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/text/Bidi.html)

### RUN_DIRECTION_LTR

public static final [TextAttribute](TextAttribute.md) RUN_DIRECTION_LTR

Left-to-right run direction.
  See Also:
        * [RUN_DIRECTION](#RUN_DIRECTION)

### RUN_DIRECTION_RTL

public static final [TextAttribute](TextAttribute.md) RUN_DIRECTION_RTL

Right-to-left run direction.
  See Also:
        * [RUN_DIRECTION](#RUN_DIRECTION)

### FONT

public static final [TextAttribute](TextAttribute.md) FONT

Specifies a font for a text interval. The value should be an instance of [Font](Font.md).

### STRIKETHROUGH

public static final [TextAttribute](TextAttribute.md) STRIKETHROUGH

Strike through

### UNDERLINE

public static final [TextAttribute](TextAttribute.md) UNDERLINE

Underline. The value should be an instance of [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html).

## Method Details

### values

public static [TextAttribute](TextAttribute.md)[] values()

Returns an array containing the constants of this enum class, in the order they are declared.
  Returns: an array containing the constants of this enum class, in the order they are declared
### valueOf

public static [TextAttribute](TextAttribute.md) valueOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the enum constant of this class with the specified name. The string must match *exactly* an identifier used to declare an enum constant in this class. (Extraneous whitespace characters are not permitted.)
  Parameters: name - the name of the enum constant to be returned. Returns: the enum constant with the specified name Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if this enum class has no constant with the specified name [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the argument is null
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
