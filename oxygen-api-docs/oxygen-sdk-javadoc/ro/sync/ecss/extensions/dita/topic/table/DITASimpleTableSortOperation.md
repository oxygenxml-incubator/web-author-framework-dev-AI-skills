Package [ro.sync.ecss.extensions.dita.topic.table](package-summary.md)

# Class DITASimpleTableSortOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.sort.SortOperation](../../../commons/sort/SortOperation.md)
        * [ro.sync.ecss.extensions.commons.sort.TableSortOperation](../../../commons/sort/TableSortOperation.md)
            * [ro.sync.ecss.extensions.commons.sort.SimpleTableSortOperation](../../../commons/sort/SimpleTableSortOperation.md)
                * ro.sync.ecss.extensions.dita.topic.table.DITASimpleTableSortOperation
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DITASimpleTableSortOperation extends [SimpleTableSortOperation](../../../commons/sort/SimpleTableSortOperation.md)
DITA simple table sort operation implementation.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.sort.[SortOperation](../../../commons/sort/SortOperation.md)
 [authorAccess](../../../commons/sort/SortOperation.md#authorAccess), [COLUMN](../../../commons/sort/SortOperation.md#COLUMN)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [DITASimpleTableSortOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [isHeadElement](#isHeadElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Returns true if the given node is the table header element.
  boolean [isRowElement](#isRowElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Returns true if the given node is a table row.
  boolean [isTableElement](#isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Return true if the given node is the table element.

### Methods inherited from class ro.sync.ecss.extensions.commons.sort.[SimpleTableSortOperation](../../../commons/sort/SimpleTableSortOperation.md)
 [forceSortAll](../../../commons/sort/SimpleTableSortOperation.md#forceSortAll()), [getRowIndexForTableBody](../../../commons/sort/SimpleTableSortOperation.md#getRowIndexForTableBody(ro.sync.ecss.extensions.api.node.AuthorNode)), [getSortCriteria](../../../commons/sort/SimpleTableSortOperation.md#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement)), [getSortKeysValues](../../../commons/sort/SimpleTableSortOperation.md#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation)), [getSortParent](../../../commons/sort/SimpleTableSortOperation.md#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess)), [isCaretInColumn](../../../commons/sort/SimpleTableSortOperation.md#isCaretInColumn(ro.sync.ecss.extensions.api.AuthorAccess,int)), [isIgnored](../../../commons/sort/SimpleTableSortOperation.md#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class ro.sync.ecss.extensions.commons.sort.[TableSortOperation](../../../commons/sort/TableSortOperation.md)
 [canBeSorted](../../../commons/sort/TableSortOperation.md#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D)), [getHelpPageID](../../../commons/sort/TableSortOperation.md#getHelpPageID())
### Methods inherited from class ro.sync.ecss.extensions.commons.sort.[SortOperation](../../../commons/sort/SortOperation.md)
 [doOperation](../../../commons/sort/SortOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../commons/sort/SortOperation.md#getArguments()), [getDescription](../../../commons/sort/SortOperation.md#getDescription()), [getNonIgnoredChildren](../../../commons/sort/SortOperation.md#getNonIgnoredChildren(ro.sync.ecss.extensions.api.node.AuthorElement)), [getSelectedNonIgnoredChildrenInterval](../../../commons/sort/SortOperation.md#getSelectedNonIgnoredChildrenInterval(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTextContentToSort](../../../commons/sort/SortOperation.md#getTextContentToSort(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITASimpleTableSortOperation

public DITASimpleTableSortOperation()

## Method Details

### isTableElement

public boolean isTableElement([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from class: [SimpleTableSortOperation](../../../commons/sort/SimpleTableSortOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement))
Return true if the given node is the table element.
  Specified by: [isTableElement](../../../commons/sort/SimpleTableSortOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [SimpleTableSortOperation](../../../commons/sort/SimpleTableSortOperation.md) Parameters: node - The node to be checked. Returns: true if the given node is the table element. See Also:
        * [SimpleTableSortOperation.isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../commons/sort/SimpleTableSortOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement))

### isHeadElement

public boolean isHeadElement([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from class: [SimpleTableSortOperation](../../../commons/sort/SimpleTableSortOperation.md#isHeadElement(ro.sync.ecss.extensions.api.node.AuthorElement))
Returns true if the given node is the table header element.
  Specified by: [isHeadElement](../../../commons/sort/SimpleTableSortOperation.md#isHeadElement(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [SimpleTableSortOperation](../../../commons/sort/SimpleTableSortOperation.md) Parameters: node - The node to be checked. Returns: true if the given node is the table header. See Also:
        * [SimpleTableSortOperation.isHeadElement(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../commons/sort/SimpleTableSortOperation.md#isHeadElement(ro.sync.ecss.extensions.api.node.AuthorElement))

### isRowElement

public boolean isRowElement([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from class: [SimpleTableSortOperation](../../../commons/sort/SimpleTableSortOperation.md#isRowElement(ro.sync.ecss.extensions.api.node.AuthorElement))
Returns true if the given node is a table row.
  Specified by: [isRowElement](../../../commons/sort/SimpleTableSortOperation.md#isRowElement(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [SimpleTableSortOperation](../../../commons/sort/SimpleTableSortOperation.md) Parameters: node - The node to be checked. Returns: true when the given node is a table row element. See Also:
        * [SimpleTableSortOperation.isRowElement(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../commons/sort/SimpleTableSortOperation.md#isRowElement(ro.sync.ecss.extensions.api.node.AuthorElement))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
