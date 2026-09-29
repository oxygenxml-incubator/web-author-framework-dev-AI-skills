Package [ro.sync.ecss.extensions.tei.table](package-summary.md)

# Class SplitCellAboveBelowOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../../commons/table/operations/AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.SplitCellAboveBelowOperationBase](../../commons/table/operations/SplitCellAboveBelowOperationBase.md)
            * ro.sync.ecss.extensions.tei.table.SplitCellAboveBelowOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md), [TEIConstants](TEIConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class SplitCellAboveBelowOperation extends [SplitCellAboveBelowOperationBase](../../commons/table/operations/SplitCellAboveBelowOperationBase.md)implements [TEIConstants](TEIConstants.md)
Operation used to split a table cell above or below.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../commons/table/operations/AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../../commons/table/operations/AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../../commons/table/operations/AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.tei.table.[TEIConstants](TEIConstants.md)
 [ATTRIBUTE_NAME_COLS](TEIConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_ID](TEIConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_ROWS](TEIConstants.md#ATTRIBUTE_NAME_ROWS), [ATTRIBUTE_NAME_XML_ID](TEIConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_CELL](TEIConstants.md#ELEMENT_NAME_CELL), [ELEMENT_NAME_ROW](TEIConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_TABLE](TEIConstants.md#ELEMENT_NAME_TABLE)
## Constructor Summary
 Constructors
Constructor

Description
 [SplitCellAboveBelowOperation](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredAttributes](#getIgnoredAttributes())()

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[SplitCellAboveBelowOperationBase](../../commons/table/operations/SplitCellAboveBelowOperationBase.md)
 [doOperationInternal](../../commons/table/operations/SplitCellAboveBelowOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../commons/table/operations/SplitCellAboveBelowOperationBase.md#getArguments()), [getDescription](../../commons/table/operations/SplitCellAboveBelowOperationBase.md#getDescription()), [splitCell](../../commons/table/operations/SplitCellAboveBelowOperationBase.md#splitCell(ro.sync.ecss.extensions.api.node.AuthorElement,ro.sync.ecss.extensions.api.AuthorAccess,boolean))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../commons/table/operations/AbstractTableOperation.md)
 [createEmptyCell](../../commons/table/operations/AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../../commons/table/operations/AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../../commons/table/operations/AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../../commons/table/operations/AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../../commons/table/operations/AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../../commons/table/operations/AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SplitCellAboveBelowOperation

public SplitCellAboveBelowOperation()

Constructor.

## Method Details

### getIgnoredAttributes

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredAttributes()
  Specified by: [getIgnoredAttributes](../../commons/table/operations/SplitCellAboveBelowOperationBase.md#getIgnoredAttributes()) in class [SplitCellAboveBelowOperationBase](../../commons/table/operations/SplitCellAboveBelowOperationBase.md) Returns: The attributes which should be skipped, when creating a copy of the split cell. See Also:
        * [SplitCellAboveBelowOperationBase.getIgnoredAttributes()](../../commons/table/operations/SplitCellAboveBelowOperationBase.md#getIgnoredAttributes())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
