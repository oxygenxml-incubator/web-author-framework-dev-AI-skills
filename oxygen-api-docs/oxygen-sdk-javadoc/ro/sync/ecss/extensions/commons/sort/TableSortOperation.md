Package [ro.sync.ecss.extensions.commons.sort](package-summary.md)

# Class TableSortOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.sort.SortOperation](SortOperation.md)
        * ro.sync.ecss.extensions.commons.sort.TableSortOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   Direct Known Subclasses: [CALSAndHTMLTableSortOperation](../table/operations/cals/CALSAndHTMLTableSortOperation.md), [SimpleTableSortOperation](SimpleTableSortOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class TableSortOperation extends [SortOperation](SortOperation.md)
Base table sort operation.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.sort.[SortOperation](SortOperation.md)
 [authorAccess](SortOperation.md#authorAccess), [COLUMN](SortOperation.md#COLUMN)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [TableSortOperation](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 void [canBeSorted](#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D))([AuthorElement](../../api/node/AuthorElement.md) parent, int[] selectedNonIgnoredChildrenInterval)
Check if the parent element selected children can be sorted.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID())()
Get the ID of the help page which will be called by the end user.
  protected abstract int [getRowIndexForTableBody](#getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) table)
Returns the visual row index of the actual table body if the table has separate head, foot element and table group elements.

### Methods inherited from class ro.sync.ecss.extensions.commons.sort.[SortOperation](SortOperation.md)
 [doOperation](SortOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [forceSortAll](SortOperation.md#forceSortAll()), [getArguments](SortOperation.md#getArguments()), [getDescription](SortOperation.md#getDescription()), [getNonIgnoredChildren](SortOperation.md#getNonIgnoredChildren(ro.sync.ecss.extensions.api.node.AuthorElement)), [getSelectedNonIgnoredChildrenInterval](SortOperation.md#getSelectedNonIgnoredChildrenInterval(ro.sync.ecss.extensions.api.node.AuthorElement)), [getSortCriteria](SortOperation.md#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement)), [getSortKeysValues](SortOperation.md#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation)), [getSortParent](SortOperation.md#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess)), [getTextContentToSort](SortOperation.md#getTextContentToSort(ro.sync.ecss.extensions.api.node.AuthorNode)), [isIgnored](SortOperation.md#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TableSortOperation

public TableSortOperation()

Constructor.

## Method Details

### canBeSorted

public void canBeSorted([AuthorElement](../../api/node/AuthorElement.md) parent, int[] selectedNonIgnoredChildrenInterval)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from class: [SortOperation](SortOperation.md#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D))
Check if the parent element selected children can be sorted. For example a table row containing a cell with rowspan cannot be sorted and stops the operation.
  Specified by: [canBeSorted](SortOperation.md#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D)) in class [SortOperation](SortOperation.md) Parameters: parent - The parent of the elements which will be sorted. selectedNonIgnoredChildrenInterval - The interval of selected children indices. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - When the given node is not sortable. For example a table row containing a cell with multiple rowspan stops the operation. See Also:
        * [SortOperation.canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement, int[])](SortOperation.md#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D))

### getRowIndexForTableBody

protected abstract int getRowIndexForTableBody([AuthorNode](../../api/node/AuthorNode.md) table)

Returns the visual row index of the actual table body if the table has separate head, foot element and table group elements.

### getHelpPageID

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID()
 Description copied from class: [SortOperation](SortOperation.md#getHelpPageID())
Get the ID of the help page which will be called by the end user.
  Overrides: [getHelpPageID](SortOperation.md#getHelpPageID()) in class [SortOperation](SortOperation.md) Returns: the ID of the help page which will be called by the end user or null. See Also:
        * [SortOperation.getHelpPageID()](SortOperation.md#getHelpPageID())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
