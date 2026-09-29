Package [ro.sync.ecss.extensions.dita.topic.table.cals](package-summary.md)

# Class SplitCellAboveBelowOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.SplitCellAboveBelowOperationBase](../../../../commons/table/operations/SplitCellAboveBelowOperationBase.md)
            * ro.sync.ecss.extensions.dita.topic.table.cals.SplitCellAboveBelowOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [CALSConstants](../../../../commons/table/operations/cals/CALSConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class SplitCellAboveBelowOperation extends [SplitCellAboveBelowOperationBase](../../../../commons/table/operations/SplitCellAboveBelowOperationBase.md)implements [CALSConstants](../../../../commons/table/operations/cals/CALSConstants.md)
Operation for splitting a DITA table cell above or below.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../../../../commons/table/operations/AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../../../../commons/table/operations/AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](../../../../commons/table/operations/cals/CALSConstants.md)
 [ATTRIBUTE_NAME_ALIGN](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ALIGN), [ATTRIBUTE_NAME_COLNAME](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLNAME), [ATTRIBUTE_NAME_COLNUM](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLNUM), [ATTRIBUTE_NAME_COLS](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_COLSEP](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLSEP), [ATTRIBUTE_NAME_COLWIDTH](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLWIDTH), [ATTRIBUTE_NAME_ID](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_MOREROWS](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_MOREROWS), [ATTRIBUTE_NAME_NAMEEND](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_NAMEEND), [ATTRIBUTE_NAME_NAMEST](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_NAMEST), [ATTRIBUTE_NAME_ROWSEP](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ROWSEP), [ATTRIBUTE_NAME_SPANNAME](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_SPANNAME), [ATTRIBUTE_NAME_TABLE_WIDTH](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_TABLE_WIDTH), [ATTRIBUTE_NAME_XML_ID](../../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_COLSPEC](../../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_COLSPEC), [ELEMENT_NAME_ENTRY](../../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_ENTRY), [ELEMENT_NAME_INFORMALTABLE](../../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_ROW](../../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_SPANSPEC](../../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_SPANSPEC), [ELEMENT_NAME_TABLE](../../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TGROUP](../../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_TGROUP)
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

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[SplitCellAboveBelowOperationBase](../../../../commons/table/operations/SplitCellAboveBelowOperationBase.md)
 [doOperationInternal](../../../../commons/table/operations/SplitCellAboveBelowOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../../commons/table/operations/SplitCellAboveBelowOperationBase.md#getArguments()), [getDescription](../../../../commons/table/operations/SplitCellAboveBelowOperationBase.md#getDescription()), [splitCell](../../../../commons/table/operations/SplitCellAboveBelowOperationBase.md#splitCell(ro.sync.ecss.extensions.api.node.AuthorElement,ro.sync.ecss.extensions.api.AuthorAccess,boolean))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
 [createEmptyCell](../../../../commons/table/operations/AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../../../../commons/table/operations/AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../../../../commons/table/operations/AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../../../../commons/table/operations/AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../../../../commons/table/operations/AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../../../../commons/table/operations/AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SplitCellAboveBelowOperation

public SplitCellAboveBelowOperation()

Constructor.

## Method Details

### getIgnoredAttributes

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredAttributes()
  Specified by: [getIgnoredAttributes](../../../../commons/table/operations/SplitCellAboveBelowOperationBase.md#getIgnoredAttributes()) in class [SplitCellAboveBelowOperationBase](../../../../commons/table/operations/SplitCellAboveBelowOperationBase.md) Returns: The attributes which should be skipped, when creating a copy of the split cell. See Also:
        * [SplitCellAboveBelowOperationBase.getIgnoredAttributes()](../../../../commons/table/operations/SplitCellAboveBelowOperationBase.md#getIgnoredAttributes())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
