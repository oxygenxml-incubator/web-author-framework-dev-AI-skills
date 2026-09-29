Package [ro.sync.ecss.extensions.api.table.operations](package-summary.md)

# Class AuthorTableInsertRowArguments

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertRowArguments
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorTableInsertRowArguments extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Holds the arguments for [AuthorTableOperationsHandler.handlePasteRows(AuthorTableInsertRowArguments)](AuthorTableOperationsHandler.md#handlePasteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertRowArguments)) method.
  Since: 21
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorTableInsertRowArguments](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,int))([AuthorAccess](../../AuthorAccess.md) authorAccess, [AuthorDocumentFragment](../../node/AuthorDocumentFragment.md)[] rowFragments, int insertOffset)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorAccess](../../AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()

 int [getInsertOffset](#getInsertOffset())()

 [AuthorDocumentFragment](../../node/AuthorDocumentFragment.md)[] [getRowFragments](#getRowFragments())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorTableInsertRowArguments

public AuthorTableInsertRowArguments([AuthorAccess](../../AuthorAccess.md) authorAccess, [AuthorDocumentFragment](../../node/AuthorDocumentFragment.md)[] rowFragments, int insertOffset)

Constructor.
  Parameters: authorAccess - The Author access. rowFragments - The array containing the rows nodes that are inserted insertOffset - The offset where the rows are inserted.
## Method Details

### getAuthorAccess

public [AuthorAccess](../../AuthorAccess.md) getAuthorAccess()
  Returns: Returns the access to Author operation.
### getRowFragments

public [AuthorDocumentFragment](../../node/AuthorDocumentFragment.md)[] getRowFragments()
  Returns: Returns the array containing the row nodes that are inserted.
### getInsertOffset

public int getInsertOffset()
  Returns: Returns the offset where the rows are inserted.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
