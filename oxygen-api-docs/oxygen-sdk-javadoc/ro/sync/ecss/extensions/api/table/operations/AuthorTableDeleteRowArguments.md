Package [ro.sync.ecss.extensions.api.table.operations](package-summary.md)

# Class AuthorTableDeleteRowArguments

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowArguments
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorTableDeleteRowArguments extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Holds the arguments for [AuthorTableOperationsHandler.handleDeleteRow(AuthorTableDeleteRowArguments)](AuthorTableOperationsHandler.md#handleDeleteRow(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowArguments)) method.
  Since: 14
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorTableDeleteRowArguments](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ContentInterval))([AuthorAccess](../../AuthorAccess.md) authorAccess, [ContentInterval](../../ContentInterval.md) rowInterval)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorAccess](../../AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()

 [ContentInterval](../../ContentInterval.md) [getRowInterval](#getRowInterval())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorTableDeleteRowArguments

public AuthorTableDeleteRowArguments([AuthorAccess](../../AuthorAccess.md) authorAccess, [ContentInterval](../../ContentInterval.md) rowInterval)

Constructor.
  Parameters: authorAccess - The Author access. rowInterval - The content interval (containing the **inclusive** start offset and **exclusive** end offset) determining the row that must be deleted.
## Method Details

### getAuthorAccess

public [AuthorAccess](../../AuthorAccess.md) getAuthorAccess()
  Returns: Returns the access to Author operation.
### getRowInterval

public [ContentInterval](../../ContentInterval.md) getRowInterval()
  Returns: Returns the content interval (containing the **inclusive** start offset and **exclusive** end offset) determining the row that must be deleted.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
