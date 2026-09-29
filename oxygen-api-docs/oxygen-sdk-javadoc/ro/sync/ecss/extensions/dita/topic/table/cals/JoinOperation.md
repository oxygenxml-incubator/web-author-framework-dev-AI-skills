Package [ro.sync.ecss.extensions.dita.topic.table.cals](package-summary.md)

# Class JoinOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.JoinOperationBase](../../../../commons/table/operations/JoinOperationBase.md)
            * [ro.sync.ecss.extensions.commons.table.operations.cals.JoinOperation](../../../../commons/table/operations/cals/JoinOperation.md)
                * ro.sync.ecss.extensions.dita.topic.table.cals.JoinOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class JoinOperation extends [JoinOperation](../../../../commons/table/operations/cals/JoinOperation.md)
Operation for joining the content of selected cells.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[JoinOperationBase](../../../../commons/table/operations/JoinOperationBase.md)
 [CURSOR_OUTSIDE_THE_TABLE_ERROR_MESSAGE](../../../../commons/table/operations/JoinOperationBase.md#CURSOR_OUTSIDE_THE_TABLE_ERROR_MESSAGE), [RECTANGULAR_SELECTIONS_ERROR_MESSAGE](../../../../commons/table/operations/JoinOperationBase.md#RECTANGULAR_SELECTIONS_ERROR_MESSAGE), [SELECT_AT_LEAST_TWO_ADJACENT_CELLS_ERROR_MESSAGE](../../../../commons/table/operations/JoinOperationBase.md#SELECT_AT_LEAST_TWO_ADJACENT_CELLS_ERROR_MESSAGE)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../../../../commons/table/operations/AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../../../../commons/table/operations/AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [JoinOperation](#%3Cinit%3E())()
Constructor.
  [JoinOperation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) tableHelper)
Constructor.

## Method Summary

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.cals.[JoinOperation](../../../../commons/table/operations/cals/JoinOperation.md)
 [generateColumnSpecifications](../../../../commons/table/operations/cals/JoinOperation.md#generateColumnSpecifications(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[JoinOperationBase](../../../../commons/table/operations/JoinOperationBase.md)
 [doOperationInternal](../../../../commons/table/operations/JoinOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../../commons/table/operations/JoinOperationBase.md#getArguments()), [getDescription](../../../../commons/table/operations/JoinOperationBase.md#getDescription()), [joinCells](../../../../commons/table/operations/JoinOperationBase.md#joinCells(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.util.List))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
 [createEmptyCell](../../../../commons/table/operations/AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../../../../commons/table/operations/AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../../../../commons/table/operations/AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../../../../commons/table/operations/AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../../../../commons/table/operations/AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../../../../commons/table/operations/AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### JoinOperation

public JoinOperation()

Constructor.

### JoinOperation

public JoinOperation([AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) tableHelper)

Constructor.
  Parameters: tableHelper - The table helper.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
