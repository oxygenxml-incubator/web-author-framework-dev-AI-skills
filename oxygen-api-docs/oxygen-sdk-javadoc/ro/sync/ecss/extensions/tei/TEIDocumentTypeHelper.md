Package [ro.sync.ecss.extensions.tei](package-summary.md)

# Class TEIDocumentTypeHelper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.AbstractDocumentTypeHelper](../commons/AbstractDocumentTypeHelper.md)
        * ro.sync.ecss.extensions.tei.TEIDocumentTypeHelper
   All Implemented Interfaces: [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md), [TEIConstants](table/TEIConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class TEIDocumentTypeHelper extends [AbstractDocumentTypeHelper](../commons/AbstractDocumentTypeHelper.md)implements [TEIConstants](table/TEIConstants.md)
Implementation of the document type helper for TEI.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.[AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md)
 [TYPE_CELL](../commons/table/operations/AuthorTableHelper.md#TYPE_CELL), [TYPE_ROW](../commons/table/operations/AuthorTableHelper.md#TYPE_ROW), [TYPE_TABLE](../commons/table/operations/AuthorTableHelper.md#TYPE_TABLE)
### Fields inherited from interface ro.sync.ecss.extensions.tei.table.[TEIConstants](table/TEIConstants.md)
 [ATTRIBUTE_NAME_COLS](table/TEIConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_ID](table/TEIConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_ROWS](table/TEIConstants.md#ATTRIBUTE_NAME_ROWS), [ATTRIBUTE_NAME_XML_ID](table/TEIConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_CELL](table/TEIConstants.md#ELEMENT_NAME_CELL), [ELEMENT_NAME_ROW](table/TEIConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_TABLE](table/TEIConstants.md#ELEMENT_NAME_TABLE)
## Constructor Summary
 Constructors
Constructor

Description
 [TEIDocumentTypeHelper](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [checkTableColSpanIsDefined](#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) tableCellSpanProvider, [AuthorElement](../api/node/AuthorElement.md) cellElement)
For TEI the column span is always defined.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredCellIDAttributes](#getIgnoredCellIDAttributes())()
Gets the ID attribute names which should be skipped when inserting a new column or row and the attributes from source cell fragments must be copied.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredColumnAttributes](#getIgnoredColumnAttributes())()
Gets the attributes which should be skipped when inserting a new column and the attributes from source cell fragments must be copied.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredRowAttributes](#getIgnoredRowAttributes())()
Gets the attributes which should be skipped when using the current row as template for insert operation.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableCellElementNames](#getTableCellElementNames())()
Returns the possible local names of the elements that represents a table cell.
  [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) [getTableCellSpanProvider](#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../api/node/AuthorElement.md) tableElement)
Create the table cell span provider for a specific table element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableElementLocalName](#getTableElementLocalName())()
Returns the possible local names of the elements that represents a table.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableRowElementNames](#getTableRowElementNames())()
Return the possible local names of the elements that represent a table row.
  void [updateTableColSpan](#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) tableCellSpanProvider, [AuthorElement](../api/node/AuthorElement.md) cellElement, int startCol, int endCol)
Update the 'cols' attribute.
  void [updateTableColumnNumber](#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorElement](../api/node/AuthorElement.md) tableElement, int colNumber)
Updates the 'cols' attribute.
  void [updateTableRowNumber](#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorElement](../api/node/AuthorElement.md) tableElement, int relativeValue)
Updates the 'rows' attribute.
  void [updateTableRowSpan](#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorElement](../api/node/AuthorElement.md) cellElement, int rowSpan)
Update the 'rows' attribute.

### Methods inherited from class ro.sync.ecss.extensions.commons.[AbstractDocumentTypeHelper](../commons/AbstractDocumentTypeHelper.md)
 [getAllowedCellAttributesToCopy](../commons/AbstractDocumentTypeHelper.md#getAllowedCellAttributesToCopy()), [getTableElementForDeletion](../commons/AbstractDocumentTypeHelper.md#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode)), [isColspec](../commons/AbstractDocumentTypeHelper.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorNode)), [isContentReference](../commons/AbstractDocumentTypeHelper.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)), [isElement](../commons/AbstractDocumentTypeHelper.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTable](../commons/AbstractDocumentTypeHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode)), [isTableCell](../commons/AbstractDocumentTypeHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode)), [isTableRow](../commons/AbstractDocumentTypeHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TEIDocumentTypeHelper

public TEIDocumentTypeHelper()

## Method Details

### checkTableColSpanIsDefined

public void checkTableColSpanIsDefined([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) tableCellSpanProvider, [AuthorElement](../api/node/AuthorElement.md) cellElement)throws [AuthorOperationException](../api/AuthorOperationException.md)

For TEI the column span is always defined.
  Specified by: [checkTableColSpanIsDefined](../commons/table/operations/AuthorTableHelper.md#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableCellSpanProvider - The table cell span provider. cellElement - The cell element to be tested. Throws: [AuthorOperationException](../api/AuthorOperationException.md) - When the column span is not defined for the table cell. See Also:
        * [AuthorTableHelper.checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement)](../commons/table/operations/AuthorTableHelper.md#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))

### getTableCellElementNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableCellElementNames()
 Description copied from class: [AbstractDocumentTypeHelper](../commons/AbstractDocumentTypeHelper.md#getTableCellElementNames())
Returns the possible local names of the elements that represents a table cell.
  Specified by: [getTableCellElementNames](../commons/AbstractDocumentTypeHelper.md#getTableCellElementNames()) in class [AbstractDocumentTypeHelper](../commons/AbstractDocumentTypeHelper.md) Returns: The local names of the elements that represents a table cell. Not null. See Also:
        * [AbstractDocumentTypeHelper.getTableCellElementNames()](../commons/AbstractDocumentTypeHelper.md#getTableCellElementNames())

### getTableElementLocalName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableElementLocalName()
 Description copied from class: [AbstractDocumentTypeHelper](../commons/AbstractDocumentTypeHelper.md#getTableElementLocalName())
Returns the possible local names of the elements that represents a table.
  Specified by: [getTableElementLocalName](../commons/AbstractDocumentTypeHelper.md#getTableElementLocalName()) in class [AbstractDocumentTypeHelper](../commons/AbstractDocumentTypeHelper.md) Returns: The local names of the elements that represents a table. See Also:
        * [AbstractDocumentTypeHelper.getTableElementLocalName()](../commons/AbstractDocumentTypeHelper.md#getTableElementLocalName())

### getTableRowElementNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableRowElementNames()
 Description copied from class: [AbstractDocumentTypeHelper](../commons/AbstractDocumentTypeHelper.md#getTableRowElementNames())
Return the possible local names of the elements that represent a table row.
  Specified by: [getTableRowElementNames](../commons/AbstractDocumentTypeHelper.md#getTableRowElementNames()) in class [AbstractDocumentTypeHelper](../commons/AbstractDocumentTypeHelper.md) Returns: The local names of the elements that represent a table row. See Also:
        * [AbstractDocumentTypeHelper.getTableRowElementNames()](../commons/AbstractDocumentTypeHelper.md#getTableRowElementNames())

### getTableCellSpanProvider

public [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) getTableCellSpanProvider([AuthorElement](../api/node/AuthorElement.md) tableElement)
 Description copied from interface: [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))
Create the table cell span provider for a specific table element.
  Specified by: [getTableCellSpanProvider](../commons/table/operations/AuthorTableHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md) Parameters: tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. Returns: The table cell span provider. Must not be null. See Also:
        * [AuthorTableHelper.getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement)](../commons/table/operations/AuthorTableHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))

### updateTableColSpan

public void updateTableColSpan([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../api/AuthorTableCellSpanProvider.md) tableCellSpanProvider, [AuthorElement](../api/node/AuthorElement.md) cellElement, int startCol, int endCol)

Update the 'cols' attribute.
  Specified by: [updateTableColSpan](../commons/table/operations/AuthorTableHelper.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)) in interface [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableCellSpanProvider - The object responsible for providing information about the cell spanning. cellElement - The cell element whose column span will be updated. startCol - The new index of start column. It is 1 based and inclusive. endCol - The new index of end column. It is 1 based and inclusive. See Also:
        * [AuthorTableHelper.updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement, int, int)](../commons/table/operations/AuthorTableHelper.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))

### updateTableRowSpan

public void updateTableRowSpan([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorElement](../api/node/AuthorElement.md) cellElement, int rowSpan)

Update the 'rows' attribute.
  Specified by: [updateTableRowSpan](../commons/table/operations/AuthorTableHelper.md#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. cellElement - The cell element whose row span will be updated. rowSpan - The new row span value. It is 1 based. See Also:
        * [AuthorTableHelper.updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](../commons/table/operations/AuthorTableHelper.md#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))

### updateTableColumnNumber

public void updateTableColumnNumber([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorElement](../api/node/AuthorElement.md) tableElement, int colNumber)

Updates the 'cols' attribute.
  Specified by: [updateTableColumnNumber](../commons/table/operations/AuthorTableHelper.md#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. colNumber - The updated number of columns. See Also:
        * [AuthorTableHelper.updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](../commons/table/operations/AuthorTableHelper.md#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))

### updateTableRowNumber

public void updateTableRowNumber([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorElement](../api/node/AuthorElement.md) tableElement, int relativeValue)

Updates the 'rows' attribute.
  Specified by: [updateTableRowNumber](../commons/table/operations/AuthorTableHelper.md#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. relativeValue - The number of rows to increase or decrease the current number of table rows. If the number of rows must be decreased then the argument must be negative. See Also:
        * [AuthorTableHelper.updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](../commons/table/operations/AuthorTableHelper.md#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))

### getIgnoredRowAttributes

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredRowAttributes()
 Description copied from interface: [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md#getIgnoredRowAttributes())
Gets the attributes which should be skipped when using the current row as template for insert operation.
  Specified by: [getIgnoredRowAttributes](../commons/table/operations/AuthorTableHelper.md#getIgnoredRowAttributes()) in interface [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md) Returns: The attributes which should be skipped. See Also:
        * [AuthorTableHelper.getIgnoredRowAttributes()](../commons/table/operations/AuthorTableHelper.md#getIgnoredRowAttributes())

### getIgnoredCellIDAttributes

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredCellIDAttributes()
 Description copied from interface: [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md#getIgnoredCellIDAttributes())
Gets the ID attribute names which should be skipped when inserting a new column or row and the attributes from source cell fragments must be copied.
  Specified by: [getIgnoredCellIDAttributes](../commons/table/operations/AuthorTableHelper.md#getIgnoredCellIDAttributes()) in interface [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md) Returns: The ID attributes which should be skipped. See Also:
        * [AuthorTableHelper.getIgnoredCellIDAttributes()](../commons/table/operations/AuthorTableHelper.md#getIgnoredCellIDAttributes())

### getIgnoredColumnAttributes

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredColumnAttributes()
 Description copied from interface: [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md#getIgnoredColumnAttributes())
Gets the attributes which should be skipped when inserting a new column and the attributes from source cell fragments must be copied.
  Specified by: [getIgnoredColumnAttributes](../commons/table/operations/AuthorTableHelper.md#getIgnoredColumnAttributes()) in interface [AuthorTableHelper](../commons/table/operations/AuthorTableHelper.md) Returns: The attributes which should be skipped. See Also:
        * [AuthorTableHelper.getIgnoredColumnAttributes()](../commons/table/operations/AuthorTableHelper.md#getIgnoredColumnAttributes())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
