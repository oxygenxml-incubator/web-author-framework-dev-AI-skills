Package [ro.sync.ecss.extensions.commons.table.operations.cals](package-summary.md)

# Class CALSAndHTMLTableSortOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.sort.SortOperation](../../../sort/SortOperation.md)
        * [ro.sync.ecss.extensions.commons.sort.TableSortOperation](../../../sort/TableSortOperation.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.CALSAndHTMLTableSortOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md)   Direct Known Subclasses: [DITACALSTableSortOperation](../../../../dita/topic/table/DITACALSTableSortOperation.md), [DocbookCALSTableSortOperation](../../../../docbook/table/DocbookCALSTableSortOperation.md), [XHTMLTableSortOperation](../xhtml/XHTMLTableSortOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class CALSAndHTMLTableSortOperation extends [TableSortOperation](../../../sort/TableSortOperation.md)
Table sort operation base for CALS and HTML tables.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.sort.[SortOperation](../../../sort/SortOperation.md)
 [authorAccess](../../../sort/SortOperation.md#authorAccess), [COLUMN](../../../sort/SortOperation.md#COLUMN)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [CALSAndHTMLTableSortOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [forceSortAll](#forceSortAll())()

 protected int [getRowIndexForTableBody](#getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../api/node/AuthorNode.md) parent)
Returns the visual row index of the actual table body if the table has separate head, foot element and table group elements.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](../../../sort/CriterionInformation.md)> [getSortCriteria](#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../api/node/AuthorElement.md) parent)
Obtain the sort criterion.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getSortKeysValues](#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation))([AuthorNode](../../../../api/node/AuthorNode.md) node, [SortCriteriaInformation](../../../sort/SortCriteriaInformation.md) sortInfo)
Obtain the values of the keys that can be used for sorting.
  [AuthorElement](../../../../api/node/AuthorElement.md) [getSortParent](#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess))(int offset, [AuthorAccess](../../../../api/AuthorAccess.md) authorAccess)
Obtain the parent node of all the nodes which will be sorted.
  boolean [isCaretInColumn](#isCaretInColumn(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, int columnNumber)
Checks if the caret is in a cell which is in the given column.
  boolean [isIgnored](#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../api/node/AuthorNode.md) node)
Checks if a given node is ignored when sorting.
  abstract boolean [isTable](#isTable(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../api/node/AuthorElement.md) element)
Returns true if the given element is a table header element.
  abstract boolean [isTableBody](#isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../api/node/AuthorElement.md) element)
Returns true if the given element is the table body element.
  abstract boolean [isTableFoot](#isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../api/node/AuthorElement.md) element)
Returns true if the given element is a table footer element.
  abstract boolean [isTableGroup](#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../api/node/AuthorElement.md) element)
Returns true if the given element is a table header element.
  abstract boolean [isTableHead](#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../api/node/AuthorElement.md) element)
Returns true if the given element is a table header element.
  abstract boolean [isTableRow](#isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../api/node/AuthorElement.md) element)
Returns true if the given element is a table row element.

### Methods inherited from class ro.sync.ecss.extensions.commons.sort.[TableSortOperation](../../../sort/TableSortOperation.md)
 [canBeSorted](../../../sort/TableSortOperation.md#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D)), [getHelpPageID](../../../sort/TableSortOperation.md#getHelpPageID())
### Methods inherited from class ro.sync.ecss.extensions.commons.sort.[SortOperation](../../../sort/SortOperation.md)
 [doOperation](../../../sort/SortOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../sort/SortOperation.md#getArguments()), [getDescription](../../../sort/SortOperation.md#getDescription()), [getNonIgnoredChildren](../../../sort/SortOperation.md#getNonIgnoredChildren(ro.sync.ecss.extensions.api.node.AuthorElement)), [getSelectedNonIgnoredChildrenInterval](../../../sort/SortOperation.md#getSelectedNonIgnoredChildrenInterval(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTextContentToSort](../../../sort/SortOperation.md#getTextContentToSort(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CALSAndHTMLTableSortOperation

public CALSAndHTMLTableSortOperation()

## Method Details

### getSortParent

public [AuthorElement](../../../../api/node/AuthorElement.md) getSortParent(int offset, [AuthorAccess](../../../../api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from class: [SortOperation](../../../sort/SortOperation.md#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess))
Obtain the parent node of all the nodes which will be sorted.
  Specified by: [getSortParent](../../../sort/SortOperation.md#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess)) in class [SortOperation](../../../sort/SortOperation.md) Parameters: offset - The offset where the operation was invoked. authorAccess - The [AuthorAccess](../../../../api/AuthorAccess.md). Returns: The parent node of the nodes which will be sorted. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - When the offset is negative or greater than the content length. See Also:
        * [SortOperation.getSortParent(int, ro.sync.ecss.extensions.api.AuthorAccess)](../../../sort/SortOperation.md#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess))

### isIgnored

public boolean isIgnored([AuthorNode](../../../../api/node/AuthorNode.md) node)
 Description copied from class: [SortOperation](../../../sort/SortOperation.md#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))
Checks if a given node is ignored when sorting.
  Specified by: [isIgnored](../../../sort/SortOperation.md#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [SortOperation](../../../sort/SortOperation.md) Parameters: node - The node to be checked. Returns: true if the given node is ignored when sorting. See Also:
        * [SortOperation.isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../sort/SortOperation.md#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))

### getSortKeysValues

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getSortKeysValues([AuthorNode](../../../../api/node/AuthorNode.md) node, [SortCriteriaInformation](../../../sort/SortCriteriaInformation.md) sortInfo)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from class: [SortOperation](../../../sort/SortOperation.md#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation))
Obtain the values of the keys that can be used for sorting.
  Specified by: [getSortKeysValues](../../../sort/SortOperation.md#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation)) in class [SortOperation](../../../sort/SortOperation.md) Parameters: node - The element which will be sorted. sortInfo - The sort information corresponding to the user choice. Returns: an array containing the values of the keys which can be used for sorting. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - If the text content cannot be obtained. See Also:
        * [SortOperation.getSortKeysValues(AuthorNode, SortCriteriaInformation)](../../../sort/SortOperation.md#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation))

### getSortCriteria

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](../../../sort/CriterionInformation.md)> getSortCriteria([AuthorElement](../../../../api/node/AuthorElement.md) parent)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from class: [SortOperation](../../../sort/SortOperation.md#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement))
Obtain the sort criterion.
  Specified by: [getSortCriteria](../../../sort/SortOperation.md#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [SortOperation](../../../sort/SortOperation.md) Parameters: parent - The parent node of the nodes which will be sorted. Returns: A [SortCriteriaInformation](../../../sort/SortCriteriaInformation.md) containing the [CriterionInformation](../../../sort/CriterionInformation.md) objects. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) See Also:
        * [SortOperation.getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../sort/SortOperation.md#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement))

### forceSortAll

protected boolean forceSortAll()
  Overrides: [forceSortAll](../../../sort/SortOperation.md#forceSortAll()) in class [SortOperation](../../../sort/SortOperation.md) Returns: true if the sort operation should not use the selected element and should always sort all elements. See Also:
        * [SortOperation.forceSortAll()](../../../sort/SortOperation.md#forceSortAll())

### isCaretInColumn

public boolean isCaretInColumn([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, int columnNumber)

Checks if the caret is in a cell which is in the given column.
  Parameters: authorAccess - The author access. columnNumber - The number of the column in which to check. Returns: true if the given column has a cell which contains the caret.
### getRowIndexForTableBody

protected int getRowIndexForTableBody([AuthorNode](../../../../api/node/AuthorNode.md) parent)
 Description copied from class: [TableSortOperation](../../../sort/TableSortOperation.md#getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode))
Returns the visual row index of the actual table body if the table has separate head, foot element and table group elements.
  Specified by: [getRowIndexForTableBody](../../../sort/TableSortOperation.md#getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [TableSortOperation](../../../sort/TableSortOperation.md) See Also:
        * [TableSortOperation.getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../sort/TableSortOperation.md#getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode))

### isTableBody

public abstract boolean isTableBody([AuthorElement](../../../../api/node/AuthorElement.md) element)

Returns true if the given element is the table body element.
  Parameters: element - The element to be checked. Returns: true if the given element is the table body element.
### isTableRow

public abstract boolean isTableRow([AuthorElement](../../../../api/node/AuthorElement.md) element)

Returns true if the given element is a table row element.
  Parameters: element - The element to be checked. Returns: true if the given element is a table row element.
### isTableHead

public abstract boolean isTableHead([AuthorElement](../../../../api/node/AuthorElement.md) element)

Returns true if the given element is a table header element.
  Parameters: element - The element to be checked. Returns: true if the given element is a table header element.
### isTableFoot

public abstract boolean isTableFoot([AuthorElement](../../../../api/node/AuthorElement.md) element)

Returns true if the given element is a table footer element.
  Parameters: element - The element to be checked. Returns: true if the given element is a table footer element.
### isTable

public abstract boolean isTable([AuthorElement](../../../../api/node/AuthorElement.md) element)

Returns true if the given element is a table header element.
  Parameters: element - The element to be checked. Returns: true if the given element is a table header element.
### isTableGroup

public abstract boolean isTableGroup([AuthorElement](../../../../api/node/AuthorElement.md) element)

Returns true if the given element is a table header element.
  Parameters: element - The element to be checked. Returns: true if the given element is a table header element.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
