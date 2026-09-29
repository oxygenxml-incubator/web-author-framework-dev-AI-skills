Package [ro.sync.ecss.extensions.dita.topic.table.simpletable](package-summary.md)

# Class InsertRowOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md)
            * ro.sync.ecss.extensions.dita.topic.table.simpletable.InsertRowOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [InsertTableCellsContentConstants](../../../../commons/table/operations/InsertTableCellsContentConstants.md), [SimpleTableConstants](SimpleTableConstants.md)   Direct Known Subclasses: [InsertSingleRowOperation](InsertSingleRowOperation.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertRowOperation extends [InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md)implements [SimpleTableConstants](SimpleTableConstants.md), [InsertTableCellsContentConstants](../../../../commons/table/operations/InsertTableCellsContentConstants.md)
Operation used to insert a simple table row for DITA.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [cellContent](#cellContent)
The fragment that must be introduced in the table cells

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md)
 [CUSTOM_INSERTION_ARGUMENT_DESCRIPTOR](../../../../commons/table/operations/InsertRowOperationBase.md#CUSTOM_INSERTION_ARGUMENT_DESCRIPTOR)
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
Constructor

Description
 [InsertRowOperation](#%3Cinit%3E())()
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

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md)
 [createCellXMLFragment](../../../../commons/table/operations/InsertRowOperationBase.md#createCellXMLFragment(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,java.lang.String%5B%5D,java.lang.String)), [getArguments](../../../../commons/table/operations/InsertRowOperationBase.md#getArguments()), [getDescription](../../../../commons/table/operations/InsertRowOperationBase.md#getDescription()), [getRowXMLFragment](../../../../commons/table/operations/InsertRowOperationBase.md#getRowXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String,int,int)), [insertRows](../../../../commons/table/operations/InsertRowOperationBase.md#insertRows(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorElement,int,java.lang.String)), [removeCustomInsertionDescriptor](../../../../commons/table/operations/InsertRowOperationBase.md#removeCustomInsertionDescriptor(ro.sync.ecss.extensions.api.ArgumentDescriptor%5B%5D)), [useCurrentRowTemplateOnInsert](../../../../commons/table/operations/InsertRowOperationBase.md#useCurrentRowTemplateOnInsert())
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
 [createEmptyCell](../../../../commons/table/operations/AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../../../../commons/table/operations/AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../../../../commons/table/operations/AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../../../../commons/table/operations/AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../../../../commons/table/operations/AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../../../../commons/table/operations/AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
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

## Method Details

### doOperationInternal

protected void doOperationInternal([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from class: [AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation.
  Overrides: [doOperationInternal](../../../../commons/table/operations/InsertRowOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [InsertRowOperationBase.doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../../../../commons/table/operations/InsertRowOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### getCellElementName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCellElementName([AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int columnIndex)
 Description copied from class: [InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))
Get the name of the element that represents a cell.
  Specified by: [getCellElementName](../../../../commons/table/operations/InsertRowOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in class [InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md) Parameters: tableElement - The table element columnIndex - The column index. Returns: The name of the element that represent a cell in the table. See Also:
        * [InsertRowOperationBase.getCellElementName(AuthorElement, int)](../../../../commons/table/operations/InsertRowOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))

### getRowElementName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRowElementName([AuthorElement](../../../../api/node/AuthorElement.md) tableElement)
 Description copied from class: [InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement))
Get the name of the element that represents a row.
  Specified by: [getRowElementName](../../../../commons/table/operations/InsertRowOperationBase.md#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md) Parameters: tableElement - The table parent element. Returns: The name of the element that represent a row in the table. See Also:
        * [InsertRowOperationBase.getRowElementName(AuthorElement)](../../../../commons/table/operations/InsertRowOperationBase.md#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement))

### getDefaultContentForEmptyCells

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultContentForEmptyCells()
 Description copied from class: [InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md#getDefaultContentForEmptyCells())
Get the default content that must be introduced in empty cells.
  Overrides: [getDefaultContentForEmptyCells](../../../../commons/table/operations/InsertRowOperationBase.md#getDefaultContentForEmptyCells()) in class [InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md) Returns: The default content that must be introduced in empty cells. Default: null. See Also:
        * [InsertRowOperationBase.getDefaultContentForEmptyCells()](../../../../commons/table/operations/InsertRowOperationBase.md#getDefaultContentForEmptyCells())

### getOperationArguments

protected [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md)[] getOperationArguments()
 Description copied from class: [InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md#getOperationArguments())
Get the array of arguments used for this operation. The first argument defines the location where the operation will be executed as an xpath expression, the second one defines the relative position to the node obtained from the XPath location, the third is the namespace argument descriptor and the forth specifies if the user desires the insertion of multiple rows or not. For the second argument included in the returned arguments descriptor array, the allowed values are:  [AuthorConstants.POSITION_BEFORE](../../../../api/AuthorConstants.md#POSITION_BEFORE), [AuthorConstants.POSITION_AFTER](../../../../api/AuthorConstants.md#POSITION_AFTER), [AuthorConstants.POSITION_INSIDE_FIRST](../../../../api/AuthorConstants.md#POSITION_INSIDE_FIRST) [AuthorConstants.POSITION_INSIDE_LAST](../../../../api/AuthorConstants.md#POSITION_INSIDE_LAST)
  Overrides: [getOperationArguments](../../../../commons/table/operations/InsertRowOperationBase.md#getOperationArguments()) in class [InsertRowOperationBase](../../../../commons/table/operations/InsertRowOperationBase.md) Returns: The array with the arguments of the operation. See Also:
        * [InsertRowOperationBase.getOperationArguments()](../../../../commons/table/operations/InsertRowOperationBase.md#getOperationArguments())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
