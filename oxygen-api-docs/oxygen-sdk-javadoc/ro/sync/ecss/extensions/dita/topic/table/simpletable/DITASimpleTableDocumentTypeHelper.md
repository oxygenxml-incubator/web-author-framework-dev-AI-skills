Package [ro.sync.ecss.extensions.dita.topic.table.simpletable](package-summary.md)

# Class DITASimpleTableDocumentTypeHelper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md)
        * ro.sync.ecss.extensions.dita.topic.table.simpletable.DITASimpleTableDocumentTypeHelper
   All Implemented Interfaces: [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md), [SimpleTableConstants](SimpleTableConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class DITASimpleTableDocumentTypeHelper extends [AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md)implements [SimpleTableConstants](SimpleTableConstants.md)
Implementation of the document type helper for DITA simple table model

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.[AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md)
 [TYPE_CELL](../../../../commons/table/operations/AuthorTableHelper.md#TYPE_CELL), [TYPE_ROW](../../../../commons/table/operations/AuthorTableHelper.md#TYPE_ROW), [TYPE_TABLE](../../../../commons/table/operations/AuthorTableHelper.md#TYPE_TABLE)
### Fields inherited from interface ro.sync.ecss.extensions.dita.topic.table.simpletable.[SimpleTableConstants](SimpleTableConstants.md)
 [ATTRIBUTE_NAME_ID](SimpleTableConstants.md#ATTRIBUTE_NAME_ID), [ELEMENT_NAME_CHDESC_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHDESC_CHOICETABLE), [ELEMENT_NAME_CHDESCHD_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHDESCHD_CHOICETABLE), [ELEMENT_NAME_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHOICETABLE), [ELEMENT_NAME_CHOPTION_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHOPTION_CHOICETABLE), [ELEMENT_NAME_CHOPTIONHD_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHOPTIONHD_CHOICETABLE), [ELEMENT_NAME_ENTRY_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_ENTRY_SIMPLETABLE), [ELEMENT_NAME_HEADER_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_HEADER_CHOICETABLE), [ELEMENT_NAME_HEADER_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_HEADER_PROPERTIES), [ELEMENT_NAME_HEADER_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_HEADER_SIMPLETABLE), [ELEMENT_NAME_PROPDESC_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPDESC_PROPERTIES), [ELEMENT_NAME_PROPDESCHD_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPDESCHD_PROPERTIES), [ELEMENT_NAME_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPERTIES), [ELEMENT_NAME_PROPTYPE_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPTYPE_PROPERTIES), [ELEMENT_NAME_PROPTYPEHD_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPTYPEHD_PROPERTIES), [ELEMENT_NAME_PROPVALUE_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPVALUE_PROPERTIES), [ELEMENT_NAME_PROPVALUEHD_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPVALUEHD_PROPERTIES), [ELEMENT_NAME_ROW_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_ROW_CHOICETABLE), [ELEMENT_NAME_ROW_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_ROW_PROPERTIES), [ELEMENT_NAME_ROW_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_ROW_SIMPLETABLE), [ELEMENT_NAME_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_SIMPLETABLE)
## Constructor Summary
 Constructors
Constructor

Description
 [DITASimpleTableDocumentTypeHelper](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [checkTableColSpanIsDefined](#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSpanSupport, [AuthorElement](../../../../api/node/AuthorElement.md) cellElement)
Check if the column span is defined for a table cell.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredCellIDAttributes](#getIgnoredCellIDAttributes())()
Gets the ID attribute names which should be skipped when inserting a new column or row and the attributes from source cell fragments must be copied.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredColumnAttributes](#getIgnoredColumnAttributes())()
Gets the attributes which should be skipped when inserting a new column and the attributes from source cell fragments must be copied.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredRowAttributes](#getIgnoredRowAttributes())()
Gets the attributes which should be skipped when using the current row as template for insert operation.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableCellElementNames](#getTableCellElementNames())()
Returns the possible local names of the elements that represents a table cell.
  [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) [getTableCellSpanProvider](#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../api/node/AuthorElement.md) tgroupElement)
Creates a [DITASimpleTableCellSpanProvider](../../../../commons/table/support/DITASimpleTableCellSpanProvider.md) over the table element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableElementLocalName](#getTableElementLocalName())()
Returns the possible local names of the elements that represents a table.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTableRowElementNames](#getTableRowElementNames())()
Return the possible local names of the elements that represent a table row.
  boolean [isContentReference](#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../api/node/AuthorNode.md) node)
Check if this node references another node which should replace it entirely.
  boolean [isTable](#isTable(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../api/node/AuthorNode.md) node)
Check if an [AuthorNode](../../../../api/node/AuthorNode.md) is a table node.
  boolean [isTableCell](#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../api/node/AuthorNode.md) node)
Check if an [AuthorNode](../../../../api/node/AuthorNode.md) is a table cell node.
  boolean [isTableRow](#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../api/node/AuthorNode.md) node)
Check if an [AuthorNode](../../../../api/node/AuthorNode.md) is a table row node.
  void [updateTableColSpan](#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../../api/node/AuthorElement.md) cellElem, int startCol, int endCol)
Update the column span of the cell by modifying the indices of start and end column.
  void [updateTableColumnNumber](#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int colsNumber)
Update the table columns number.
  void [updateTableRowNumber](#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int rowsNumber)
Update the table rows number.
  void [updateTableRowSpan](#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) cellElem, int rowSpan)
Updates the cell row span to a specified value.

### Methods inherited from class ro.sync.ecss.extensions.commons.[AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md)
 [getAllowedCellAttributesToCopy](../../../../commons/AbstractDocumentTypeHelper.md#getAllowedCellAttributesToCopy()), [getTableElementForDeletion](../../../../commons/AbstractDocumentTypeHelper.md#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode)), [isColspec](../../../../commons/AbstractDocumentTypeHelper.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorNode)), [isElement](../../../../commons/AbstractDocumentTypeHelper.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITASimpleTableDocumentTypeHelper

public DITASimpleTableDocumentTypeHelper()

## Method Details

### getTableCellElementNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableCellElementNames()
 Description copied from class: [AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md#getTableCellElementNames())
Returns the possible local names of the elements that represents a table cell.
  Specified by: [getTableCellElementNames](../../../../commons/AbstractDocumentTypeHelper.md#getTableCellElementNames()) in class [AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md) Returns: The local names of the elements that represents a table cell. Not null. See Also:
        * [AbstractDocumentTypeHelper.getTableCellElementNames()](../../../../commons/AbstractDocumentTypeHelper.md#getTableCellElementNames())

### isTableCell

public boolean isTableCell([AuthorNode](../../../../api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if an [AuthorNode](../../../../api/node/AuthorNode.md) is a table cell node.
  Specified by: [isTableCell](../../../../commons/table/operations/AuthorTableHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) Overrides: [isTableCell](../../../../commons/AbstractDocumentTypeHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md) Parameters: node - The [AuthorNode](../../../../api/node/AuthorNode.md) to be checked. Returns: true if the node is a table cell node, false otherwise. See Also:
        * [AbstractDocumentTypeHelper.isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../../commons/AbstractDocumentTypeHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode))

### getTableRowElementNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableRowElementNames()
 Description copied from class: [AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md#getTableRowElementNames())
Return the possible local names of the elements that represent a table row.
  Specified by: [getTableRowElementNames](../../../../commons/AbstractDocumentTypeHelper.md#getTableRowElementNames()) in class [AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md) Returns: The local names of the elements that represent a table row. See Also:
        * [AbstractDocumentTypeHelper.getTableRowElementNames()](../../../../commons/AbstractDocumentTypeHelper.md#getTableRowElementNames())

### isTableRow

public boolean isTableRow([AuthorNode](../../../../api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if an [AuthorNode](../../../../api/node/AuthorNode.md) is a table row node.
  Specified by: [isTableRow](../../../../commons/table/operations/AuthorTableHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) Overrides: [isTableRow](../../../../commons/AbstractDocumentTypeHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md) Parameters: node - The [AuthorNode](../../../../api/node/AuthorNode.md) to be checked. Returns: true if the node is a table row node, false otherwise. See Also:
        * [AbstractDocumentTypeHelper.isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../../commons/AbstractDocumentTypeHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))

### getTableElementLocalName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTableElementLocalName()
 Description copied from class: [AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md#getTableElementLocalName())
Returns the possible local names of the elements that represents a table.
  Specified by: [getTableElementLocalName](../../../../commons/AbstractDocumentTypeHelper.md#getTableElementLocalName()) in class [AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md) Returns: The local names of the elements that represents a table. See Also:
        * [AbstractDocumentTypeHelper.getTableElementLocalName()](../../../../commons/AbstractDocumentTypeHelper.md#getTableElementLocalName())

### isTable

public boolean isTable([AuthorNode](../../../../api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if an [AuthorNode](../../../../api/node/AuthorNode.md) is a table node.
  Specified by: [isTable](../../../../commons/table/operations/AuthorTableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) Overrides: [isTable](../../../../commons/AbstractDocumentTypeHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md) Parameters: node - The [AuthorNode](../../../../api/node/AuthorNode.md) to be checked. Returns: true if the node is a table node, false otherwise. See Also:
        * [AbstractDocumentTypeHelper.isTable(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../../commons/AbstractDocumentTypeHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorNode))

### checkTableColSpanIsDefined

public void checkTableColSpanIsDefined([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSpanSupport, [AuthorElement](../../../../api/node/AuthorElement.md) cellElement)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))
Check if the column span is defined for a table cell.
 I.E. for DocBook the column span is defined by the 'colspec' element. If it is missing then the column span is not defined.

  Specified by: [checkTableColSpanIsDefined](../../../../commons/table/operations/AuthorTableHelper.md#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableSpanSupport - The table cell span provider. cellElement - The cell element to be tested. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - When the column span is not defined for the table cell. See Also:
        * [AuthorTableHelper.checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement)](../../../../commons/table/operations/AuthorTableHelper.md#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))

### updateTableColSpan

public void updateTableColSpan([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSupport, [AuthorElement](../../../../api/node/AuthorElement.md) cellElem, int startCol, int endCol)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))
Update the column span of the cell by modifying the indices of start and end column. For example, for the DocBook CALS tables the namest and nameend attributes will be set according to the startCol and endCol supplied values.
  Specified by: [updateTableColSpan](../../../../commons/table/operations/AuthorTableHelper.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)) in interface [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableSupport - The object responsible for providing information about the cell spanning. cellElem - The cell element whose column span will be updated. startCol - The new index of start column. It is 1 based and inclusive. endCol - The new index of end column. It is 1 based and inclusive. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - When the column specifications for start or end columns are missing. See Also:
        * [AuthorTableHelper.updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement, int, int)](../../../../commons/table/operations/AuthorTableHelper.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))

### getTableCellSpanProvider

public [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) getTableCellSpanProvider([AuthorElement](../../../../api/node/AuthorElement.md) tgroupElement)

Creates a [DITASimpleTableCellSpanProvider](../../../../commons/table/support/DITASimpleTableCellSpanProvider.md) over the table element.
  Specified by: [getTableCellSpanProvider](../../../../commons/table/operations/AuthorTableHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) Parameters: tgroupElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. Returns: The table cell span provider. Must not be null. See Also:
        * [AuthorTableHelper.getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../../commons/table/operations/AuthorTableHelper.md#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))

### updateTableRowSpan

public void updateTableRowSpan([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) cellElem, int rowSpan)
 Description copied from interface: [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))
Updates the cell row span to a specified value. For example, for the DocBook CALS tables the morerows attribute value will be updated.
  Specified by: [updateTableRowSpan](../../../../commons/table/operations/AuthorTableHelper.md#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. cellElem - The cell element whose row span will be updated. rowSpan - The new row span value. It is 1 based. See Also:
        * [AuthorTableHelper.updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](../../../../commons/table/operations/AuthorTableHelper.md#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))

### updateTableColumnNumber

public void updateTableColumnNumber([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int colsNumber)
 Description copied from interface: [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))
Update the table columns number. For example, for the DocBook CALS tables the cols attribute value will be updated.
  Specified by: [updateTableColumnNumber](../../../../commons/table/operations/AuthorTableHelper.md#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. colsNumber - The updated number of columns. See Also:
        * [AuthorTableHelper.updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](../../../../commons/table/operations/AuthorTableHelper.md#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))

### updateTableRowNumber

public void updateTableRowNumber([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement, int rowsNumber)
 Description copied from interface: [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))
Update the table rows number.
  Specified by: [updateTableRowNumber](../../../../commons/table/operations/AuthorTableHelper.md#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. rowsNumber - The number of rows to increase or decrease the current number of table rows. If the number of rows must be decreased then the argument must be negative. See Also:
        * [AuthorTableHelper.updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorElement, int)](../../../../commons/table/operations/AuthorTableHelper.md#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))

### getIgnoredColumnAttributes

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredColumnAttributes()
 Description copied from interface: [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md#getIgnoredColumnAttributes())
Gets the attributes which should be skipped when inserting a new column and the attributes from source cell fragments must be copied.
  Specified by: [getIgnoredColumnAttributes](../../../../commons/table/operations/AuthorTableHelper.md#getIgnoredColumnAttributes()) in interface [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) Returns: The attributes which should be skipped. See Also:
        * [AuthorTableHelper.getIgnoredColumnAttributes()](../../../../commons/table/operations/AuthorTableHelper.md#getIgnoredColumnAttributes())

### getIgnoredRowAttributes

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredRowAttributes()
 Description copied from interface: [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md#getIgnoredRowAttributes())
Gets the attributes which should be skipped when using the current row as template for insert operation.
  Specified by: [getIgnoredRowAttributes](../../../../commons/table/operations/AuthorTableHelper.md#getIgnoredRowAttributes()) in interface [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) Returns: The attributes which should be skipped. See Also:
        * [AuthorTableHelper.getIgnoredRowAttributes()](../../../../commons/table/operations/AuthorTableHelper.md#getIgnoredRowAttributes())

### getIgnoredCellIDAttributes

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredCellIDAttributes()
 Description copied from interface: [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md#getIgnoredCellIDAttributes())
Gets the ID attribute names which should be skipped when inserting a new column or row and the attributes from source cell fragments must be copied.
  Specified by: [getIgnoredCellIDAttributes](../../../../commons/table/operations/AuthorTableHelper.md#getIgnoredCellIDAttributes()) in interface [AuthorTableHelper](../../../../commons/table/operations/AuthorTableHelper.md) Returns: The ID attributes which should be skipped. See Also:
        * [AuthorTableHelper.getIgnoredCellIDAttributes()](../../../../commons/table/operations/AuthorTableHelper.md#getIgnoredCellIDAttributes())

### isContentReference

public boolean isContentReference([AuthorNode](../../../../api/node/AuthorNode.md) node)
 Description copied from class: [AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if this node references another node which should replace it entirely. This is used in the tables to replace conreffed table rows entirely
  Overrides: [isContentReference](../../../../commons/AbstractDocumentTypeHelper.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [AbstractDocumentTypeHelper](../../../../commons/AbstractDocumentTypeHelper.md) Parameters: node - The node Returns: true if this node references another node which should replace it entirely. See Also:
        * [AbstractDocumentTypeHelper.isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../../commons/AbstractDocumentTypeHelper.md#isContentReference(ro.sync.ecss.extensions.api.node.AuthorNode))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
