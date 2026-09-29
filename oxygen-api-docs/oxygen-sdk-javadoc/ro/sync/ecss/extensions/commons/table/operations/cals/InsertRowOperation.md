Package [ro.sync.ecss.extensions.commons.table.operations.cals](package-summary.md)

# Class InsertRowOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase](../InsertRowOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.InsertRowOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [CALSConstants](CALSConstants.md), [InsertTableCellsContentConstants](../InsertTableCellsContentConstants.md)   Direct Known Subclasses: [InsertRowOperation](../../../../dita/topic/table/cals/InsertRowOperation.md), [InsertSingleRowOperation](InsertSingleRowOperation.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertRowOperation extends [InsertRowOperationBase](../InsertRowOperationBase.md)implements [CALSConstants](CALSConstants.md), [InsertTableCellsContentConstants](../InsertTableCellsContentConstants.md)
Operation used to insert a table row for DocBook v.4 or v.5 and for DITA CALS tables..

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [cellContent](#cellContent)
The fragment that must be introduced in the table cells

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertRowOperationBase](../InsertRowOperationBase.md)
 [CUSTOM_INSERTION_ARGUMENT_DESCRIPTOR](../InsertRowOperationBase.md#CUSTOM_INSERTION_ARGUMENT_DESCRIPTOR)
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
 [InsertRowOperation](#%3Cinit%3E())()
Constructor.
  [InsertRowOperation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](../AuthorTableHelper.md) helper)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [doOperationInternal](#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../../api/ArgumentsMap.md) args)
Perform the actual operation.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCellElementName](#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int columnIndex)
Get the name of the element that represents a cell.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultContentForEmptyCells](#getDefaultContentForEmptyCells())()
Get the default content that must be introduced in empty cells.
  protected [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md)[] [getOperationArguments](#getOperationArguments())()
Get the array of arguments used for this operation.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRowElementName](#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../api/node/AuthorElement.md) tableElement)
Get the name of the element that represents a row.
  protected boolean [useCurrentRowTemplateOnInsert](#useCurrentRowTemplateOnInsert())()

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertRowOperationBase](../InsertRowOperationBase.md)
 [createCellXMLFragment](../InsertRowOperationBase.md#createCellXMLFragment(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,java.lang.String%5B%5D,java.lang.String)), [getArguments](../InsertRowOperationBase.md#getArguments()), [getDescription](../InsertRowOperationBase.md#getDescription()), [getRowXMLFragment](../InsertRowOperationBase.md#getRowXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String,int,int)), [insertRows](../InsertRowOperationBase.md#insertRows(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorElement,int,java.lang.String)), [removeCustomInsertionDescriptor](../InsertRowOperationBase.md#removeCustomInsertionDescriptor(ro.sync.ecss.extensions.api.ArgumentDescriptor%5B%5D))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [createEmptyCell](../AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### cellContent

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cellContent

The fragment that must be introduced in the table cells

## Constructor Details

### InsertRowOperation

public InsertRowOperation()

Constructor.

### InsertRowOperation

public InsertRowOperation([AuthorTableHelper](../AuthorTableHelper.md) helper)

Constructor.
  Parameters: helper - Table helper
## Method Details

### doOperationInternal

protected void doOperationInternal([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from class: [AbstractTableOperation](../AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation.
  Overrides: [doOperationInternal](../InsertRowOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [InsertRowOperationBase](../InsertRowOperationBase.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AbstractTableOperation.doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### getCellElementName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCellElementName([AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int columnIndex)
 Description copied from class: [InsertRowOperationBase](../InsertRowOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))
Get the name of the element that represents a cell.
  Specified by: [getCellElementName](../InsertRowOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in class [InsertRowOperationBase](../InsertRowOperationBase.md) Parameters: tableElement - The table element columnIndex - The column index. Returns: The name of the element that represent a cell in the table. See Also:
        * [InsertRowOperationBase.getCellElementName(AuthorElement, int)](../InsertRowOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))

### getRowElementName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRowElementName([AuthorElement](../../../../api/node/AuthorElement.md) tableElement)
 Description copied from class: [InsertRowOperationBase](../InsertRowOperationBase.md#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement))
Get the name of the element that represents a row.
  Specified by: [getRowElementName](../InsertRowOperationBase.md#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [InsertRowOperationBase](../InsertRowOperationBase.md) Parameters: tableElement - The table parent element. Returns: The name of the element that represent a row in the table. See Also:
        * [InsertRowOperationBase.getRowElementName(AuthorElement)](../InsertRowOperationBase.md#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement))

### useCurrentRowTemplateOnInsert

protected boolean useCurrentRowTemplateOnInsert()
  Overrides: [useCurrentRowTemplateOnInsert](../InsertRowOperationBase.md#useCurrentRowTemplateOnInsert()) in class [InsertRowOperationBase](../InsertRowOperationBase.md) Returns: true if the current row template should be used to create the new row that must be inserted. Default: false See Also:
        * [InsertRowOperationBase.useCurrentRowTemplateOnInsert()](../InsertRowOperationBase.md#useCurrentRowTemplateOnInsert())

### getOperationArguments

protected [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md)[] getOperationArguments()
 Description copied from class: [InsertRowOperationBase](../InsertRowOperationBase.md#getOperationArguments())
Get the array of arguments used for this operation. The first argument defines the location where the operation will be executed as an xpath expression, the second one defines the relative position to the node obtained from the XPath location, the third is the namespace argument descriptor and the forth specifies if the user desires the insertion of multiple rows or not. For the second argument included in the returned arguments descriptor array, the allowed values are:  [AuthorConstants.POSITION_BEFORE](../../../../api/AuthorConstants.md#POSITION_BEFORE), [AuthorConstants.POSITION_AFTER](../../../../api/AuthorConstants.md#POSITION_AFTER), [AuthorConstants.POSITION_INSIDE_FIRST](../../../../api/AuthorConstants.md#POSITION_INSIDE_FIRST) [AuthorConstants.POSITION_INSIDE_LAST](../../../../api/AuthorConstants.md#POSITION_INSIDE_LAST)
  Overrides: [getOperationArguments](../InsertRowOperationBase.md#getOperationArguments()) in class [InsertRowOperationBase](../InsertRowOperationBase.md) Returns: The array with the arguments of the operation. See Also:
        * [InsertRowOperationBase.getOperationArguments()](../InsertRowOperationBase.md#getOperationArguments())

### getDefaultContentForEmptyCells

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultContentForEmptyCells()
 Description copied from class: [InsertRowOperationBase](../InsertRowOperationBase.md#getDefaultContentForEmptyCells())
Get the default content that must be introduced in empty cells.
  Overrides: [getDefaultContentForEmptyCells](../InsertRowOperationBase.md#getDefaultContentForEmptyCells()) in class [InsertRowOperationBase](../InsertRowOperationBase.md) Returns: The default content that must be introduced in empty cells. Default: null. See Also:
        * [InsertRowOperationBase.getDefaultContentForEmptyCells()](../InsertRowOperationBase.md#getDefaultContentForEmptyCells())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
