Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorTableColumnWidthProvider
    All Superinterfaces: [Extension](Extension.md)   All Known Implementing Classes: [AuthorTableColumnWidthProviderBase](AuthorTableColumnWidthProviderBase.md), [CALSandHTMLTableCellInfoProvider](../commons/table/support/CALSandHTMLTableCellInfoProvider.md), [CALSandHTMLTableCellSpanProvider](../commons/table/spansupport/CALSandHTMLTableCellSpanProvider.md), [CALSTableCellInfoProvider](../commons/table/support/CALSTableCellInfoProvider.md), [CALSTableCellSpanProvider](../commons/table/spansupport/CALSTableCellSpanProvider.md), [DITACALSTableCellInfoProvider](../commons/table/support/DITACALSTableCellInfoProvider.md), [DITATableCellInfoProvider](../commons/table/support/DITATableCellInfoProvider.md), [DITATableCellSepInfoProvider](../commons/table/support/DITATableCellSepInfoProvider.md), [DocbookTableCellSepInfoProvider](../docbook/table/DocbookTableCellSepInfoProvider.md), [HTMLTableCellInfoProvider](../commons/table/support/HTMLTableCellInfoProvider.md), [HTMLTableCellSpanProvider](../commons/table/spansupport/HTMLTableCellSpanProvider.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorTableColumnWidthProviderextends [Extension](Extension.md)
This is an interface for classes which are responsible for providing information and handling modifications regarding table and column widths. It should be implemented when the author extension being developed offers support for editing data in tabular form.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [commitColumnWidthModifications](#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String))([AuthorDocumentController](AuthorDocumentController.md) authorDocumentController, [WidthRepresentation](WidthRepresentation.md)[] colWidths, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Updates the column widths in the document and in the column layout model.
  void [commitTableWidthModification](#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String))([AuthorDocumentController](AuthorDocumentController.md) authorDocumentController, int newTableWidth, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Commit the table width modification.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WidthRepresentation](WidthRepresentation.md)> [getCellWidth](#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorElement](node/AuthorElement.md) cellElement, int colNumberStart, int colSpan)
Get the width representation for the cell represented by the cellElement.
  [WidthRepresentation](WidthRepresentation.md) [getTableWidth](#getTableWidth(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Returns a non null [WidthRepresentation](WidthRepresentation.md) if the table width is currently known.
  void [init](#init(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) tableElement)
This method is called when starting to compute the layout for a table.
  boolean [isAcceptingFixedColumnWidths](#isAcceptingFixedColumnWidths(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Check if the table column widths can be represented as fixed values.
  boolean [isAcceptingPercentageColumnWidths](#isAcceptingPercentageColumnWidths(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Check if the table column widths can be represented as percentage values.
  boolean [isAcceptingProportionalColumnWidths](#isAcceptingProportionalColumnWidths(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Check if the table column widths can be represented as proportional values.
  boolean [isTableAcceptingWidth](#isTableAcceptingWidth(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Used to determine if the table accepts width specification.
  boolean [isTableAndColumnsResizable](#isTableAndColumnsResizable(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
This method is used to check if the table and/or table columns can be resized.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Method Details

### getCellWidth

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WidthRepresentation](WidthRepresentation.md)> getCellWidth([AuthorElement](node/AuthorElement.md) cellElement, int colNumberStart, int colSpan)

Get the width representation for the cell represented by the cellElement. For example for a CALS table cell the list with the width representations is obtained by computing the column span and then determining the [WidthRepresentation](WidthRepresentation.md)for each column the cell spans across.
  Parameters: cellElement - The node that represents a table cell in CSS. colNumberStart - The column number the cell starts at. colSpan - The column span of the cell. Returns: The list with the [WidthRepresentation](WidthRepresentation.md) of the specified cell element or null if the cell width cannot be computed. If the cell spans over multiple columns then the returned list will contain one [WidthRepresentation](WidthRepresentation.md) for each column the cell spans over.
### init

void init([AuthorElement](node/AuthorElement.md) tableElement)

This method is called when starting to compute the layout for a table. Its intended to extract information from the element representing the table only once, not on every getColSpan() or getRowSpan() call.  Example: for a DocBook table we identify and cache the 'colspec' and 'spanspec' elements from that table. A new instance of the table column width provider is used for every table in a document so cached data cannot be reused between different tables.
  Parameters: tableElement - The element representing a table (it has the CSS display property set on 'table').
### commitColumnWidthModifications

void commitColumnWidthModifications([AuthorDocumentController](AuthorDocumentController.md) authorDocumentController, [WidthRepresentation](WidthRepresentation.md)[] colWidths, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)throws [AuthorOperationException](AuthorOperationException.md)

Updates the column widths in the document and in the column layout model. For example, for the DocBook CALS tables the method updates the columns width specifications in the source document by setting the colwidth attribute value of the colspec elements. New colspec elements will be added if needed.
  Parameters: authorDocumentController - The [AuthorDocumentController](AuthorDocumentController.md) used to commit the table modifications in the document. colWidths - The new column [WidthRepresentation](WidthRepresentation.md) to set. The column widths must be ordered according to the corresponding column numbers. tableCellsTagName - The cells tag name. Used to identify the table type (e.g. 'entry' for CALS or 'td' for HTML). Throws: [AuthorOperationException](AuthorOperationException.md) - If the operation fails.
### commitTableWidthModification

void commitTableWidthModification([AuthorDocumentController](AuthorDocumentController.md) authorDocumentController, int newTableWidth, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)throws [AuthorOperationException](AuthorOperationException.md)

Commit the table width modification. For example in the case of DocBook HTML tables sets the width attribute value of the table element.
  Parameters: authorDocumentController - The [AuthorDocumentController](AuthorDocumentController.md) used to commit the table width modifications in the document. newTableWidth - The new table [WidthRepresentation](WidthRepresentation.md) to set. The value is given in pixels. tableCellsTagName - The cells tag name. Used to identify the table type (e.g. 'entry' for CALS or 'td' for HTML). Throws: [AuthorOperationException](AuthorOperationException.md) - If the operation fails.
### isTableAcceptingWidth

boolean isTableAcceptingWidth([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)

Used to determine if the table accepts width specification. For example, for the DocBook CALS tables which do not accept an width attribute the method will return false.
  Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. 'entry' for CALS or 'td' for HTML). Returns: true if the table type denoted by the tableCellsTagName accepts width specification of any kind.
### getTableWidth

[WidthRepresentation](WidthRepresentation.md) getTableWidth([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)

Returns a non null [WidthRepresentation](WidthRepresentation.md) if the table width is currently known. For the DocBook HTML tables it returns the [WidthRepresentation](WidthRepresentation.md) obtained by analyzing the width attribute value of the table element.
  Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. 'entry' for CALS or 'td' for HTML). Returns: A non null value if the table width is specified. Otherwise null.
### isTableAndColumnsResizable

boolean isTableAndColumnsResizable([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)

This method is used to check if the table and/or table columns can be resized. For example in the case of the DocBook CALS tables will return trueonly if the given table cells tag name is equal to 'entry'.
  Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. CALS or HTML). Returns: true if the size of the table or the table cells can be adjusted.
### isAcceptingFixedColumnWidths

boolean isAcceptingFixedColumnWidths([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)

Check if the table column widths can be represented as fixed values.
  Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. CALS or HTML). Returns: true if the table column widths can be represented in fixed values.
### isAcceptingProportionalColumnWidths

boolean isAcceptingProportionalColumnWidths([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)

Check if the table column widths can be represented as proportional values.
  Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. CALS or HTML). Returns: true if the table column widths can be represented in proportional values.
### isAcceptingPercentageColumnWidths

boolean isAcceptingPercentageColumnWidths([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)

Check if the table column widths can be represented as percentage values.
  Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. CALS or HTML). Returns: true if the table column widths can be represented in percentage values.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
