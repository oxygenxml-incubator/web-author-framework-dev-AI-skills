Package [ro.sync.ecss.extensions.tei.table](package-summary.md)

# Class SplitOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../../commons/table/operations/AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.SplitOperationBase](../../commons/table/operations/SplitOperationBase.md)
            * ro.sync.ecss.extensions.tei.table.SplitOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md), [TEIConstants](TEIConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class SplitOperation extends [SplitOperationBase](../../commons/table/operations/SplitOperationBase.md)implements [TEIConstants](TEIConstants.md)
Operation for splitting the selected table cell (or the cell at caret when there is no selection).

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

 protected [InsertColumnOperationBase](../../commons/table/operations/InsertColumnOperationBase.md) [getInsertColumnOperation](#getInsertColumnOperation())()
Get the insert column operation to be used when splitting cells that have no initial span.
  protected [InsertRowOperationBase](../../commons/table/operations/InsertRowOperationBase.md) [getInsertRowOperation](#getInsertRowOperation())()
Get the insert row operation to be used when splitting cells that have no initial span.
  protected [JoinOperationBase](../../commons/table/operations/JoinOperationBase.md) [getJoinOperation](#getJoinOperation())()
Get the join operation to be used when splitting cells that have no initial span.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[SplitOperationBase](../../commons/table/operations/SplitOperationBase.md)
 [doOperationInternal](../../commons/table/operations/SplitOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../commons/table/operations/SplitOperationBase.md#getArguments()), [getDescription](../../commons/table/operations/SplitOperationBase.md#getDescription())
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../commons/table/operations/AbstractTableOperation.md)
 [createEmptyCell](../../commons/table/operations/AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../../commons/table/operations/AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../../commons/table/operations/AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../../commons/table/operations/AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../../commons/table/operations/AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../../commons/table/operations/AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SplitOperation

public SplitOperation()

Constructor.

## Method Details

### getIgnoredAttributesForRowSplit

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredAttributesForRowSplit()
  Specified by: [getIgnoredAttributesForRowSplit](../../commons/table/operations/SplitOperationBase.md#getIgnoredAttributesForRowSplit()) in class [SplitOperationBase](../../commons/table/operations/SplitOperationBase.md) Returns: The attributes which should be skipped, when creating a copy of the split cell. See Also:
        * [SplitOperationBase.getIgnoredAttributesForRowSplit()](../../commons/table/operations/SplitOperationBase.md#getIgnoredAttributesForRowSplit())

### getIgnoredAttributesForColumnSplit

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredAttributesForColumnSplit()
  Specified by: [getIgnoredAttributesForColumnSplit](../../commons/table/operations/SplitOperationBase.md#getIgnoredAttributesForColumnSplit()) in class [SplitOperationBase](../../commons/table/operations/SplitOperationBase.md) Returns: The attributes which should be skipped when creating a copy of the split cell. See Also:
        * [SplitOperationBase.getIgnoredAttributesForColumnSplit()](../../commons/table/operations/SplitOperationBase.md#getIgnoredAttributesForColumnSplit())

### getInsertRowOperation

protected [InsertRowOperationBase](../../commons/table/operations/InsertRowOperationBase.md) getInsertRowOperation()
 Description copied from class: [SplitOperationBase](../../commons/table/operations/SplitOperationBase.md#getInsertRowOperation())
Get the insert row operation to be used when splitting cells that have no initial span.
  Specified by: [getInsertRowOperation](../../commons/table/operations/SplitOperationBase.md#getInsertRowOperation()) in class [SplitOperationBase](../../commons/table/operations/SplitOperationBase.md) See Also:
        * [SplitOperationBase.getInsertRowOperation()](../../commons/table/operations/SplitOperationBase.md#getInsertRowOperation())

### getInsertColumnOperation

protected [InsertColumnOperationBase](../../commons/table/operations/InsertColumnOperationBase.md) getInsertColumnOperation()
 Description copied from class: [SplitOperationBase](../../commons/table/operations/SplitOperationBase.md#getInsertColumnOperation())
Get the insert column operation to be used when splitting cells that have no initial span.
  Specified by: [getInsertColumnOperation](../../commons/table/operations/SplitOperationBase.md#getInsertColumnOperation()) in class [SplitOperationBase](../../commons/table/operations/SplitOperationBase.md) See Also:
        * [SplitOperationBase.getInsertColumnOperation()](../../commons/table/operations/SplitOperationBase.md#getInsertColumnOperation())

### getJoinOperation

protected [JoinOperationBase](../../commons/table/operations/JoinOperationBase.md) getJoinOperation()
 Description copied from class: [SplitOperationBase](../../commons/table/operations/SplitOperationBase.md#getJoinOperation())
Get the join operation to be used when splitting cells that have no initial span.
  Specified by: [getJoinOperation](../../commons/table/operations/SplitOperationBase.md#getJoinOperation()) in class [SplitOperationBase](../../commons/table/operations/SplitOperationBase.md) See Also:
        * [SplitOperationBase.getJoinOperation()](../../commons/table/operations/SplitOperationBase.md#getJoinOperation())

### getHelpPageID

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID()
 Description copied from class: [SplitOperationBase](../../commons/table/operations/SplitOperationBase.md#getHelpPageID())
Get the ID of the help page which will be called by the end user.
  Overrides: [getHelpPageID](../../commons/table/operations/SplitOperationBase.md#getHelpPageID()) in class [SplitOperationBase](../../commons/table/operations/SplitOperationBase.md) Returns: the ID of the help page which will be called by the end user or null. See Also:
        * [SplitOperationBase.getHelpPageID()](../../commons/table/operations/SplitOperationBase.md#getHelpPageID())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
