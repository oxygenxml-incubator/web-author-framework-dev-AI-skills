Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorTableCellSepProvider
    All Superinterfaces: [Extension](Extension.md)   All Known Implementing Classes: [CALSTableCellInfoProvider](../commons/table/support/CALSTableCellInfoProvider.md), [CALSTableCellSpanProvider](../commons/table/spansupport/CALSTableCellSpanProvider.md), [DITACALSTableCellInfoProvider](../commons/table/support/DITACALSTableCellInfoProvider.md), [DITATableCellSepInfoProvider](../commons/table/support/DITATableCellSepInfoProvider.md), [DocbookTableCellSepInfoProvider](../docbook/table/DocbookTableCellSepInfoProvider.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorTableCellSepProviderextends [Extension](Extension.md)
This is an interface for classes which are responsible for providing information about the cell separators: "rowsep" and "colsep". It should be implemented when the author extension being developed offers support for editing data in tabular form.
  See Also:
* "http://www.docbook.org/tdg5/en/html/cals.table.html"
* "http://docs.oasis-open.org/dita/v1.0/langspec/table.html"
* "https://www.oasis-open.org/specs/tm9901.html"

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [getColSep](#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](node/AuthorElement.md) cellElement, int columnIndex)
Checks if a separator should be placed at the cell right.
  boolean [getRowSep](#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](node/AuthorElement.md) cellElement, int columnIndex)
Checks if a separator should be placed at the cell bottom.
  void [init](#init(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) tableElement)
This method is called when starting to compute the layout for a table.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Method Details

### getColSep

boolean getColSep([AuthorElement](node/AuthorElement.md) cellElement, int columnIndex)

Checks if a separator should be placed at the cell right. Note that if the cell is the last from its row, the separator is not painted even if this method returns true.
  Parameters: cellElement - The node that represents a table cell in CSS. columnIndex - The index of the column, used to identify the colspec associated to the cell. The colspec can give information about the colsep. 1 based. Returns: true if a separator should be placed at its right, false otherwise.
### getRowSep

boolean getRowSep([AuthorElement](node/AuthorElement.md) cellElement, int columnIndex)

Checks if a separator should be placed at the cell bottom. Note that if the cell is on the last row, the separator is not painted even if this method returns true.
  Parameters: cellElement - The node that represents a table cell in CSS. columnIndex - The index of the column, used to identify the rowspec associated to the cell. The rowspec can give information about the colsep. 1 based. Returns: true if a separator should be placed at its right, false otherwise.
### init

void init([AuthorElement](node/AuthorElement.md) tableElement)

This method is called when starting to compute the layout for a table. Its intended to extract information from the element representing the table only once, not on every getColSep() or getRowSep() call. Example: for a CALS table we identify and cache the colsep and rowsep elements from that table. A new instance of the table cell span provider is used for every table in a document so cached data cannot be used between different tables..
  Parameters: tableElement - The [AuthorElement](node/AuthorElement.md) representing a table (it has the CSS display property set on 'table').
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
