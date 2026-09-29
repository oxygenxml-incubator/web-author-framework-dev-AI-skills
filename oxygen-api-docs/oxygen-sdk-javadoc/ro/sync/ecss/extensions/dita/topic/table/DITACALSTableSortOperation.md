Package [ro.sync.ecss.extensions.dita.topic.table](package-summary.md)

# Class DITACALSTableSortOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.sort.SortOperation](../../../commons/sort/SortOperation.md)
        * [ro.sync.ecss.extensions.commons.sort.TableSortOperation](../../../commons/sort/TableSortOperation.md)
            * [ro.sync.ecss.extensions.commons.table.operations.cals.CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md)
                * ro.sync.ecss.extensions.dita.topic.table.DITACALSTableSortOperation
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DITACALSTableSortOperation extends [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md)
DITA CALS table sort operation implementation.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.sort.[SortOperation](../../../commons/sort/SortOperation.md)
 [authorAccess](../../../commons/sort/SortOperation.md#authorAccess), [COLUMN](../../../commons/sort/SortOperation.md#COLUMN)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [DITACALSTableSortOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [isTable](#isTable(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) element)
Returns true if the given element is a table header element.
  boolean [isTableBody](#isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Returns true if the given element is the table body element.
  boolean [isTableFoot](#isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) element)
Returns true if the given element is a table footer element.
  boolean [isTableGroup](#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) element)
Returns true if the given element is a table header element.
  boolean [isTableHead](#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Returns true if the given element is a table header element.
  boolean [isTableRow](#isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Returns true if the given element is a table row element.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.cals.[CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md)
 [forceSortAll](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#forceSortAll()), [getRowIndexForTableBody](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode)), [getSortCriteria](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement)), [getSortKeysValues](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation)), [getSortParent](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess)), [isCaretInColumn](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isCaretInColumn(ro.sync.ecss.extensions.api.AuthorAccess,int)), [isIgnored](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class ro.sync.ecss.extensions.commons.sort.[TableSortOperation](../../../commons/sort/TableSortOperation.md)
 [canBeSorted](../../../commons/sort/TableSortOperation.md#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D)), [getHelpPageID](../../../commons/sort/TableSortOperation.md#getHelpPageID())
### Methods inherited from class ro.sync.ecss.extensions.commons.sort.[SortOperation](../../../commons/sort/SortOperation.md)
 [doOperation](../../../commons/sort/SortOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../commons/sort/SortOperation.md#getArguments()), [getDescription](../../../commons/sort/SortOperation.md#getDescription()), [getNonIgnoredChildren](../../../commons/sort/SortOperation.md#getNonIgnoredChildren(ro.sync.ecss.extensions.api.node.AuthorElement)), [getSelectedNonIgnoredChildrenInterval](../../../commons/sort/SortOperation.md#getSelectedNonIgnoredChildrenInterval(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTextContentToSort](../../../commons/sort/SortOperation.md#getTextContentToSort(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITACALSTableSortOperation

public DITACALSTableSortOperation()

## Method Details

### isTableBody

public boolean isTableBody([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from class: [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement))
Returns true if the given element is the table body element.
  Specified by: [isTableBody](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md) Parameters: node - The element to be checked. Returns: true if the given element is the table body element. See Also:
        * [CALSAndHTMLTableSortOperation.isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTableRow

public boolean isTableRow([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from class: [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement))
Returns true if the given element is a table row element.
  Specified by: [isTableRow](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md) Parameters: node - The element to be checked. Returns: true if the given element is a table row element. See Also:
        * [CALSAndHTMLTableSortOperation.isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTableHead

public boolean isTableHead([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from class: [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement))
Returns true if the given element is a table header element.
  Specified by: [isTableHead](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md) Parameters: node - The element to be checked. Returns: true if the given element is a table header element. See Also:
        * [CALSAndHTMLTableSortOperation.isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTableFoot

public boolean isTableFoot([AuthorElement](../../../api/node/AuthorElement.md) element)
 Description copied from class: [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement))
Returns true if the given element is a table footer element.
  Specified by: [isTableFoot](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md) Parameters: element - The element to be checked. Returns: true if the given element is a table footer element. See Also:
        * [CALSAndHTMLTableSortOperation.isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTable

public boolean isTable([AuthorElement](../../../api/node/AuthorElement.md) element)
 Description copied from class: [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTable(ro.sync.ecss.extensions.api.node.AuthorElement))
Returns true if the given element is a table header element.
  Specified by: [isTable](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTable(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md) Parameters: element - The element to be checked. Returns: true if the given element is a table header element. See Also:
        * [CALSAndHTMLTableSortOperation.isTable(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTable(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTableGroup

public boolean isTableGroup([AuthorElement](../../../api/node/AuthorElement.md) element)
 Description copied from class: [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement))
Returns true if the given element is a table header element.
  Specified by: [isTableGroup](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [CALSAndHTMLTableSortOperation](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md) Parameters: element - The element to be checked. Returns: true if the given element is a table header element. See Also:
        * [CALSAndHTMLTableSortOperation.isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
