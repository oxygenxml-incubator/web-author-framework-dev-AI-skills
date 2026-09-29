Package [ro.sync.ecss.extensions.commons.table.support](package-summary.md)

# Class CALSTableCellInfoProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
        * ro.sync.ecss.extensions.commons.table.support.CALSTableCellInfoProvider
   All Implemented Interfaces: [AuthorTableCellSepProvider](../../../api/AuthorTableCellSepProvider.md), [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md), [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md), [Extension](../../../api/Extension.md), [CALSConstants](../operations/cals/CALSConstants.md)   Direct Known Subclasses: [CALSTableCellSpanProvider](../spansupport/CALSTableCellSpanProvider.md), [DITACALSTableCellInfoProvider](DITACALSTableCellInfoProvider.md), [DITATableCellSepInfoProvider](DITATableCellSepInfoProvider.md), [DocbookTableCellSepInfoProvider](../../../docbook/table/DocbookTableCellSepInfoProvider.md)   @API(type=INTERNAL, src=PUBLIC) public class CALSTableCellInfoProvider extends [AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)implements [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md), [CALSConstants](../operations/cals/CALSConstants.md), [AuthorTableCellSepProvider](../../../api/AuthorTableCellSepProvider.md)
Provides informations about the cell spanning and column width for Docbook CALS tables.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [WidthRepresentation](../../../api/WidthRepresentation.md) [DEFAULT_WIDTH_REPRESENTATION](#DEFAULT_WIDTH_REPRESENTATION)
The default width representation.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CALSColSpanSpec](CALSColSpanSpec.md)> [spanspecInfos](#spanspecInfos)
The list with the CALSColSpanSpec containing information about the columns span specification for this table.

### Fields inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
 [errorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#errorsListener)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](../operations/cals/CALSConstants.md)
 [ATTRIBUTE_NAME_ALIGN](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ALIGN), [ATTRIBUTE_NAME_COLNAME](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLNAME), [ATTRIBUTE_NAME_COLNUM](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLNUM), [ATTRIBUTE_NAME_COLS](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_COLSEP](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLSEP), [ATTRIBUTE_NAME_COLWIDTH](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLWIDTH), [ATTRIBUTE_NAME_ID](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_MOREROWS](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_MOREROWS), [ATTRIBUTE_NAME_NAMEEND](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_NAMEEND), [ATTRIBUTE_NAME_NAMEST](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_NAMEST), [ATTRIBUTE_NAME_ROWSEP](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ROWSEP), [ATTRIBUTE_NAME_SPANNAME](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_SPANNAME), [ATTRIBUTE_NAME_TABLE_WIDTH](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_TABLE_WIDTH), [ATTRIBUTE_NAME_XML_ID](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_COLSPEC](../operations/cals/CALSConstants.md#ELEMENT_NAME_COLSPEC), [ELEMENT_NAME_ENTRY](../operations/cals/CALSConstants.md#ELEMENT_NAME_ENTRY), [ELEMENT_NAME_INFORMALTABLE](../operations/cals/CALSConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_ROW](../operations/cals/CALSConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_SPANSPEC](../operations/cals/CALSConstants.md#ELEMENT_NAME_SPANSPEC), [ELEMENT_NAME_TABLE](../operations/cals/CALSConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TGROUP](../operations/cals/CALSConstants.md#ELEMENT_NAME_TGROUP)
## Constructor Summary
 Constructors
Constructor

Description
 [CALSTableCellInfoProvider](#%3Cinit%3E())()
Constructor.
  [CALSTableCellInfoProvider](#%3Cinit%3E(boolean))(boolean colsepAndRowSepAreVisibleByDefault)
Constructor.
  [CALSTableCellInfoProvider](#%3Cinit%3E(boolean,ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutErrorsListener))(boolean colsepAndRowSepAreVisibleByDefault, [TableLayoutErrorsListener](errorscanner/TableLayoutErrorsListener.md) errorsListener)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [commitColumnWidthModifications](#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String))([AuthorDocumentController](../../../api/AuthorDocumentController.md) authorDocumentController, [WidthRepresentation](../../../api/WidthRepresentation.md)[] colWidths, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Updates the columns width specifications in the source document by setting the colwidth attribute value of the colspec elements and by adding new colspecelements if needed.
  void [commitTableWidthModification](#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String))([AuthorDocumentController](../../../api/AuthorDocumentController.md) authorDocumentController, int newTableWidth, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Sets the width attribute value of the table element.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WidthRepresentation](../../../api/WidthRepresentation.md)> [getAllColspecWidthRepresentations](#getAllColspecWidthRepresentations())()
Get all with representations defined in all colspecs.
  [CALSColSpanSpec](CALSColSpanSpec.md) [getCellSpanSpec](#getCellSpanSpec(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) cellElement)
Find the column span specification for a table cell.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WidthRepresentation](../../../api/WidthRepresentation.md)> [getCellWidth](#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorElement](../../../api/node/AuthorElement.md) cellElement, int colNumberStart, int colSpan)
The list with the width representations for the given cell is obtained by computing the column span and then determining the [WidthRepresentation](../../../api/WidthRepresentation.md)for each column the cell spans across.
  boolean [getColSep](#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../api/node/AuthorElement.md) cellElem, int columnIndex)
Checks if a separator should be placed at the cell right.
  [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) [getColSpan](#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) cellElem)
Compute the number of columns the cell spans across by looking at the 'spanspec' attribute.
  int[] [getColSpanInterval](#getColSpanInterval(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) cellElem)
Compute the interval a cell spans across by looking at the 'spanspec' attribute.
  [CALSColSpec](CALSColSpec.md) [getColSpec](#getColSpec(int))(int columnNumber)
Find the column specification for the given column number.
  [CALSColSpec](CALSColSpec.md) [getColSpec](#getColSpec(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colSpecName)
Find a column specification by name.
  [AuthorElement](../../../api/node/AuthorElement.md) [getColSpecElement](#getColSpecElement(ro.sync.ecss.extensions.commons.table.support.CALSColSpec))([CALSColSpec](CALSColSpec.md) colspec)
Find a column specification element.
  [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[CALSColSpec](CALSColSpec.md)> [getColSpecs](#getColSpecs())()
Returns the column specification set corresponding to the CALS table.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 boolean [getRowSep](#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../api/node/AuthorElement.md) cellElem, int columnIndex)
Checks if a separator should be placed at the cell bottom.
  [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) [getRowSpan](#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) cellElement)
Compute the number of rows the cells span across by looking at the morerows attribute.
  [WidthRepresentation](../../../api/WidthRepresentation.md) [getTableWidth](#getTableWidth(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Returns the [WidthRepresentation](../../../api/WidthRepresentation.md) obtained by analyzing the width attribute value of the table element.
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
  protected boolean [isColspec](#isColspec(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) child)
Check if the child is a column specification.
  boolean [isTableAcceptingWidth](#isTableAcceptingWidth(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
The DocBook CALS tables do not accept width specification.
  boolean [isTableAndColumnsResizable](#isTableAndColumnsResizable(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
It returns true only if the given table cells tag name is equal to 'entry'.
  protected boolean [isTableCell](#isTableCell(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Check if the name of an element is a table cell.
  protected boolean [isTableElement](#isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) element)
Check if this element is a table element.
  protected boolean [isTgroupElement](#isTgroupElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) element)
Check if this element is a tgroup element.

### Methods inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
 [getErrorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#getErrorsListener()), [isPreferPercentageColumnWidths](../../../api/AuthorTableColumnWidthProviderBase.md#isPreferPercentageColumnWidths(java.lang.String)), [setErrorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#setErrorsListener(ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutErrorsListener))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### DEFAULT_WIDTH_REPRESENTATION

public static final [WidthRepresentation](../../../api/WidthRepresentation.md) DEFAULT_WIDTH_REPRESENTATION

The default width representation. PUBLIC BECAUSE IT WAS USED IN OLDER VERSIONS AS API.

### spanspecInfos

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CALSColSpanSpec](CALSColSpanSpec.md)> spanspecInfos

The list with the CALSColSpanSpec containing information about the columns span specification for this table.

## Constructor Details

### CALSTableCellInfoProvider

public CALSTableCellInfoProvider(boolean colsepAndRowSepAreVisibleByDefault)

Constructor.
  Parameters: colsepAndRowSepAreVisibleByDefault - The default visibility for the rowsep and colsep. (i.e. if no colsep or rowsep attributes are present in the table).
### CALSTableCellInfoProvider

public CALSTableCellInfoProvider()

Constructor. The default visibility for the rowsep and colsep. (i.e. if no colsep or rowsep attributes are present in the table) is hidden.

### CALSTableCellInfoProvider

public CALSTableCellInfoProvider(boolean colsepAndRowSepAreVisibleByDefault, [TableLayoutErrorsListener](errorscanner/TableLayoutErrorsListener.md) errorsListener)

Constructor.
  Parameters: colsepAndRowSepAreVisibleByDefault - The default visibility for the rowsep and colsep. (i.e. if no colsep or rowsep attributes are present in the table). errorsListener - Table layout errors listener.
## Method Details

### getColSpan

public [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) getColSpan([AuthorElement](../../../api/node/AuthorElement.md) cellElem)

Compute the number of columns the cell spans across by looking at the 'spanspec' attribute. In case the 'spanspec' attribute is missing then the column span is defined by the 'namest' and 'nameend' attribute.
  Specified by: [getColSpan](../../../api/AuthorTableCellSpanProvider.md#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) Parameters: cellElem - The node that represents a table cell in CSS. Returns: The number of columns this cell spans across (the minimum returned value must be 1) or null if not specified. See Also:
        * [AuthorTableCellSpanProvider.getColSpan(AuthorElement)](../../../api/AuthorTableCellSpanProvider.md#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement))

### getColSpanInterval

public int[] getColSpanInterval([AuthorElement](../../../api/node/AuthorElement.md) cellElem)

Compute the interval a cell spans across by looking at the 'spanspec' attribute. In case the 'spanspec' attribute is missing then the column span is defined by the 'namest' and 'nameend' attribute.
  Parameters: cellElem - Cell we want to check for spans. Returns: The interval a cell spans. Can be null
### getRowSpan

public [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) getRowSpan([AuthorElement](../../../api/node/AuthorElement.md) cellElement)

Compute the number of rows the cells span across by looking at the morerows attribute.
  Specified by: [getRowSpan](../../../api/AuthorTableCellSpanProvider.md#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) Parameters: cellElement - The [AuthorElement](../../../api/node/AuthorElement.md) that represents a table cell in CSS. Returns: The number of rows this cell spans across (the minimum returned value must be 1) or null if not specified. See Also:
        * [AuthorTableCellSpanProvider.getRowSpan(AuthorElement)](../../../api/AuthorTableCellSpanProvider.md#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement))

### init

public void init([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
 Description copied from interface: [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement))
This method is called when starting to compute the layout for a table. Its intended to extract information from the element representing the table only once, not on every getColSpan() or getRowSpan() call. Example: for a DocBook table we identify and cache the colspec and spanspec elements from that table. A new instance of the table cell span provider is used for every table in a document so cached data cannot be used between different tables..
  Specified by: [init](../../../api/AuthorTableCellSepProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSepProvider](../../../api/AuthorTableCellSepProvider.md) Specified by: [init](../../../api/AuthorTableCellSpanProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) Specified by: [init](../../../api/AuthorTableColumnWidthProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: tableElement - The [AuthorElement](../../../api/node/AuthorElement.md) representing a table (it has the CSS display property set on 'table'). See Also:
        * [AuthorTableColumnWidthProvider.init(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../api/AuthorTableColumnWidthProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement))

### isColspec

protected boolean isColspec([AuthorElement](../../../api/node/AuthorElement.md) child)

Check if the child is a column specification.
  Parameters: child - The child Returns: true if the child is a column specification.
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../../api/Extension.md#getDescription()) in interface [Extension](../../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

### getCellSpanSpec

public [CALSColSpanSpec](CALSColSpanSpec.md) getCellSpanSpec([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) cellElement)

Find the column span specification for a table cell. If 'spanname' attribute is present the corresponding span specification will be returned. Otherwise a new span specification will be returned looking at the name of columns spanned by the cell.
  Parameters: authorAccess - The author access. cellElement - The table cell element. Returns: The cell span specification. Null when column specifications are not defined.
### getColSpec

public [CALSColSpec](CALSColSpec.md) getColSpec([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colSpecName)

Find a column specification by name.
  Parameters: colSpecName - The name of column specification. Returns: The column specification or null if no column specification is defined for the given colspec name.
### getColSpec

public [CALSColSpec](CALSColSpec.md) getColSpec(int columnNumber)

Find the column specification for the given column number.
  Parameters: columnNumber - The column number, one based. Returns: The column specification or null if no column specification is defined for the given column number. 1 based.
### getColSpecElement

public [AuthorElement](../../../api/node/AuthorElement.md) getColSpecElement([CALSColSpec](CALSColSpec.md) colspec)

Find a column specification element.
  Parameters: colspec - The column specification. Returns: The column specification element or null if no column corresponds to the given specification.
### getColSpecs

public [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[CALSColSpec](CALSColSpec.md)> getColSpecs()

Returns the column specification set corresponding to the CALS table. The list is ordered ascending by the column specification index ('colnum' attribute).
  Returns: The column specifications set.
### hasColumnSpecifications

public boolean hasColumnSpecifications([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
 Description copied from interface: [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement))
This method tells if the table contains column specifications. For example the CALS table model requires colspec elements to be present.
  Specified by: [hasColumnSpecifications](../../../api/AuthorTableCellSpanProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) Parameters: tableElement - The [AuthorElement](../../../api/node/AuthorElement.md) that is rendered as a table. Returns: true if some column specification info is present or if the table doesn't require any column specification info. See Also:
        * [AuthorTableCellSpanProvider.hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../api/AuthorTableCellSpanProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement))

### getCellWidth

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WidthRepresentation](../../../api/WidthRepresentation.md)> getCellWidth([AuthorElement](../../../api/node/AuthorElement.md) cellElement, int colNumberStart, int colSpan)

The list with the width representations for the given cell is obtained by computing the column span and then determining the [WidthRepresentation](../../../api/WidthRepresentation.md)for each column the cell spans across.
  Specified by: [getCellWidth](../../../api/AuthorTableColumnWidthProvider.md#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: cellElement - The node that represents a table cell in CSS. colNumberStart - The column number the cell starts at. colSpan - The column span of the cell. Returns: The list with the [WidthRepresentation](../../../api/WidthRepresentation.md) of the specified cell element or null if the cell width cannot be computed. If the cell spans over multiple columns then the returned list will contain one [WidthRepresentation](../../../api/WidthRepresentation.md) for each column the cell spans over. See Also:
        * [AuthorTableColumnWidthProvider.getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement, int, int)](../../../api/AuthorTableColumnWidthProvider.md#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int))

### commitColumnWidthModifications

public void commitColumnWidthModifications([AuthorDocumentController](../../../api/AuthorDocumentController.md) authorDocumentController, [WidthRepresentation](../../../api/WidthRepresentation.md)[] colWidths, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Updates the columns width specifications in the source document by setting the colwidth attribute value of the colspec elements and by adding new colspecelements if needed.
  Specified by: [commitColumnWidthModifications](../../../api/AuthorTableColumnWidthProvider.md#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: authorDocumentController - The [AuthorDocumentController](../../../api/AuthorDocumentController.md) used to commit the table modifications in the document. colWidths - The new column [WidthRepresentation](../../../api/WidthRepresentation.md) to set. The column widths must be ordered according to the corresponding column numbers. tableCellsTagName - The cells tag name. Used to identify the table type (e.g. 'entry' for CALS or 'td' for HTML). Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - If the operation fails. See Also:
        * [AuthorTableColumnWidthProvider.commitColumnWidthModifications(AuthorDocumentController, ro.sync.ecss.extensions.api.WidthRepresentation[], java.lang.String)](../../../api/AuthorTableColumnWidthProvider.md#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String))

### isTableCell

protected boolean isTableCell([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)

Check if the name of an element is a table cell.
  Parameters: tableCellsTagName - The name of an element. Returns: true if the name of an element is a table cell.
### commitTableWidthModification

public void commitTableWidthModification([AuthorDocumentController](../../../api/AuthorDocumentController.md) authorDocumentController, int newTableWidth, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Sets the width attribute value of the table element.
  Specified by: [commitTableWidthModification](../../../api/AuthorTableColumnWidthProvider.md#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: authorDocumentController - The [AuthorDocumentController](../../../api/AuthorDocumentController.md) used to commit the table width modifications in the document. newTableWidth - The new table [WidthRepresentation](../../../api/WidthRepresentation.md) to set. The value is given in pixels. tableCellsTagName - The cells tag name. Used to identify the table type (e.g. 'entry' for CALS or 'td' for HTML). Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - If the operation fails. See Also:
        * [AuthorTableColumnWidthProvider.commitTableWidthModification(AuthorDocumentController, int, java.lang.String)](../../../api/AuthorTableColumnWidthProvider.md#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String))

### getTableWidth

public [WidthRepresentation](../../../api/WidthRepresentation.md) getTableWidth([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)

Returns the [WidthRepresentation](../../../api/WidthRepresentation.md) obtained by analyzing the width attribute value of the table element.
  Specified by: [getTableWidth](../../../api/AuthorTableColumnWidthProvider.md#getTableWidth(java.lang.String)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. 'entry' for CALS or 'td' for HTML). Returns: A non null value if the table width is specified. Otherwise null. See Also:
        * [AuthorTableColumnWidthProvider.getTableWidth(java.lang.String)](../../../api/AuthorTableColumnWidthProvider.md#getTableWidth(java.lang.String))

### isTableAcceptingWidth

public boolean isTableAcceptingWidth([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)

The DocBook CALS tables do not accept width specification.
  Specified by: [isTableAcceptingWidth](../../../api/AuthorTableColumnWidthProvider.md#isTableAcceptingWidth(java.lang.String)) in interface [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md) Parameters: tableCellsTagName - The cells tag name. Used to identify the table type (e.g. 'entry' for CALS or 'td' for HTML). Returns: true if the table type denoted by the tableCellsTagName accepts width specification of any kind. See Also:
        * [AuthorTableColumnWidthProvider.isTableAcceptingWidth(java.lang.String)](../../../api/AuthorTableColumnWidthProvider.md#isTableAcceptingWidth(java.lang.String))

### isTableAndColumnsResizable

public boolean isTableAndColumnsResizable([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)

It returns true only if the given table cells tag name is equal to 'entry'.
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

### getColSep

public boolean getColSep([AuthorElement](../../../api/node/AuthorElement.md) cellElem, int columnIndex)
 Description copied from interface: [AuthorTableCellSepProvider](../../../api/AuthorTableCellSepProvider.md#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))
Checks if a separator should be placed at the cell right. Note that if the cell is the last from its row, the separator is not painted even if this method returns true.
  Specified by: [getColSep](../../../api/AuthorTableCellSepProvider.md#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableCellSepProvider](../../../api/AuthorTableCellSepProvider.md) Parameters: cellElem - The node that represents a table cell in CSS. columnIndex - The index of the column, used to identify the colspec associated to the cell. The colspec can give information about the colsep. 1 based. Returns: true if a separator should be placed at its right, false otherwise. See Also:
        * [AuthorTableCellSepProvider.getColSep(ro.sync.ecss.extensions.api.node.AuthorElement, int)](../../../api/AuthorTableCellSepProvider.md#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))

### getRowSep

public boolean getRowSep([AuthorElement](../../../api/node/AuthorElement.md) cellElem, int columnIndex)
 Description copied from interface: [AuthorTableCellSepProvider](../../../api/AuthorTableCellSepProvider.md#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))
Checks if a separator should be placed at the cell bottom. Note that if the cell is on the last row, the separator is not painted even if this method returns true.
  Specified by: [getRowSep](../../../api/AuthorTableCellSepProvider.md#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableCellSepProvider](../../../api/AuthorTableCellSepProvider.md) Parameters: cellElem - The node that represents a table cell in CSS. columnIndex - The index of the column, used to identify the rowspec associated to the cell. The rowspec can give information about the colsep. 1 based. Returns: true if a separator should be placed at its right, false otherwise. See Also:
        * [AuthorTableCellSepProvider.getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement, int)](../../../api/AuthorTableCellSepProvider.md#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))

### isTableElement

protected boolean isTableElement([AuthorElement](../../../api/node/AuthorElement.md) element)

Check if this element is a table element.
  Parameters: element - The analyzed element. Returns: true if this element is a CALS table element.
### isTgroupElement

protected boolean isTgroupElement([AuthorElement](../../../api/node/AuthorElement.md) element)

Check if this element is a tgroup element.
  Parameters: element - The analyzed element. Returns: true if this element is a CALS tgroup element.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
