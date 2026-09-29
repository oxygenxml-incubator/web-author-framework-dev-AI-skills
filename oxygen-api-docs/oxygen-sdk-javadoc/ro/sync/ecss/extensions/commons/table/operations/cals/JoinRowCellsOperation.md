Package [ro.sync.ecss.extensions.commons.table.operations.cals](package-summary.md)

# Class JoinRowCellsOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.JoinRowCellsOperationBase](../JoinRowCellsOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.JoinRowCellsOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [CALSConstants](CALSConstants.md)   Direct Known Subclasses: [JoinRowCellsOperation](../../../../dita/topic/table/cals/JoinRowCellsOperation.md)   @API(type=INTERNAL, src=PUBLIC) public class JoinRowCellsOperation extends [JoinRowCellsOperationBase](../JoinRowCellsOperationBase.md)implements [CALSConstants](CALSConstants.md)
This is the CALS tables implementation of the operation used to join the content of two or more cells from the same table row. If selection exists, the cell at selection start offset determines the destination cell where the content of the next cells will be moved. If there is no selection, then the caret must be between two table cells. The operation modifies the namest and nameendattributes of the destination cell.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md)
 [ATTRIBUTE_NAME_ALIGN](CALSConstants.md#ATTRIBUTE_NAME_ALIGN), [ATTRIBUTE_NAME_COLNAME](CALSConstants.md#ATTRIBUTE_NAME_COLNAME), [ATTRIBUTE_NAME_COLNUM](CALSConstants.md#ATTRIBUTE_NAME_COLNUM), [ATTRIBUTE_NAME_COLS](CALSConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_COLSEP](CALSConstants.md#ATTRIBUTE_NAME_COLSEP), [ATTRIBUTE_NAME_COLWIDTH](CALSConstants.md#ATTRIBUTE_NAME_COLWIDTH), [ATTRIBUTE_NAME_ID](CALSConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_MOREROWS](CALSConstants.md#ATTRIBUTE_NAME_MOREROWS), [ATTRIBUTE_NAME_NAMEEND](CALSConstants.md#ATTRIBUTE_NAME_NAMEEND), [ATTRIBUTE_NAME_NAMEST](CALSConstants.md#ATTRIBUTE_NAME_NAMEST), [ATTRIBUTE_NAME_ROWSEP](CALSConstants.md#ATTRIBUTE_NAME_ROWSEP), [ATTRIBUTE_NAME_SPANNAME](CALSConstants.md#ATTRIBUTE_NAME_SPANNAME), [ATTRIBUTE_NAME_TABLE_WIDTH](CALSConstants.md#ATTRIBUTE_NAME_TABLE_WIDTH), [ATTRIBUTE_NAME_XML_ID](CALSConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_COLSPEC](CALSConstants.md#ELEMENT_NAME_COLSPEC), [ELEMENT_NAME_ENTRY](CALSConstants.md#ELEMENT_NAME_ENTRY), [ELEMENT_NAME_INFORMALTABLE](CALSConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_ROW](CALSConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_SPANSPEC](CALSConstants.md#ELEMENT_NAME_SPANSPEC), [ELEMENT_NAME_TABLE](CALSConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TGROUP](CALSConstants.md#ELEMENT_NAME_TGROUP)
## Constructor Summary
 Constructors
Constructor

Description
 [JoinRowCellsOperation](#%3Cinit%3E())()
Constructor.
  [JoinRowCellsOperation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](../AuthorTableHelper.md) tableHelper)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [generateColumnSpecifications](#generateColumnSpecifications(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSpanSupport, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement)
Generates column specifications for the given table and inserts them into it.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[JoinRowCellsOperationBase](../JoinRowCellsOperationBase.md)
 [doOperationInternal](../JoinRowCellsOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../JoinRowCellsOperationBase.md#getArguments()), [getCell](../JoinRowCellsOperationBase.md#getCell(ro.sync.ecss.extensions.api.AuthorAccess,int,boolean)), [getDescription](../JoinRowCellsOperationBase.md#getDescription())
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [createEmptyCell](../AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### JoinRowCellsOperation

public JoinRowCellsOperation([AuthorTableHelper](../AuthorTableHelper.md) tableHelper)

Constructor.
  Parameters: tableHelper - The table helper
### JoinRowCellsOperation

public JoinRowCellsOperation()

Constructor.

## Method Details

### generateColumnSpecifications

protected void generateColumnSpecifications([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSpanSupport, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)

Generates column specifications for the given table and inserts them into it.
  Specified by: [generateColumnSpecifications](../JoinRowCellsOperationBase.md#generateColumnSpecifications(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement)) in class [JoinRowCellsOperationBase](../JoinRowCellsOperationBase.md) Parameters: authorAccess - Access. tableSpanSupport - Span support. tableElement - The table element. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - Failed to insert the column specifications into the table.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
