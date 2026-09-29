Package [ro.sync.ecss.extensions.api.table.operations](package-summary.md)

# Class TableRowsSpecificationInformation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.table.operations.TableRowsSpecificationInformation
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [AuthorContentMetadata](../../../../component/AuthorContentMetadata.md)   @API(type=EXTENDABLE, src=PUBLIC) public class TableRowsSpecificationInformation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorContentMetadata](../../../../component/AuthorContentMetadata.md)
Contains information about rows (like the place where empty cells must be inserted to compensate the spanning cells). It can be extended to provide specific table rows properties for different types of tables or document types. This information is requested when table rows are copied or dragged and it can be used when the rows must be inserted in the document (on paste or drop). Please note that when a column is copied the table column specification information will be copied into the clipboard (the AuthorClipboardObject contains a field of [TableRowsSpecificationInformation](TableRowsSpecificationInformation.md) type), so it will be serialized.
  Since: 18 See Also:
* [Serialized Form](../../../../../../../serialized-form.md#ro.sync.ecss.extensions.api.table.operations.TableRowsSpecificationInformation)

## Constructor Summary
 Constructors
Constructor

Description
 [TableRowsSpecificationInformation](#%3Cinit%3E(int))(int sourceTableColumnsCount)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addSpanningCellIndexes](#addSpanningCellIndexes(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)> indexes)
Add spanning cells indexes.
  int [getSourceTableColumnsCount](#getSourceTableColumnsCount())()
The number of columns from source table.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)>> [getSpanningCellIndexes](#getSpanningCellIndexes())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TableRowsSpecificationInformation

public TableRowsSpecificationInformation(int sourceTableColumnsCount)

Constructor.
  Parameters: sourceTableColumnsCount - The number of columns from source table.
## Method Details

### addSpanningCellIndexes

public void addSpanningCellIndexes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)> indexes)

Add spanning cells indexes.
  Parameters: indexes - Spanning cell indexes (starts with 0)
### getSpanningCellIndexes

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)>> getSpanningCellIndexes()
  Returns: Returns the spanning cell indexes.
### getSourceTableColumnsCount

public int getSourceTableColumnsCount()

The number of columns from source table.
  Returns: Returns the sourceTableColumnsCount.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
