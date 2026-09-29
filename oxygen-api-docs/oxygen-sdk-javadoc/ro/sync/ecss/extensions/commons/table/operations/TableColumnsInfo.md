Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class TableColumnsInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.operations.TableColumnsInfo
   @API(type=INTERNAL, src=PUBLIC) public class TableColumnsInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Contains information about the columns to be inserted.

## Constructor Summary
 Constructors
Constructor

Description
 [TableColumnsInfo](#%3Cinit%3E())()
Constructor.
  [TableColumnsInfo](#%3Cinit%3E(int,boolean))(int columnsNumber, boolean insertAfter)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getColumnsNumber](#getColumnsNumber())()
Get the number of columns.
  boolean [isInsertAfter](#isInsertAfter())()
Check if we should insert after.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TableColumnsInfo

public TableColumnsInfo()

Constructor.

### TableColumnsInfo

public TableColumnsInfo(int columnsNumber, boolean insertAfter)

Constructor.
  Parameters: columnsNumber - the number of columns. insertAfter - true to insert after.
## Method Details

### getColumnsNumber

public int getColumnsNumber()

Get the number of columns.
  Returns: Returns the columnsNumber.
### isInsertAfter

public boolean isInsertAfter()

Check if we should insert after.
  Returns: Returns the insertAfter.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
