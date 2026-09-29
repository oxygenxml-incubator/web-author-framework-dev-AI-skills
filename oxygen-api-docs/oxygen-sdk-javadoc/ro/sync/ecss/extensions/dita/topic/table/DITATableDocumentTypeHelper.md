Package [ro.sync.ecss.extensions.dita.topic.table](package-summary.md)

# Class DITATableDocumentTypeHelper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md)
        * [ro.sync.ecss.extensions.commons.table.operations.cals.CALSDocumentTypeHelper](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md)
            * ro.sync.ecss.extensions.dita.topic.table.DITATableDocumentTypeHelper
   All Implemented Interfaces: [AuthorTableHelper](../../../commons/table/operations/AuthorTableHelper.md), [CALSConstants](../../../commons/table/operations/cals/CALSConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class DITATableDocumentTypeHelper extends [CALSDocumentTypeHelper](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md)
Implementation of the document type helper for DITA CALS table model. Looks at class attribute values.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.[AuthorTableHelper](../../../commons/table/operations/AuthorTableHelper.md)
 [TYPE_CELL](../../../commons/table/operations/AuthorTableHelper.md#TYPE_CELL), [TYPE_ROW](../../../commons/table/operations/AuthorTableHelper.md#TYPE_ROW), [TYPE_TABLE](../../../commons/table/operations/AuthorTableHelper.md#TYPE_TABLE)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](../../../commons/table/operations/cals/CALSConstants.md)
 [ATTRIBUTE_NAME_ALIGN](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ALIGN), [ATTRIBUTE_NAME_COLNAME](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLNAME), [ATTRIBUTE_NAME_COLNUM](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLNUM), [ATTRIBUTE_NAME_COLS](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_COLSEP](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLSEP), [ATTRIBUTE_NAME_COLWIDTH](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLWIDTH), [ATTRIBUTE_NAME_ID](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_MOREROWS](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_MOREROWS), [ATTRIBUTE_NAME_NAMEEND](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_NAMEEND), [ATTRIBUTE_NAME_NAMEST](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_NAMEST), [ATTRIBUTE_NAME_ROWSEP](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ROWSEP), [ATTRIBUTE_NAME_SPANNAME](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_SPANNAME), [ATTRIBUTE_NAME_TABLE_WIDTH](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_TABLE_WIDTH), [ATTRIBUTE_NAME_XML_ID](../../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_COLSPEC](../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_COLSPEC), [ELEMENT_NAME_ENTRY](../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_ENTRY), [ELEMENT_NAME_INFORMALTABLE](../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_ROW](../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_SPANSPEC](../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_SPANSPEC), [ELEMENT_NAME_TABLE](../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TGROUP](../../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_TGROUP)
## Constructor Summary
 Constructors
Constructor

Description
 [DITATableDocumentTypeHelper](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableCellElementNames](#getTableCellElementNames())()
Returns the possible local names of the elements that represents a table cell.
  [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) [getTableCellSpanProvider](#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) tgroupElement)
Creates an AuthorTableCellSpanProvider corresponding to the table element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableElementLocalName](#getTableElementLocalName())()
Returns the possible local names of the elements that represents a table.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableRowElementNames](#getTableRowElementNames())()
Return the possible local names of the elements that represent a table row.
  protected boolean [isActuallyTableAndNotTgroup](#isActuallyTableAndNotTgroup(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
Check if the given node is a DITA table (not a tgroup, but actually a table).
  boolean [isColspec](#isColspec(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
Check if a node is a colspec node.
  boolean [isContentReference](#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
Check if this node references another node which should replace it entirely.
  boolean [isTable](#isTable(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
Check if an [AuthorNode](../../../api/node/AuthorNode.md) is a table node.
  boolean [isTableCell](#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
Check if an [AuthorNode](../../../api/node/AuthorNode.md) is a table cell node.
  boolean [isTableRow](#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
Check if an [AuthorNode](../../../api/node/AuthorNode.md) is a table row node.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.cals.[CALSDocumentTypeHelper](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md)
 [checkTableColSpanIsDefined](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement)), [getAllowedCellAttributesToCopy](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#getAllowedCellAttributesToCopy()), [getIgnoredCellIDAttributes](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#getIgnoredCellIDAttributes()), [getIgnoredColumnAttributes](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#getIgnoredColumnAttributes()), [getIgnoredRowAttributes](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#getIgnoredRowAttributes()), [getTableElementForDeletion](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode)), [limitRowSpan](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#limitRowSpan(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D)), [updateTableColSpan](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [updateTableColumnNumber](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)), [updateTableRowNumber](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)), [updateTableRowSpan](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))
### Methods inherited from class ro.sync.ecss.extensions.commons.[AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md)
 [isElement](../../../commons/AbstractDocumentTypeHelper.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITATableDocumentTypeHelper

public DITATableDocumentTypeHelper()

## Method Details

### getTableCellElementNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableCellElementNames()
 Description copied from class: [AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md#getTableCellElementNames())
Returns the possible local names of the elements that represents a table cell.
  Overrides: [getTableCellElementNames](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#getTableCellElementNames()) in class [CALSDocumentTypeHelper](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md) Returns: The local names of the elements that represents a table cell. Not null. See Also:
        * [AbstractDocumentTypeHelper.getTableCellElementNames()](../../../commons/AbstractDocumentTypeHelper.md#getTableCellElementNames())

### isTableCell

public boolean isTableCell([AuthorNode](../../../api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorTableHelper](../../../commons/table/operations/AuthorTableHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if an [AuthorNode](../../../api/node/AuthorNode.md) is a table cell node.
  Specified by: [isTableCell](../../../commons/table/operations/AuthorTableHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](../../../commons/table/operations/AuthorTableHelper.md) Overrides: [isTableCell](../../../commons/AbstractDocumentTypeHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md) Parameters: node - The [AuthorNode](../../../api/node/AuthorNode.md) to be checked. Returns: true if the node is a table cell node, false otherwise. See Also:
        * [AbstractDocumentTypeHelper.isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../commons/AbstractDocumentTypeHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode))

### isColspec

public boolean isColspec([AuthorNode](../../../api/node/AuthorNode.md) node)
 Description copied from class: [AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if a node is a colspec node.
  Specified by: [isColspec](../../../commons/table/operations/AuthorTableHelper.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](../../../commons/table/operations/AuthorTableHelper.md) Overrides: [isColspec](../../../commons/AbstractDocumentTypeHelper.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md) Parameters: node - The node. Returns: true if a node is a colspec node. See Also:
        * [AbstractDocumentTypeHelper.isColspec(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../commons/AbstractDocumentTypeHelper.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorNode))

### getTableRowElementNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableRowElementNames()
 Description copied from class: [AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md#getTableRowElementNames())
Return the possible local names of the elements that represent a table row.
  Overrides: [getTableRowElementNames](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#getTableRowElementNames()) in class [CALSDocumentTypeHelper](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md) Returns: The local names of the elements that represent a table row. See Also:
        * [AbstractDocumentTypeHelper.getTableRowElementNames()](../../../commons/AbstractDocumentTypeHelper.md#getTableRowElementNames())

### isTableRow

public boolean isTableRow([AuthorNode](../../../api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorTableHelper](../../../commons/table/operations/AuthorTableHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if an [AuthorNode](../../../api/node/AuthorNode.md) is a table row node.
  Specified by: [isTableRow](../../../commons/table/operations/AuthorTableHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](../../../commons/table/operations/AuthorTableHelper.md) Overrides: [isTableRow](../../../commons/AbstractDocumentTypeHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md) Parameters: node - The [AuthorNode](../../../api/node/AuthorNode.md) to be checked. Returns: true if the node is a table row node, false otherwise. See Also:
        * [AbstractDocumentTypeHelper.isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../commons/AbstractDocumentTypeHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))

### getTableElementLocalName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableElementLocalName()
 Description copied from class: [AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md#getTableElementLocalName())
Returns the possible local names of the elements that represents a table.
  Overrides: [getTableElementLocalName](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#getTableElementLocalName()) in class [CALSDocumentTypeHelper](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md) Returns: The local names of the elements that represents a table. See Also:
        * [AbstractDocumentTypeHelper.getTableElementLocalName()](../../../commons/AbstractDocumentTypeHelper.md#getTableElementLocalName())

### isTable

public boolean isTable([AuthorNode](../../../api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorTableHelper](../../../commons/table/operations/AuthorTableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if an [AuthorNode](../../../api/node/AuthorNode.md) is a table node.
  Specified by: [isTable](../../../commons/table/operations/AuthorTableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](../../../commons/table/operations/AuthorTableHelper.md) Overrides: [isTable](../../../commons/AbstractDocumentTypeHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md) Parameters: node - The [AuthorNode](../../../api/node/AuthorNode.md) to be checked. Returns: true if the node is a table node, false otherwise. See Also:
        * [AbstractDocumentTypeHelper.isTable(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../commons/AbstractDocumentTypeHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode))

### isContentReference

public boolean isContentReference([AuthorNode](../../../api/node/AuthorNode.md) node)
 Description copied from class: [AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if this node references another node which should replace it entirely. This is used in the tables to replace conreffed table rows entirely
  Overrides: [isContentReference](../../../commons/AbstractDocumentTypeHelper.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md) Parameters: node - The node Returns: true if this node references another node which should replace it entirely. See Also:
        * [AbstractDocumentTypeHelper.isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../commons/AbstractDocumentTypeHelper.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode))

### isActuallyTableAndNotTgroup

protected boolean isActuallyTableAndNotTgroup([AuthorNode](../../../api/node/AuthorNode.md) node)

Check if the given node is a DITA table (not a tgroup, but actually a table).
  Overrides: [isActuallyTableAndNotTgroup](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#isActuallyTableAndNotTgroup(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [CALSDocumentTypeHelper](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md) Parameters: node - the node for which we perform the check. Returns: true is the given node is a table element (with the class attribute containing **topic/table**). See Also:
        * [CALSDocumentTypeHelper.isActuallyTableAndNotTgroup(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#isActuallyTableAndNotTgroup(ro.sync.ecss.extensions.api.node.AuthorNode))

### getTableCellSpanProvider

public [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) getTableCellSpanProvider([AuthorElement](../../../api/node/AuthorElement.md) tgroupElement)
 Description copied from class: [CALSDocumentTypeHelper](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))
Creates an AuthorTableCellSpanProvider corresponding to the table element.
  Specified by: [getTableCellSpanProvider](../../../commons/table/operations/AuthorTableHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableHelper](../../../commons/table/operations/AuthorTableHelper.md) Overrides: [getTableCellSpanProvider](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [CALSDocumentTypeHelper](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md) Parameters: tgroupElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. Returns: The table cell span provider. Must not be null. See Also:
        * [CALSDocumentTypeHelper.getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../commons/table/operations/cals/CALSDocumentTypeHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
