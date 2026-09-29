Package [ro.sync.ecss.extensions.commons.table.operations.cals](package-summary.md)

# Class JoinOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.JoinOperationBase](../JoinOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.JoinOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md)   Direct Known Subclasses: [JoinOperation](../../../../dita/topic/table/cals/JoinOperation.md)   @API(type=INTERNAL, src=PUBLIC) public class JoinOperation extends [JoinOperationBase](../JoinOperationBase.md)
Operation for joining the content of selected cells.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[JoinOperationBase](../JoinOperationBase.md)
 [CURSOR_OUTSIDE_THE_TABLE_ERROR_MESSAGE](../JoinOperationBase.md#CURSOR_OUTSIDE_THE_TABLE_ERROR_MESSAGE), [RECTANGULAR_SELECTIONS_ERROR_MESSAGE](../JoinOperationBase.md#RECTANGULAR_SELECTIONS_ERROR_MESSAGE), [SELECT_AT_LEAST_TWO_ADJACENT_CELLS_ERROR_MESSAGE](../JoinOperationBase.md#SELECT_AT_LEAST_TWO_ADJACENT_CELLS_ERROR_MESSAGE)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [JoinOperation](#%3Cinit%3E())()
Constructor.
  [JoinOperation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](../AuthorTableHelper.md) tableHelper)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [generateColumnSpecifications](#generateColumnSpecifications(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSpanSupport, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement)
Generates column specifications for the given table and inserts them into it.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[JoinOperationBase](../JoinOperationBase.md)
 [doOperationInternal](../JoinOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../JoinOperationBase.md#getArguments()), [getDescription](../JoinOperationBase.md#getDescription()), [joinCells](../JoinOperationBase.md#joinCells(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.util.List))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [createEmptyCell](../AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### JoinOperation

public JoinOperation([AuthorTableHelper](../AuthorTableHelper.md) tableHelper)

Constructor.
  Parameters: tableHelper - The table helper
### JoinOperation

public JoinOperation()

Constructor.

## Method Details

### generateColumnSpecifications

protected void generateColumnSpecifications([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSpanSupport, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)

Generates column specifications for the given table and inserts them into it.
  Specified by: [generateColumnSpecifications](../JoinOperationBase.md#generateColumnSpecifications(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement)) in class [JoinOperationBase](../JoinOperationBase.md) Parameters: authorAccess - Access. tableSpanSupport - Span support. tableElement - The table element. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - Failed to insert the column specifications into the table.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
