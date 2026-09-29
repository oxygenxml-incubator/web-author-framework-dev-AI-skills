Package [ro.sync.ecss.extensions.dita.topic.table.simpletable](package-summary.md)

# Class InsertColumnOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md)
            * ro.sync.ecss.extensions.dita.topic.table.simpletable.InsertColumnOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [InsertTableCellsContentConstants](../../../../commons/table/operations/InsertTableCellsContentConstants.md), [SimpleTableConstants](SimpleTableConstants.md)   Direct Known Subclasses: [InsertSingleColumnOperation](InsertSingleColumnOperation.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertColumnOperation extends [InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md)implements [SimpleTableConstants](SimpleTableConstants.md), [InsertTableCellsContentConstants](../../../../commons/table/operations/InsertTableCellsContentConstants.md)
Operation used to insert one or more DITA simple table columns.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [cellContent](#cellContent)
The fragment that must be introduced in the table cells

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md)
 [INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR](../../../../commons/table/operations/InsertColumnOperationBase.md#INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR), [POSITION_ARGUMENT](../../../../commons/table/operations/InsertColumnOperationBase.md#POSITION_ARGUMENT), [POSITION_ARGUMENT_DESCRIPTOR](../../../../commons/table/operations/InsertColumnOperationBase.md#POSITION_ARGUMENT_DESCRIPTOR)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../../../../commons/table/operations/AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../../../../commons/table/operations/AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.[InsertTableCellsContentConstants](../../../../commons/table/operations/InsertTableCellsContentConstants.md)
 [CELL_FRAGMENT_ARGUMENT](../../../../commons/table/operations/InsertTableCellsContentConstants.md#CELL_FRAGMENT_ARGUMENT), [CELL_FRAGMENT_ARGUMENT_IN_ARRAY](../../../../commons/table/operations/InsertTableCellsContentConstants.md#CELL_FRAGMENT_ARGUMENT_IN_ARRAY), [CELL_FRAGMENT_ARGUMENT_NAME](../../../../commons/table/operations/InsertTableCellsContentConstants.md#CELL_FRAGMENT_ARGUMENT_NAME)
### Fields inherited from interface ro.sync.ecss.extensions.dita.topic.table.simpletable.[SimpleTableConstants](SimpleTableConstants.md)
 [ATTRIBUTE_NAME_ID](SimpleTableConstants.md#ATTRIBUTE_NAME_ID), [ELEMENT_NAME_CHDESC_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHDESC_CHOICETABLE), [ELEMENT_NAME_CHDESCHD_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHDESCHD_CHOICETABLE), [ELEMENT_NAME_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHOICETABLE), [ELEMENT_NAME_CHOPTION_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHOPTION_CHOICETABLE), [ELEMENT_NAME_CHOPTIONHD_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHOPTIONHD_CHOICETABLE), [ELEMENT_NAME_ENTRY_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_ENTRY_SIMPLETABLE), [ELEMENT_NAME_HEADER_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_HEADER_CHOICETABLE), [ELEMENT_NAME_HEADER_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_HEADER_PROPERTIES), [ELEMENT_NAME_HEADER_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_HEADER_SIMPLETABLE), [ELEMENT_NAME_PROPDESC_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPDESC_PROPERTIES), [ELEMENT_NAME_PROPDESCHD_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPDESCHD_PROPERTIES), [ELEMENT_NAME_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPERTIES), [ELEMENT_NAME_PROPTYPE_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPTYPE_PROPERTIES), [ELEMENT_NAME_PROPTYPEHD_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPTYPEHD_PROPERTIES), [ELEMENT_NAME_PROPVALUE_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPVALUE_PROPERTIES), [ELEMENT_NAME_PROPVALUEHD_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPVALUEHD_PROPERTIES), [ELEMENT_NAME_ROW_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_ROW_CHOICETABLE), [ELEMENT_NAME_ROW_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_ROW_PROPERTIES), [ELEMENT_NAME_ROW_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_ROW_SIMPLETABLE), [ELEMENT_NAME_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_SIMPLETABLE)
## Constructor Summary
 Constructors
Modifier

Constructor

Description
   [InsertColumnOperation](#%3Cinit%3E())()
Constructor.
  protected  [InsertColumnOperation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) documentTypeHelper)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [doOperationInternal](#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../../api/ArgumentsMap.md) args)
Perform the actual operation.
  [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCellElementName](#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../../api/node/AuthorElement.md) rowElement, int newColumnIndex)
Get the name of the element that will be inserted as a cell into the table.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultContentForEmptyCells](#getDefaultContentForEmptyCells())()
Get the default content that must be introduced in empty cells.
  protected void [updateColumnCellsSpan](#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../../api/node/AuthorElement.md) tableElem, int newColumnIndex, [TableColumnSpecificationInformation](../../../../api/table/operations/TableColumnSpecificationInformation.md) columnSpecification, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, int noOfColumnsToBeInserted)
Increments the column span of the cells intersecting the new column.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md)
 [getDescription](../../../../commons/table/operations/InsertColumnOperationBase.md#getDescription()), [insertColumns](../../../../commons/table/operations/InsertColumnOperationBase.md#insertColumns(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,boolean,ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase,int,int,ro.sync.ecss.extensions.api.node.AuthorElement)), [insertColumns](../../../../commons/table/operations/InsertColumnOperationBase.md#insertColumns(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String,int,int)), [performInsertColumn](../../../../commons/table/operations/InsertColumnOperationBase.md#performInsertColumn(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,boolean,ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase,ro.sync.ecss.extensions.commons.table.operations.InsertTableOperationBase)), [removeMultipleInsertionDescriptor](../../../../commons/table/operations/InsertColumnOperationBase.md#removeMultipleInsertionDescriptor(ro.sync.ecss.extensions.api.ArgumentDescriptor%5B%5D))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
 [createEmptyCell](../../../../commons/table/operations/AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../../../../commons/table/operations/AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../../../../commons/table/operations/AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../../../../commons/table/operations/AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../../../../commons/table/operations/AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../../../../commons/table/operations/AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
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

protected InsertColumnOperation([AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) documentTypeHelper)

Constructor.
  Parameters: documentTypeHelper - Document type helper, has methods specific to a document type.
## Method Details

### doOperationInternal

protected void doOperationInternal([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from class: [AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation.
  Overrides: [doOperationInternal](../../../../commons/table/operations/InsertColumnOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [InsertColumnOperationBase.doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../../../../commons/table/operations/InsertColumnOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### getCellElementName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCellElementName([AuthorElement](../../../../api/node/AuthorElement.md) rowElement, int newColumnIndex)
 Description copied from class: [InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))
Get the name of the element that will be inserted as a cell into the table.
  Specified by: [getCellElementName](../../../../commons/table/operations/InsertColumnOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in class [InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md) Parameters: rowElement - The row element where the new cell will be inserted. newColumnIndex - The new column index. 0 based. Returns: The name of cell element. See Also:
        * [InsertColumnOperationBase.getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement, int)](../../../../commons/table/operations/InsertColumnOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))

### getDefaultContentForEmptyCells

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultContentForEmptyCells()
 Description copied from class: [InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md#getDefaultContentForEmptyCells())
Get the default content that must be introduced in empty cells.
  Overrides: [getDefaultContentForEmptyCells](../../../../commons/table/operations/InsertColumnOperationBase.md#getDefaultContentForEmptyCells()) in class [InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md) Returns: The default content that must be introduced in empty cells. Default: null. See Also:
        * [InsertColumnOperationBase.getDefaultContentForEmptyCells()](../../../../commons/table/operations/InsertColumnOperationBase.md#getDefaultContentForEmptyCells())

### getArguments

public [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md)[] getArguments()
  Specified by: [getArguments](../../../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../../../api/AuthorOperation.md) Overrides: [getArguments](../../../../commons/table/operations/InsertColumnOperationBase.md#getArguments()) in class [InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md) Returns: An array of [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [InsertColumnOperationBase.getArguments()](../../../../commons/table/operations/InsertColumnOperationBase.md#getArguments())

### updateColumnCellsSpan

protected void updateColumnCellsSpan([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../../api/node/AuthorElement.md) tableElem, int newColumnIndex, [TableColumnSpecificationInformation](../../../../api/table/operations/TableColumnSpecificationInformation.md) columnSpecification, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, int noOfColumnsToBeInserted)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from class: [InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int))
Increments the column span of the cells intersecting the new column. A cell intersects the column to insert if its start column index is less than the new column index and the end column index of the cell is greater or equal than the new column (startColSpan < newColumnIndex && endColSpan >= newColumnIndex).
  Overrides: [updateColumnCellsSpan](../../../../commons/table/operations/InsertColumnOperationBase.md#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int)) in class [InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableSupport - The table cell span provider. tableElem - The table element. newColumnIndex - The index of the column to insert. columnSpecification - The table column specification data. namespace - The namespace to be used. noOfColumnsToBeInserted - The number of columns to be inserted. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - When the insertion fails. See Also:
        * [InsertColumnOperationBase.updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement, int, ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation, java.lang.String, int)](../../../../commons/table/operations/InsertColumnOperationBase.md#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
