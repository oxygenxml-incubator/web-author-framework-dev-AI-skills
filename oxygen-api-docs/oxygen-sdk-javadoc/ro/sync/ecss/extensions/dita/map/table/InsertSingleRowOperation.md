Package [ro.sync.ecss.extensions.dita.map.table](package-summary.md)

# Class InsertSingleRowOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../../../commons/table/operations/AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md)
            * [ro.sync.ecss.extensions.dita.map.table.InsertRowOperation](InsertRowOperation.md)
                * ro.sync.ecss.extensions.dita.map.table.InsertSingleRowOperation
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md), [ReltableConstants](ReltableConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertSingleRowOperation extends [InsertRowOperation](InsertRowOperation.md)
Operation used to insert a reltable row for DITA. It does not allow custom insertion of multiple rows, and thus is webapp-compatible.

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
 [InsertSingleRowOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [getOperationArguments](#getOperationArguments())()
Get the array of arguments used for this operation.

### Methods inherited from class ro.sync.ecss.extensions.dita.map.table.[InsertRowOperation](InsertRowOperation.md)
 [getCellElementName](InsertRowOperation.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int)), [getRowElementName](InsertRowOperation.md#getRowElementName(ro.sync.ecss.extensions.api.node.AuthorElement))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md)
 [createCellXMLFragment](../../../commons/table/operations/InsertRowOperationBase.md#createCellXMLFragment(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,java.lang.String%5B%5D,java.lang.String)), [doOperationInternal](../../../commons/table/operations/InsertRowOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../commons/table/operations/InsertRowOperationBase.md#getArguments()), [getDefaultContentForEmptyCells](../../../commons/table/operations/InsertRowOperationBase.md#getDefaultContentForEmptyCells()), [getDescription](../../../commons/table/operations/InsertRowOperationBase.md#getDescription()), [getRowXMLFragment](../../../commons/table/operations/InsertRowOperationBase.md#getRowXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String,int,int)), [insertRows](../../../commons/table/operations/InsertRowOperationBase.md#insertRows(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorElement,int,java.lang.String)), [removeCustomInsertionDescriptor](../../../commons/table/operations/InsertRowOperationBase.md#removeCustomInsertionDescriptor(ro.sync.ecss.extensions.api.ArgumentDescriptor%5B%5D)), [useCurrentRowTemplateOnInsert](../../../commons/table/operations/InsertRowOperationBase.md#useCurrentRowTemplateOnInsert())
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../commons/table/operations/AbstractTableOperation.md)
 [createEmptyCell](../../../commons/table/operations/AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../../../commons/table/operations/AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../../../commons/table/operations/AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../../../commons/table/operations/AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../../../commons/table/operations/AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../../../commons/table/operations/AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### InsertSingleRowOperation

public InsertSingleRowOperation()

## Method Details

### getOperationArguments

protected [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] getOperationArguments()
 Description copied from class: [InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md#getOperationArguments())
Get the array of arguments used for this operation. The first argument defines the location where the operation will be executed as an xpath expression, the second one defines the relative position to the node obtained from the XPath location, the third is the namespace argument descriptor and the forth specifies if the user desires the insertion of multiple rows or not. For the second argument included in the returned arguments descriptor array, the allowed values are:  [AuthorConstants.POSITION_BEFORE](../../../api/AuthorConstants.md#POSITION_BEFORE), [AuthorConstants.POSITION_AFTER](../../../api/AuthorConstants.md#POSITION_AFTER), [AuthorConstants.POSITION_INSIDE_FIRST](../../../api/AuthorConstants.md#POSITION_INSIDE_FIRST) [AuthorConstants.POSITION_INSIDE_LAST](../../../api/AuthorConstants.md#POSITION_INSIDE_LAST)
  Overrides: [getOperationArguments](../../../commons/table/operations/InsertRowOperationBase.md#getOperationArguments()) in class [InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md) Returns: The array with the arguments of the operation. See Also:
        * [InsertRowOperationBase.getOperationArguments()](../../../commons/table/operations/InsertRowOperationBase.md#getOperationArguments())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
