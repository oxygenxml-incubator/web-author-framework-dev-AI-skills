Package [ro.sync.ecss.extensions.commons.sort](package-summary.md)

# Class SortOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.sort.SortOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   Direct Known Subclasses: [DITAListSortOperation](DITAListSortOperation.md), [DocbookListSortOperation](DocbookListSortOperation.md), [TableSortOperation](TableSortOperation.md), [TEIListSortOperation](TEIListSortOperation.md), [XHTMLListSortOperation](XHTMLListSortOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class SortOperation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorOperation](../../api/AuthorOperation.md)
Sort operations base class.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [AuthorAccess](../../api/AuthorAccess.md) [authorAccess](#authorAccess)
The Author access.
  protected static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [COLUMN](#COLUMN)
String used in the default name for the sorting criterion.

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [SortOperation](#%3Cinit%3E(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) selElementsString, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) allElementsString)
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract void [canBeSorted](#canBeSorted(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D))([AuthorElement](../../api/node/AuthorElement.md) parent, int[] selectedNonIgnoredChildrenInterval)
Check if the parent element selected children can be sorted.
  void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)
Perform the actual operation.
  protected boolean [forceSortAll](#forceSortAll())()

 [ArgumentDescriptor](../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID())()
Get the ID of the help page which will be called by the end user.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](../../api/node/AuthorNode.md)> [getNonIgnoredChildren](#getNonIgnoredChildren(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) parent)
Returns a list of non ignored children.
  int[] [getSelectedNonIgnoredChildrenInterval](#getSelectedNonIgnoredChildrenInterval(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) parent)
Return the interval of sortable nodes indices covered by selection.
  abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> [getSortCriteria](#getSortCriteria(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) parent)
Obtain the sort criterion.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getSortKeysValues](#getSortKeysValues(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation))([AuthorNode](../../api/node/AuthorNode.md) node, [SortCriteriaInformation](SortCriteriaInformation.md) sortInfo)
Obtain the values of the keys that can be used for sorting.
  abstract [AuthorElement](../../api/node/AuthorElement.md) [getSortParent](#getSortParent(int,ro.sync.ecss.extensions.api.AuthorAccess))(int offset, [AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Obtain the parent node of all the nodes which will be sorted.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTextContentToSort](#getTextContentToSort(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
Given a node obtain the content to be used during the sort operation.
  abstract boolean [isIgnored](#isIgnored(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
Checks if a given node is ignored when sorting.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### COLUMN

protected static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) COLUMN

String used in the default name for the sorting criterion.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.sort.SortOperation.COLUMN)

### authorAccess

protected [AuthorAccess](../../api/AuthorAccess.md) authorAccess

The Author access.

## Constructor Details

### SortOperation

public SortOperation([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) selElementsString, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) allElementsString)

Constructor.
  Parameters: selElementsString - The name of the "selected elements" radio combo. allElementsString - The name of the "all elements" radio combo.
## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../api/Extension.md#getDescription()) in interface [Extension](../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

### doOperation

public void doOperation([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation. You can check if the operation was invoked from the oXygen standalone application or from the oXygen plugin for Eclipse by using the method: [ApplicationInformationAccess.getPlatform()](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()). To get to the [Workspace](../../../../exml/workspace/api/Workspace.md) you may use: [AuthorAccess.getWorkspaceAccess()](../../api/AuthorAccess.md#getWorkspaceAccess()).
  Specified by: [doOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in interface [AuthorOperation](../../api/AuthorOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AuthorOperation.doOperation(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### canBeSorted

public abstract void canBeSorted([AuthorElement](../../api/node/AuthorElement.md) parent, int[] selectedNonIgnoredChildrenInterval)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Check if the parent element selected children can be sorted. For example a table row containing a cell with rowspan cannot be sorted and stops the operation.
  Parameters: parent - The parent of the elements which will be sorted. selectedNonIgnoredChildrenInterval - The interval of selected children indices. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - When the given node is not sortable. For example a table row containing a cell with multiple rowspan stops the operation.
### getSelectedNonIgnoredChildrenInterval

public int[] getSelectedNonIgnoredChildrenInterval([AuthorElement](../../api/node/AuthorElement.md) parent)

Return the interval of sortable nodes indices covered by selection.
  Parameters: parent - The parent node for the sortable nodes. Returns: An interval of sortable nodes indices that can be sorted. Typically it returns a non-null interval when the selected sortable nodes from parent are part of a continuous sequence. If the selection must be ignored or the sequence of selected nodes is discontinuous it returns null.
### forceSortAll

protected boolean forceSortAll()
  Returns: true if the sort operation should not use the selected element and should always sort all elements.
### getNonIgnoredChildren

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](../../api/node/AuthorNode.md)> getNonIgnoredChildren([AuthorElement](../../api/node/AuthorElement.md) parent)

Returns a list of non ignored children.
  Parameters: parent - The parent node. Returns: A list of non ignored children.
### getSortParent

public abstract [AuthorElement](../../api/node/AuthorElement.md) getSortParent(int offset, [AuthorAccess](../../api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Obtain the parent node of all the nodes which will be sorted.
  Parameters: offset - The offset where the operation was invoked. authorAccess - The [AuthorAccess](../../api/AuthorAccess.md). Returns: The parent node of the nodes which will be sorted. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - When the offset is negative or greater than the content length.
### isIgnored

public abstract boolean isIgnored([AuthorNode](../../api/node/AuthorNode.md) node)

Checks if a given node is ignored when sorting.
  Parameters: node - The node to be checked. Returns: true if the given node is ignored when sorting.
### getSortKeysValues

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getSortKeysValues([AuthorNode](../../api/node/AuthorNode.md) node, [SortCriteriaInformation](SortCriteriaInformation.md) sortInfo)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Obtain the values of the keys that can be used for sorting.
  Parameters: node - The element which will be sorted. sortInfo - The sort information corresponding to the user choice. Returns: an array containing the values of the keys which can be used for sorting. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - If the text content cannot be obtained.
### getSortCriteria

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> getSortCriteria([AuthorElement](../../api/node/AuthorElement.md) parent)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Obtain the sort criterion.
  Parameters: parent - The parent node of the nodes which will be sorted. Returns: A [SortCriteriaInformation](SortCriteriaInformation.md) containing the [CriterionInformation](CriterionInformation.md) objects. Throws: [AuthorOperationException](../../api/AuthorOperationException.md)
### getArguments

public [ArgumentDescriptor](../../api/ArgumentDescriptor.md)[] getArguments()
  Specified by: [getArguments](../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../api/AuthorOperation.md) Returns: An array of [ArgumentDescriptor](../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../api/AuthorOperation.md#getArguments())

### getTextContentToSort

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTextContentToSort([AuthorNode](../../api/node/AuthorNode.md) node)

Given a node obtain the content to be used during the sort operation. In general this text does not contain the deleted changes and the leading or trailing spaces.
  Parameters: node - The node to get the value for. Returns: The test to be considered as sort key value.
### getHelpPageID

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID()

Get the ID of the help page which will be called by the end user.
  Returns: the ID of the help page which will be called by the end user or null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
