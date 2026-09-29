Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class JoinOperationBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](AbstractTableOperation.md)
        * ro.sync.ecss.extensions.commons.table.operations.JoinOperationBase
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   Direct Known Subclasses: [JoinOperation](cals/JoinOperation.md), [JoinOperation](xhtml/JoinOperation.md), [JoinOperation](../../../tei/table/JoinOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class JoinOperationBase extends [AbstractTableOperation](AbstractTableOperation.md)
Operation for joining the content of selected cells.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CURSOR_OUTSIDE_THE_TABLE_ERROR_MESSAGE](#CURSOR_OUTSIDE_THE_TABLE_ERROR_MESSAGE)
Cursor outlide the table error message
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [RECTANGULAR_SELECTIONS_ERROR_MESSAGE](#RECTANGULAR_SELECTIONS_ERROR_MESSAGE)
Rectangular selection error message
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SELECT_AT_LEAST_TWO_ADJACENT_CELLS_ERROR_MESSAGE](#SELECT_AT_LEAST_TWO_ADJACENT_CELLS_ERROR_MESSAGE)
Select at least two adjacent cells

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [JoinOperationBase](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](AuthorTableHelper.md) tableHelper)
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [doOperationInternal](#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)
Join the contents of selected cells.
  protected abstract void [generateColumnSpecifications](#generateColumnSpecifications(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) tableCellSpanProvider, [AuthorElement](../../../api/node/AuthorElement.md) tableElement)
Generates column specifications for the given table and inserts them into the document.
  [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 void [joinCells](#joinCells(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.util.List))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> cellElements)
Join table cells.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md)
 [createEmptyCell](AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### CURSOR_OUTSIDE_THE_TABLE_ERROR_MESSAGE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CURSOR_OUTSIDE_THE_TABLE_ERROR_MESSAGE

Cursor outlide the table error message
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.JoinOperationBase.CURSOR_OUTSIDE_THE_TABLE_ERROR_MESSAGE)

### SELECT_AT_LEAST_TWO_ADJACENT_CELLS_ERROR_MESSAGE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SELECT_AT_LEAST_TWO_ADJACENT_CELLS_ERROR_MESSAGE

Select at least two adjacent cells
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.JoinOperationBase.SELECT_AT_LEAST_TWO_ADJACENT_CELLS_ERROR_MESSAGE)

### RECTANGULAR_SELECTIONS_ERROR_MESSAGE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) RECTANGULAR_SELECTIONS_ERROR_MESSAGE

Rectangular selection error message
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.JoinOperationBase.RECTANGULAR_SELECTIONS_ERROR_MESSAGE)

## Constructor Details

### JoinOperationBase

public JoinOperationBase([AuthorTableHelper](AuthorTableHelper.md) tableHelper)

Constructor.
  Parameters: tableHelper - Table helper with methods specific to a document type.
## Method Details

### doOperationInternal

protected void doOperationInternal([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)throws [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html), [AuthorOperationException](../../../api/AuthorOperationException.md)

Join the contents of selected cells.
  Specified by: [doOperationInternal](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [AbstractTableOperation](AbstractTableOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - Thrown when one or more arguments are illegal. [AuthorOperationException](../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AbstractTableOperation.doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### joinCells

public void joinCells([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> cellElements)throws [AuthorOperationException](../../../api/AuthorOperationException.md), [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Join table cells.
  Parameters: authorAccess - The author access. tableElement - The table element. cellElements - The cells fragments. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

### getArguments

public [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] getArguments()
  Returns: An array of [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments())

### generateColumnSpecifications

protected abstract void generateColumnSpecifications([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) tableCellSpanProvider, [AuthorElement](../../../api/node/AuthorElement.md) tableElement)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Generates column specifications for the given table and inserts them into the document.
  Parameters: authorAccess - Author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableCellSpanProvider - Table cell span provider. tableElement - The table element. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - Failed to insert the column specifications into the table.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
