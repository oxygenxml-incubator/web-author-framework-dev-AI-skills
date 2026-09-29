Package [ro.sync.ecss.extensions.commons.table.support](package-summary.md)

# Class DITATableCellInfoProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
        * ro.sync.ecss.extensions.commons.table.support.DITATableCellInfoProvider
   All Implemented Interfaces: [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md), [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md), [Extension](../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DITATableCellInfoProvider extends [AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)implements [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md)
Provides information about the column width for DITA tables.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
 [errorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#errorsListener)
## Constructor Summary
 Constructors
Constructor

Description
 [DITATableCellInfoProvider](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [commitColumnWidthModifications](#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String))([AuthorDocumentController](../../../api/AuthorDocumentController.md) authorDocumentController, [WidthRepresentation](../../../api/WidthRepresentation.md)[] colWidths, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Updates the column widths in the document and in the column layout model.
  void [commitTableWidthModification](#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String))([AuthorDocumentController](../../../api/AuthorDocumentController.md) authorDocumentController, int newTableWidth, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Commit the table width modification.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WidthRepresentation](../../../api/WidthRepresentation.md)> [getAllColspecWidthRepresentations](#getAllColspecWidthRepresentations())()
Get all with representations defined in all colspecs.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WidthRepresentation](../../../api/WidthRepresentation.md)> [getCellWidth](#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorElement](../../../api/node/AuthorElement.md) cellElement, int colNumberStart, int colSpan)
Get the width representation for the cell represented by the cellElement.
  [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) [getColSpan](#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) cellElement)
Get the number of columns the given cell spans across.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) [getRowSpan](#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) cellElement)
Get the number of rows that the given cell spans across.
  [WidthRepresentation](../../../api/WidthRepresentation.md) [getTableWidth](#getTableWidth(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Returns a non null [WidthRepresentation](../../../api/WidthRepresentation.md) if the table width is currently known.
  boolean [hasColumnSpecifications](#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
This method tells if the table contains column specifications.
  void [init](#init(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
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

### Methods inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
 [getErrorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#getErrorsListener()), [isPreferPercentageColumnWidths](../../../api/AuthorTableColumnWidthProviderBase.md#isPreferPercentageColumnWidths(java.lang.String)), [setErrorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#setErrorsListener(ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutErrorsListener))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITATableCellInfoProvider

public DITATableCellInfoProvider()

## Method Details

### init

public void init([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
 Description copied from interface: [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement))
This method is called when starting to compute the layout for a table. Its intended to extract information from the element representing the table only once, not on every getColSpan() or getRowSpan() call. Example: for a DocBook table we identify and cache the colspec and spanspec elements from that table. A new instance of the table cell span provider is used for every table in a document so cached data cannot be used between different tables..
  Specified by: [init](../../../api/AuthorTableCellSpanProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) Specified by: [init](../../../api/AuthorTableColumnWidthProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: tableElement - The [AuthorElement](../../../api/node/AuthorElement.md) representing a table (it has the CSS display property set on 'table'). See Also:
        * [AuthorTableCellSpanProvider.init(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../api/AuthorTableCellSpanProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement))

### getColSpan

public [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) getColSpan([AuthorElement](../../../api/node/AuthorElement.md) cellElement)
 Description copied from interface: [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement))
Get the number of columns the given cell spans across. For example, for the DocBook CALS tables the number of columns the cell spans across is computed by looking at the spanspec attribute. In case the spanspec attribute is missing then the column span is defined by the namest and nameend attribute.
  Specified by: [getColSpan](../../../api/AuthorTableCellSpanProvider.md#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) Parameters: cellElement - The node that represents a table cell in CSS. Returns: The number of columns this cell spans across (the minimum returned value must be 1) or null if not specified. See Also:
        * [AuthorTableCellSpanProvider.getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../api/AuthorTableCellSpanProvider.md#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement))

### getRowSpan

public [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) getRowSpan([AuthorElement](../../../api/node/AuthorElement.md) cellElement)
 Description copied from interface: [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement))
Get the number of rows that the given cell spans across. For example, for the DocBook CALS tables this value is computed by looking at the morerows attribute.
  Specified by: [getRowSpan](../../../api/AuthorTableCellSpanProvider.md#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) Parameters: cellElement - The [AuthorElement](../../../api/node/AuthorElement.md) that represents a table cell in CSS. Returns: The number of rows this cell spans across (the minimum returned value must be 1) or null if not specified. See Also:
        * [AuthorTableCellSpanProvider.getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../api/AuthorTableCellSpanProvider.md#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement))

### hasColumnSpecifications

public boolean hasColumnSpecifications([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
 Description copied from interface: [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement))
This method tells if the table contains column specifications. For example the CALS table model requires colspec elements to be present.
  Specified by: [hasColumnSpecifications](../../../api/AuthorTableCellSpanProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) Parameters: tableElement - The [AuthorElement](../../../api/node/AuthorElement.md) that is rendered as a table. Returns: true if some column specification info is present or if the table doesn't require any column specification info. See Also:
        * [AuthorTableCellSpanProvider.hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../api/AuthorTableCellSpanProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../../api/Extension.md#getDescription()) in interface [Extension](../../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

### getCellWidth

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WidthRepresentation](../../../api/WidthRepresentation.md)> getCellWidth([AuthorElement](../../../api/node/AuthorElement.md) cellElement, int colNumberStart, int colSpan)
 Description copied from interface: [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int))
Get the width representation for the cell represented by the cellElement. For example for a CALS table cell the list with the width representations is obtained by computing the column span and then determining the [WidthRepresentation](../../../api/WidthRepresentation.md)for each column the cell spans across.
  Specified by: [getCellWidth](../../../api/AuthorTableColumnWidthProvider.md#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: cellElement - The node that represents a table cell in CSS. colNumberStart - The column number the cell starts at. colSpan - The column span of the cell. Returns: The list with the [WidthRepresentation](../../../api/WidthRepresentation.md) of the specified cell element or null if the cell width cannot be computed. If the cell spans over multiple columns then the returned list will contain one [WidthRepresentation](../../../api/WidthRepresentation.md) for each column the cell spans over. See Also:
        * [AuthorTableColumnWidthProvider.getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement, int, int)](../../../api/AuthorTableColumnWidthProvider.md#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int))

### commitColumnWidthModifications

public void commitColumnWidthModifications([AuthorDocumentController](../../../api/AuthorDocumentController.md) authorDocumentController, [WidthRepresentation](../../../api/WidthRepresentation.md)[] colWidths, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)throws [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String))
Updates the column widths in the document and in the column layout model. For example, for the DocBook CALS tables the method updates the columns width specifications in the source document by setting the colwidth attribute value of the colspec elements. New colspec elements will be added if needed.
  Specified by: [commitColumnWidthModifications](../../../api/AuthorTableColumnWidthProvider.md#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: authorDocumentController - The [AuthorDocumentController](../../../api/AuthorDocumentController.md) used to commit the table modifications in the document. colWidths - The new column [WidthRepresentation](../../../api/WidthRepresentation.md) to set. The column widths must be ordered according to the corresponding column numbers. tableCellsTagName - The cells tag name. Used to identify the table type (e.g. 'entry' for CALS or 'td' for HTML). Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - If the operation fails. See Also:
        * [AuthorTableColumnWidthProvider.commitColumnWidthModifications(AuthorDocumentController, ro.sync.ecss.extensions.api.WidthRepresentation[], java.lang.String)](../../../api/AuthorTableColumnWidthProvider.md#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String))

### commitTableWidthModification

public void commitTableWidthModification([AuthorDocumentController](../../../api/AuthorDocumentController.md) authorDocumentController, int newTableWidth, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)throws [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String))
Commit the table width modification. For example in the case of DocBook HTML tables sets the width attribute value of the table element.
  Specified by: [commitTableWidthModification](../../../api/AuthorTableColumnWidthProvider.md#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: authorDocumentController - The [AuthorDocumentController](../../../api/AuthorDocumentController.md) used to commit the table width modifications in the document. newTableWidth - The new table [WidthRepresentation](../../../api/WidthRepresentation.md) to set. The value is given in pixels. tableCellsTagName - The cells tag name. Used to identify the table type (e.g. 'entry' for CALS or 'td' for HTML). Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - If the operation fails. See Also:
        * [AuthorTableColumnWidthProvider.commitTableWidthModification(AuthorDocumentController, int, java.lang.String)](../../../api/AuthorTableColumnWidthProvider.md#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String))

### getTableWidth

public [WidthRepresentation](../../../api/WidthRepresentation.md) getTableWidth([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
 Description copied from interface: [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md#getTableWidth(java.lang.String))
Returns a non null [WidthRepresentation](../../../api/WidthRepresentation.md) if the table width is currently known. For the DocBook HTML tables it returns the [WidthRepresentation](../../../api/WidthRepresentation.md) obtained by analyzing the width attribute value of the table element.
  Specified by: [getTableWidth](../../../api/AuthorTableColumnWidthProvider.md#getTableWidth(java.lang.String)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. 'entry' for CALS or 'td' for HTML). Returns: A non null value if the table width is specified. Otherwise null. See Also:
        * [AuthorTableColumnWidthProvider.getTableWidth(java.lang.String)](../../../api/AuthorTableColumnWidthProvider.md#getTableWidth(java.lang.String))

### isTableAcceptingWidth

public boolean isTableAcceptingWidth([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
 Description copied from interface: [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md#isTableAcceptingWidth(java.lang.String))
Used to determine if the table accepts width specification. For example, for the DocBook CALS tables which do not accept an width attribute the method will return false.
  Specified by: [isTableAcceptingWidth](../../../api/AuthorTableColumnWidthProvider.md#isTableAcceptingWidth(java.lang.String)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. 'entry' for CALS or 'td' for HTML). Returns: true if the table type denoted by the tableCellsTagName accepts width specification of any kind. See Also:
        * [AuthorTableColumnWidthProvider.isTableAcceptingWidth(java.lang.String)](../../../api/AuthorTableColumnWidthProvider.md#isTableAcceptingWidth(java.lang.String))

### isTableAndColumnsResizable

public boolean isTableAndColumnsResizable([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
 Description copied from interface: [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md#isTableAndColumnsResizable(java.lang.String))
This method is used to check if the table and/or table columns can be resized. For example in the case of the DocBook CALS tables will return trueonly if the given table cells tag name is equal to 'entry'.
  Specified by: [isTableAndColumnsResizable](../../../api/AuthorTableColumnWidthProvider.md#isTableAndColumnsResizable(java.lang.String)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. CALS or HTML). Returns: true if the size of the table or the table cells can be adjusted. See Also:
        * [AuthorTableColumnWidthProvider.isTableAndColumnsResizable(java.lang.String)](../../../api/AuthorTableColumnWidthProvider.md#isTableAndColumnsResizable(java.lang.String))

### isAcceptingFixedColumnWidths

public boolean isAcceptingFixedColumnWidths([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
 Description copied from interface: [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md#isAcceptingFixedColumnWidths(java.lang.String))
Check if the table column widths can be represented as fixed values.
  Specified by: [isAcceptingFixedColumnWidths](../../../api/AuthorTableColumnWidthProvider.md#isAcceptingFixedColumnWidths(java.lang.String)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. CALS or HTML). Returns: true if the table column widths can be represented in fixed values. See Also:
        * [AuthorTableColumnWidthProvider.isAcceptingFixedColumnWidths(java.lang.String)](../../../api/AuthorTableColumnWidthProvider.md#isAcceptingFixedColumnWidths(java.lang.String))

### isAcceptingPercentageColumnWidths

public boolean isAcceptingPercentageColumnWidths([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
 Description copied from interface: [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md#isAcceptingPercentageColumnWidths(java.lang.String))
Check if the table column widths can be represented as percentage values.
  Specified by: [isAcceptingPercentageColumnWidths](../../../api/AuthorTableColumnWidthProvider.md#isAcceptingPercentageColumnWidths(java.lang.String)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. CALS or HTML). Returns: true if the table column widths can be represented in percentage values. See Also:
        * [AuthorTableColumnWidthProvider.isAcceptingPercentageColumnWidths(java.lang.String)](../../../api/AuthorTableColumnWidthProvider.md#isAcceptingPercentageColumnWidths(java.lang.String))

### isAcceptingProportionalColumnWidths

public boolean isAcceptingProportionalColumnWidths([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
 Description copied from interface: [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md#isAcceptingProportionalColumnWidths(java.lang.String))
Check if the table column widths can be represented as proportional values.
  Specified by: [isAcceptingProportionalColumnWidths](../../../api/AuthorTableColumnWidthProvider.md#isAcceptingProportionalColumnWidths(java.lang.String)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. CALS or HTML). Returns: true if the table column widths can be represented in proportional values. See Also:
        * [AuthorTableColumnWidthProvider.isAcceptingProportionalColumnWidths(java.lang.String)](../../../api/AuthorTableColumnWidthProvider.md#isAcceptingProportionalColumnWidths(java.lang.String))

### getAllColspecWidthRepresentations

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WidthRepresentation](../../../api/WidthRepresentation.md)> getAllColspecWidthRepresentations()
 Description copied from class: [AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md#getAllColspecWidthRepresentations())
Get all with representations defined in all colspecs. If a colspec does not specify a width, it is supposed to be 1\*. If the table group specifies more columns than colspecs, those widths are supposed to be 1\*.
  Specified by: [getAllColspecWidthRepresentations](../../../api/AuthorTableColumnWidthProviderBase.md#getAllColspecWidthRepresentations()) in class [AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md) Returns: All width representations from the defined colspecs. See Also:
        * [AuthorTableColumnWidthProviderBase.getAllColspecWidthRepresentations()](../../../api/AuthorTableColumnWidthProviderBase.md#getAllColspecWidthRepresentations())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
