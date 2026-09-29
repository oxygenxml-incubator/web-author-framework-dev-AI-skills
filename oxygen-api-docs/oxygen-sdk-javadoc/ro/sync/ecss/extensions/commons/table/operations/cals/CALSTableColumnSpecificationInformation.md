Package [ro.sync.ecss.extensions.commons.table.operations.cals](package-summary.md)

# Class CALSTableColumnSpecificationInformation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation](../../../../api/table/operations/TableColumnSpecificationInformation.md)
        * ro.sync.ecss.extensions.commons.table.operations.cals.CALSTableColumnSpecificationInformation
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [AuthorContentMetadata](../../../../../component/AuthorContentMetadata.md)   @API(type=INTERNAL, src=PUBLIC) public class CALSTableColumnSpecificationInformation extends [TableColumnSpecificationInformation](../../../../api/table/operations/TableColumnSpecificationInformation.md)
Information about CALS table column specification. Holds informations like column width and column name. It is used on table column insertion operations handling, to keep the original column name and width unchanged (for example when a CALS column is copied this information is kept into the clipboard and then used on paste column operation, as values for the inserted column colspec attributes).
  See Also:
* [Serialized Form](../../../../../../../../serialized-form.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSTableColumnSpecificationInformation)

## Constructor Summary
 Constructors
Constructor

Description
 [CALSTableColumnSpecificationInformation](#%3Cinit%3E(ro.sync.ecss.extensions.api.WidthRepresentation,java.lang.String))([WidthRepresentation](../../../../api/WidthRepresentation.md) widthRepresentation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) columnName)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getColumnName](#getColumnName())()
Gets the column name.
  void [setColumnName](#setColumnName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colName)
Set the column name.

### Methods inherited from class ro.sync.ecss.extensions.api.table.operations.[TableColumnSpecificationInformation](../../../../api/table/operations/TableColumnSpecificationInformation.md)
 [getWidthRepresentation](../../../../api/table/operations/TableColumnSpecificationInformation.md#getWidthRepresentation())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CALSTableColumnSpecificationInformation

public CALSTableColumnSpecificationInformation([WidthRepresentation](../../../../api/WidthRepresentation.md) widthRepresentation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) columnName)

Constructor.
  Parameters: widthRepresentation - The column width representation that specifies the fixed and relative width determined from the column specification. columnName - The column name.
## Method Details

### getColumnName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getColumnName()

Gets the column name.
  Returns: Returns the column name.
### setColumnName

public void setColumnName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colName)

Set the column name.
  Parameters: colName - The new column name.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
