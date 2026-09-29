Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class TableRowsInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.operations.TableRowsInfo
   @API(type=INTERNAL, src=PUBLIC) public class TableRowsInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Contains information about the rows to be inserted.

## Constructor Summary
 Constructors
Constructor

Description
 [TableRowsInfo](#%3Cinit%3E())()
Constructor.
  [TableRowsInfo](#%3Cinit%3E(int,boolean))(int rowsNumber, boolean insertBelow)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getRowsNumber](#getRowsNumber())()
Get the number of rows.
  boolean [isInsertBelow](#isInsertBelow())()
Check if we should insert below.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TableRowsInfo

public TableRowsInfo()

Constructor.

### TableRowsInfo

public TableRowsInfo(int rowsNumber, boolean insertBelow)

Constructor.
  Parameters: rowsNumber - The number of rows. insertBelow - true to insert below.
## Method Details

### getRowsNumber

public int getRowsNumber()

Get the number of rows.
  Returns: Returns the rows number.
### isInsertBelow

public boolean isInsertBelow()

Check if we should insert below.
  Returns: Returns true if we should insert below.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
