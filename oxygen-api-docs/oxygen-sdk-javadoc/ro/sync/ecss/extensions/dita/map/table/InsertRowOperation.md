Package [ro.sync.ecss.extensions.dita.map.table](package-summary.md)

# Class InsertRowOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../../../commons/table/operations/AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md)
            * ro.sync.ecss.extensions.dita.map.table.InsertRowOperation
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md), [ReltableConstants](ReltableConstants.md)   Direct Known Subclasses: [InsertSingleRowOperation](InsertSingleRowOperation.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertRowOperation extends [InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md)implements [ReltableConstants](ReltableConstants.md)
Operation used to insert a reltable row for DITA.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md)
 [CUSTOM_INSERTION_ARGUMENT_DESCRIPTOR](../../../commons/table/operations/InsertRowOperationBase.md#CUSTOM_INSERTION_ARGUMENT_DESCRIPTOR)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../commons/table/operations/AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../../../commons/table/operations/AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../../../commons/table/operations/AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.dita.map.table.[ReltableConstants](ReltableConstants.md)
 [ATTRIBUTE_NAME_ID](ReltableConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_TYPE](ReltableConstants.md#ATTRIBUTE_NAME_TYPE), [ELEMENT_NAME_ENTRY](ReltableConstants.md#ELEMENT_NAME_ENTRY), [ELEMENT_NAME_HEADER](ReltableConstants.md#ELEMENT_NAME_HEADER), [ELEMENT_NAME_HEADER_ENTRY](ReltableConstants.md#ELEMENT_NAME_HEADER_ENTRY), [ELEMENT_NAME_ROW](ReltableConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_TABLE](ReltableConstants.md#ELEMENT_NAME_TABLE)
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
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCellElementName](#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../api/node/AuthorElement.md) tableElement, int columnIndex)
Get the name of the element that represents a cell.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRowElementName](#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
Get the name of the element that represents a row.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md)
 [createCellXMLFragment](../../../commons/table/operations/InsertRowOperationBase.md#createCellXMLFragment(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,java.lang.String%5B%5D,java.lang.String)), [doOperationInternal](../../../commons/table/operations/InsertRowOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../commons/table/operations/InsertRowOperationBase.md#getArguments()), [getDefaultContentForEmptyCells](../../../commons/table/operations/InsertRowOperationBase.md#getDefaultContentForEmptyCells()), [getDescription](../../../commons/table/operations/InsertRowOperationBase.md#getDescription()), [getOperationArguments](../../../commons/table/operations/InsertRowOperationBase.md#getOperationArguments()), [getRowXMLFragment](../../../commons/table/operations/InsertRowOperationBase.md#getRowXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String,int,int)), [insertRows](../../../commons/table/operations/InsertRowOperationBase.md#insertRows(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorElement,int,java.lang.String)), [removeCustomInsertionDescriptor](../../../commons/table/operations/InsertRowOperationBase.md#removeCustomInsertionDescriptor(ro.sync.ecss.extensions.api.ArgumentDescriptor%5B%5D)), [useCurrentRowTemplateOnInsert](../../../commons/table/operations/InsertRowOperationBase.md#useCurrentRowTemplateOnInsert())
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../commons/table/operations/AbstractTableOperation.md)
 [createEmptyCell](../../../commons/table/operations/AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../../../commons/table/operations/AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../../../commons/table/operations/AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../../../commons/table/operations/AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../../../commons/table/operations/AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../../../commons/table/operations/AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### InsertRowOperation

public InsertRowOperation()

Constructor.

## Method Details

### getCellElementName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCellElementName([AuthorElement](../../../api/node/AuthorElement.md) tableElement, int columnIndex)
 Description copied from class: [InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))
Get the name of the element that represents a cell.
  Specified by: [getCellElementName](../../../commons/table/operations/InsertRowOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in class [InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md) Parameters: tableElement - The table element columnIndex - The column index. Returns: The name of the element that represent a cell in the table. See Also:
        * [InsertRowOperationBase.getCellElementName(AuthorElement, int)](../../../commons/table/operations/InsertRowOperationBase.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int))

### getRowElementName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRowElementName([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
 Description copied from class: [InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement))
Get the name of the element that represents a row.
  Specified by: [getRowElementName](../../../commons/table/operations/InsertRowOperationBase.md#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md) Parameters: tableElement - The table parent element. Returns: The name of the element that represent a row in the table. See Also:
        * [InsertRowOperationBase.getRowElementName(AuthorElement)](../../../commons/table/operations/InsertRowOperationBase.md#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
