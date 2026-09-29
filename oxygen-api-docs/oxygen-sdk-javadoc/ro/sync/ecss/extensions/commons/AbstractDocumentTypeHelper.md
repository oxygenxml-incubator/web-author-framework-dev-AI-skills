Package [ro.sync.ecss.extensions.commons](package-summary.md)

# Class AbstractDocumentTypeHelper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.AbstractDocumentTypeHelper
   All Implemented Interfaces: [AuthorTableHelper](table/operations/AuthorTableHelper.md)   Direct Known Subclasses: [CALSDocumentTypeHelper](table/operations/cals/CALSDocumentTypeHelper.md), [DITARelTableDocumentTypeHelper](../dita/map/table/DITARelTableDocumentTypeHelper.md), [DITASimpleTableDocumentTypeHelper](../dita/topic/table/simpletable/DITASimpleTableDocumentTypeHelper.md), [TEIDocumentTypeHelper](../tei/TEIDocumentTypeHelper.md), [XHTMLDocumentTypeHelper](table/operations/xhtml/XHTMLDocumentTypeHelper.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class AbstractDocumentTypeHelper extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorTableHelper](table/operations/AuthorTableHelper.md)
Abstract implementation of the document type helper.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.[AuthorTableHelper](table/operations/AuthorTableHelper.md)
 [TYPE_CELL](table/operations/AuthorTableHelper.md#TYPE_CELL), [TYPE_ROW](table/operations/AuthorTableHelper.md#TYPE_ROW), [TYPE_TABLE](table/operations/AuthorTableHelper.md#TYPE_TABLE)
## Constructor Summary
 Constructors
Constructor

Description
 [AbstractDocumentTypeHelper](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getAllowedCellAttributesToCopy](#getAllowedCellAttributesToCopy())()
Get a list of allowed cell attributes to copy when creating a new row based on an older one.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableCellElementNames](#getTableCellElementNames())()
Returns the possible local names of the elements that represents a table cell.
  [AuthorNode](../api/node/AuthorNode.md) [getTableElementForDeletion](#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) element)
When we delete all the rows or all the columns of a table, we also want to delete the entire table element.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableElementLocalName](#getTableElementLocalName())()
Returns the possible local names of the elements that represents a table.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableRowElementNames](#getTableRowElementNames())()
Return the possible local names of the elements that represent a table row.
  boolean [isColspec](#isColspec(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Check if a node is a colspec node.
  boolean [isContentReference](#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Check if this node references another node which should replace it entirely.
  protected boolean [isElement](#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([AuthorNode](../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elemLocalName)
Test if a given node is an element and has the a specific local name.
  boolean [isTable](#isTable(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Check if an [AuthorNode](../api/node/AuthorNode.md) is a table node.
  boolean [isTableCell](#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Check if an [AuthorNode](../api/node/AuthorNode.md) is a table cell node.
  boolean [isTableRow](#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Check if an [AuthorNode](../api/node/AuthorNode.md) is a table row node.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.commons.table.operations.[AuthorTableHelper](table/operations/AuthorTableHelper.md)
 [checkTableColSpanIsDefined](table/operations/AuthorTableHelper.md#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement)), [getIgnoredCellIDAttributes](table/operations/AuthorTableHelper.md#getIgnoredCellIDAttributes()), [getIgnoredColumnAttributes](table/operations/AuthorTableHelper.md#getIgnoredColumnAttributes()), [getIgnoredRowAttributes](table/operations/AuthorTableHelper.md#getIgnoredRowAttributes()), [getTableCellSpanProvider](table/operations/AuthorTableHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement)), [updateTableColSpan](table/operations/AuthorTableHelper.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [updateTableColumnNumber](table/operations/AuthorTableHelper.md#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)), [updateTableRowNumber](table/operations/AuthorTableHelper.md#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)), [updateTableRowSpan](table/operations/AuthorTableHelper.md#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))
## Constructor Details

### AbstractDocumentTypeHelper

public AbstractDocumentTypeHelper()

## Method Details

### isElement

protected boolean isElement([AuthorNode](../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elemLocalName)

Test if a given node is an element and has the a specific local name.
  Parameters: node - The [AuthorNode](../api/node/AuthorNode.md) to be checked. elemLocalName - The local name of the element. Returns: true if the given [AuthorNode](../api/node/AuthorNode.md) is an element and its local name matches the given string.
### isTableCell

public boolean isTableCell([AuthorNode](../api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorTableHelper](table/operations/AuthorTableHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if an [AuthorNode](../api/node/AuthorNode.md) is a table cell node.
  Specified by: [isTableCell](table/operations/AuthorTableHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](table/operations/AuthorTableHelper.md) Parameters: node - The [AuthorNode](../api/node/AuthorNode.md) to be checked. Returns: true if the node is a table cell node, false otherwise. See Also:
        * [AuthorTableHelper.isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode)](table/operations/AuthorTableHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode))

### isTable

public boolean isTable([AuthorNode](../api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorTableHelper](table/operations/AuthorTableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if an [AuthorNode](../api/node/AuthorNode.md) is a table node.
  Specified by: [isTable](table/operations/AuthorTableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](table/operations/AuthorTableHelper.md) Parameters: node - The [AuthorNode](../api/node/AuthorNode.md) to be checked. Returns: true if the node is a table node, false otherwise. See Also:
        * [AuthorTableHelper.isTable(ro.sync.ecss.extensions.api.node.AuthorNode)](table/operations/AuthorTableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode))

### isTableRow

public boolean isTableRow([AuthorNode](../api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorTableHelper](table/operations/AuthorTableHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if an [AuthorNode](../api/node/AuthorNode.md) is a table row node.
  Specified by: [isTableRow](table/operations/AuthorTableHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](table/operations/AuthorTableHelper.md) Parameters: node - The [AuthorNode](../api/node/AuthorNode.md) to be checked. Returns: true if the node is a table row node, false otherwise. See Also:
        * [AuthorTableHelper.isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode)](table/operations/AuthorTableHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))

### getTableElementForDeletion

public [AuthorNode](../api/node/AuthorNode.md) getTableElementForDeletion([AuthorNode](../api/node/AuthorNode.md) element)
 Description copied from interface: [AuthorTableHelper](table/operations/AuthorTableHelper.md#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode))
When we delete all the rows or all the columns of a table, we also want to delete the entire table element. OBS: For CALS tables we don't want to delete only the "tgroup", but the parent table element itself.
  Specified by: [getTableElementForDeletion](table/operations/AuthorTableHelper.md#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](table/operations/AuthorTableHelper.md) Parameters: element - the node whose parent table we are looking for. Returns: the table element to be deleted. See Also:
        * [AuthorTableHelper.getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode)](table/operations/AuthorTableHelper.md#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode))

### getTableCellElementNames

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableCellElementNames()

Returns the possible local names of the elements that represents a table cell.
  Returns: The local names of the elements that represents a table cell. Not null.
### getTableRowElementNames

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableRowElementNames()

Return the possible local names of the elements that represent a table row.
  Returns: The local names of the elements that represent a table row.
### getTableElementLocalName

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableElementLocalName()

Returns the possible local names of the elements that represents a table.
  Returns: The local names of the elements that represents a table.
### getAllowedCellAttributesToCopy

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getAllowedCellAttributesToCopy()

Get a list of allowed cell attributes to copy when creating a new row based on an older one.
  Returns: a list of allowed cell attributes to copy when creating a new row. If it returns null, the list of ignored attributes will be used by default.
### isContentReference

public boolean isContentReference([AuthorNode](../api/node/AuthorNode.md) node)

Check if this node references another node which should replace it entirely. This is used in the tables to replace conreffed table rows entirely
  Parameters: node - The node Returns: true if this node references another node which should replace it entirely.
### isColspec

public boolean isColspec([AuthorNode](../api/node/AuthorNode.md) node)

Check if a node is a colspec node.
  Specified by: [isColspec](table/operations/AuthorTableHelper.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](table/operations/AuthorTableHelper.md) Parameters: node - The node. Returns: true if a node is a colspec node.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
