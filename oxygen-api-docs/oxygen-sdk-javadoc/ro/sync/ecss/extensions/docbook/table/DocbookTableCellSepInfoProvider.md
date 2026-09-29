Package [ro.sync.ecss.extensions.docbook.table](package-summary.md)

# Class DocbookTableCellSepInfoProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorTableColumnWidthProviderBase](../../api/AuthorTableColumnWidthProviderBase.md)
        * [ro.sync.ecss.extensions.commons.table.support.CALSTableCellInfoProvider](../../commons/table/support/CALSTableCellInfoProvider.md)
            * ro.sync.ecss.extensions.docbook.table.DocbookTableCellSepInfoProvider
   All Implemented Interfaces: [AuthorTableCellSepProvider](../../api/AuthorTableCellSepProvider.md), [AuthorTableCellSpanProvider](../../api/AuthorTableCellSpanProvider.md), [AuthorTableColumnWidthProvider](../../api/AuthorTableColumnWidthProvider.md), [Extension](../../api/Extension.md), [CALSConstants](../../commons/table/operations/cals/CALSConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class DocbookTableCellSepInfoProvider extends [CALSTableCellInfoProvider](../../commons/table/support/CALSTableCellInfoProvider.md)
A DITA cell separators provider. The same as a CALS one, but also knows about the simple table.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.support.[CALSTableCellInfoProvider](../../commons/table/support/CALSTableCellInfoProvider.md)
 [DEFAULT_WIDTH_REPRESENTATION](../../commons/table/support/CALSTableCellInfoProvider.md#DEFAULT_WIDTH_REPRESENTATION), [spanspecInfos](../../commons/table/support/CALSTableCellInfoProvider.md#spanspecInfos)
### Fields inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../api/AuthorTableColumnWidthProviderBase.md)
 [errorsListener](../../api/AuthorTableColumnWidthProviderBase.md#errorsListener)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](../../commons/table/operations/cals/CALSConstants.md)
 [ATTRIBUTE_NAME_ALIGN](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ALIGN), [ATTRIBUTE_NAME_COLNAME](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLNAME), [ATTRIBUTE_NAME_COLNUM](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLNUM), [ATTRIBUTE_NAME_COLS](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_COLSEP](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLSEP), [ATTRIBUTE_NAME_COLWIDTH](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLWIDTH), [ATTRIBUTE_NAME_ID](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_MOREROWS](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_MOREROWS), [ATTRIBUTE_NAME_NAMEEND](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_NAMEEND), [ATTRIBUTE_NAME_NAMEST](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_NAMEST), [ATTRIBUTE_NAME_ROWSEP](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ROWSEP), [ATTRIBUTE_NAME_SPANNAME](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_SPANNAME), [ATTRIBUTE_NAME_TABLE_WIDTH](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_TABLE_WIDTH), [ATTRIBUTE_NAME_XML_ID](../../commons/table/operations/cals/CALSConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_COLSPEC](../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_COLSPEC), [ELEMENT_NAME_ENTRY](../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_ENTRY), [ELEMENT_NAME_INFORMALTABLE](../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_ROW](../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_SPANSPEC](../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_SPANSPEC), [ELEMENT_NAME_TABLE](../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TGROUP](../../commons/table/operations/cals/CALSConstants.md#ELEMENT_NAME_TGROUP)
## Constructor Summary
 Constructors
Constructor

Description
 [DocbookTableCellSepInfoProvider](#%3Cinit%3E())()
The default in DITA is not to present the separators.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [getColSep](#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../api/node/AuthorElement.md) cellElement, int columnIndex)
Special case for the topic/simpletable.
  boolean [getRowSep](#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../api/node/AuthorElement.md) cellElement, int columnIndex)
Special case for the topic/simpletable.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.support.[CALSTableCellInfoProvider](../../commons/table/support/CALSTableCellInfoProvider.md)
 [commitColumnWidthModifications](../../commons/table/support/CALSTableCellInfoProvider.md#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String)), [commitTableWidthModification](../../commons/table/support/CALSTableCellInfoProvider.md#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String)), [getAllColspecWidthRepresentations](../../commons/table/support/CALSTableCellInfoProvider.md#getAllColspecWidthRepresentations()), [getCellSpanSpec](../../commons/table/support/CALSTableCellInfoProvider.md#getCellSpanSpec(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement)), [getCellWidth](../../commons/table/support/CALSTableCellInfoProvider.md#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getColSpan](../../commons/table/support/CALSTableCellInfoProvider.md#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement)), [getColSpanInterval](../../commons/table/support/CALSTableCellInfoProvider.md#getColSpanInterval(ro.sync.ecss.extensions.api.node.AuthorElement)), [getColSpec](../../commons/table/support/CALSTableCellInfoProvider.md#getColSpec(int)), [getColSpec](../../commons/table/support/CALSTableCellInfoProvider.md#getColSpec(java.lang.String)), [getColSpecElement](../../commons/table/support/CALSTableCellInfoProvider.md#getColSpecElement(ro.sync.ecss.extensions.commons.table.support.CALSColSpec)), [getColSpecs](../../commons/table/support/CALSTableCellInfoProvider.md#getColSpecs()), [getDescription](../../commons/table/support/CALSTableCellInfoProvider.md#getDescription()), [getRowSpan](../../commons/table/support/CALSTableCellInfoProvider.md#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTableWidth](../../commons/table/support/CALSTableCellInfoProvider.md#getTableWidth(java.lang.String)), [hasColumnSpecifications](../../commons/table/support/CALSTableCellInfoProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement)), [init](../../commons/table/support/CALSTableCellInfoProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement)), [isAcceptingFixedColumnWidths](../../commons/table/support/CALSTableCellInfoProvider.md#isAcceptingFixedColumnWidths(java.lang.String)), [isAcceptingPercentageColumnWidths](../../commons/table/support/CALSTableCellInfoProvider.md#isAcceptingPercentageColumnWidths(java.lang.String)), [isAcceptingProportionalColumnWidths](../../commons/table/support/CALSTableCellInfoProvider.md#isAcceptingProportionalColumnWidths(java.lang.String)), [isColspec](../../commons/table/support/CALSTableCellInfoProvider.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableAcceptingWidth](../../commons/table/support/CALSTableCellInfoProvider.md#isTableAcceptingWidth(java.lang.String)), [isTableAndColumnsResizable](../../commons/table/support/CALSTableCellInfoProvider.md#isTableAndColumnsResizable(java.lang.String)), [isTableCell](../../commons/table/support/CALSTableCellInfoProvider.md#isTableCell(java.lang.String)), [isTableElement](../../commons/table/support/CALSTableCellInfoProvider.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTgroupElement](../../commons/table/support/CALSTableCellInfoProvider.md#isTgroupElement(ro.sync.ecss.extensions.api.node.AuthorElement))
### Methods inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../api/AuthorTableColumnWidthProviderBase.md)
 [getErrorsListener](../../api/AuthorTableColumnWidthProviderBase.md#getErrorsListener()), [isPreferPercentageColumnWidths](../../api/AuthorTableColumnWidthProviderBase.md#isPreferPercentageColumnWidths(java.lang.String)), [setErrorsListener](../../api/AuthorTableColumnWidthProviderBase.md#setErrorsListener(ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutErrorsListener))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DocbookTableCellSepInfoProvider

public DocbookTableCellSepInfoProvider()

The default in DITA is not to present the separators.

## Method Details

### getColSep

public boolean getColSep([AuthorElement](../../api/node/AuthorElement.md) cellElement, int columnIndex)

Special case for the topic/simpletable. Always return true for them.
  Specified by: [getColSep](../../api/AuthorTableCellSepProvider.md#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableCellSepProvider](../../api/AuthorTableCellSepProvider.md) Overrides: [getColSep](../../commons/table/support/CALSTableCellInfoProvider.md#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in class [CALSTableCellInfoProvider](../../commons/table/support/CALSTableCellInfoProvider.md) Parameters: cellElement - The node that represents a table cell in CSS. columnIndex - The index of the column, used to identify the colspec associated to the cell. The colspec can give information about the colsep. 1 based. Returns: true if a separator should be placed at its right, false otherwise. See Also:
        * [AuthorTableCellSepProvider.getColSep(ro.sync.ecss.extensions.api.node.AuthorElement, int)](../../api/AuthorTableCellSepProvider.md#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))

### getRowSep

public boolean getRowSep([AuthorElement](../../api/node/AuthorElement.md) cellElement, int columnIndex)

Special case for the topic/simpletable. Always return true for them.
  Specified by: [getRowSep](../../api/AuthorTableCellSepProvider.md#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableCellSepProvider](../../api/AuthorTableCellSepProvider.md) Overrides: [getRowSep](../../commons/table/support/CALSTableCellInfoProvider.md#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in class [CALSTableCellInfoProvider](../../commons/table/support/CALSTableCellInfoProvider.md) Parameters: cellElement - The node that represents a table cell in CSS. columnIndex - The index of the column, used to identify the rowspec associated to the cell. The rowspec can give information about the colsep. 1 based. Returns: true if a separator should be placed at its right, false otherwise. See Also:
        * [AuthorTableCellSepProvider.getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement, int)](../../api/AuthorTableCellSepProvider.md#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
