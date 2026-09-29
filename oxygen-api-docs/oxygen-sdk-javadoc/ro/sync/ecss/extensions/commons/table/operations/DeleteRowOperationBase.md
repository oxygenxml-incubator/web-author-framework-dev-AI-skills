Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class DeleteRowOperationBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](AbstractTableOperation.md)
        * ro.sync.ecss.extensions.commons.table.operations.DeleteRowOperationBase
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   Direct Known Subclasses: [DeleteRowOperation](cals/DeleteRowOperation.md), [DeleteRowOperation](xhtml/DeleteRowOperation.md), [DeleteRowOperation](../../../dita/map/table/DeleteRowOperation.md), [DeleteRowOperation](../../../dita/topic/table/cals/DeleteRowOperation.md), [DeleteRowOperation](../../../dita/topic/table/simpletable/DeleteRowOperation.md), [DeleteRowOperation](../../../tei/table/DeleteRowOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class DeleteRowOperationBase extends [AbstractTableOperation](AbstractTableOperation.md)
Operation used to delete table rows. If there is a selection in the table all the rows that intersect that selection are removed. If there is no selection in the table, the row at caret is deleted.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [DeleteRowOperationBase](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](AuthorTableHelper.md) documentTypeHelper)
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected abstract [SplitCellAboveBelowOperationBase](SplitCellAboveBelowOperationBase.md) [createSplitCellOperation](#createSplitCellOperation())()
Create the split cell operation.
  final void [doOperationInternal](#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)
Delete the table rows.
  [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()
No arguments for this operation.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 boolean [performDeleteRows](#performDeleteRows(ro.sync.ecss.extensions.api.AuthorAccess,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, int startRowOffset, int endRowOffset)
Delete table rows.
  boolean [performDeleteRows](#performDeleteRows(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../../api/ContentInterval.md)> contentIntervals)
Delete table rows.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md)
 [createEmptyCell](AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DeleteRowOperationBase

public DeleteRowOperationBase([AuthorTableHelper](AuthorTableHelper.md) documentTypeHelper)

Constructor.
  Parameters: documentTypeHelper - The table helper specific to a document type. An implementation of [AuthorTableHelper](AuthorTableHelper.md).
## Method Details

### performDeleteRows

public boolean performDeleteRows([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../../api/ContentInterval.md)> contentIntervals)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Delete table rows. The rows that must be deleted are determined in the following order:
        * by the list of content intervals if not null
        * all the rows that intersect the selection
        * the row at caret offset

  Parameters: authorAccess - The access to Author operations. contentIntervals - The content intervals that intersects the rows that must be deleted. Each interval contains two integers, one for start interval offset and one for end interval offset. Returns: true if the rows are deleted. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md)
### performDeleteRows

public boolean performDeleteRows([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, int startRowOffset, int endRowOffset)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Delete table rows. The row that must be deleted is determined in the following order:
        * by startRowOffset and endRowOffset if both are bigger than 0
        * all the rows that intersect the selection
        * the row at caret offset

  Parameters: authorAccess - The access to Author operations. startRowOffset - The start row offset. endRowOffset - The end row offset. Returns: true if at least one row is deleted. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) [AuthorOperationException](../../../api/AuthorOperationException.md)
### doOperationInternal

public final void doOperationInternal([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Delete the table rows. For this operation the caret must be inside a table cell.
  Specified by: [doOperationInternal](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [AbstractTableOperation](AbstractTableOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AbstractTableOperation.doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### getArguments

public [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] getArguments()

No arguments for this operation.
  Returns: An array of [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments())

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

### createSplitCellOperation

protected abstract [SplitCellAboveBelowOperationBase](SplitCellAboveBelowOperationBase.md) createSplitCellOperation()

Create the split cell operation. The operation is needed to split the cells that span over multiple rows and start on the row to be deleted.
  Returns: The split cell operation.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
