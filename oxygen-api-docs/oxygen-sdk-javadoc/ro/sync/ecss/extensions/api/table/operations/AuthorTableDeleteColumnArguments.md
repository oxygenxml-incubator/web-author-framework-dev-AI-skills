Package [ro.sync.ecss.extensions.api.table.operations](package-summary.md)

# Class AuthorTableDeleteColumnArguments

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteColumnArguments
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorTableDeleteColumnArguments extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Holds the arguments for [AuthorTableOperationsHandler.handleDeleteColumn(AuthorTableDeleteColumnArguments)](AuthorTableOperationsHandler.md#handleDeleteColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteColumnArguments)) method.
  Since: 14
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorTableDeleteColumnArguments](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List))([AuthorAccess](../../AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../ContentInterval.md)> columnCellsIntervals)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorAccess](../../AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../ContentInterval.md)> [getColumnCellsIntervals](#getColumnCellsIntervals())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorTableDeleteColumnArguments

public AuthorTableDeleteColumnArguments([AuthorAccess](../../AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../ContentInterval.md)> columnCellsIntervals)

Constructor.
  Parameters: authorAccess - The Author access. columnCellsIntervals - The list of intervals of the cells that compose the deleted column. Each [ContentInterval](../../ContentInterval.md) contains the start and end offsets of the cells.
## Method Details

### getAuthorAccess

public [AuthorAccess](../../AuthorAccess.md) getAuthorAccess()
  Returns: Returns the access to Author operation.
### getColumnCellsIntervals

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../ContentInterval.md)> getColumnCellsIntervals()
  Returns: Returns the list of intervals of the cells that compose the deleted column.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
