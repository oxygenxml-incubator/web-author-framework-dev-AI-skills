Package [ro.sync.ecss.extensions.api.table.operations](package-summary.md)

# Class AuthorTableArguments

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.table.operations.AuthorTableArguments
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorTableArguments extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Holds the arguments for [AuthorTableOperationsHandler.handleCreateTable(AuthorTableArguments)](AuthorTableOperationsHandler.md#handleCreateTable(ro.sync.ecss.extensions.api.table.operations.AuthorTableArguments)) method.
  Since: 21.1
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorTableArguments](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int))([AuthorAccess](../../AuthorAccess.md) authorAccess, int insertOffset, int rows, int columns)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorAccess](../../AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()

 int [getColumns](#getColumns())()

 int [getInsertOffset](#getInsertOffset())()

 int [getRows](#getRows())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorTableArguments

public AuthorTableArguments([AuthorAccess](../../AuthorAccess.md) authorAccess, int insertOffset, int rows, int columns)

Constructor.
  Parameters: authorAccess - The Author access. insertOffset - The offset where the rows are inserted. rows - number of rows needed for the new table. columns - number of columns needed for the new table.
## Method Details

### getAuthorAccess

public [AuthorAccess](../../AuthorAccess.md) getAuthorAccess()
  Returns: Returns the access to Author operation.
### getInsertOffset

public int getInsertOffset()
  Returns: Returns the offset where the rows are inserted.
### getRows

public int getRows()
  Returns: Returns the rows.
### getColumns

public int getColumns()
  Returns: Returns the columns.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
