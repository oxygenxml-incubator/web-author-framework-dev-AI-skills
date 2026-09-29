Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class InsertRowOperationBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](AbstractTableOperation.md)
        * ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   Direct Known Subclasses: [InsertRowOperation](cals/InsertRowOperation.md), [InsertRowOperation](xhtml/InsertRowOperation.md), [InsertRowOperation](../../../dita/map/table/InsertRowOperation.md), [InsertRowOperation](../../../dita/topic/table/simpletable/InsertRowOperation.md), [InsertRowOperation](../../../tei/table/InsertRowOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class InsertRowOperationBase extends [AbstractTableOperation](AbstractTableOperation.md)
Abstract class for operation used to insert a table row.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected static final [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) [CUSTOM_INSERTION_ARGUMENT_DESCRIPTOR](#CUSTOM_INSERTION_ARGUMENT_DESCRIPTOR)
Argument descriptor for the argument that specifies whether a custom insertion should be used.

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [InsertRowOperationBase](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](AuthorTableHelper.md) documentTypeHelper)
Constructor.

## Method Summary
  All MethodsStatic MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [createCellXMLFragment](#createCellXMLFragment(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,java.lang.String%5B%5D,java.lang.String))([AuthorElement](../../../api/node/AuthorElement.md) cell, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] skippedAttributes, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedAttributes, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cellContent)
Create a cell XML fragment by copying the element and attributes from a given cell element.
  protected void [doOperationInternal](#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)
Perform the actual operation.
  [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()
The operation will display a dialog for choose table attributes.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCellElementName](#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../api/node/AuthorElement.md) tableElement, int columnIndex)
Get the name of the element that represents a cell.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultContentForEmptyCells](#getDefaultContentForEmptyCells())()
Get the default content that must be introduced in empty cells.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [getOperationArguments](#getOperationArguments())()
Get the array of arguments used for this operation.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRowElementName](#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
Get the name of the element that represents a row.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRowXMLFragment](#getRowXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newCellFragment, int newCellColumnIndex, int initialNumberOfColumns)
Creates the XML fragment representing a new table row to be inserted.
  void [insertRows](#insertRows(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorElement,int,java.lang.String))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xPathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorNode](../../../api/node/AuthorNode.md) nodeAtCaret, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, int noOfRowsToBeInserted, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)
Insert rows.
  protected static [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [removeCustomInsertionDescriptor](#removeCustomInsertionDescriptor(ro.sync.ecss.extensions.api.ArgumentDescriptor%5B%5D))([ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] superArguments)
Removes the argument descriptor for custom insertion from an arguments list.
  protected boolean [useCurrentRowTemplateOnInsert](#useCurrentRowTemplateOnInsert())()

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md)
 [createEmptyCell](AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### CUSTOM_INSERTION_ARGUMENT_DESCRIPTOR

protected static final [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) CUSTOM_INSERTION_ARGUMENT_DESCRIPTOR

Argument descriptor for the argument that specifies whether a custom insertion should be used.

## Constructor Details

### InsertRowOperationBase

public InsertRowOperationBase([AuthorTableHelper](AuthorTableHelper.md) documentTypeHelper)

Constructor.
  Parameters: documentTypeHelper - Author Document type helper, has methods specific to a document type.
## Method Details

### getOperationArguments

protected [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] getOperationArguments()

Get the array of arguments used for this operation. The first argument defines the location where the operation will be executed as an xpath expression, the second one defines the relative position to the node obtained from the XPath location, the third is the namespace argument descriptor and the forth specifies if the user desires the insertion of multiple rows or not. For the second argument included in the returned arguments descriptor array, the allowed values are:  [AuthorConstants.POSITION_BEFORE](../../../api/AuthorConstants.md#POSITION_BEFORE), [AuthorConstants.POSITION_AFTER](../../../api/AuthorConstants.md#POSITION_AFTER), [AuthorConstants.POSITION_INSIDE_FIRST](../../../api/AuthorConstants.md#POSITION_INSIDE_FIRST) [AuthorConstants.POSITION_INSIDE_LAST](../../../api/AuthorConstants.md#POSITION_INSIDE_LAST)
  Returns: The array with the arguments of the operation.
### doOperationInternal

protected void doOperationInternal([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from class: [AbstractTableOperation](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation.
  Specified by: [doOperationInternal](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [AbstractTableOperation](AbstractTableOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AbstractTableOperation.doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### insertRows

public void insertRows([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xPathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorNode](../../../api/node/AuthorNode.md) nodeAtCaret, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, int noOfRowsToBeInserted, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [AuthorOperationException](../../../api/AuthorOperationException.md)

Insert rows.
  Parameters: authorAccess - The author access. xPathLocation - The xPath location. namespace - The rows namespace. nodeAtCaret - The node at caret tableElement - The parent table element. noOfRowsToBeInserted - Number of rows to be inserted. relativePosition - One of [AuthorConstants.POSITION_AFTER](../../../api/AuthorConstants.md#POSITION_AFTER) or [AuthorConstants.POSITION_BEFORE](../../../api/AuthorConstants.md#POSITION_BEFORE) constants. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [AuthorOperationException](../../../api/AuthorOperationException.md)
### getRowXMLFragment

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRowXMLFragment([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newCellFragment, int newCellColumnIndex, int initialNumberOfColumns)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Creates the XML fragment representing a new table row to be inserted.
  Parameters: authorAccess - The author access. tableElement - The table element. namespace - The namespace of the table row. newCellFragment - The row will contain an additional cell added at the given column index. newCellColumnIndex - The column index of the additional cell initialNumberOfColumns - The initial number of columns. Returns: The XML fragment to be inserted. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### createCellXMLFragment

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) createCellXMLFragment([AuthorElement](../../../api/node/AuthorElement.md) cell, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] skippedAttributes, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedAttributes, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cellContent)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create a cell XML fragment by copying the element and attributes from a given cell element.
  Parameters: cell - The cell to copy the element name and attributes from. skippedAttributes - List of skipped attributes names. cellContent - The cell content. Returns: The cell fragment. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### getArguments

public [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] getArguments()

The operation will display a dialog for choose table attributes.
  Returns: An array of [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments())

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

### getCellElementName

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCellElementName([AuthorElement](../../../api/node/AuthorElement.md) tableElement, int columnIndex)

Get the name of the element that represents a cell.
  Parameters: tableElement - The table element columnIndex - The column index. Returns: The name of the element that represent a cell in the table.
### getRowElementName

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRowElementName([AuthorElement](../../../api/node/AuthorElement.md) tableElement)

Get the name of the element that represents a row.
  Parameters: tableElement - The table parent element. Returns: The name of the element that represent a row in the table.
### useCurrentRowTemplateOnInsert

protected boolean useCurrentRowTemplateOnInsert()
  Returns: true if the current row template should be used to create the new row that must be inserted. Default: false
### getDefaultContentForEmptyCells

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultContentForEmptyCells()

Get the default content that must be introduced in empty cells.
  Returns: The default content that must be introduced in empty cells. Default: null. Since: 14.1
### removeCustomInsertionDescriptor

protected static [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] removeCustomInsertionDescriptor([ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] superArguments)

Removes the argument descriptor for custom insertion from an arguments list.
  Parameters: superArguments - The input arguments list. Returns: The filtered arguments list.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
