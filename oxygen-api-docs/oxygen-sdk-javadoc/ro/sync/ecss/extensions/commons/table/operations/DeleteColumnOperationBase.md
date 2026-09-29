Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class DeleteColumnOperationBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](AbstractTableOperation.md)
        * ro.sync.ecss.extensions.commons.table.operations.DeleteColumnOperationBase
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   Direct Known Subclasses: [DeleteColumnOperation](cals/DeleteColumnOperation.md), [DeleteColumnOperation](xhtml/DeleteColumnOperation.md), [DeleteColumnOperation](../../../dita/map/table/DeleteColumnOperation.md), [DeleteColumnOperation](../../../dita/topic/table/simpletable/DeleteColumnOperation.md), [DeleteColumnOperation](../../../tei/table/DeleteColumnOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class DeleteColumnOperationBase extends [AbstractTableOperation](AbstractTableOperation.md)
Base implementation for operations used to delete table columns. If there are selections in the table, all the columns that intersect the selections are removed. If there is no selection in the table, the column at caret is deleted.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)> [deletedColumnsIndices](#deletedColumnsIndices)
The index of the deleted column.
  protected [AuthorElement](../../../api/node/AuthorElement.md) [tableElem](#tableElem)
The table element.

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [DeleteColumnOperationBase](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](AuthorTableHelper.md) documentTypeHelper)
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [canDeleteColumn](#canDeleteColumn())()

 protected void [doOperationInternal](#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)
Delete the table column at the caret position.
  [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()
No arguments for this operation.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 boolean [performDeleteColumn](#performDeleteColumn(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,boolean))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../../api/ContentInterval.md)> columnIntervals, boolean placeCaretInNextCell)
Delete table columns.
  protected void [updateAppliableColWidthsNumber](#updateAppliableColWidthsNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElem, int deletedColumnIndex)
If the table has anything else to update when a column is deleted...
  protected void [updateColspec](#updateColspec(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.Integer))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) deletedColumnIndex)
Update the colspec of a table for a given column.
  protected abstract void [updateTableColSpan](#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) spanProvider, [AuthorElement](../../../api/node/AuthorElement.md) cell, int colStartIndex, int colEndIndex)
Update the column span for the table cell that is included into the deleted column.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md)
 [createEmptyCell](AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### tableElem

protected [AuthorElement](../../../api/node/AuthorElement.md) tableElem

The table element.

### deletedColumnsIndices

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)> deletedColumnsIndices

The index of the deleted column.

## Constructor Details

### DeleteColumnOperationBase

public DeleteColumnOperationBase([AuthorTableHelper](AuthorTableHelper.md) documentTypeHelper)

Constructor.
  Parameters: documentTypeHelper - The table helper specific to a document type. An implementation of [AuthorTableHelper](AuthorTableHelper.md).
## Method Details

### performDeleteColumn

public boolean performDeleteColumn([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../../api/ContentInterval.md)> columnIntervals, boolean placeCaretInNextCell)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Delete table columns. The columns are detected in the following order:
        * from the given column intervals
        * from the selection
        * from the caret position

  Parameters: authorAccess - The access to Author operations. columnIntervals - The intervals of the column to be deleted. If null, the column at caret offset is deleted. placeCaretInNextCell - true to place caret in the next cell. Returns: true if a column is deleted Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) [AuthorOperationException](../../../api/AuthorOperationException.md)
### updateColspec

protected void updateColspec([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) deletedColumnIndex)

Update the colspec of a table for a given column.
  Parameters: authorAccess - The Author access. deletedColumnIndex - The index of the deleted column.
### updateAppliableColWidthsNumber

protected void updateAppliableColWidthsNumber([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElem, int deletedColumnIndex)

If the table has anything else to update when a column is deleted...
  Parameters: authorAccess - The author access. tableElem - The table access. deletedColumnIndex - The deleted column index.
### doOperationInternal

protected void doOperationInternal([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Delete the table column at the caret position. For this operation the caret must be inside a table cell.
  Specified by: [doOperationInternal](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [AbstractTableOperation](AbstractTableOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AbstractTableOperation.doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### updateTableColSpan

protected abstract void updateTableColSpan([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) spanProvider, [AuthorElement](../../../api/node/AuthorElement.md) cell, int colStartIndex, int colEndIndex)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Update the column span for the table cell that is included into the deleted column.
  Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. spanProvider - The table span provider. The object responsible for providing information about the cell spanning. cell - The table cell. colStartIndex - The new column start index, 1 based. colEndIndex - The new column end index, 1 based. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - When the operation fails.
### getArguments

public [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] getArguments()

No arguments for this operation.
  Returns: An array of [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments())

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

### canDeleteColumn

protected boolean canDeleteColumn()
  Returns: true if a column from the specified table can be deleted. false otherwise.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
