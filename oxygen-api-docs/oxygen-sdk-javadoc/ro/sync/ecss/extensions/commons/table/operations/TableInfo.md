Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class TableInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.operations.TableInfo
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)   @API(type=INTERNAL, src=PUBLIC) public class TableInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)
Contains information about the table element (number of rows, columns, table title).
  See Also:
* [Serialized Form](../../../../../../../serialized-form.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo)

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [DEFAULT_COLUMNS_COUNT](#DEFAULT_COLUMNS_COUNT)
Default number of columns
  static final int [DEFAULT_COLUMNS_COUNT_CHOICE_TABLE](#DEFAULT_COLUMNS_COUNT_CHOICE_TABLE)
Default number of columns for DITA choice table.
  static final int [DEFAULT_COLUMNS_COUNT_PROPERTIES_TABLE](#DEFAULT_COLUMNS_COUNT_PROPERTIES_TABLE)
Default number of columns for Properties table
  static final int [DEFAULT_ROWS_COUNT](#DEFAULT_ROWS_COUNT)
Default number of rows
  static final int [MAX_COLUMNS_COUNT](#MAX_COLUMNS_COUNT)
Maximum number of columns for CALS and simple tables.
  static final int [MAX_COLUMNS_COUNT_PROPERTIES_TABLE](#MAX_COLUMNS_COUNT_PROPERTIES_TABLE)
Maximum number of columns for CALS and simple tables.
  static final int [MIN_COLUMNS_COUNT](#MIN_COLUMNS_COUNT)
Minimum number of columns for CALS and simple tables.
  static final int [MIN_COLUMNS_COUNT_PROPERTIES_TABLE](#MIN_COLUMNS_COUNT_PROPERTIES_TABLE)
Minimum number of columns for CALS and simple tables.
  static final int [MIN_ROWS_COUNT](#MIN_ROWS_COUNT)
Minimum number of rows.
  static final int [TABLE_MODEL_CALS](#TABLE_MODEL_CALS)
Constant for CALS table model.
  static final int [TABLE_MODEL_CUSTOM](#TABLE_MODEL_CUSTOM)
Constant for custom table model specific for a document type (proprietary table model).
  static final int [TABLE_MODEL_DITA_CHOICE](#TABLE_MODEL_DITA_CHOICE)
The choice table model for DITA.
  static final int [TABLE_MODEL_DITA_PROPERTIES](#TABLE_MODEL_DITA_PROPERTIES)
The properties table model for DITA.
  static final int [TABLE_MODEL_DITA_SIMPLE](#TABLE_MODEL_DITA_SIMPLE)
The simple table model for DITA.
  static final int [TABLE_MODEL_HTML](#TABLE_MODEL_HTML)
Constant for HTML table model.
  static final int [TABLE_MODEL_NONE](#TABLE_MODEL_NONE)
Constant for no table model.

## Constructor Summary
 Constructors
Constructor

Description
 [TableInfo](#%3Cinit%3E(java.lang.String,int,int,boolean,boolean,java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, int rowsNumber, int columnsNumber, boolean generateHeader, boolean generateFooter, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) frame, int tableModel)
Constructor.
  [TableInfo](#%3Cinit%3E(java.lang.String,int,int,boolean,boolean,java.lang.String,int,ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.ColumnWidthsType,java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, int rowsNumber, int columnsNumber, boolean generateHeader, boolean generateFooter, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) frame, int tableModel, [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md) columnsWidthsType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rowsep, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colsep, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) align)
Constructor.
  [TableInfo](#%3Cinit%3E(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> fieldValues)  Deprecated.
Use [TableInfo(Map, int)](#%3Cinit%3E(java.util.Map,int)) instead because the table operation can also convert lists to tables and we need to provide a minimum number of rows.
   [TableInfo](#%3Cinit%3E(java.util.Map,int))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> fieldValues, int rows)
Constructs a table info from a map that contains the values of its fields.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAlign](#getAlign())()
Obtain the value for the alignment attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getColsep](#getColsep())()
Obtain the value for the column separator attribute.
  int [getColumnsNumber](#getColumnsNumber())()
Return the number of columns.
  [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md) [getColumnsWidthsType](#getColumnsWidthsType())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFrame](#getFrame())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRowsep](#getRowsep())()
Obtain the value for the row separator attribute.
  int [getRowsNumber](#getRowsNumber())()
Return the number of rows.
  int [getTableModel](#getTableModel())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTitle](#getTitle())()
Returns the title of the table.
  boolean [isGenerateFooter](#isGenerateFooter())()

 boolean [isGenerateHeader](#isGenerateHeader())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### TABLE_MODEL_NONE

public static final int TABLE_MODEL_NONE

Constant for no table model.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.TABLE_MODEL_NONE)

### TABLE_MODEL_HTML

public static final int TABLE_MODEL_HTML

Constant for HTML table model.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.TABLE_MODEL_HTML)

### TABLE_MODEL_CALS

public static final int TABLE_MODEL_CALS

Constant for CALS table model.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.TABLE_MODEL_CALS)

### TABLE_MODEL_CUSTOM

public static final int TABLE_MODEL_CUSTOM

Constant for custom table model specific for a document type (proprietary table model).
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.TABLE_MODEL_CUSTOM)

### TABLE_MODEL_DITA_SIMPLE

public static final int TABLE_MODEL_DITA_SIMPLE

The simple table model for DITA.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.TABLE_MODEL_DITA_SIMPLE)

### TABLE_MODEL_DITA_CHOICE

public static final int TABLE_MODEL_DITA_CHOICE

The choice table model for DITA.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.TABLE_MODEL_DITA_CHOICE)

### TABLE_MODEL_DITA_PROPERTIES

public static final int TABLE_MODEL_DITA_PROPERTIES

The properties table model for DITA.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.TABLE_MODEL_DITA_PROPERTIES)

### MIN_ROWS_COUNT

public static final int MIN_ROWS_COUNT

Minimum number of rows.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.MIN_ROWS_COUNT)

### DEFAULT_ROWS_COUNT

public static final int DEFAULT_ROWS_COUNT

Default number of rows
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.DEFAULT_ROWS_COUNT)

### DEFAULT_COLUMNS_COUNT_CHOICE_TABLE

public static final int DEFAULT_COLUMNS_COUNT_CHOICE_TABLE

Default number of columns for DITA choice table.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.DEFAULT_COLUMNS_COUNT_CHOICE_TABLE)

### DEFAULT_COLUMNS_COUNT

public static final int DEFAULT_COLUMNS_COUNT

Default number of columns
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.DEFAULT_COLUMNS_COUNT)

### DEFAULT_COLUMNS_COUNT_PROPERTIES_TABLE

public static final int DEFAULT_COLUMNS_COUNT_PROPERTIES_TABLE

Default number of columns for Properties table
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.DEFAULT_COLUMNS_COUNT_PROPERTIES_TABLE)

### MIN_COLUMNS_COUNT

public static final int MIN_COLUMNS_COUNT

Minimum number of columns for CALS and simple tables.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.MIN_COLUMNS_COUNT)

### MIN_COLUMNS_COUNT_PROPERTIES_TABLE

public static final int MIN_COLUMNS_COUNT_PROPERTIES_TABLE

Minimum number of columns for CALS and simple tables.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.MIN_COLUMNS_COUNT_PROPERTIES_TABLE)

### MAX_COLUMNS_COUNT

public static final int MAX_COLUMNS_COUNT

Maximum number of columns for CALS and simple tables.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.MAX_COLUMNS_COUNT)

### MAX_COLUMNS_COUNT_PROPERTIES_TABLE

public static final int MAX_COLUMNS_COUNT_PROPERTIES_TABLE

Maximum number of columns for CALS and simple tables.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableInfo.MAX_COLUMNS_COUNT_PROPERTIES_TABLE)

## Constructor Details

### TableInfo

public TableInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, int rowsNumber, int columnsNumber, boolean generateHeader, boolean generateFooter, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) frame, int tableModel)

Constructor.
  Parameters: title - The table title. rowsNumber - The number of rows. columnsNumber - The number of columns. generateHeader - If true generate table header. generateFooter - If true generate table footer. frame - Specifies how the table is to be framed. tableModel - The table model type. One of the constants: [TABLE_MODEL_CALS](#TABLE_MODEL_CALS), [TABLE_MODEL_CUSTOM](#TABLE_MODEL_CUSTOM), [TABLE_MODEL_DITA_SIMPLE](#TABLE_MODEL_DITA_SIMPLE), [TABLE_MODEL_HTML](#TABLE_MODEL_HTML), [TABLE_MODEL_DITA_CHOICE](#TABLE_MODEL_DITA_CHOICE), [TABLE_MODEL_DITA_PROPERTIES](#TABLE_MODEL_DITA_PROPERTIES).
### TableInfo

public TableInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, int rowsNumber, int columnsNumber, boolean generateHeader, boolean generateFooter, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) frame, int tableModel, [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md) columnsWidthsType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rowsep, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colsep, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) align)

Constructor.
  Parameters: title - The table title. rowsNumber - The number of rows. columnsNumber - The number of columns. generateHeader - If true generate table header. generateFooter - If true generate table footer. frame - Specifies how the table is to be framed. tableModel - The table model type. One of the constants: [TABLE_MODEL_CALS](#TABLE_MODEL_CALS), [TABLE_MODEL_CUSTOM](#TABLE_MODEL_CUSTOM), [TABLE_MODEL_DITA_SIMPLE](#TABLE_MODEL_DITA_SIMPLE), [TABLE_MODEL_HTML](#TABLE_MODEL_HTML), [TABLE_MODEL_DITA_CHOICE](#TABLE_MODEL_DITA_CHOICE), [TABLE_MODEL_DITA_PROPERTIES](#TABLE_MODEL_DITA_PROPERTIES). columnsWidthsType - The columns widths type. rowsep - Specifies the row separator value. colsep - Specifies the column separator value align - Specifies the alignment for the current table.
### TableInfo

public TableInfo([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> fieldValues, int rows)

Constructs a table info from a map that contains the values of its fields.
  Parameters: fieldValues - The map that contains the values for the operation fields. rows - If greater than 0, the enforced number of rows, used when the user converts a list with that many items to a table. If 0 or negative, it is ignored.
### TableInfo

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public TableInfo([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> fieldValues)
 Deprecated.
Use [TableInfo(Map, int)](#%3Cinit%3E(java.util.Map,int)) instead because the table operation can also convert lists to tables and we need to provide a minimum number of rows.

Constructs a table info from a map that contains the values of its fields.
  Parameters: fieldValues - The map that contains the values for the operation fields.
## Method Details

### getTitle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTitle()

Returns the title of the table.
  Returns: The title of the table.
### getRowsNumber

public int getRowsNumber()

Return the number of rows.
  Returns: The number of rows.
### getColumnsNumber

public int getColumnsNumber()

Return the number of columns.
  Returns: The number of columns.
### isGenerateHeader

public boolean isGenerateHeader()
  Returns: If true then table header will be generated.
### isGenerateFooter

public boolean isGenerateFooter()
  Returns: If true then table footer will be generated.
### getFrame

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFrame()
  Returns: Specifies the table frame.
### getRowsep

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRowsep()

Obtain the value for the row separator attribute.
  Returns: Specifies the row separator value.
### getColsep

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getColsep()

Obtain the value for the column separator attribute.
  Returns: Specifies the column separator value.
### getAlign

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAlign()

Obtain the value for the alignment attribute.
  Returns: Specifies the alignment value.
### getTableModel

public int getTableModel()
  Returns: Returns the table model. One of the constants: [TABLE_MODEL_CALS](#TABLE_MODEL_CALS), [TABLE_MODEL_CUSTOM](#TABLE_MODEL_CUSTOM), [TABLE_MODEL_DITA_SIMPLE](#TABLE_MODEL_DITA_SIMPLE), [TABLE_MODEL_HTML](#TABLE_MODEL_HTML), [TABLE_MODEL_DITA_CHOICE](#TABLE_MODEL_DITA_CHOICE), [TABLE_MODEL_DITA_PROPERTIES](#TABLE_MODEL_DITA_PROPERTIES).
### getColumnsWidthsType

public [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md) getColumnsWidthsType()
  Returns: Returns the columns widths type(proportional, fixed, dynamic).
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
