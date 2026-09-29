Package [ro.sync.ecss.extensions.dita.map.table](package-summary.md)

# Class DeleteColumnOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../../../commons/table/operations/AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.DeleteColumnOperationBase](../../../commons/table/operations/DeleteColumnOperationBase.md)
            * ro.sync.ecss.extensions.dita.map.table.DeleteColumnOperation
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md), [ReltableConstants](ReltableConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class DeleteColumnOperation extends [DeleteColumnOperationBase](../../../commons/table/operations/DeleteColumnOperationBase.md)implements [ReltableConstants](ReltableConstants.md)
Operation used to delete a DITA map reltable column.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[DeleteColumnOperationBase](../../../commons/table/operations/DeleteColumnOperationBase.md)
 [deletedColumnsIndices](../../../commons/table/operations/DeleteColumnOperationBase.md#deletedColumnsIndices), [tableElem](../../../commons/table/operations/DeleteColumnOperationBase.md#tableElem)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../commons/table/operations/AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../../../commons/table/operations/AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../../../commons/table/operations/AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.dita.map.table.[ReltableConstants](ReltableConstants.md)
 [ATTRIBUTE_NAME_ID](ReltableConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_TYPE](ReltableConstants.md#ATTRIBUTE_NAME_TYPE), [ELEMENT_NAME_ENTRY](ReltableConstants.md#ELEMENT_NAME_ENTRY), [ELEMENT_NAME_HEADER](ReltableConstants.md#ELEMENT_NAME_HEADER), [ELEMENT_NAME_HEADER_ENTRY](ReltableConstants.md#ELEMENT_NAME_HEADER_ENTRY), [ELEMENT_NAME_ROW](ReltableConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_TABLE](ReltableConstants.md#ELEMENT_NAME_TABLE)
## Constructor Summary
 Constructors
Constructor

Description
 [DeleteColumnOperation](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [updateTableColSpan](#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) spanProvider, [AuthorElement](../../../api/node/AuthorElement.md) cell, int colStartIndex, int colEndIndex)
Update the column span for the table cell that is included into the deleted column.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[DeleteColumnOperationBase](../../../commons/table/operations/DeleteColumnOperationBase.md)
 [canDeleteColumn](../../../commons/table/operations/DeleteColumnOperationBase.md#canDeleteColumn()), [doOperationInternal](../../../commons/table/operations/DeleteColumnOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../commons/table/operations/DeleteColumnOperationBase.md#getArguments()), [getDescription](../../../commons/table/operations/DeleteColumnOperationBase.md#getDescription()), [performDeleteColumn](../../../commons/table/operations/DeleteColumnOperationBase.md#performDeleteColumn(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,boolean)), [updateAppliableColWidthsNumber](../../../commons/table/operations/DeleteColumnOperationBase.md#updateAppliableColWidthsNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)), [updateColspec](../../../commons/table/operations/DeleteColumnOperationBase.md#updateColspec(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.Integer))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../commons/table/operations/AbstractTableOperation.md)
 [createEmptyCell](../../../commons/table/operations/AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../../../commons/table/operations/AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../../../commons/table/operations/AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../../../commons/table/operations/AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../../../commons/table/operations/AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../../../commons/table/operations/AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DeleteColumnOperation

public DeleteColumnOperation()

Constructor.

## Method Details

### updateTableColSpan

protected void updateTableColSpan([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) spanProvider, [AuthorElement](../../../api/node/AuthorElement.md) cell, int colStartIndex, int colEndIndex)throws [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from class: [DeleteColumnOperationBase](../../../commons/table/operations/DeleteColumnOperationBase.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))
Update the column span for the table cell that is included into the deleted column.
  Specified by: [updateTableColSpan](../../../commons/table/operations/DeleteColumnOperationBase.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)) in class [DeleteColumnOperationBase](../../../commons/table/operations/DeleteColumnOperationBase.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. spanProvider - The table span provider. The object responsible for providing information about the cell spanning. cell - The table cell. colStartIndex - The new column start index, 1 based. colEndIndex - The new column end index, 1 based. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - When the operation fails. See Also:
        * [DeleteColumnOperationBase.updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement, int, int)](../../../commons/table/operations/DeleteColumnOperationBase.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
