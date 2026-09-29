Package [ro.sync.ecss.extensions.api.table.operations](package-summary.md)

# Class AuthorTableDeleteRowsArguments

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowsArguments
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorTableDeleteRowsArguments extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Holds the arguments for [AuthorTableOperationsHandler.handleDeleteRows(AuthorTableDeleteRowsArguments)](AuthorTableOperationsHandler.md#handleDeleteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowsArguments)) method.
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorTableDeleteRowsArguments](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List))([AuthorAccess](../../AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../ContentInterval.md)> contentIntervals)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorAccess](../../AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../ContentInterval.md)> [getContentIntervals](#getContentIntervals())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorTableDeleteRowsArguments

public AuthorTableDeleteRowsArguments([AuthorAccess](../../AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../ContentInterval.md)> contentIntervals)

Constructor.
  Parameters: authorAccess - The Author access. contentIntervals - The content intervals (containing the **inclusive** start offset and **exclusive** end offset) determining the rows that must be deleted. The rows that must be deleted are all the rows that intersects the given content intervals.
## Method Details

### getAuthorAccess

public [AuthorAccess](../../AuthorAccess.md) getAuthorAccess()
  Returns: Returns the access to Author operation.
### getContentIntervals

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../ContentInterval.md)> getContentIntervals()
  Returns: Returns the list of content intervals (containing the **inclusive** start offset and **exclusive** end offset) determining the row that must be deleted.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
