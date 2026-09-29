Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class InsertColumnOperationBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](AbstractTableOperation.md)
        * ro.sync.ecss.extensions.commons.table.operations.InsertColumnOperationBase
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   Direct Known Subclasses: [InsertColumnOperation](cals/InsertColumnOperation.md), [InsertColumnOperation](xhtml/InsertColumnOperation.md), [InsertColumnOperation](../../../dita/map/table/InsertColumnOperation.md), [InsertColumnOperation](../../../dita/topic/table/simpletable/InsertColumnOperation.md), [InsertColumnOperation](../../../tei/table/InsertColumnOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class InsertColumnOperationBase extends [AbstractTableOperation](AbstractTableOperation.md)
Operation used to insert a table column.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) [INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR](#INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR)
The insertMultipleColumns argument descriptor.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [POSITION_ARGUMENT](#POSITION_ARGUMENT)
The insertPosition argument descriptor.
  static final [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) [POSITION_ARGUMENT_DESCRIPTOR](#POSITION_ARGUMENT_DESCRIPTOR)
The position argument descriptor.

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [InsertColumnOperationBase](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](AuthorTableHelper.md) documentTypeHelper)
Constructor.

## Method Summary
  All MethodsStatic MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [doOperationInternal](#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)
Perform the actual operation.
  [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCellElementName](#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../api/node/AuthorElement.md) rowElement, int newColumnIndex)
Get the name of the element that will be inserted as a cell into the table.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultContentForEmptyCells](#getDefaultContentForEmptyCells())()
Get the default content that must be introduced in empty cells.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()
Get the description for this operation.
  void [insertColumns](#insertColumns(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,boolean,ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase,int,int,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertPosition, [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)[] fragments, [TableColumnSpecificationInformation](../../../api/table/operations/TableColumnSpecificationInformation.md) columnSpecification, boolean cellsFragments, [InsertRowOperationBase](InsertRowOperationBase.md) insertRowOperation, int caretOffset, int noOfColumnsToBeInserted, [AuthorElement](../../../api/node/AuthorElement.md) tableElement)
Insert columns in a table
  void [insertColumns](#insertColumns(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertPosition, int caretOffset, int noOfColumnsToBeInserted)
Insert columns in a table
  void [performInsertColumn](#performInsertColumn(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,boolean,ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase,ro.sync.ecss.extensions.commons.table.operations.InsertTableOperationBase))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)[] fragments, [TableColumnSpecificationInformation](../../../api/table/operations/TableColumnSpecificationInformation.md) columnSpecification, boolean cellsFragments, [InsertRowOperationBase](InsertRowOperationBase.md) insertRowOperation, [InsertTableOperationBase](InsertTableOperationBase.md) insertTableOperation)
Insert column.
  protected static [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [removeMultipleInsertionDescriptor](#removeMultipleInsertionDescriptor(ro.sync.ecss.extensions.api.ArgumentDescriptor%5B%5D))([ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] superArguments)
Removes the argument descriptor for multiple insertion from an arguments list.
  protected void [updateColumnCellsSpan](#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../api/node/AuthorElement.md) tableElem, int newColumnIndex, [TableColumnSpecificationInformation](../../../api/table/operations/TableColumnSpecificationInformation.md) columnSpecification, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, int noOfColumnsToBeInserted)
Increments the column span of the cells intersecting the new column.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md)
 [createEmptyCell](AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### POSITION_ARGUMENT

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) POSITION_ARGUMENT

The insertPosition argument descriptor.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.InsertColumnOperationBase.POSITION_ARGUMENT)

### INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR

public static final [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR

The insertMultipleColumns argument descriptor.

### POSITION_ARGUMENT_DESCRIPTOR

public static final [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) POSITION_ARGUMENT_DESCRIPTOR

The position argument descriptor.

## Constructor Details

### InsertColumnOperationBase

public InsertColumnOperationBase([AuthorTableHelper](AuthorTableHelper.md) documentTypeHelper)

Constructor.
  Parameters: documentTypeHelper - Document type helper, has methods specific to a document type.
## Method Details

### doOperationInternal

protected void doOperationInternal([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from class: [AbstractTableOperation](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation.
  Specified by: [doOperationInternal](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [AbstractTableOperation](AbstractTableOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AbstractTableOperation.doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### performInsertColumn

public void performInsertColumn([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)[] fragments, [TableColumnSpecificationInformation](../../../api/table/operations/TableColumnSpecificationInformation.md) columnSpecification, boolean cellsFragments, [InsertRowOperationBase](InsertRowOperationBase.md) insertRowOperation, [InsertTableOperationBase](InsertTableOperationBase.md) insertTableOperation)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Insert column.
  Parameters: authorAccess - The author access. namespace - The cells namespace. fragments - An array of AuthorDocumentFragments that are used as content of the inserted cells. columnSpecification - The column specification data. cellsFragments - If the value is true then the fragments where originally cells. insertRowOperation - The insert row operation used to insert new rows when there are fragments that cannot be inserted in the new column. insertTableOperation - The insert table operation used to insert the column wrapped in a new table when the insert offset is not inside a table. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) [AuthorOperationException](../../../api/AuthorOperationException.md)
### insertColumns

public void insertColumns([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertPosition, int caretOffset, int noOfColumnsToBeInserted)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [AuthorOperationException](../../../api/AuthorOperationException.md)

Insert columns in a table
  Parameters: authorAccess - The author access. tableElement - The table element. namespace - The table elements namespace. insertPosition - The insert position. One of [AuthorConstants.POSITION_AFTER](../../../api/AuthorConstants.md#POSITION_AFTER) or [AuthorConstants.POSITION_BEFORE](../../../api/AuthorConstants.md#POSITION_BEFORE) constants. caretOffset - The caret offset. noOfColumnsToBeInserted - The number of columns to be inserted. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [AuthorOperationException](../../../api/AuthorOperationException.md)
### insertColumns

public void insertColumns([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertPosition, [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)[] fragments, [TableColumnSpecificationInformation](../../../api/table/operations/TableColumnSpecificationInformation.md) columnSpecification, boolean cellsFragments, [InsertRowOperationBase](InsertRowOperationBase.md) insertRowOperation, int caretOffset, int noOfColumnsToBeInserted, [AuthorElement](../../../api/node/AuthorElement.md) tableElement)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [AuthorOperationException](../../../api/AuthorOperationException.md)

Insert columns in a table
  Parameters: authorAccess - The author access. namespace - The table elements namespace. insertPosition - The insert position. One of [AuthorConstants.POSITION_AFTER](../../../api/AuthorConstants.md#POSITION_AFTER) or [AuthorConstants.POSITION_BEFORE](../../../api/AuthorConstants.md#POSITION_BEFORE) constants. fragments - The fragments to be inserted in cells columnSpecification - Column specification information cellsFragments - If the value is true then the fragments where originally cells. insertRowOperation - Insert row operation. caretOffset - The caret offset. noOfColumnsToBeInserted - The number of columns to be inserted. tableElement - The table element. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [AuthorOperationException](../../../api/AuthorOperationException.md)
### updateColumnCellsSpan

protected void updateColumnCellsSpan([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../api/node/AuthorElement.md) tableElem, int newColumnIndex, [TableColumnSpecificationInformation](../../../api/table/operations/TableColumnSpecificationInformation.md) columnSpecification, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, int noOfColumnsToBeInserted)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Increments the column span of the cells intersecting the new column. A cell intersects the column to insert if its start column index is less than the new column index and the end column index of the cell is greater or equal than the new column (startColSpan < newColumnIndex && endColSpan >= newColumnIndex).
  Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableSupport - The table cell span provider. tableElem - The table element. newColumnIndex - The index of the column to insert. columnSpecification - The table column specification data. namespace - The namespace to be used. noOfColumnsToBeInserted - The number of columns to be inserted. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - When the insertion fails.
### getArguments

public [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] getArguments()
  Returns: An array of [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments())

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()

Get the description for this operation.
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

### getCellElementName

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCellElementName([AuthorElement](../../../api/node/AuthorElement.md) rowElement, int newColumnIndex)

Get the name of the element that will be inserted as a cell into the table.
  Parameters: rowElement - The row element where the new cell will be inserted. newColumnIndex - The new column index. 0 based. Returns: The name of cell element.
### getDefaultContentForEmptyCells

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultContentForEmptyCells()

Get the default content that must be introduced in empty cells.
  Returns: The default content that must be introduced in empty cells. Default: null. Since: 14.1
### removeMultipleInsertionDescriptor

protected static [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] removeMultipleInsertionDescriptor([ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] superArguments)

Removes the argument descriptor for multiple insertion from an arguments list.
  Parameters: superArguments - The input arguments list. Returns: The filtered arguments list.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
