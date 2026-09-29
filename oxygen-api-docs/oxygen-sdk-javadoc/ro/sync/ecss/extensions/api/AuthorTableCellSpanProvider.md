Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorTableCellSpanProvider
    All Superinterfaces: [Extension](Extension.md)   All Known Implementing Classes: [CALSandHTMLTableCellInfoProvider](../commons/table/support/CALSandHTMLTableCellInfoProvider.md), [CALSandHTMLTableCellSpanProvider](../commons/table/spansupport/CALSandHTMLTableCellSpanProvider.md), [CALSTableCellInfoProvider](../commons/table/support/CALSTableCellInfoProvider.md), [CALSTableCellSpanProvider](../commons/table/spansupport/CALSTableCellSpanProvider.md), [DITACALSTableCellInfoProvider](../commons/table/support/DITACALSTableCellInfoProvider.md), [DITASimpleTableCellSpanProvider](../commons/table/support/DITASimpleTableCellSpanProvider.md), [DITATableCellInfoProvider](../commons/table/support/DITATableCellInfoProvider.md), [DITATableCellSepInfoProvider](../commons/table/support/DITATableCellSepInfoProvider.md), [DocbookTableCellSepInfoProvider](../docbook/table/DocbookTableCellSepInfoProvider.md), [HTMLTableCellInfoProvider](../commons/table/support/HTMLTableCellInfoProvider.md), [HTMLTableCellSpanProvider](../commons/table/spansupport/HTMLTableCellSpanProvider.md), [ReltableCellSpanProvider](../dita/map/table/ReltableCellSpanProvider.md), [TEITableCellSpanProvider](../commons/table/spansupport/TEITableCellSpanProvider.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorTableCellSpanProviderextends [Extension](Extension.md)
This is an interface for classes which are responsible for providing information about the cell spanning. It should be implemented when the author extension being developed offers support for editing data in tabular form.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) [getColSpan](#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) cellElement)
Get the number of columns the given cell spans across.
  [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) [getRowSpan](#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) cellElement)
Get the number of rows that the given cell spans across.
  boolean [hasColumnSpecifications](#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) tableElement)
This method tells if the table contains column specifications.
  void [init](#init(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) tableElement)
This method is called when starting to compute the layout for a table.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Method Details

### getColSpan

[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) getColSpan([AuthorElement](node/AuthorElement.md) cellElement)

Get the number of columns the given cell spans across. For example, for the DocBook CALS tables the number of columns the cell spans across is computed by looking at the spanspec attribute. In case the spanspec attribute is missing then the column span is defined by the namest and nameend attribute.
  Parameters: cellElement - The node that represents a table cell in CSS. Returns: The number of columns this cell spans across (the minimum returned value must be 1) or null if not specified.
### getRowSpan

[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) getRowSpan([AuthorElement](node/AuthorElement.md) cellElement)

Get the number of rows that the given cell spans across. For example, for the DocBook CALS tables this value is computed by looking at the morerows attribute.
  Parameters: cellElement - The [AuthorElement](node/AuthorElement.md) that represents a table cell in CSS. Returns: The number of rows this cell spans across (the minimum returned value must be 1) or null if not specified.
### init

void init([AuthorElement](node/AuthorElement.md) tableElement)

This method is called when starting to compute the layout for a table. Its intended to extract information from the element representing the table only once, not on every getColSpan() or getRowSpan() call. Example: for a DocBook table we identify and cache the colspec and spanspec elements from that table. A new instance of the table cell span provider is used for every table in a document so cached data cannot be used between different tables..
  Parameters: tableElement - The [AuthorElement](node/AuthorElement.md) representing a table (it has the CSS display property set on 'table').
### hasColumnSpecifications

boolean hasColumnSpecifications([AuthorElement](node/AuthorElement.md) tableElement)

This method tells if the table contains column specifications. For example the CALS table model requires colspec elements to be present.
  Parameters: tableElement - The [AuthorElement](node/AuthorElement.md) that is rendered as a table. Returns: true if some column specification info is present or if the table doesn't require any column specification info.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
