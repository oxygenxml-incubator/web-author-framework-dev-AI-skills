Package [ro.sync.ecss.extensions.commons.table.support.errorscanner](package-summary.md)

# Enum Class CALSAndHTMLTableLayoutProblem

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md)>
        * ro.sync.ecss.extensions.commons.table.support.errorscanner.CALSAndHTMLTableLayoutProblem
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md)>, [Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html), [TableLayoutProblem](TableLayoutProblem.md)   @API(type=INTERNAL, src=PUBLIC) public enum CALSAndHTMLTableLayoutProblem extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md)> implements [TableLayoutProblem](TableLayoutProblem.md)
CALS table layout problem

## Nested Class Summary

## Nested classes/interfaces inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [Enum.EnumDesc](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html) extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)>>
## Nested classes/interfaces inherited from interface ro.sync.ecss.extensions.commons.table.support.errorscanner.[TableLayoutProblem](TableLayoutProblem.md)
 [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md)
## Enum Constant Summary
 Enum Constants
Enum Constant

Description
 [ATTRIBUTE_VALUE_NOT_INTEGER](#ATTRIBUTE_VALUE_NOT_INTEGER)
A specific attribute must have a numeric value en: "The {0} attribute must have a numeric value.
  [CELL_OVERFLOW_SPECIFIED_COLUMN_COUNT](#CELL_OVERFLOW_SPECIFIED_COLUMN_COUNT)
Table cell overflows the specified columns count
  [CELL_OVERLAPPING](#CELL_OVERLAPPING)
A cell was already occupied en: "The cell[{0}][{1}] is already occupied." {0} is the row number {1} is the column number
  [CELL_OVERLAPS_ONE_OR_MORE_PREVIOUS_CELLS](#CELL_OVERLAPS_ONE_OR_MORE_PREVIOUS_CELLS)
Cells overlapping error(as generals as it can be)
  [CELL_OVERLAPS_PREVIOUS_CELL](#CELL_OVERLAPS_PREVIOUS_CELL)
This cell overlaps previous cell.
  [COLS_DIFFERENT_THAN_COLUMNS](#COLS_DIFFERENT_THAN_COLUMNS)
There is a difference between the cols value and the number of actual columns en: "The number of table columns determined from the table structure ({0}) is different than the value of the {1} attribute: ({2})." {0} is the table columns count {1} the name of the (cols) attribute {2} the value of the (cols) attribute
  [COLSPECS_DIFFERENT_THAN_COLUMNS](#COLSPECS_DIFFERENT_THAN_COLUMNS)
There is a difference between the number of colspecs and the number of actual columns en: "The number of table columns determined from the table structure ({0}) is different than the number of colspecs ({1})." {0} is the table columns count {1} is the colspecs number
  [COLUMN_NAME_INCORRECT](#COLUMN_NAME_INCORRECT)
The column name from the namest or nameend attribute value is not found in column specifications en: "The column name ({0}) from the {1} attribute value is not found in column specifications." {0} the column name specified in the table {2} the name of the attribute that specifies the wrong column name
  [COLUMN_NUMBER_IS_INCORRECT](#COLUMN_NUMBER_IS_INCORRECT)
The columns should be assigned consecutive numbers
  [COLUMN_NUMBERING_SHOULD_BEGIN_FROM_ONE](#COLUMN_NUMBERING_SHOULD_BEGIN_FROM_ONE)
Column numbering should begin from 1.
  [COLUMN_WIDTH_NO_MEASURING_UNITS_VALUE_INCORRECT](#COLUMN_WIDTH_NO_MEASURING_UNITS_VALUE_INCORRECT)
The column width value is not valid according to the specification.
  [COLUMN_WIDTH_VALUE_INCORRECT](#COLUMN_WIDTH_VALUE_INCORRECT)
The column width value is not valid according to the specification.
  [DUPLICATE_COLSPEC_NAME](#DUPLICATE_COLSPEC_NAME)
en: Duplicate column name {'0'} {0} - the name of the column
  [DUPLICATE_COLSPEC_NUMBER](#DUPLICATE_COLSPEC_NUMBER)
Duplicate colspec's colnum.
  [NAMEST_LESS_THAN_NAMEEND](#NAMEST_LESS_THAN_NAMEEND)
The column index determined from namest attribute value is less than the column index determined from nameend.
  [ROW_CELL_COUNT_OVERFLOW](#ROW_CELL_COUNT_OVERFLOW)
The number of cells in the row overflows the number of table columns en: "The number of cells in the row ({0}) is greater than the value ({1}) of the table {2} attribute." {0} is the row cells count {1} the value of the table attribute that counts the columns number (cols) {2} the name of the table attribute that counts the columns number (cols)
  [ROW_CELL_COUNT_UNDERFLOW](#ROW_CELL_COUNT_UNDERFLOW)
The number of cells in the row is less than the number of table columns en: "The number of cells in the row ({0}) is less than the value ({1}) of the table {2} attribute." {0} is the row cells count {1} the value of the table attribute that counts the columns number (cols) {2} the name of the table attribute that counts the columns number (cols)
  [ROW_HAS_COLNAME_AND_NAMEST_OR_NAMEEND](#ROW_HAS_COLNAME_AND_NAMEST_OR_NAMEEND)
Column name (colname) attribute must not be present when column name start (namest) or column name end (nameend) are specified.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessage](#getMessage())()

 [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md) [getSeverity](#getSeverity())()

 static [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) [valueOf](#valueOf(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the enum constant of this class with the specified name.
  static [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md)[] [values](#values())()
Returns an array containing the constants of this enum class, in the order they are declared.

### Methods inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#clone()), [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#compareTo(E)), [describeConstable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#describeConstable()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#finalize()), [getDeclaringClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#getDeclaringClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#hashCode()), [name](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#name()), [ordinal](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#ordinal()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#toString()), [valueOf](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#valueOf(java.lang.Class,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Enum Constant Details

### ATTRIBUTE_VALUE_NOT_INTEGER

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) ATTRIBUTE_VALUE_NOT_INTEGER

A specific attribute must have a numeric value en: "The {0} attribute must have a numeric value. The current value is: {1}." {0} is the attribute name {1} is the attribute value

### CELL_OVERLAPPING

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) CELL_OVERLAPPING

A cell was already occupied en: "The cell[{0}][{1}] is already occupied." {0} is the row number {1} is the column number

### NAMEST_LESS_THAN_NAMEEND

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) NAMEST_LESS_THAN_NAMEEND

The column index determined from namest attribute value is less than the column index determined from nameend. en: "The column index determined from namest ({0}) attribute value is greater than the column index determined from nameend ({1})." {0} the namest attribute value {1} the nameend attribute value

### COLSPECS_DIFFERENT_THAN_COLUMNS

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) COLSPECS_DIFFERENT_THAN_COLUMNS

There is a difference between the number of colspecs and the number of actual columns en: "The number of table columns determined from the table structure ({0}) is different than the number of colspecs ({1})." {0} is the table columns count {1} is the colspecs number

### COLS_DIFFERENT_THAN_COLUMNS

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) COLS_DIFFERENT_THAN_COLUMNS

There is a difference between the cols value and the number of actual columns en: "The number of table columns determined from the table structure ({0}) is different than the value of the {1} attribute: ({2})." {0} is the table columns count {1} the name of the (cols) attribute {2} the value of the (cols) attribute

### ROW_CELL_COUNT_OVERFLOW

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) ROW_CELL_COUNT_OVERFLOW

The number of cells in the row overflows the number of table columns en: "The number of cells in the row ({0}) is greater than the value ({1}) of the table {2} attribute." {0} is the row cells count {1} the value of the table attribute that counts the columns number (cols) {2} the name of the table attribute that counts the columns number (cols)

### ROW_CELL_COUNT_UNDERFLOW

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) ROW_CELL_COUNT_UNDERFLOW

The number of cells in the row is less than the number of table columns en: "The number of cells in the row ({0}) is less than the value ({1}) of the table {2} attribute." {0} is the row cells count {1} the value of the table attribute that counts the columns number (cols) {2} the name of the table attribute that counts the columns number (cols)

### COLUMN_NAME_INCORRECT

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) COLUMN_NAME_INCORRECT

The column name from the namest or nameend attribute value is not found in column specifications en: "The column name ({0}) from the {1} attribute value is not found in column specifications." {0} the column name specified in the table {2} the name of the attribute that specifies the wrong column name

### COLUMN_WIDTH_VALUE_INCORRECT

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) COLUMN_WIDTH_VALUE_INCORRECT

The column width value is not valid according to the specification. en: "The column width ({0}) should be a mixture of proportional or measuring unit numbers." {0} the column name specified in the table

### COLUMN_WIDTH_NO_MEASURING_UNITS_VALUE_INCORRECT

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) COLUMN_WIDTH_NO_MEASURING_UNITS_VALUE_INCORRECT

The column width value is not valid according to the specification. en: "The column width ({0}) must not contain measuring unit numbers." {0} the column name specified in the table

### CELL_OVERLAPS_PREVIOUS_CELL

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) CELL_OVERLAPS_PREVIOUS_CELL

This cell overlaps previous cell.

### DUPLICATE_COLSPEC_NAME

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) DUPLICATE_COLSPEC_NAME

en: Duplicate column name {'0'} {0} - the name of the column

### COLUMN_NUMBERING_SHOULD_BEGIN_FROM_ONE

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) COLUMN_NUMBERING_SHOULD_BEGIN_FROM_ONE

Column numbering should begin from 1.

### CELL_OVERFLOW_SPECIFIED_COLUMN_COUNT

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) CELL_OVERFLOW_SPECIFIED_COLUMN_COUNT

Table cell overflows the specified columns count

### COLUMN_NUMBER_IS_INCORRECT

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) COLUMN_NUMBER_IS_INCORRECT

The columns should be assigned consecutive numbers

### DUPLICATE_COLSPEC_NUMBER

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) DUPLICATE_COLSPEC_NUMBER

Duplicate colspec's colnum.

### CELL_OVERLAPS_ONE_OR_MORE_PREVIOUS_CELLS

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) CELL_OVERLAPS_ONE_OR_MORE_PREVIOUS_CELLS

Cells overlapping error(as generals as it can be)

### ROW_HAS_COLNAME_AND_NAMEST_OR_NAMEEND

public static final [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) ROW_HAS_COLNAME_AND_NAMEST_OR_NAMEEND

Column name (colname) attribute must not be present when column name start (namest) or column name end (nameend) are specified.

## Method Details

### values

public static [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md)[] values()

Returns an array containing the constants of this enum class, in the order they are declared.
  Returns: an array containing the constants of this enum class, in the order they are declared
### valueOf

public static [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md) valueOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the enum constant of this class with the specified name. The string must match *exactly* an identifier used to declare an enum constant in this class. (Extraneous whitespace characters are not permitted.)
  Parameters: name - the name of the enum constant to be returned. Returns: the enum constant with the specified name Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if this enum class has no constant with the specified name [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the argument is null
### getMessage

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessage()
  Specified by: [getMessage](TableLayoutProblem.md#getMessage()) in interface [TableLayoutProblem](TableLayoutProblem.md) Returns: Returns the problem message to be presented to the user. See Also:
        * [TableLayoutProblem.getMessage()](TableLayoutProblem.md#getMessage())

### getSeverity

public [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md) getSeverity()
  Specified by: [getSeverity](TableLayoutProblem.md#getSeverity()) in interface [TableLayoutProblem](TableLayoutProblem.md) Returns: Returns the problem severity, one of [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md) constants. See Also:
        * [TableLayoutProblem.getSeverity()](TableLayoutProblem.md#getSeverity())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
