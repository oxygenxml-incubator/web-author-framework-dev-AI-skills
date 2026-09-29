Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class SplitOperationBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](AbstractTableOperation.md)
        * ro.sync.ecss.extensions.commons.table.operations.SplitOperationBase
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   Direct Known Subclasses: [SplitOperation](cals/SplitOperation.md), [SplitOperation](xhtml/SplitOperation.md), [SplitOperation](../../../dita/topic/table/cals/SplitOperation.md), [SplitOperation](../../../tei/table/SplitOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class SplitOperationBase extends [AbstractTableOperation](AbstractTableOperation.md)
Operation for splitting the selected table cell (or the cell at caret when there is no selection), if it spans over multiple rows or columns

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [SplitOperationBase](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](AuthorTableHelper.md) tableHelper)
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [doOperationInternal](#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)
Split the selected table cell (or the cell at caret when there is no selection), if it spans over multiple rows or columns
  [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID())()
Get the ID of the help page which will be called by the end user.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredAttributesForColumnSplit](#getIgnoredAttributesForColumnSplit())()

 protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredAttributesForRowSplit](#getIgnoredAttributesForRowSplit())()

 protected abstract [InsertColumnOperationBase](InsertColumnOperationBase.md) [getInsertColumnOperation](#getInsertColumnOperation())()
Get the insert column operation to be used when splitting cells that have no initial span.
  protected abstract [InsertRowOperationBase](InsertRowOperationBase.md) [getInsertRowOperation](#getInsertRowOperation())()
Get the insert row operation to be used when splitting cells that have no initial span.
  protected abstract [JoinOperationBase](JoinOperationBase.md) [getJoinOperation](#getJoinOperation())()
Get the join operation to be used when splitting cells that have no initial span.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md)
 [createEmptyCell](AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SplitOperationBase

public SplitOperationBase([AuthorTableHelper](AuthorTableHelper.md) tableHelper)

Constructor.
  Parameters: tableHelper - Table helper with methods specific to a document type.
## Method Details

### doOperationInternal

protected void doOperationInternal([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Split the selected table cell (or the cell at caret when there is no selection), if it spans over multiple rows or columns
  Specified by: [doOperationInternal](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [AbstractTableOperation](AbstractTableOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AbstractTableOperation.doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### getInsertRowOperation

protected abstract [InsertRowOperationBase](InsertRowOperationBase.md) getInsertRowOperation()

Get the insert row operation to be used when splitting cells that have no initial span.

### getInsertColumnOperation

protected abstract [InsertColumnOperationBase](InsertColumnOperationBase.md) getInsertColumnOperation()

Get the insert column operation to be used when splitting cells that have no initial span.

### getJoinOperation

protected abstract [JoinOperationBase](JoinOperationBase.md) getJoinOperation()

Get the join operation to be used when splitting cells that have no initial span.

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

### getArguments

public [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] getArguments()
  Returns: An array of [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [getArguments()](#getArguments())

### getIgnoredAttributesForRowSplit

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredAttributesForRowSplit()
  Returns: The attributes which should be skipped, when creating a copy of the split cell.
### getIgnoredAttributesForColumnSplit

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredAttributesForColumnSplit()
  Returns: The attributes which should be skipped when creating a copy of the split cell.
### getHelpPageID

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID()

Get the ID of the help page which will be called by the end user.
  Returns: the ID of the help page which will be called by the end user or null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
