Package [ro.sync.ecss.extensions.commons.table.operations.cals](package-summary.md)

# Class SplitOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.SplitOperationBase](../SplitOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.SplitOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [CALSConstants](CALSConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class SplitOperation extends [SplitOperationBase](../SplitOperationBase.md)implements [CALSConstants](CALSConstants.md)
Operation for splitting the selected table cell (or the cell at caret when there is no selection).

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md)
 [ATTRIBUTE_NAME_ALIGN](CALSConstants.md#ATTRIBUTE_NAME_ALIGN), [ATTRIBUTE_NAME_COLNAME](CALSConstants.md#ATTRIBUTE_NAME_COLNAME), [ATTRIBUTE_NAME_COLNUM](CALSConstants.md#ATTRIBUTE_NAME_COLNUM), [ATTRIBUTE_NAME_COLS](CALSConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_COLSEP](CALSConstants.md#ATTRIBUTE_NAME_COLSEP), [ATTRIBUTE_NAME_COLWIDTH](CALSConstants.md#ATTRIBUTE_NAME_COLWIDTH), [ATTRIBUTE_NAME_ID](CALSConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_MOREROWS](CALSConstants.md#ATTRIBUTE_NAME_MOREROWS), [ATTRIBUTE_NAME_NAMEEND](CALSConstants.md#ATTRIBUTE_NAME_NAMEEND), [ATTRIBUTE_NAME_NAMEST](CALSConstants.md#ATTRIBUTE_NAME_NAMEST), [ATTRIBUTE_NAME_ROWSEP](CALSConstants.md#ATTRIBUTE_NAME_ROWSEP), [ATTRIBUTE_NAME_SPANNAME](CALSConstants.md#ATTRIBUTE_NAME_SPANNAME), [ATTRIBUTE_NAME_TABLE_WIDTH](CALSConstants.md#ATTRIBUTE_NAME_TABLE_WIDTH), [ATTRIBUTE_NAME_XML_ID](CALSConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_COLSPEC](CALSConstants.md#ELEMENT_NAME_COLSPEC), [ELEMENT_NAME_ENTRY](CALSConstants.md#ELEMENT_NAME_ENTRY), [ELEMENT_NAME_INFORMALTABLE](CALSConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_ROW](CALSConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_SPANSPEC](CALSConstants.md#ELEMENT_NAME_SPANSPEC), [ELEMENT_NAME_TABLE](CALSConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TGROUP](CALSConstants.md#ELEMENT_NAME_TGROUP)
## Constructor Summary
 Constructors
Constructor

Description
 [SplitOperation](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID())()
Get the ID of the help page which will be called by the end user.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredAttributesForColumnSplit](#getIgnoredAttributesForColumnSplit())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredAttributesForRowSplit](#getIgnoredAttributesForRowSplit())()

 protected [InsertColumnOperationBase](../InsertColumnOperationBase.md) [getInsertColumnOperation](#getInsertColumnOperation())()
Get the insert column operation to be used when splitting cells that have no initial span.
  protected [InsertRowOperationBase](../InsertRowOperationBase.md) [getInsertRowOperation](#getInsertRowOperation())()
Get the insert row operation to be used when splitting cells that have no initial span.
  protected [JoinOperationBase](../JoinOperationBase.md) [getJoinOperation](#getJoinOperation())()
Get the join operation to be used when splitting cells that have no initial span.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[SplitOperationBase](../SplitOperationBase.md)
 [doOperationInternal](../SplitOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../SplitOperationBase.md#getArguments()), [getDescription](../SplitOperationBase.md#getDescription())
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [createEmptyCell](../AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SplitOperation

public SplitOperation()

Constructor.

## Method Details

### getIgnoredAttributesForRowSplit

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredAttributesForRowSplit()
  Specified by: [getIgnoredAttributesForRowSplit](../SplitOperationBase.md#getIgnoredAttributesForRowSplit()) in class [SplitOperationBase](../SplitOperationBase.md) Returns: The attributes which should be skipped, when creating a copy of the split cell. See Also:
        * [SplitOperationBase.getIgnoredAttributesForRowSplit()](../SplitOperationBase.md#getIgnoredAttributesForRowSplit())

### getIgnoredAttributesForColumnSplit

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredAttributesForColumnSplit()
  Specified by: [getIgnoredAttributesForColumnSplit](../SplitOperationBase.md#getIgnoredAttributesForColumnSplit()) in class [SplitOperationBase](../SplitOperationBase.md) Returns: The attributes which should be skipped when creating a copy of the split cell. See Also:
        * [SplitOperationBase.getIgnoredAttributesForColumnSplit()](../SplitOperationBase.md#getIgnoredAttributesForColumnSplit())

### getInsertRowOperation

protected [InsertRowOperationBase](../InsertRowOperationBase.md) getInsertRowOperation()
 Description copied from class: [SplitOperationBase](../SplitOperationBase.md#getInsertRowOperation())
Get the insert row operation to be used when splitting cells that have no initial span.
  Specified by: [getInsertRowOperation](../SplitOperationBase.md#getInsertRowOperation()) in class [SplitOperationBase](../SplitOperationBase.md) See Also:
        * [SplitOperationBase.getInsertRowOperation()](../SplitOperationBase.md#getInsertRowOperation())

### getInsertColumnOperation

protected [InsertColumnOperationBase](../InsertColumnOperationBase.md) getInsertColumnOperation()
 Description copied from class: [SplitOperationBase](../SplitOperationBase.md#getInsertColumnOperation())
Get the insert column operation to be used when splitting cells that have no initial span.
  Specified by: [getInsertColumnOperation](../SplitOperationBase.md#getInsertColumnOperation()) in class [SplitOperationBase](../SplitOperationBase.md) See Also:
        * [SplitOperationBase.getInsertColumnOperation()](../SplitOperationBase.md#getInsertColumnOperation())

### getJoinOperation

protected [JoinOperationBase](../JoinOperationBase.md) getJoinOperation()
 Description copied from class: [SplitOperationBase](../SplitOperationBase.md#getJoinOperation())
Get the join operation to be used when splitting cells that have no initial span.
  Specified by: [getJoinOperation](../SplitOperationBase.md#getJoinOperation()) in class [SplitOperationBase](../SplitOperationBase.md) See Also:
        * [SplitOperationBase.getJoinOperation()](../SplitOperationBase.md#getJoinOperation())

### getHelpPageID

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID()
 Description copied from class: [SplitOperationBase](../SplitOperationBase.md#getHelpPageID())
Get the ID of the help page which will be called by the end user.
  Overrides: [getHelpPageID](../SplitOperationBase.md#getHelpPageID()) in class [SplitOperationBase](../SplitOperationBase.md) Returns: the ID of the help page which will be called by the end user or null. See Also:
        * [SplitOperationBase.getHelpPageID()](../SplitOperationBase.md#getHelpPageID())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
