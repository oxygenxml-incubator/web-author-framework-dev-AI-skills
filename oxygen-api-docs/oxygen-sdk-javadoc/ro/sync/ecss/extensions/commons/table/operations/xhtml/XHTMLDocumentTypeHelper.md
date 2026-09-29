Package [ro.sync.ecss.extensions.commons.table.operations.xhtml](package-summary.md)

# Class XHTMLDocumentTypeHelper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md)
        * ro.sync.ecss.extensions.commons.table.operations.xhtml.XHTMLDocumentTypeHelper
   All Implemented Interfaces: [AuthorTableHelper](../AuthorTableHelper.md), [XHTMLConstants](XHTMLConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class XHTMLDocumentTypeHelper extends [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md)implements [XHTMLConstants](XHTMLConstants.md)
Implementation of the document type helper for XHTML.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [TABLE_ELEMENT_NAMES](#TABLE_ELEMENT_NAMES)
Table element names.

### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.[AuthorTableHelper](../AuthorTableHelper.md)
 [TYPE_CELL](../AuthorTableHelper.md#TYPE_CELL), [TYPE_ROW](../AuthorTableHelper.md#TYPE_ROW), [TYPE_TABLE](../AuthorTableHelper.md#TYPE_TABLE)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.xhtml.[XHTMLConstants](XHTMLConstants.md)
 [ATTRIBUTE_NAME_COLSPAN](XHTMLConstants.md#ATTRIBUTE_NAME_COLSPAN), [ATTRIBUTE_NAME_ID](XHTMLConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_ROWSPAN](XHTMLConstants.md#ATTRIBUTE_NAME_ROWSPAN), [ATTRIBUTE_NAME_XML_ID](XHTMLConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_INFORMALTABLE](XHTMLConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_TABLE](XHTMLConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TD](XHTMLConstants.md#ELEMENT_NAME_TD), [ELEMENT_NAME_TH](XHTMLConstants.md#ELEMENT_NAME_TH), [ELEMENT_NAME_THEAD](XHTMLConstants.md#ELEMENT_NAME_THEAD), [ELEMENT_NAME_TR](XHTMLConstants.md#ELEMENT_NAME_TR)
## Constructor Summary
 Constructors
Constructor

Description
 [XHTMLDocumentTypeHelper](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [checkTableColSpanIsDefined](#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSpanSupport, [AuthorElement](../../../../api/node/AuthorElement.md) cellElement)
For XHTML, the column span is always defined.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredCellIDAttributes](#getIgnoredCellIDAttributes())()
Gets the ID attribute names which should be skipped when inserting a new column or row and the attributes from source cell fragments must be copied.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredColumnAttributes](#getIgnoredColumnAttributes())()
Gets the attributes which should be skipped when inserting a new column and the attributes from source cell fragments must be copied.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredRowAttributes](#getIgnoredRowAttributes())()
Gets the attributes which should be skipped when using the current row as template for insert operation.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableCellElementNames](#getTableCellElementNames())()
Returns the possible local names of the elements that represents a table cell.
  [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) [getTableCellSpanProvider](#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../api/node/AuthorElement.md) tableElement)
Create the table cell span provider for a specific table element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableElementLocalName](#getTableElementLocalName())()
Returns the possible local names of the elements that represents a table.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableRowElementNames](#getTableRowElementNames())()
Return the possible local names of the elements that represent a table row.
  void [updateTableColSpan](#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../../api/node/AuthorElement.md) cellElement, int startCol, int endCol)
Update the 'colspan' attribute.
  void [updateTableColumnNumber](#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int colNum)
Update the table columns number.
  void [updateTableRowNumber](#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int rowsNumber)
Update the table rows number.
  void [updateTableRowSpan](#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) cellElement, int rowSpan)
Updates the cell row span to a specified value.

### Methods inherited from class ro.sync.ecss.extensions.commons.[AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md)
 [getAllowedCellAttributesToCopy](../../../AbstractDocumentTypeHelper.md#getAllowedCellAttributesToCopy()), [getTableElementForDeletion](../../../AbstractDocumentTypeHelper.md#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode)), [isColspec](../../../AbstractDocumentTypeHelper.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorNode)), [isContentReference](../../../AbstractDocumentTypeHelper.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)), [isElement](../../../AbstractDocumentTypeHelper.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTable](../../../AbstractDocumentTypeHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode)), [isTableCell](../../../AbstractDocumentTypeHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode)), [isTableRow](../../../AbstractDocumentTypeHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### TABLE_ELEMENT_NAMES

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] TABLE_ELEMENT_NAMES

Table element names.

## Constructor Details

### XHTMLDocumentTypeHelper

public XHTMLDocumentTypeHelper()

## Method Details

### checkTableColSpanIsDefined

public void checkTableColSpanIsDefined([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSpanSupport, [AuthorElement](../../../../api/node/AuthorElement.md) cellElement)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)

For XHTML, the column span is always defined.
  Specified by: [checkTableColSpanIsDefined](../AuthorTableHelper.md#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableSpanSupport - The table cell span provider. cellElement - The cell element to be tested. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - When the column span is not defined for the table cell. See Also:
        * [AuthorTableHelper.checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement)](../AuthorTableHelper.md#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))

### getTableCellElementNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableCellElementNames()
 Description copied from class: [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md#getTableCellElementNames())
Returns the possible local names of the elements that represents a table cell.
  Specified by: [getTableCellElementNames](../../../AbstractDocumentTypeHelper.md#getTableCellElementNames()) in class [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md) Returns: The local names of the elements that represents a table cell. Not null. See Also:
        * [AbstractDocumentTypeHelper.getTableCellElementNames()](../../../AbstractDocumentTypeHelper.md#getTableCellElementNames())

### getTableElementLocalName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableElementLocalName()
 Description copied from class: [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md#getTableElementLocalName())
Returns the possible local names of the elements that represents a table.
  Specified by: [getTableElementLocalName](../../../AbstractDocumentTypeHelper.md#getTableElementLocalName()) in class [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md) Returns: The local names of the elements that represents a table. See Also:
        * [AbstractDocumentTypeHelper.getTableElementLocalName()](../../../AbstractDocumentTypeHelper.md#getTableElementLocalName())

### getTableRowElementNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableRowElementNames()
 Description copied from class: [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md#getTableRowElementNames())
Return the possible local names of the elements that represent a table row.
  Specified by: [getTableRowElementNames](../../../AbstractDocumentTypeHelper.md#getTableRowElementNames()) in class [AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md) Returns: The local names of the elements that represent a table row. See Also:
        * [AbstractDocumentTypeHelper.getTableRowElementNames()](../../../AbstractDocumentTypeHelper.md#getTableRowElementNames())

### getTableCellSpanProvider

public [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) getTableCellSpanProvider([AuthorElement](../../../../api/node/AuthorElement.md) tableElement)
 Description copied from interface: [AuthorTableHelper](../AuthorTableHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))
Create the table cell span provider for a specific table element.
  Specified by: [getTableCellSpanProvider](../AuthorTableHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Parameters: tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. Returns: The table cell span provider. Must not be null. See Also:
        * [AuthorTableHelper.getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement)](../AuthorTableHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))

### updateTableColSpan

public void updateTableColSpan([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../../api/node/AuthorElement.md) cellElement, int startCol, int endCol)

Update the 'colspan' attribute.
  Specified by: [updateTableColSpan](../AuthorTableHelper.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableSupport - The object responsible for providing information about the cell spanning. cellElement - The cell element whose column span will be updated. startCol - The new index of start column. It is 1 based and inclusive. endCol - The new index of end column. It is 1 based and inclusive. See Also:
        * [AuthorTableHelper.updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement, int, int)](../AuthorTableHelper.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))

### updateTableRowSpan

public void updateTableRowSpan([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) cellElement, int rowSpan)
 Description copied from interface: [AuthorTableHelper](../AuthorTableHelper.md#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))
Updates the cell row span to a specified value. For example, for the DocBook CALS tables the morerows attribute value will be updated.
  Specified by: [updateTableRowSpan](../AuthorTableHelper.md#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. cellElement - The cell element whose row span will be updated. rowSpan - The new row span value. It is 1 based. See Also:
        * [AuthorTableHelper.updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](../AuthorTableHelper.md#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))

### updateTableColumnNumber

public void updateTableColumnNumber([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int colNum)
 Description copied from interface: [AuthorTableHelper](../AuthorTableHelper.md#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))
Update the table columns number. For example, for the DocBook CALS tables the cols attribute value will be updated.
  Specified by: [updateTableColumnNumber](../AuthorTableHelper.md#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. colNum - The updated number of columns. See Also:
        * [AuthorTableHelper.updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](../AuthorTableHelper.md#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))

### updateTableRowNumber

public void updateTableRowNumber([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int rowsNumber)
 Description copied from interface: [AuthorTableHelper](../AuthorTableHelper.md#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))
Update the table rows number.
  Specified by: [updateTableRowNumber](../AuthorTableHelper.md#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableHelper](../AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. rowsNumber - The number of rows to increase or decrease the current number of table rows. If the number of rows must be decreased then the argument must be negative. See Also:
        * [AuthorTableHelper.updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](../AuthorTableHelper.md#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))

### getIgnoredColumnAttributes

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredColumnAttributes()
 Description copied from interface: [AuthorTableHelper](../AuthorTableHelper.md#getIgnoredColumnAttributes())
Gets the attributes which should be skipped when inserting a new column and the attributes from source cell fragments must be copied.
  Specified by: [getIgnoredColumnAttributes](../AuthorTableHelper.md#getIgnoredColumnAttributes()) in interface [AuthorTableHelper](../AuthorTableHelper.md) Returns: The attributes which should be skipped. See Also:
        * [AuthorTableHelper.getIgnoredColumnAttributes()](../AuthorTableHelper.md#getIgnoredColumnAttributes())

### getIgnoredCellIDAttributes

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredCellIDAttributes()
 Description copied from interface: [AuthorTableHelper](../AuthorTableHelper.md#getIgnoredCellIDAttributes())
Gets the ID attribute names which should be skipped when inserting a new column or row and the attributes from source cell fragments must be copied.
  Specified by: [getIgnoredCellIDAttributes](../AuthorTableHelper.md#getIgnoredCellIDAttributes()) in interface [AuthorTableHelper](../AuthorTableHelper.md) Returns: The ID attributes which should be skipped. See Also:
        * [AuthorTableHelper.getIgnoredCellIDAttributes()](../AuthorTableHelper.md#getIgnoredCellIDAttributes())

### getIgnoredRowAttributes

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredRowAttributes()
 Description copied from interface: [AuthorTableHelper](../AuthorTableHelper.md#getIgnoredRowAttributes())
Gets the attributes which should be skipped when using the current row as template for insert operation.
  Specified by: [getIgnoredRowAttributes](../AuthorTableHelper.md#getIgnoredRowAttributes()) in interface [AuthorTableHelper](../AuthorTableHelper.md) Returns: The attributes which should be skipped. See Also:
        * [AuthorTableHelper.getIgnoredRowAttributes()](../AuthorTableHelper.md#getIgnoredRowAttributes())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
