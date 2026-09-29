Package [ro.sync.ecss.extensions.api.table.operations](package-summary.md)

# Class AuthorTableInsertColumnArguments

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertColumnArguments
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorTableInsertColumnArguments extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Holds the arguments for [AuthorTableOperationsHandler.handleInsertColumn(AuthorTableInsertColumnArguments)](AuthorTableOperationsHandler.md#handleInsertColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertColumnArguments)) method.
  Since: 14
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorTableInsertColumnArguments](#%3Cinit%3E(int,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,boolean,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation))(int insertOffset, [AuthorDocumentFragment](../../node/AuthorDocumentFragment.md)[] columnFragments, boolean fragmentsWrappedInCells, [AuthorAccess](../../AuthorAccess.md) authorAccess, [TableColumnSpecificationInformation](TableColumnSpecificationInformation.md) columnSpecification)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [areFragmentsWrappedInCells](#areFragmentsWrappedInCells())()

 [AuthorAccess](../../AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()

 [AuthorDocumentFragment](../../node/AuthorDocumentFragment.md)[] [getColumnFragments](#getColumnFragments())()

 [TableColumnSpecificationInformation](TableColumnSpecificationInformation.md) [getColumnSpecificationInformation](#getColumnSpecificationInformation())()
Returns the column specification information of a table column.
  int [getInsertOffset](#getInsertOffset())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorTableInsertColumnArguments

public AuthorTableInsertColumnArguments(int insertOffset, [AuthorDocumentFragment](../../node/AuthorDocumentFragment.md)[] columnFragments, boolean fragmentsWrappedInCells, [AuthorAccess](../../AuthorAccess.md) authorAccess, [TableColumnSpecificationInformation](TableColumnSpecificationInformation.md) columnSpecification)

Constructor.
  Parameters: insertOffset - The offset where the column is inserted. columnFragments - The array containing the cells nodes that compose an Author table column. fragmentsWrappedInCells - true if the given column fragments represents the cells nodes or only the content of the cells nodes. authorAccess - The Author access. columnSpecification - Table column specification information that is requested when a column is copied or dragged, from [AuthorTableOperationsHandler.getColumnSpecification(AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](AuthorTableOperationsHandler.md#getColumnSpecification(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))method. It can be null if no information is specified for table column.
## Method Details

### getAuthorAccess

public [AuthorAccess](../../AuthorAccess.md) getAuthorAccess()
  Returns: Returns the access to Author operation.
### getColumnFragments

public [AuthorDocumentFragment](../../node/AuthorDocumentFragment.md)[] getColumnFragments()
  Returns: Returns the array containing the cells nodes that compose an Author table column.
### getInsertOffset

public int getInsertOffset()
  Returns: Returns the offset where the column is inserted.
### areFragmentsWrappedInCells

public boolean areFragmentsWrappedInCells()
  Returns: Returns true if the given column fragments represents the cells nodes or only the content of the cells nodes.
### getColumnSpecificationInformation

public [TableColumnSpecificationInformation](TableColumnSpecificationInformation.md) getColumnSpecificationInformation()

Returns the column specification information of a table column. This information is requested when a column is copied or dragged, from [AuthorTableOperationsHandler.getColumnSpecification(AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](AuthorTableOperationsHandler.md#getColumnSpecification(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))method.
  Returns: Returns information about column specification (like column specified width). It can be null if no information is specified for table column.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
