Package [ro.sync.ecss.extensions.commons.sort](package-summary.md)

# Class DITAListSortOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.sort.SortOperation](SortOperation.md)
        * ro.sync.ecss.extensions.commons.sort.DITAListSortOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DITAListSortOperation extends [SortOperation](SortOperation.md)
DITA list sort operation implementation.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.sort.[SortOperation](SortOperation.md)
 [authorAccess](SortOperation.md#authorAccess), [COLUMN](SortOperation.md#COLUMN)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [DITAListSortOperation](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [canBeSorted](#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D))([AuthorElement](../../api/node/AuthorElement.md) parent, int[] selectedNonIgnoredChildrenInterval)
Check if the parent element selected children can be sorted.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID())()
Get the ID of the help page which will be called by the end user.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> [getSortCriteria](#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) parent)
Obtain the sort criterion.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getSortKeysValues](#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation))([AuthorNode](../../api/node/AuthorNode.md) node, [SortCriteriaInformation](SortCriteriaInformation.md) sortInfo)
Obtain the values of the keys that can be used for sorting.
  [AuthorElement](../../api/node/AuthorElement.md) [getSortParent](#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess))(int offset, [AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Obtain the parent node of all the nodes which will be sorted.
  boolean [isIgnored](#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
Checks if a given node is ignored when sorting.

### Methods inherited from class ro.sync.ecss.extensions.commons.sort.[SortOperation](SortOperation.md)
 [doOperation](SortOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [forceSortAll](SortOperation.md#forceSortAll()), [getArguments](SortOperation.md#getArguments()), [getDescription](SortOperation.md#getDescription()), [getNonIgnoredChildren](SortOperation.md#getNonIgnoredChildren(ro.sync.ecss.extensions.api.node.AuthorElement)), [getSelectedNonIgnoredChildrenInterval](SortOperation.md#getSelectedNonIgnoredChildrenInterval(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTextContentToSort](SortOperation.md#getTextContentToSort(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAListSortOperation

public DITAListSortOperation()

Constructor.

## Method Details

### getSortParent

public [AuthorElement](../../api/node/AuthorElement.md) getSortParent(int offset, [AuthorAccess](../../api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from class: [SortOperation](SortOperation.md#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess))
Obtain the parent node of all the nodes which will be sorted.
  Specified by: [getSortParent](SortOperation.md#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess)) in class [SortOperation](SortOperation.md) Parameters: offset - The offset where the operation was invoked. authorAccess - The [AuthorAccess](../../api/AuthorAccess.md). Returns: The parent node of the nodes which will be sorted. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - When the offset is negative or greater than the content length. See Also:
        * [SortOperation.getSortParent(int, ro.sync.ecss.extensions.api.AuthorAccess)](SortOperation.md#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess))

### isIgnored

public boolean isIgnored([AuthorNode](../../api/node/AuthorNode.md) node)
 Description copied from class: [SortOperation](SortOperation.md#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))
Checks if a given node is ignored when sorting.
  Specified by: [isIgnored](SortOperation.md#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [SortOperation](SortOperation.md) Parameters: node - The node to be checked. Returns: true if the given node is ignored when sorting. See Also:
        * [SortOperation.isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode)](SortOperation.md#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))

### canBeSorted

public void canBeSorted([AuthorElement](../../api/node/AuthorElement.md) parent, int[] selectedNonIgnoredChildrenInterval)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from class: [SortOperation](SortOperation.md#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D))
Check if the parent element selected children can be sorted. For example a table row containing a cell with rowspan cannot be sorted and stops the operation.
  Specified by: [canBeSorted](SortOperation.md#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D)) in class [SortOperation](SortOperation.md) Parameters: parent - The parent of the elements which will be sorted. selectedNonIgnoredChildrenInterval - The interval of selected children indices. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - When the given node is not sortable. For example a table row containing a cell with multiple rowspan stops the operation. See Also:
        * [SortOperation.canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement, int[])](SortOperation.md#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D))

### getSortKeysValues

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getSortKeysValues([AuthorNode](../../api/node/AuthorNode.md) node, [SortCriteriaInformation](SortCriteriaInformation.md) sortInfo)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from class: [SortOperation](SortOperation.md#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation))
Obtain the values of the keys that can be used for sorting.
  Specified by: [getSortKeysValues](SortOperation.md#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation)) in class [SortOperation](SortOperation.md) Parameters: node - The element which will be sorted. sortInfo - The sort information corresponding to the user choice. Returns: an array containing the values of the keys which can be used for sorting. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - If the text content cannot be obtained. See Also:
        * [SortOperation.getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode, ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation)](SortOperation.md#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation))

### getSortCriteria

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> getSortCriteria([AuthorElement](../../api/node/AuthorElement.md) parent)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from class: [SortOperation](SortOperation.md#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement))
Obtain the sort criterion.
  Specified by: [getSortCriteria](SortOperation.md#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [SortOperation](SortOperation.md) Parameters: parent - The parent node of the nodes which will be sorted. Returns: A [SortCriteriaInformation](SortCriteriaInformation.md) containing the [CriterionInformation](CriterionInformation.md) objects. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) See Also:
        * [SortOperation.getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement)](SortOperation.md#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement))

### getHelpPageID

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID()
 Description copied from class: [SortOperation](SortOperation.md#getHelpPageID())
Get the ID of the help page which will be called by the end user.
  Overrides: [getHelpPageID](SortOperation.md#getHelpPageID()) in class [SortOperation](SortOperation.md) Returns: the ID of the help page which will be called by the end user or null. See Also:
        * [SortOperation.getHelpPageID()](SortOperation.md#getHelpPageID())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
