Package [ro.sync.ecss.extensions.commons.table.operations.cals](package-summary.md)

# Class InsertColumnOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.InsertColumnOperationBase](../InsertColumnOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.InsertColumnOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [CALSConstants](CALSConstants.md), [InsertTableCellsContentConstants](../InsertTableCellsContentConstants.md)   Direct Known Subclasses: [InsertColumnOperation](../../../../dita/topic/table/cals/InsertColumnOperation.md), [InsertSingleColumnOperation](InsertSingleColumnOperation.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertColumnOperation extends [InsertColumnOperationBase](../InsertColumnOperationBase.md)implements [CALSConstants](CALSConstants.md), [InsertTableCellsContentConstants](../InsertTableCellsContentConstants.md)
Operation used to insert one or more CALS table columns.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [cellContent](#cellContent)
The fragment that must be introduced in the table cells

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](../InsertColumnOperationBase.md)
 [INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR](../InsertColumnOperationBase.md#INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR), [POSITION_ARGUMENT](../InsertColumnOperationBase.md#POSITION_ARGUMENT), [POSITION_ARGUMENT_DESCRIPTOR](../InsertColumnOperationBase.md#POSITION_ARGUMENT_DESCRIPTOR)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md)
 [ATTRIBUTE_NAME_ALIGN](CALSConstants.md#ATTRIBUTE_NAME_ALIGN), [ATTRIBUTE_NAME_COLNAME](CALSConstants.md#ATTRIBUTE_NAME_COLNAME), [ATTRIBUTE_NAME_COLNUM](CALSConstants.md#ATTRIBUTE_NAME_COLNUM), [ATTRIBUTE_NAME_COLS](CALSConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_COLSEP](CALSConstants.md#ATTRIBUTE_NAME_COLSEP), [ATTRIBUTE_NAME_COLWIDTH](CALSConstants.md#ATTRIBUTE_NAME_COLWIDTH), [ATTRIBUTE_NAME_ID](CALSConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_MOREROWS](CALSConstants.md#ATTRIBUTE_NAME_MOREROWS), [ATTRIBUTE_NAME_NAMEEND](CALSConstants.md#ATTRIBUTE_NAME_NAMEEND), [ATTRIBUTE_NAME_NAMEST](CALSConstants.md#ATTRIBUTE_NAME_NAMEST), [ATTRIBUTE_NAME_ROWSEP](CALSConstants.md#ATTRIBUTE_NAME_ROWSEP), [ATTRIBUTE_NAME_SPANNAME](CALSConstants.md#ATTRIBUTE_NAME_SPANNAME), [ATTRIBUTE_NAME_TABLE_WIDTH](CALSConstants.md#ATTRIBUTE_NAME_TABLE_WIDTH), [ATTRIBUTE_NAME_XML_ID](CALSConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_COLSPEC](CALSConstants.md#ELEMENT_NAME_COLSPEC), [ELEMENT_NAME_ENTRY](CALSConstants.md#ELEMENT_NAME_ENTRY), [ELEMENT_NAME_INFORMALTABLE](CALSConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_ROW](CALSConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_SPANSPEC](CALSConstants.md#ELEMENT_NAME_SPANSPEC), [ELEMENT_NAME_TABLE](CALSConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TGROUP](CALSConstants.md#ELEMENT_NAME_TGROUP)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.[InsertTableCellsContentConstants](../InsertTableCellsContentConstants.md)
 [CELL_FRAGMENT_ARGUMENT](../InsertTableCellsContentConstants.md#CELL_FRAGMENT_ARGUMENT), [CELL_FRAGMENT_ARGUMENT_IN_ARRAY](../InsertTableCellsContentConstants.md#CELL_FRAGMENT_ARGUMENT_IN_ARRAY), [CELL_FRAGMENT_ARGUMENT_NAME](../InsertTableCellsContentConstants.md#CELL_FRAGMENT_ARGUMENT_NAME)
## Constructor Summary
 Constructors
Constructor

Description
 [InsertColumnOperation](#%3Cinit%3E())()
Constructor.
  [InsertColumnOperation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](../AuthorTableHelper.md) tableHelper)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [doOperationInternal](#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../../api/ArgumentsMap.md) args)
Perform the actual operation.
  [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCellElementName](#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../../api/node/AuthorElement.md) row, int newColumnIndex)
Get the name of the element that will be inserted as a cell into the table.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultColWidthValue](#getDefaultColWidthValue())()
Get the default col width value.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultContentForEmptyCells](#getDefaultContentForEmptyCells())()
Get the default content that must be introduced in empty cells.
  protected void [updateColumnCellsSpan](#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../../api/node/AuthorElement.md) tgroup, int newColumnIndex, [TableColumnSpecificationInformation](../../../../api/table/operations/TableColumnSpecificationInformation.md) columnSpecification, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, int noOfColumnsToBeInserted)
Overwrite the base implementation.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](../InsertColumnOperationBase.md)
 [getDescription](../InsertColumnOperationBase.md#getDescription()), [insertColumns](../InsertColumnOperationBase.md#insertColumns(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,boolean,ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase,int,int,ro.sync.ecss.extensions.api.node.AuthorElement)), [insertColumns](../InsertColumnOperationBase.md#insertColumns(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String,int,int)), [performInsertColumn](../InsertColumnOperationBase.md#performInsertColumn(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,boolean,ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase,ro.sync.ecss.extensions.commons.table.operations.InsertTableOperationBase)), [removeMultipleInsertionDescriptor](../InsertColumnOperationBase.md#removeMultipleInsertionDescriptor(ro.sync.ecss.extensions.api.ArgumentDescriptor%5B%5D))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [createEmptyCell](../AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### cellContent

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cellContent

The fragment that must be introduced in the table cells

## Constructor Details

### InsertColumnOperation

public InsertColumnOperation()

Constructor.

### InsertColumnOperation

public InsertColumnOperation([AuthorTableHelper](../AuthorTableHelper.md) tableHelper)

Constructor.
  Parameters: tableHelper - The table helper
## Method Details

### doOperationInternal

protected void doOperationInternal([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from class: [AbstractTableOperation](../AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation.
  Overrides: [doOperationInternal](../InsertColumnOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [InsertColumnOperationBase](../InsertColumnOperationBase.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [InsertColumnOperationBase.doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../InsertColumnOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### updateColumnCellsSpan

protected void updateColumnCellsSpan([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../../api/node/AuthorElement.md) tgroup, int newColumnIndex, [TableColumnSpecificationInformation](../../../../api/table/operations/TableColumnSpecificationInformation.md) columnSpecification, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, int noOfColumnsToBeInserted)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)

Overwrite the base implementation. For CALS tables the column specifications must be updated.
  Overrides: [updateColumnCellsSpan](../InsertColumnOperationBase.md#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int)) in class [InsertColumnOperationBase](../InsertColumnOperationBase.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableSupport - The table cell span provider. tgroup - The table element. newColumnIndex - The index of the column to insert. columnSpecification - The table column specification data. namespace - The namespace to be used. noOfColumnsToBeInserted - The number of columns to be inserted. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - When the insertion fails. See Also:
        * [InsertColumnOperationBase.updateColumnCellsSpan(AuthorAccess, AuthorTableCellSpanProvider, AuthorElement, int, TableColumnSpecificationInformation, String, int)](../InsertColumnOperationBase.md#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int))

### getDefaultColWidthValue

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultColWidthValue()

Get the default col width value. Can be overwritten by an implementor.
  Returns: The default col width value.
### getCellElementName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCellElementName([AuthorElement](../../../../api/node/AuthorElement.md) row, int newColumnIndex)
 Description copied from class: [InsertColumnOperationBase](../InsertColumnOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))
Get the name of the element that will be inserted as a cell into the table.
  Specified by: [getCellElementName](../InsertColumnOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in class [InsertColumnOperationBase](../InsertColumnOperationBase.md) Parameters: row - The row element where the new cell will be inserted. newColumnIndex - The new column index. 0 based. Returns: The name of cell element. See Also:
        * [InsertColumnOperationBase.getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement, int)](../InsertColumnOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))

### getDefaultContentForEmptyCells

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultContentForEmptyCells()
 Description copied from class: [InsertColumnOperationBase](../InsertColumnOperationBase.md#getDefaultContentForEmptyCells())
Get the default content that must be introduced in empty cells.
  Overrides: [getDefaultContentForEmptyCells](../InsertColumnOperationBase.md#getDefaultContentForEmptyCells()) in class [InsertColumnOperationBase](../InsertColumnOperationBase.md) Returns: The default content that must be introduced in empty cells. Default: null. See Also:
        * [InsertColumnOperationBase.getDefaultContentForEmptyCells()](../InsertColumnOperationBase.md#getDefaultContentForEmptyCells())

### getArguments

public [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md)[] getArguments()
  Specified by: [getArguments](../../../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../../../api/AuthorOperation.md) Overrides: [getArguments](../InsertColumnOperationBase.md#getArguments()) in class [InsertColumnOperationBase](../InsertColumnOperationBase.md) Returns: An array of [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [InsertColumnOperationBase.getArguments()](../InsertColumnOperationBase.md#getArguments())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
