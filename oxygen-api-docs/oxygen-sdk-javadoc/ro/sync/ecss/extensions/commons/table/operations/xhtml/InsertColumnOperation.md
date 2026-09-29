Package [ro.sync.ecss.extensions.commons.table.operations.xhtml](package-summary.md)

# Class InsertColumnOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.InsertColumnOperationBase](../InsertColumnOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.xhtml.InsertColumnOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [XHTMLConstants](XHTMLConstants.md)   Direct Known Subclasses: [InsertSingleColumnOperation](InsertSingleColumnOperation.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertColumnOperation extends [InsertColumnOperationBase](../InsertColumnOperationBase.md)implements [XHTMLConstants](XHTMLConstants.md)
Operation used to insert one or more XHTML table columns.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](../InsertColumnOperationBase.md)
 [INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR](../InsertColumnOperationBase.md#INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR), [POSITION_ARGUMENT](../InsertColumnOperationBase.md#POSITION_ARGUMENT), [POSITION_ARGUMENT_DESCRIPTOR](../InsertColumnOperationBase.md#POSITION_ARGUMENT_DESCRIPTOR)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.xhtml.[XHTMLConstants](XHTMLConstants.md)
 [ATTRIBUTE_NAME_COLSPAN](XHTMLConstants.md#ATTRIBUTE_NAME_COLSPAN), [ATTRIBUTE_NAME_ID](XHTMLConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_ROWSPAN](XHTMLConstants.md#ATTRIBUTE_NAME_ROWSPAN), [ATTRIBUTE_NAME_XML_ID](XHTMLConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_INFORMALTABLE](XHTMLConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_TABLE](XHTMLConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TD](XHTMLConstants.md#ELEMENT_NAME_TD), [ELEMENT_NAME_TH](XHTMLConstants.md#ELEMENT_NAME_TH), [ELEMENT_NAME_TR](XHTMLConstants.md#ELEMENT_NAME_TR)
## Constructor Summary
 Constructors
Modifier

Constructor

Description
   [InsertColumnOperation](#%3Cinit%3E())()
Constructor.
  protected  [InsertColumnOperation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](../AuthorTableHelper.md) documentTypeHelper)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCellElementName](#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../../api/node/AuthorElement.md) rowElement, int newColumnIndex)
Get the name of the element that will be inserted as a cell into the table.
  protected void [updateColumnCellsSpan](#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../../api/node/AuthorElement.md) tableElem, int newColumnIndex, [TableColumnSpecificationInformation](../../../../api/table/operations/TableColumnSpecificationInformation.md) columnSpecification, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, int noOfColumnsToBeInserted)
Increments the column span of the cells intersecting the new column.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](../InsertColumnOperationBase.md)
 [doOperationInternal](../InsertColumnOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../InsertColumnOperationBase.md#getArguments()), [getDefaultContentForEmptyCells](../InsertColumnOperationBase.md#getDefaultContentForEmptyCells()), [getDescription](../InsertColumnOperationBase.md#getDescription()), [insertColumns](../InsertColumnOperationBase.md#insertColumns(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,boolean,ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase,int,int,ro.sync.ecss.extensions.api.node.AuthorElement)), [insertColumns](../InsertColumnOperationBase.md#insertColumns(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String,int,int)), [performInsertColumn](../InsertColumnOperationBase.md#performInsertColumn(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,boolean,ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase,ro.sync.ecss.extensions.commons.table.operations.InsertTableOperationBase)), [removeMultipleInsertionDescriptor](../InsertColumnOperationBase.md#removeMultipleInsertionDescriptor(ro.sync.ecss.extensions.api.ArgumentDescriptor%5B%5D))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [createEmptyCell](../AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### InsertColumnOperation

public InsertColumnOperation()

Constructor.

### InsertColumnOperation

protected InsertColumnOperation([AuthorTableHelper](../AuthorTableHelper.md) documentTypeHelper)

Constructor.
  Parameters: documentTypeHelper - Document type helper, has methods specific to a document type.
## Method Details

### getCellElementName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCellElementName([AuthorElement](../../../../api/node/AuthorElement.md) rowElement, int newColumnIndex)
 Description copied from class: [InsertColumnOperationBase](../InsertColumnOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))
Get the name of the element that will be inserted as a cell into the table.
  Specified by: [getCellElementName](../InsertColumnOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in class [InsertColumnOperationBase](../InsertColumnOperationBase.md) Parameters: rowElement - The row element where the new cell will be inserted. newColumnIndex - The new column index. 0 based. Returns: The name of cell element. See Also:
        * [InsertColumnOperationBase.getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement, int)](../InsertColumnOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))

### updateColumnCellsSpan

protected void updateColumnCellsSpan([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../../api/node/AuthorElement.md) tableElem, int newColumnIndex, [TableColumnSpecificationInformation](../../../../api/table/operations/TableColumnSpecificationInformation.md) columnSpecification, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, int noOfColumnsToBeInserted)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from class: [InsertColumnOperationBase](../InsertColumnOperationBase.md#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int))
Increments the column span of the cells intersecting the new column. A cell intersects the column to insert if its start column index is less than the new column index and the end column index of the cell is greater or equal than the new column (startColSpan < newColumnIndex && endColSpan >= newColumnIndex).
  Overrides: [updateColumnCellsSpan](../InsertColumnOperationBase.md#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int)) in class [InsertColumnOperationBase](../InsertColumnOperationBase.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableSupport - The table cell span provider. tableElem - The table element. newColumnIndex - The index of the column to insert. columnSpecification - The table column specification data. namespace - The namespace to be used. noOfColumnsToBeInserted - The number of columns to be inserted. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - When the insertion fails. See Also:
        * [InsertColumnOperationBase.updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement, int, ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation, java.lang.String, int)](../InsertColumnOperationBase.md#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
