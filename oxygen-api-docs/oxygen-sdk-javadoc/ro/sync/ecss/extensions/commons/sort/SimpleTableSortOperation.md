Package [ro.sync.ecss.extensions.commons.sort](package-summary.md)

# Class SimpleTableSortOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.sort.SortOperation](SortOperation.md)
        * [ro.sync.ecss.extensions.commons.sort.TableSortOperation](TableSortOperation.md)
            * ro.sync.ecss.extensions.commons.sort.SimpleTableSortOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   Direct Known Subclasses: [DITASimpleTableSortOperation](../../dita/topic/table/DITASimpleTableSortOperation.md), [TEITableSortOperation](../../tei/table/TEITableSortOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class SimpleTableSortOperation extends [TableSortOperation](TableSortOperation.md)
Sort operation for simple tables

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.sort.[SortOperation](SortOperation.md)
 [authorAccess](SortOperation.md#authorAccess), [COLUMN](SortOperation.md#COLUMN)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [SimpleTableSortOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [forceSortAll](#forceSortAll())()

 protected int [getRowIndexForTableBody](#getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) table)
Returns the visual row index of the actual table body if the table has separate head, foot element and table group elements.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> [getSortCriteria](#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) parent)
Obtain the sort criterion.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getSortKeysValues](#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation))([AuthorNode](../../api/node/AuthorNode.md) node, [SortCriteriaInformation](SortCriteriaInformation.md) sortInfo)
Obtain the values of the keys that can be used for sorting.
  [AuthorElement](../../api/node/AuthorElement.md) [getSortParent](#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess))(int offset, [AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Get the table element whose rows will be sorted.
  boolean [isCaretInColumn](#isCaretInColumn(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, int columnNumber)
Checks if the caret is in a cell which is in the given column.
  abstract boolean [isHeadElement](#isHeadElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) node)
Returns true if the given node is the table header element.
  boolean [isIgnored](#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
Checks if a given node is ignored when sorting.
  abstract boolean [isRowElement](#isRowElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) node)
Returns true if the given node is a table row.
  abstract boolean [isTableElement](#isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) node)
Return true if the given node is the table element.

### Methods inherited from class ro.sync.ecss.extensions.commons.sort.[TableSortOperation](TableSortOperation.md)
 [canBeSorted](TableSortOperation.md#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D)), [getHelpPageID](TableSortOperation.md#getHelpPageID())
### Methods inherited from class ro.sync.ecss.extensions.commons.sort.[SortOperation](SortOperation.md)
 [doOperation](SortOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](SortOperation.md#getArguments()), [getDescription](SortOperation.md#getDescription()), [getNonIgnoredChildren](SortOperation.md#getNonIgnoredChildren(ro.sync.ecss.extensions.api.node.AuthorElement)), [getSelectedNonIgnoredChildrenInterval](SortOperation.md#getSelectedNonIgnoredChildrenInterval(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTextContentToSort](SortOperation.md#getTextContentToSort(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SimpleTableSortOperation

public SimpleTableSortOperation()

## Method Details

### getSortParent

public [AuthorElement](../../api/node/AuthorElement.md) getSortParent(int offset, [AuthorAccess](../../api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Get the table element whose rows will be sorted.
  Specified by: [getSortParent](SortOperation.md#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess)) in class [SortOperation](SortOperation.md) Parameters: offset - The offset where the operation was invoked. authorAccess - The [AuthorAccess](../../api/AuthorAccess.md). Returns: The parent node of the nodes which will be sorted. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) See Also:
        * [SortOperation.getSortParent(int, ro.sync.ecss.extensions.api.AuthorAccess)](SortOperation.md#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess))

### isIgnored

public boolean isIgnored([AuthorNode](../../api/node/AuthorNode.md) node)
 Description copied from class: [SortOperation](SortOperation.md#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))
Checks if a given node is ignored when sorting.
  Specified by: [isIgnored](SortOperation.md#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [SortOperation](SortOperation.md) Parameters: node - The node to be checked. Returns: true if the given node is ignored when sorting. See Also:
        * [SortOperation.isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode)](SortOperation.md#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))

### getSortKeysValues

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getSortKeysValues([AuthorNode](../../api/node/AuthorNode.md) node, [SortCriteriaInformation](SortCriteriaInformation.md) sortInfo)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from class: [SortOperation](SortOperation.md#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation))
Obtain the values of the keys that can be used for sorting.
  Specified by: [getSortKeysValues](SortOperation.md#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation)) in class [SortOperation](SortOperation.md) Parameters: node - The element which will be sorted. sortInfo - The sort information corresponding to the user choice. Returns: an array containing the values of the keys which can be used for sorting. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - If the text content cannot be obtained. See Also:
        * [SortOperation.getSortKeysValues(AuthorNode, SortCriteriaInformation)](SortOperation.md#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation))

### getSortCriteria

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> getSortCriteria([AuthorElement](../../api/node/AuthorElement.md) parent)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from class: [SortOperation](SortOperation.md#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement))
Obtain the sort criterion.
  Specified by: [getSortCriteria](SortOperation.md#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [SortOperation](SortOperation.md) Parameters: parent - The parent node of the nodes which will be sorted. Returns: A [SortCriteriaInformation](SortCriteriaInformation.md) containing the [CriterionInformation](CriterionInformation.md) objects. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) See Also:
        * [SortOperation.getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement)](SortOperation.md#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement))

### forceSortAll

protected boolean forceSortAll()
  Overrides: [forceSortAll](SortOperation.md#forceSortAll()) in class [SortOperation](SortOperation.md) Returns: true if the sort operation should not use the selected element and should always sort all elements. See Also:
        * [SortOperation.forceSortAll()](SortOperation.md#forceSortAll())

### isCaretInColumn

public boolean isCaretInColumn([AuthorAccess](../../api/AuthorAccess.md) authorAccess, int columnNumber)

Checks if the caret is in a cell which is in the given column.
  Parameters: authorAccess - The author access. columnNumber - The number of the column in which to check. Returns: true if the given column has a cell which contains the caret.
### getRowIndexForTableBody

protected int getRowIndexForTableBody([AuthorNode](../../api/node/AuthorNode.md) table)
 Description copied from class: [TableSortOperation](TableSortOperation.md#getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode))
Returns the visual row index of the actual table body if the table has separate head, foot element and table group elements.
  Specified by: [getRowIndexForTableBody](TableSortOperation.md#getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [TableSortOperation](TableSortOperation.md) See Also:
        * [TableSortOperation.getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode)](TableSortOperation.md#getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode))

### isTableElement

public abstract boolean isTableElement([AuthorElement](../../api/node/AuthorElement.md) node)

Return true if the given node is the table element.
  Parameters: node - The node to be checked. Returns: true if the given node is the table element.
### isHeadElement

public abstract boolean isHeadElement([AuthorElement](../../api/node/AuthorElement.md) node)

Returns true if the given node is the table header element.
  Parameters: node - The node to be checked. Returns: true if the given node is the table header.
### isRowElement

public abstract boolean isRowElement([AuthorElement](../../api/node/AuthorElement.md) node)

Returns true if the given node is a table row.
  Parameters: node - The node to be checked. Returns: true when the given node is a table row element.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
