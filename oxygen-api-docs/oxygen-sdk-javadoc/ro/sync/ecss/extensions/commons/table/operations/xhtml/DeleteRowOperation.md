Package [ro.sync.ecss.extensions.commons.table.operations.xhtml](package-summary.md)

# Class DeleteRowOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.DeleteRowOperationBase](../DeleteRowOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.xhtml.DeleteRowOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [XHTMLConstants](XHTMLConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class DeleteRowOperation extends [DeleteRowOperationBase](../DeleteRowOperationBase.md)implements [XHTMLConstants](XHTMLConstants.md)
Operation used to delete an XHTML table row.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.xhtml.[XHTMLConstants](XHTMLConstants.md)
 [ATTRIBUTE_NAME_COLSPAN](XHTMLConstants.md#ATTRIBUTE_NAME_COLSPAN), [ATTRIBUTE_NAME_ID](XHTMLConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_ROWSPAN](XHTMLConstants.md#ATTRIBUTE_NAME_ROWSPAN), [ATTRIBUTE_NAME_XML_ID](XHTMLConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_INFORMALTABLE](XHTMLConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_TABLE](XHTMLConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TD](XHTMLConstants.md#ELEMENT_NAME_TD), [ELEMENT_NAME_TH](XHTMLConstants.md#ELEMENT_NAME_TH), [ELEMENT_NAME_THEAD](XHTMLConstants.md#ELEMENT_NAME_THEAD), [ELEMENT_NAME_TR](XHTMLConstants.md#ELEMENT_NAME_TR)
## Constructor Summary
 Constructors
Constructor

Description
 [DeleteRowOperation](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [SplitCellAboveBelowOperationBase](../SplitCellAboveBelowOperationBase.md) [createSplitCellOperation](#createSplitCellOperation())()
Create the split cell operation.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[DeleteRowOperationBase](../DeleteRowOperationBase.md)
 [doOperationInternal](../DeleteRowOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../DeleteRowOperationBase.md#getArguments()), [getDescription](../DeleteRowOperationBase.md#getDescription()), [performDeleteRows](../DeleteRowOperationBase.md#performDeleteRows(ro.sync.ecss.extensions.api.AuthorAccess,int,int)), [performDeleteRows](../DeleteRowOperationBase.md#performDeleteRows(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [createEmptyCell](../AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DeleteRowOperation

public DeleteRowOperation()

Constructor.

## Method Details

### createSplitCellOperation

protected [SplitCellAboveBelowOperationBase](../SplitCellAboveBelowOperationBase.md) createSplitCellOperation()
 Description copied from class: [DeleteRowOperationBase](../DeleteRowOperationBase.md#createSplitCellOperation())
Create the split cell operation. The operation is needed to split the cells that span over multiple rows and start on the row to be deleted.
  Specified by: [createSplitCellOperation](../DeleteRowOperationBase.md#createSplitCellOperation()) in class [DeleteRowOperationBase](../DeleteRowOperationBase.md) Returns: The split cell operation. See Also:
        * [DeleteRowOperationBase.createSplitCellOperation()](../DeleteRowOperationBase.md#createSplitCellOperation())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
