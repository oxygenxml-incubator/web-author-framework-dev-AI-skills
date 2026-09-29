Package [ro.sync.ecss.extensions.api.access](package-summary.md)

# Interface AuthorTableAccess
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorTableAccess
Provides methods for table actions and informations regarding the table content.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorElement](../node/AuthorElement.md) [getTableCellAbove](#getTableCellAbove(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../node/AuthorElement.md) cellElement)
Find the cell included into the previous row and has the same column index as the specified cell [AuthorElement](../node/AuthorElement.md).
  [AuthorElement](../node/AuthorElement.md) [getTableCellAt](#getTableCellAt(int,int,ro.sync.ecss.extensions.api.node.AuthorElement))(int row, int column, [AuthorElement](../node/AuthorElement.md) tableElement)
Obtain the cell [AuthorElement](../node/AuthorElement.md) for the given row and column in the specified table.
  [AuthorElement](../node/AuthorElement.md) [getTableCellBelow](#getTableCellBelow(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../node/AuthorElement.md) cellElement)
Find the cell included into the next row and has the same column index as the specified cell [AuthorElement](../node/AuthorElement.md).
  int[] [getTableCellIndex](#getTableCellIndex(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../node/AuthorElement.md) cellElement)
Obtain the table row and column index for the cell corresponding to the specified cell [AuthorElement](../node/AuthorElement.md).
  int[] [getTableColSpanIndices](#getTableColSpanIndices(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../node/AuthorElement.md) cellElement)
For the given cell [AuthorElement](../node/AuthorElement.md) find the start and end column defining the column span interval.
  int [getTableNumberOfColumns](#getTableNumberOfColumns(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../node/AuthorElement.md) tableElement)
Returns the number of columns for the given table [AuthorElement](../node/AuthorElement.md).
  [AuthorElement](../node/AuthorElement.md) [getTableRow](#getTableRow(int,ro.sync.ecss.extensions.api.node.AuthorElement))(int index, [AuthorElement](../node/AuthorElement.md) tableElement)
Find the table row element for the given index.
  int [getTableRowCount](#getTableRowCount(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../node/AuthorElement.md) tableElement)
Get the row count for the given table [AuthorElement](../node/AuthorElement.md).
  int[] [getTableRowSpanIndices](#getTableRowSpanIndices(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../node/AuthorElement.md) cellElement)
For the given cell [AuthorElement](../node/AuthorElement.md) find the start and end row defining the row span interval.

## Method Details

### getTableCellAbove

[AuthorElement](../node/AuthorElement.md) getTableCellAbove([AuthorElement](../node/AuthorElement.md) cellElement)

Find the cell included into the previous row and has the same column index as the specified cell [AuthorElement](../node/AuthorElement.md).
  Parameters: cellElement - The table cell element. Returns: The cell above the given one. Can be null if there is no cell above the given one or the element does not correspond to a table cell..
### getTableCellBelow

[AuthorElement](../node/AuthorElement.md) getTableCellBelow([AuthorElement](../node/AuthorElement.md) cellElement)

Find the cell included into the next row and has the same column index as the specified cell [AuthorElement](../node/AuthorElement.md).
  Parameters: cellElement - The table cell element. Returns: The cell bellow the given one. Can be null if there is no cell bellow the given one or the element does not correspond to a table cell..
### getTableCellIndex

int[] getTableCellIndex([AuthorElement](../node/AuthorElement.md) cellElement)

Obtain the table row and column index for the cell corresponding to the specified cell [AuthorElement](../node/AuthorElement.md).
  Parameters: cellElement - The table cell element. Returns: an array containing the row index on the first position and column index on second one. Both are 0 based. Can be null if the element does not correspond to a cell in a table.
### getTableCellAt

[AuthorElement](../node/AuthorElement.md) getTableCellAt(int row, int column, [AuthorElement](../node/AuthorElement.md) tableElement)

Obtain the cell [AuthorElement](../node/AuthorElement.md) for the given row and column in the specified table.
  Parameters: row - The row, 0 based. column - The column, 0 based. tableElement - The table element. Returns: The element at the specified location. Can be null if the table does not have a cell at the provided indices.
### getTableRow

[AuthorElement](../node/AuthorElement.md) getTableRow(int index, [AuthorElement](../node/AuthorElement.md) tableElement)

Find the table row element for the given index.
  Parameters: index - The index of the row to find the element for, 0 based. tableElement - The table element. Returns: The table row. Can be null if the table does not have a row at the given index.
### getTableRowCount

int getTableRowCount([AuthorElement](../node/AuthorElement.md) tableElement)

Get the row count for the given table [AuthorElement](../node/AuthorElement.md).
  Parameters: tableElement - The table element. Returns: The row count.
### getTableNumberOfColumns

int getTableNumberOfColumns([AuthorElement](../node/AuthorElement.md) tableElement)

Returns the number of columns for the given table [AuthorElement](../node/AuthorElement.md).
  Parameters: tableElement - The table element. Returns: The number of columns.
### getTableColSpanIndices

int[] getTableColSpanIndices([AuthorElement](../node/AuthorElement.md) cellElement)

For the given cell [AuthorElement](../node/AuthorElement.md) find the start and end column defining the column span interval. The indices are 0 based.
  Parameters: cellElement - The table cell element. Returns: An array containing the start span column index on the first position and the end span column index on the second one. Can be null if the element does not correspond to a cell in a table.
### getTableRowSpanIndices

int[] getTableRowSpanIndices([AuthorElement](../node/AuthorElement.md) cellElement)

For the given cell [AuthorElement](../node/AuthorElement.md) find the start and end row defining the row span interval. The indices are 0 based.
  Parameters: cellElement - The table cell element. Returns: An array containing the start span row index on the first position and the end span row index on the second one. Can be null if the element does not correspond to a cell in a table. Since: 13
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
