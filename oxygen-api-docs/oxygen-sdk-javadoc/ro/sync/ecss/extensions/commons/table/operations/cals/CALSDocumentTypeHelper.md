Package [ro.sync.ecss.extensions.commons.table.operations.cals](package-summary.md)

# Class CALSDocumentTypeHelper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md)
        * ro.sync.ecss.extensions.commons.table.operations.cals.CALSDocumentTypeHelper
   All Implemented Interfaces: [AuthorTableHelper](../AuthorTableHelper.md), [CALSConstants](CALSConstants.md)   Direct Known Subclasses: [DITATableDocumentTypeHelper](../../../../dita/topic/table/DITATableDocumentTypeHelper.md)   @API(type=INTERNAL, src=PUBLIC) public class CALSDocumentTypeHelper extends [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md)implements [CALSConstants](CALSConstants.md)
Implementation of the document type helper for CALS table model(DocBook, DITA and S1000D).

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.[AuthorTableHelper](../AuthorTableHelper.md)
 [TYPE_CELL](../AuthorTableHelper.md#TYPE_CELL), [TYPE_ROW](../AuthorTableHelper.md#TYPE_ROW), [TYPE_TABLE](../AuthorTableHelper.md#TYPE_TABLE)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md)
 [ATTRIBUTE_NAME_ALIGN](CALSConstants.md#ATTRIBUTE_NAME_ALIGN), [ATTRIBUTE_NAME_COLNAME](CALSConstants.md#ATTRIBUTE_NAME_COLNAME), [ATTRIBUTE_NAME_COLNUM](CALSConstants.md#ATTRIBUTE_NAME_COLNUM), [ATTRIBUTE_NAME_COLS](CALSConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_COLSEP](CALSConstants.md#ATTRIBUTE_NAME_COLSEP), [ATTRIBUTE_NAME_COLWIDTH](CALSConstants.md#ATTRIBUTE_NAME_COLWIDTH), [ATTRIBUTE_NAME_ID](CALSConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_MOREROWS](CALSConstants.md#ATTRIBUTE_NAME_MOREROWS), [ATTRIBUTE_NAME_NAMEEND](CALSConstants.md#ATTRIBUTE_NAME_NAMEEND), [ATTRIBUTE_NAME_NAMEST](CALSConstants.md#ATTRIBUTE_NAME_NAMEST), [ATTRIBUTE_NAME_ROWSEP](CALSConstants.md#ATTRIBUTE_NAME_ROWSEP), [ATTRIBUTE_NAME_SPANNAME](CALSConstants.md#ATTRIBUTE_NAME_SPANNAME), [ATTRIBUTE_NAME_TABLE_WIDTH](CALSConstants.md#ATTRIBUTE_NAME_TABLE_WIDTH), [ATTRIBUTE_NAME_XML_ID](CALSConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_COLSPEC](CALSConstants.md#ELEMENT_NAME_COLSPEC), [ELEMENT_NAME_ENTRY](CALSConstants.md#ELEMENT_NAME_ENTRY), [ELEMENT_NAME_INFORMALTABLE](CALSConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_ROW](CALSConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_SPANSPEC](CALSConstants.md#ELEMENT_NAME_SPANSPEC), [ELEMENT_NAME_TABLE](CALSConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TGROUP](CALSConstants.md#ELEMENT_NAME_TGROUP)
## Constructor Summary
 Constructors
Constructor

Description
 [CALSDocumentTypeHelper](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [checkTableColSpanIsDefined](#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSpanSupport, [AuthorElement](../../../../api/node/AuthorElement.md) cellElement)
Check if the column span is defined for a table cell.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getAllowedCellAttributesToCopy](#getAllowedCellAttributesToCopy())()
Get a list of allowed cell attributes to copy when creating a new row.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredCellIDAttributes](#getIgnoredCellIDAttributes())()
Gets the ID attribute names which should be skipped when inserting a new column or row and the attributes from source cell fragments must be copied.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredColumnAttributes](#getIgnoredColumnAttributes())()
Gets the attributes which should be skipped when inserting a new column and the attributes from source cell fragments must be copied.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredRowAttributes](#getIgnoredRowAttributes())()
Gets the attributes which should be skipped when using the current row as template for insert operation.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableCellElementNames](#getTableCellElementNames())()
Returns the possible local names of the elements that represents a table cell.
  [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) [getTableCellSpanProvider](#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../api/node/AuthorElement.md) tgroupElement)
Creates an AuthorTableCellSpanProvider corresponding to the table element.
  [AuthorNode](../../../../api/node/AuthorNode.md) [getTableElementForDeletion](#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../api/node/AuthorNode.md) element)
When we delete all the rows or all the columns of a table, we also want to delete the entire table element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableElementLocalName](#getTableElementLocalName())()
Returns the possible local names of the elements that represents a table.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableRowElementNames](#getTableRowElementNames())()
Return the possible local names of the elements that represent a table row.
  protected boolean [isActuallyTableAndNotTgroup](#isActuallyTableAndNotTgroup(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../api/node/AuthorNode.md) node)
Check if the given node is a CALS table (not a tgroup, but actually a table element).
  void [limitRowSpan](#limitRowSpan(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D))([AuthorDocumentFragment](../../../../api/node/AuthorDocumentFragment.md)[] rowFragments)
Limits the value of the "morerows" attribute from the given rows fragments according to the number of rows.
  void [updateTableColSpan](#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../../api/node/AuthorElement.md) cellElem, int startCol, int endCol)
Update the span information of the specified cell element.
  void [updateTableColumnNumber](#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int colsNumber)
Update the cols attribute value of the table tgroup element.
  void [updateTableRowNumber](#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int rowsNumber)
Not needed for CALS Tables.
  void [updateTableRowSpan](#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) cellElem, int rowSpan)
Update the morerows attribute value for the given cell element.

### Methods inherited from class ro.sync.ecss.extensions.commons.[AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md)
 [isColspec](../../../AbstractDocumentTypeHelper.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorNode)), [isContentReference](../../../AbstractDocumentTypeHelper.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)), [isElement](../../../AbstractDocumentTypeHelper.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTable](../../../AbstractDocumentTypeHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode)), [isTableCell](../../../AbstractDocumentTypeHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode)), [isTableRow](../../../AbstractDocumentTypeHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CALSDocumentTypeHelper

public CALSDocumentTypeHelper()

## Method Details

### getTableCellElementNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableCellElementNames()
 Description copied from class: [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md#getTableCellElementNames())
Returns the possible local names of the elements that represents a table cell.
  Specified by: [getTableCellElementNames](../../../AbstractDocumentTypeHelper.md#getTableCellElementNames()) in class [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md) Returns: The local names of the elements that represents a table cell. Not null. See Also:
        * [AbstractDocumentTypeHelper.getTableCellElementNames()](../../../AbstractDocumentTypeHelper.md#getTableCellElementNames())

### getTableRowElementNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableRowElementNames()
 Description copied from class: [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md#getTableRowElementNames())
Return the possible local names of the elements that represent a table row.
  Specified by: [getTableRowElementNames](../../../AbstractDocumentTypeHelper.md#getTableRowElementNames()) in class [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md) Returns: The local names of the elements that represent a table row. See Also:
        * [AbstractDocumentTypeHelper.getTableRowElementNames()](../../../AbstractDocumentTypeHelper.md#getTableRowElementNames())

### getTableElementLocalName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableElementLocalName()
 Description copied from class: [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md#getTableElementLocalName())
Returns the possible local names of the elements that represents a table.
  Specified by: [getTableElementLocalName](../../../AbstractDocumentTypeHelper.md#getTableElementLocalName()) in class [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md) Returns: The local names of the elements that represents a table. See Also:
        * [AbstractDocumentTypeHelper.getTableElementLocalName()](../../../AbstractDocumentTypeHelper.md#getTableElementLocalName())

### checkTableColSpanIsDefined

public void checkTableColSpanIsDefined([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSpanSupport, [AuthorElement](../../../../api/node/AuthorElement.md) cellElement)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorTableHelper](../AuthorTableHelper.md#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))
Check if the column span is defined for a table cell.
 I.E. for DocBook the column span is defined by the 'colspec' element. If it is missing then the column span is not defined.

  Specified by: [checkTableColSpanIsDefined](../AuthorTableHelper.md#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableSpanSupport - The table cell span provider. cellElement - The cell element to be tested. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - When the column span is not defined for the table cell. See Also:
        * [AuthorTableHelper.checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement)](../AuthorTableHelper.md#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))

### updateTableColSpan

public void updateTableColSpan([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../../api/node/AuthorElement.md) cellElem, int startCol, int endCol)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)

Update the span information of the specified cell element. The namest and nameend attributes will be set according to the startCol and endCol supplied values. If the spanname attribute is set, then it will be removed. If the colname attribute is set, then it will be removed.
  Specified by: [updateTableColSpan](../AuthorTableHelper.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableSupport - The object responsible for providing information about the cell spanning. cellElem - The cell element whose column span will be updated. startCol - The new index of start column. It is 1 based and inclusive. endCol - The new index of end column. It is 1 based and inclusive. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - If the supplied values for start span column and end span column do not correspond to existing columns specifications. See Also:
        * [AuthorTableHelper.updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement, int, int)](../AuthorTableHelper.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))

### getTableCellSpanProvider

public [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) getTableCellSpanProvider([AuthorElement](../../../../api/node/AuthorElement.md) tgroupElement)

Creates an AuthorTableCellSpanProvider corresponding to the table element.
  Specified by: [getTableCellSpanProvider](../AuthorTableHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Parameters: tgroupElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. Returns: The table cell span provider. Must not be null. See Also:
        * [AuthorTableHelper.getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement)](../AuthorTableHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))

### updateTableRowSpan

public void updateTableRowSpan([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) cellElem, int rowSpan)

Update the morerows attribute value for the given cell element. If the supplied value for the row span is less than or equal to 1 then the attribute will be removed.
  Specified by: [updateTableRowSpan](../AuthorTableHelper.md#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. cellElem - The cell element whose row span will be updated. rowSpan - The new row span value. It is 1 based. See Also:
        * [AuthorTableHelper.updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](../AuthorTableHelper.md#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))

### updateTableColumnNumber

public void updateTableColumnNumber([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int colsNumber)

Update the cols attribute value of the table tgroup element.
  Specified by: [updateTableColumnNumber](../AuthorTableHelper.md#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. colsNumber - The updated number of columns. See Also:
        * [AuthorTableHelper.updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](../AuthorTableHelper.md#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))

### updateTableRowNumber

public void updateTableRowNumber([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int rowsNumber)

Not needed for CALS Tables.
  Specified by: [updateTableRowNumber](../AuthorTableHelper.md#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. rowsNumber - The number of rows to increase or decrease the current number of table rows. If the number of rows must be decreased then the argument must be negative. See Also:
        * [AuthorTableHelper.updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](../AuthorTableHelper.md#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))

### getIgnoredRowAttributes

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredRowAttributes()
 Description copied from interface: [AuthorTableHelper](../AuthorTableHelper.md#getIgnoredRowAttributes())
Gets the attributes which should be skipped when using the current row as template for insert operation.
  Specified by: [getIgnoredRowAttributes](../AuthorTableHelper.md#getIgnoredRowAttributes()) in interface [AuthorTableHelper](../AuthorTableHelper.md) Returns: The attributes which should be skipped. See Also:
        * [AuthorTableHelper.getIgnoredRowAttributes()](../AuthorTableHelper.md#getIgnoredRowAttributes())

### getIgnoredCellIDAttributes

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredCellIDAttributes()
 Description copied from interface: [AuthorTableHelper](../AuthorTableHelper.md#getIgnoredCellIDAttributes())
Gets the ID attribute names which should be skipped when inserting a new column or row and the attributes from source cell fragments must be copied.
  Specified by: [getIgnoredCellIDAttributes](../AuthorTableHelper.md#getIgnoredCellIDAttributes()) in interface [AuthorTableHelper](../AuthorTableHelper.md) Returns: The ID attributes which should be skipped. See Also:
        * [AuthorTableHelper.getIgnoredCellIDAttributes()](../AuthorTableHelper.md#getIgnoredCellIDAttributes())

### getAllowedCellAttributesToCopy

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getAllowedCellAttributesToCopy()

Get a list of allowed cell attributes to copy when creating a new row.
  Overrides: [getAllowedCellAttributesToCopy](../../../AbstractDocumentTypeHelper.md#getAllowedCellAttributesToCopy()) in class [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md) Returns: a list of allowed cell attributes to copy when creating a new row.
### getIgnoredColumnAttributes

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredColumnAttributes()
 Description copied from interface: [AuthorTableHelper](../AuthorTableHelper.md#getIgnoredColumnAttributes())
Gets the attributes which should be skipped when inserting a new column and the attributes from source cell fragments must be copied.
  Specified by: [getIgnoredColumnAttributes](../AuthorTableHelper.md#getIgnoredColumnAttributes()) in interface [AuthorTableHelper](../AuthorTableHelper.md) Returns: The attributes which should be skipped. See Also:
        * [AuthorTableHelper.getIgnoredColumnAttributes()](../AuthorTableHelper.md#getIgnoredColumnAttributes())

### getTableElementForDeletion

public [AuthorNode](../../../../api/node/AuthorNode.md) getTableElementForDeletion([AuthorNode](../../../../api/node/AuthorNode.md) element)
 Description copied from interface: [AuthorTableHelper](../AuthorTableHelper.md#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode))
When we delete all the rows or all the columns of a table, we also want to delete the entire table element. OBS: For CALS tables we don't want to delete only the "tgroup", but the parent table element itself.
  Specified by: [getTableElementForDeletion](../AuthorTableHelper.md#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Overrides: [getTableElementForDeletion](../../../AbstractDocumentTypeHelper.md#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md) Parameters: element - the node whose parent table we are looking for. Returns: the table element to be deleted. See Also:
        * [getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode)](#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode))

### isActuallyTableAndNotTgroup

protected boolean isActuallyTableAndNotTgroup([AuthorNode](../../../../api/node/AuthorNode.md) node)

Check if the given node is a CALS table (not a tgroup, but actually a table element).
  Parameters: node - the node for which we perform the check. Returns: true if the given node is a table element.
### limitRowSpan

public void limitRowSpan([AuthorDocumentFragment](../../../../api/node/AuthorDocumentFragment.md)[] rowFragments)

Limits the value of the "morerows" attribute from the given rows fragments according to the number of rows. Each fragment has inside it a single table row. For example if we have 3 rows and the first row contains a cell with 'morerows=5', we'll set 'morerows=2' on the cell.
  Parameters: rowFragments - The fragments of rows to be limited.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
