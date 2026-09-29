Package [ro.sync.ecss.extensions.tei.table](package-summary.md)

# Class InsertColumnOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../../commons/table/operations/AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.InsertColumnOperationBase](../../commons/table/operations/InsertColumnOperationBase.md)
            * ro.sync.ecss.extensions.tei.table.InsertColumnOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md), [TEIConstants](TEIConstants.md)   Direct Known Subclasses: [InsertSingleColumnOperation](InsertSingleColumnOperation.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertColumnOperation extends [InsertColumnOperationBase](../../commons/table/operations/InsertColumnOperationBase.md)implements [TEIConstants](TEIConstants.md)
Operation used to insert a TEI table column.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](../../commons/table/operations/InsertColumnOperationBase.md)
 [INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR](../../commons/table/operations/InsertColumnOperationBase.md#INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR), [POSITION_ARGUMENT](../../commons/table/operations/InsertColumnOperationBase.md#POSITION_ARGUMENT), [POSITION_ARGUMENT_DESCRIPTOR](../../commons/table/operations/InsertColumnOperationBase.md#POSITION_ARGUMENT_DESCRIPTOR)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../commons/table/operations/AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../../commons/table/operations/AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../../commons/table/operations/AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.tei.table.[TEIConstants](TEIConstants.md)
 [ATTRIBUTE_NAME_COLS](TEIConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_ID](TEIConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_ROWS](TEIConstants.md#ATTRIBUTE_NAME_ROWS), [ATTRIBUTE_NAME_XML_ID](TEIConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_CELL](TEIConstants.md#ELEMENT_NAME_CELL), [ELEMENT_NAME_ROW](TEIConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_TABLE](TEIConstants.md#ELEMENT_NAME_TABLE)
## Constructor Summary
 Constructors
Constructor

Description
 [InsertColumnOperation](#%3Cinit%3E())()
Constructor.
  [InsertColumnOperation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](../../commons/table/operations/AuthorTableHelper.md) tableHelper)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCellElementName](#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../api/node/AuthorElement.md) rowElement, int newColumnIndex)
Get the name of the element that will be inserted as a cell into the table.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](../../commons/table/operations/InsertColumnOperationBase.md)
 [doOperationInternal](../../commons/table/operations/InsertColumnOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../commons/table/operations/InsertColumnOperationBase.md#getArguments()), [getDefaultContentForEmptyCells](../../commons/table/operations/InsertColumnOperationBase.md#getDefaultContentForEmptyCells()), [getDescription](../../commons/table/operations/InsertColumnOperationBase.md#getDescription()), [insertColumns](../../commons/table/operations/InsertColumnOperationBase.md#insertColumns(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,boolean,ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase,int,int,ro.sync.ecss.extensions.api.node.AuthorElement)), [insertColumns](../../commons/table/operations/InsertColumnOperationBase.md#insertColumns(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String,int,int)), [performInsertColumn](../../commons/table/operations/InsertColumnOperationBase.md#performInsertColumn(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,boolean,ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase,ro.sync.ecss.extensions.commons.table.operations.InsertTableOperationBase)), [removeMultipleInsertionDescriptor](../../commons/table/operations/InsertColumnOperationBase.md#removeMultipleInsertionDescriptor(ro.sync.ecss.extensions.api.ArgumentDescriptor%5B%5D)), [updateColumnCellsSpan](../../commons/table/operations/InsertColumnOperationBase.md#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../commons/table/operations/AbstractTableOperation.md)
 [createEmptyCell](../../commons/table/operations/AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../../commons/table/operations/AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../../commons/table/operations/AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../../commons/table/operations/AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../../commons/table/operations/AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../../commons/table/operations/AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### InsertColumnOperation

public InsertColumnOperation()

Constructor.

### InsertColumnOperation

public InsertColumnOperation([AuthorTableHelper](../../commons/table/operations/AuthorTableHelper.md) tableHelper)

Constructor.
  Parameters: tableHelper - The table helper.
## Method Details

### getCellElementName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCellElementName([AuthorElement](../../api/node/AuthorElement.md) rowElement, int newColumnIndex)
 Description copied from class: [InsertColumnOperationBase](../../commons/table/operations/InsertColumnOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))
Get the name of the element that will be inserted as a cell into the table.
  Specified by: [getCellElementName](../../commons/table/operations/InsertColumnOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in class [InsertColumnOperationBase](../../commons/table/operations/InsertColumnOperationBase.md) Parameters: rowElement - The row element where the new cell will be inserted. newColumnIndex - The new column index. 0 based. Returns: The name of cell element. See Also:
        * [InsertColumnOperationBase.getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement, int)](../../commons/table/operations/InsertColumnOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
