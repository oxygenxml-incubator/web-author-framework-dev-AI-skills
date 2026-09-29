Package [ro.sync.ecss.extensions.api](package-summary.md)

# Enum Class CursorType

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[CursorType](CursorType.md)>
        * ro.sync.ecss.extensions.api.CursorType
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CursorType](CursorType.md)>, [Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public enum CursorType extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[CursorType](CursorType.md)>
Supported cursor types for author.

## Nested Class Summary

## Nested classes/interfaces inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [Enum.EnumDesc](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html) extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)>>
## Enum Constant Summary
 Enum Constants
Enum Constant

Description
 [CURSOR_CROSSHAIR](#CURSOR_CROSSHAIR)
Cross-hair cursor
  [CURSOR_E_RESIZE](#CURSOR_E_RESIZE)
Resize East cursor.
  [CURSOR_HAND](#CURSOR_HAND)
Hand cursor
  [CURSOR_NE_RESIZE](#CURSOR_NE_RESIZE)
Resize North-East cursor.
  [CURSOR_NORMAL](#CURSOR_NORMAL)
Normal cursor
  [CURSOR_NW_RESIZE](#CURSOR_NW_RESIZE)
Resize North-West cursor.
  [CURSOR_RESIZE](#CURSOR_RESIZE)  Deprecated.
Use [CURSOR_E_RESIZE](#CURSOR_E_RESIZE) instead.
   [CURSOR_S_RESIZE](#CURSOR_S_RESIZE)
Resize South cursor.
  [CURSOR_SE_RESIZE](#CURSOR_SE_RESIZE)
Resize South-East cursor.
  [CURSOR_SELECT_CELL](#CURSOR_SELECT_CELL)
Select cell cursor.
  [CURSOR_SELECT_CELL_DOWN_LTR](#CURSOR_SELECT_CELL_DOWN_LTR)
Select cell cursor, for tables that are oriented from left to right.
  [CURSOR_SELECT_CELL_DOWN_RTL](#CURSOR_SELECT_CELL_DOWN_RTL)
Select cell cursor, for tables that are oriented from right to left.
  [CURSOR_SELECT_CELL_UP_LTR](#CURSOR_SELECT_CELL_UP_LTR)
Select cell cursor, for tables that are oriented from left to right.
  [CURSOR_SELECT_CELL_UP_RTL](#CURSOR_SELECT_CELL_UP_RTL)
Select cell cursor, for tables that are oriented from right to left.
  [CURSOR_SELECT_COLUMN](#CURSOR_SELECT_COLUMN)
Select column cursor
  [CURSOR_SELECT_ROW](#CURSOR_SELECT_ROW)  Deprecated.
You should use one of the two other constants, specifying the direction.
   [CURSOR_SELECT_ROW_LTR](#CURSOR_SELECT_ROW_LTR)
Select row cursor, for tables that are oriented from left to right.
  [CURSOR_SELECT_ROW_RTL](#CURSOR_SELECT_ROW_RTL)
Select row cursor, for tables that are oriented from right to left.
  [CURSOR_SELECT_TABLE](#CURSOR_SELECT_TABLE)  Deprecated.
You should use one of the two other constants, specifying the direction.
   [CURSOR_SELECT_TABLE_LTR](#CURSOR_SELECT_TABLE_LTR)
Select row cursor, for tables that are oriented from left to right.
  [CURSOR_SELECT_TABLE_RTL](#CURSOR_SELECT_TABLE_RTL)
Select row cursor, for tables that are oriented from right to left.
  [CURSOR_SW_RESIZE](#CURSOR_SW_RESIZE)
Resize South-West cursor.
  [CURSOR_TEXT](#CURSOR_TEXT)
Text cursor

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [isResizeCursor](#isResizeCursor())()

 static [CursorType](CursorType.md) [valueOf](#valueOf(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the enum constant of this class with the specified name.
  static [CursorType](CursorType.md)[] [values](#values())()
Returns an array containing the constants of this enum class, in the order they are declared.

### Methods inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#clone()), [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#compareTo(E)), [describeConstable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#describeConstable()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#finalize()), [getDeclaringClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#getDeclaringClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#hashCode()), [name](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#name()), [ordinal](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#ordinal()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#toString()), [valueOf](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#valueOf(java.lang.Class,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Enum Constant Details

### CURSOR_NORMAL

public static final [CursorType](CursorType.md) CURSOR_NORMAL

Normal cursor

### CURSOR_CROSSHAIR

public static final [CursorType](CursorType.md) CURSOR_CROSSHAIR

Cross-hair cursor

### CURSOR_TEXT

public static final [CursorType](CursorType.md) CURSOR_TEXT

Text cursor

### CURSOR_E_RESIZE

public static final [CursorType](CursorType.md) CURSOR_E_RESIZE

Resize East cursor.

### CURSOR_S_RESIZE

public static final [CursorType](CursorType.md) CURSOR_S_RESIZE

Resize South cursor.

### CURSOR_SE_RESIZE

public static final [CursorType](CursorType.md) CURSOR_SE_RESIZE

Resize South-East cursor.

### CURSOR_SW_RESIZE

public static final [CursorType](CursorType.md) CURSOR_SW_RESIZE

Resize South-West cursor.

### CURSOR_NE_RESIZE

public static final [CursorType](CursorType.md) CURSOR_NE_RESIZE

Resize North-East cursor.

### CURSOR_NW_RESIZE

public static final [CursorType](CursorType.md) CURSOR_NW_RESIZE

Resize North-West cursor.

### CURSOR_RESIZE

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static final [CursorType](CursorType.md) CURSOR_RESIZE
 Deprecated.
Use [CURSOR_E_RESIZE](#CURSOR_E_RESIZE) instead.

Resize horizontal cursor.

### CURSOR_HAND

public static final [CursorType](CursorType.md) CURSOR_HAND

Hand cursor

### CURSOR_SELECT_COLUMN

public static final [CursorType](CursorType.md) CURSOR_SELECT_COLUMN

Select column cursor

### CURSOR_SELECT_ROW

public static final [CursorType](CursorType.md) CURSOR_SELECT_ROW
 Deprecated.
You should use one of the two other constants, specifying the direction.

Select row cursor, for tables that are oriented from left to right.

### CURSOR_SELECT_ROW_LTR

public static final [CursorType](CursorType.md) CURSOR_SELECT_ROW_LTR

Select row cursor, for tables that are oriented from left to right.

### CURSOR_SELECT_ROW_RTL

public static final [CursorType](CursorType.md) CURSOR_SELECT_ROW_RTL

Select row cursor, for tables that are oriented from right to left.

### CURSOR_SELECT_TABLE

public static final [CursorType](CursorType.md) CURSOR_SELECT_TABLE
 Deprecated.
You should use one of the two other constants, specifying the direction.

Select table cursor, for tables that are oriented from left to right.

### CURSOR_SELECT_TABLE_LTR

public static final [CursorType](CursorType.md) CURSOR_SELECT_TABLE_LTR

Select row cursor, for tables that are oriented from left to right.

### CURSOR_SELECT_TABLE_RTL

public static final [CursorType](CursorType.md) CURSOR_SELECT_TABLE_RTL

Select row cursor, for tables that are oriented from right to left.

### CURSOR_SELECT_CELL_UP_LTR

public static final [CursorType](CursorType.md) CURSOR_SELECT_CELL_UP_LTR

Select cell cursor, for tables that are oriented from left to right. This is used when the mouse is placed in the left up corner of the cell.

### CURSOR_SELECT_CELL_DOWN_LTR

public static final [CursorType](CursorType.md) CURSOR_SELECT_CELL_DOWN_LTR

Select cell cursor, for tables that are oriented from left to right. This is used when the mouse is placed in the left down corner of the cell.

### CURSOR_SELECT_CELL_UP_RTL

public static final [CursorType](CursorType.md) CURSOR_SELECT_CELL_UP_RTL

Select cell cursor, for tables that are oriented from right to left. This is used when the mouse is placed in the right up corner of the cell.

### CURSOR_SELECT_CELL_DOWN_RTL

public static final [CursorType](CursorType.md) CURSOR_SELECT_CELL_DOWN_RTL

Select cell cursor, for tables that are oriented from right to left. This is used when the mouse is placed in the right down corner of the cell.

### CURSOR_SELECT_CELL

public static final [CursorType](CursorType.md) CURSOR_SELECT_CELL

Select cell cursor.

## Method Details

### values

public static [CursorType](CursorType.md)[] values()

Returns an array containing the constants of this enum class, in the order they are declared.
  Returns: an array containing the constants of this enum class, in the order they are declared
### valueOf

public static [CursorType](CursorType.md) valueOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the enum constant of this class with the specified name. The string must match *exactly* an identifier used to declare an enum constant in this class. (Extraneous whitespace characters are not permitted.)
  Parameters: name - the name of the enum constant to be returned. Returns: the enum constant with the specified name Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if this enum class has no constant with the specified name [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the argument is null
### isResizeCursor

public boolean isResizeCursor()
  Returns: true if this cursor is one of the resize cursors.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
