Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Interface AuthorTableHelper
    All Known Implementing Classes: [AbstractDocumentTypeHelper](../../AbstractDocumentTypeHelper.md), [CALSDocumentTypeHelper](cals/CALSDocumentTypeHelper.md), [DITARelTableDocumentTypeHelper](../../../dita/map/table/DITARelTableDocumentTypeHelper.md), [DITASimpleTableDocumentTypeHelper](../../../dita/topic/table/simpletable/DITASimpleTableDocumentTypeHelper.md), [DITATableDocumentTypeHelper](../../../dita/topic/table/DITATableDocumentTypeHelper.md), [TEIDocumentTypeHelper](../../../tei/TEIDocumentTypeHelper.md), [XHTMLDocumentTypeHelper](xhtml/XHTMLDocumentTypeHelper.md)   @API(type=INTERNAL, src=PUBLIC) public interface AuthorTableHelper
Document type specific table information helper. It contains methods that are specific to a document type and are used to obtain table and table cells related information.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [TYPE_CELL](#TYPE_CELL)
The cell type.
  static final int [TYPE_ROW](#TYPE_ROW)
The row type.
  static final int [TYPE_TABLE](#TYPE_TABLE)
The table type.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [checkTableColSpanIsDefined](#checkTableColSpanIsDefined(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) tableCellSpanProvider, [AuthorElement](../../../api/node/AuthorElement.md) cellElement)
Check if the column span is defined for a table cell.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredCellIDAttributes](#getIgnoredCellIDAttributes())()
Gets the ID attribute names which should be skipped when inserting a new column or row and the attributes from source cell fragments must be copied.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredColumnAttributes](#getIgnoredColumnAttributes())()
Gets the attributes which should be skipped when inserting a new column and the attributes from source cell fragments must be copied.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getIgnoredRowAttributes](#getIgnoredRowAttributes())()
Gets the attributes which should be skipped when using the current row as template for insert operation.
  [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) [getTableCellSpanProvider](#getTableCellSpanProvider(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
Create the table cell span provider for a specific table element.
  [AuthorNode](../../../api/node/AuthorNode.md) [getTableElementForDeletion](#getTableElementForDeletion(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
When we delete all the rows or all the columns of a table, we also want to delete the entire table element.
  boolean [isColspec](#isColspec(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
Check if a node is a colspec node.
  boolean [isTable](#isTable(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
Check if an [AuthorNode](../../../api/node/AuthorNode.md) is a table node.
  boolean [isTableCell](#isTableCell(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
Check if an [AuthorNode](../../../api/node/AuthorNode.md) is a table cell node.
  boolean [isTableRow](#isTableRow(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
Check if an [AuthorNode](../../../api/node/AuthorNode.md) is a table row node.
  void [updateTableColSpan](#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) tableCellSpanProvider, [AuthorElement](../../../api/node/AuthorElement.md) cellElem, int startCol, int endCol)
Update the column span of the cell by modifying the indices of start and end column.
  void [updateTableColumnNumber](#updateTableColumnNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, int colNum)
Update the table columns number.
  void [updateTableRowNumber](#updateTableRowNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, int relativeValue)
Update the table rows number.
  void [updateTableRowSpan](#updateTableRowSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) cellElem, int rowSpan)
Updates the cell row span to a specified value.

## Field Details

### TYPE_CELL

static final int TYPE_CELL

The cell type.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper.TYPE_CELL)

### TYPE_ROW

static final int TYPE_ROW

The row type.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper.TYPE_ROW)

### TYPE_TABLE

static final int TYPE_TABLE

The table type.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper.TYPE_TABLE)

## Method Details

### isTableCell

boolean isTableCell([AuthorNode](../../../api/node/AuthorNode.md) node)

Check if an [AuthorNode](../../../api/node/AuthorNode.md) is a table cell node.
  Parameters: node - The [AuthorNode](../../../api/node/AuthorNode.md) to be checked. Returns: true if the node is a table cell node, false otherwise.
### isTableRow

boolean isTableRow([AuthorNode](../../../api/node/AuthorNode.md) node)

Check if an [AuthorNode](../../../api/node/AuthorNode.md) is a table row node.
  Parameters: node - The [AuthorNode](../../../api/node/AuthorNode.md) to be checked. Returns: true if the node is a table row node, false otherwise.
### isTable

boolean isTable([AuthorNode](../../../api/node/AuthorNode.md) node)

Check if an [AuthorNode](../../../api/node/AuthorNode.md) is a table node.
  Parameters: node - The [AuthorNode](../../../api/node/AuthorNode.md) to be checked. Returns: true if the node is a table node, false otherwise.
### getTableCellSpanProvider

[AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) getTableCellSpanProvider([AuthorElement](../../../api/node/AuthorElement.md) tableElement)

Create the table cell span provider for a specific table element.
  Parameters: tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. Returns: The table cell span provider. Must not be null.
### checkTableColSpanIsDefined

void checkTableColSpanIsDefined([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) tableCellSpanProvider, [AuthorElement](../../../api/node/AuthorElement.md) cellElement)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Check if the column span is defined for a table cell.
 I.E. for DocBook the column span is defined by the 'colspec' element. If it is missing then the column span is not defined.

  Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableCellSpanProvider - The table cell span provider. cellElement - The cell element to be tested. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - When the column span is not defined for the table cell.
### updateTableColSpan

void updateTableColSpan([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) tableCellSpanProvider, [AuthorElement](../../../api/node/AuthorElement.md) cellElem, int startCol, int endCol)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Update the column span of the cell by modifying the indices of start and end column. For example, for the DocBook CALS tables the namest and nameend attributes will be set according to the startCol and endCol supplied values.
  Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableCellSpanProvider - The object responsible for providing information about the cell spanning. cellElem - The cell element whose column span will be updated. startCol - The new index of start column. It is 1 based and inclusive. endCol - The new index of end column. It is 1 based and inclusive. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - When the column specifications for start or end columns are missing.
### updateTableRowSpan

void updateTableRowSpan([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) cellElem, int rowSpan)

Updates the cell row span to a specified value. For example, for the DocBook CALS tables the morerows attribute value will be updated.
  Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. cellElem - The cell element whose row span will be updated. rowSpan - The new row span value. It is 1 based.
### updateTableColumnNumber

void updateTableColumnNumber([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, int colNum)

Update the table columns number. For example, for the DocBook CALS tables the cols attribute value will be updated.
  Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. colNum - The updated number of columns.
### updateTableRowNumber

void updateTableRowNumber([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, int relativeValue)

Update the table rows number.
  Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. relativeValue - The number of rows to increase or decrease the current number of table rows. If the number of rows must be decreased then the argument must be negative.
### getIgnoredRowAttributes

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredRowAttributes()

Gets the attributes which should be skipped when using the current row as template for insert operation.
  Returns: The attributes which should be skipped.
### getIgnoredColumnAttributes

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredColumnAttributes()

Gets the attributes which should be skipped when inserting a new column and the attributes from source cell fragments must be copied.
  Returns: The attributes which should be skipped.
### getIgnoredCellIDAttributes

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getIgnoredCellIDAttributes()

Gets the ID attribute names which should be skipped when inserting a new column or row and the attributes from source cell fragments must be copied.
  Returns: The ID attributes which should be skipped.
### getTableElementForDeletion

[AuthorNode](../../../api/node/AuthorNode.md) getTableElementForDeletion([AuthorNode](../../../api/node/AuthorNode.md) node)

When we delete all the rows or all the columns of a table, we also want to delete the entire table element. OBS: For CALS tables we don't want to delete only the "tgroup", but the parent table element itself.
  Parameters: node - the node whose parent table we are looking for. Returns: the table element to be deleted.
### isColspec

boolean isColspec([AuthorNode](../../../api/node/AuthorNode.md) node)

Check if a node is a colspec node.
  Parameters: node - The node. Returns: true if a node is a colspec node.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
