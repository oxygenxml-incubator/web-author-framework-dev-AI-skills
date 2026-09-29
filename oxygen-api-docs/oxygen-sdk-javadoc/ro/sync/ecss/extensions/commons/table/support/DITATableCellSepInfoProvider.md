Package [ro.sync.ecss.extensions.commons.table.support](package-summary.md)

# Class DITATableCellSepInfoProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
        * [ro.sync.ecss.extensions.commons.table.support.CALSTableCellInfoProvider](CALSTableCellInfoProvider.md)
            * ro.sync.ecss.extensions.commons.table.support.DITATableCellSepInfoProvider
   All Implemented Interfaces: [AuthorTableCellSepProvider](../../../api/AuthorTableCellSepProvider.md), [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md), [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md), [Extension](../../../api/Extension.md), [CALSConstants](../operations/cals/CALSConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class DITATableCellSepInfoProvider extends [CALSTableCellInfoProvider](CALSTableCellInfoProvider.md)
A DITA cell separators provider. The same as a CALS one, but also knows about the simple table.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.support.[CALSTableCellInfoProvider](CALSTableCellInfoProvider.md)
 [DEFAULT_WIDTH_REPRESENTATION](CALSTableCellInfoProvider.md#DEFAULT_WIDTH_REPRESENTATION), [spanspecInfos](CALSTableCellInfoProvider.md#spanspecInfos)
### Fields inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
 [errorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#errorsListener)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](../operations/cals/CALSConstants.md)
 [ATTRIBUTE_NAME_ALIGN](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ALIGN), [ATTRIBUTE_NAME_COLNAME](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLNAME), [ATTRIBUTE_NAME_COLNUM](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLNUM), [ATTRIBUTE_NAME_COLS](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_COLSEP](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLSEP), [ATTRIBUTE_NAME_COLWIDTH](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_COLWIDTH), [ATTRIBUTE_NAME_ID](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_MOREROWS](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_MOREROWS), [ATTRIBUTE_NAME_NAMEEND](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_NAMEEND), [ATTRIBUTE_NAME_NAMEST](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_NAMEST), [ATTRIBUTE_NAME_ROWSEP](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_ROWSEP), [ATTRIBUTE_NAME_SPANNAME](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_SPANNAME), [ATTRIBUTE_NAME_TABLE_WIDTH](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_TABLE_WIDTH), [ATTRIBUTE_NAME_XML_ID](../operations/cals/CALSConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_COLSPEC](../operations/cals/CALSConstants.md#ELEMENT_NAME_COLSPEC), [ELEMENT_NAME_ENTRY](../operations/cals/CALSConstants.md#ELEMENT_NAME_ENTRY), [ELEMENT_NAME_INFORMALTABLE](../operations/cals/CALSConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_ROW](../operations/cals/CALSConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_SPANSPEC](../operations/cals/CALSConstants.md#ELEMENT_NAME_SPANSPEC), [ELEMENT_NAME_TABLE](../operations/cals/CALSConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TGROUP](../operations/cals/CALSConstants.md#ELEMENT_NAME_TGROUP)
## Constructor Summary
 Constructors
Constructor

Description
 [DITATableCellSepInfoProvider](#%3Cinit%3E())()
The default in DITA is not to present the separators.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [getColSep](#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../api/node/AuthorElement.md) cellElement, int columnIndex)
Special case for the topic/simpletable.
  boolean [getRowSep](#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../api/node/AuthorElement.md) cellElement, int columnIndex)
Special case for the topic/simpletable.
  protected boolean [isTableElement](#isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) element)
Check if this element is a table element.
  protected boolean [isTgroupElement](#isTgroupElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) element)
Check if this element is a tgroup element.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.support.[CALSTableCellInfoProvider](CALSTableCellInfoProvider.md)
 [commitColumnWidthModifications](CALSTableCellInfoProvider.md#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String)), [commitTableWidthModification](CALSTableCellInfoProvider.md#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String)), [getAllColspecWidthRepresentations](CALSTableCellInfoProvider.md#getAllColspecWidthRepresentations()), [getCellSpanSpec](CALSTableCellInfoProvider.md#getCellSpanSpec(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement)), [getCellWidth](CALSTableCellInfoProvider.md#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getColSpan](CALSTableCellInfoProvider.md#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement)), [getColSpanInterval](CALSTableCellInfoProvider.md#getColSpanInterval(ro.sync.ecss.extensions.api.node.AuthorElement)), [getColSpec](CALSTableCellInfoProvider.md#getColSpec(int)), [getColSpec](CALSTableCellInfoProvider.md#getColSpec(java.lang.String)), [getColSpecElement](CALSTableCellInfoProvider.md#getColSpecElement(ro.sync.ecss.extensions.commons.table.support.CALSColSpec)), [getColSpecs](CALSTableCellInfoProvider.md#getColSpecs()), [getDescription](CALSTableCellInfoProvider.md#getDescription()), [getRowSpan](CALSTableCellInfoProvider.md#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTableWidth](CALSTableCellInfoProvider.md#getTableWidth(java.lang.String)), [hasColumnSpecifications](CALSTableCellInfoProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement)), [init](CALSTableCellInfoProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement)), [isAcceptingFixedColumnWidths](CALSTableCellInfoProvider.md#isAcceptingFixedColumnWidths(java.lang.String)), [isAcceptingPercentageColumnWidths](CALSTableCellInfoProvider.md#isAcceptingPercentageColumnWidths(java.lang.String)), [isAcceptingProportionalColumnWidths](CALSTableCellInfoProvider.md#isAcceptingProportionalColumnWidths(java.lang.String)), [isColspec](CALSTableCellInfoProvider.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableAcceptingWidth](CALSTableCellInfoProvider.md#isTableAcceptingWidth(java.lang.String)), [isTableAndColumnsResizable](CALSTableCellInfoProvider.md#isTableAndColumnsResizable(java.lang.String)), [isTableCell](CALSTableCellInfoProvider.md#isTableCell(java.lang.String))
### Methods inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
 [getErrorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#getErrorsListener()), [isPreferPercentageColumnWidths](../../../api/AuthorTableColumnWidthProviderBase.md#isPreferPercentageColumnWidths(java.lang.String)), [setErrorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#setErrorsListener(ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutErrorsListener))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITATableCellSepInfoProvider

public DITATableCellSepInfoProvider()

The default in DITA is not to present the separators.

## Method Details

### getColSep

public boolean getColSep([AuthorElement](../../../api/node/AuthorElement.md) cellElement, int columnIndex)

Special case for the topic/simpletable. Always return true for them.
  Specified by: [getColSep](../../../api/AuthorTableCellSepProvider.md#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableCellSepProvider](../../../api/AuthorTableCellSepProvider.md) Overrides: [getColSep](CALSTableCellInfoProvider.md#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in class [CALSTableCellInfoProvider](CALSTableCellInfoProvider.md) Parameters: cellElement - The node that represents a table cell in CSS. columnIndex - The index of the column, used to identify the colspec associated to the cell. The colspec can give information about the colsep. 1 based. Returns: true if a separator should be placed at its right, false otherwise. See Also:
        * [AuthorTableCellSepProvider.getColSep(ro.sync.ecss.extensions.api.node.AuthorElement, int)](../../../api/AuthorTableCellSepProvider.md#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))

### getRowSep

public boolean getRowSep([AuthorElement](../../../api/node/AuthorElement.md) cellElement, int columnIndex)

Special case for the topic/simpletable. Always return true for them.
  Specified by: [getRowSep](../../../api/AuthorTableCellSepProvider.md#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [AuthorTableCellSepProvider](../../../api/AuthorTableCellSepProvider.md) Overrides: [getRowSep](CALSTableCellInfoProvider.md#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in class [CALSTableCellInfoProvider](CALSTableCellInfoProvider.md) Parameters: cellElement - The node that represents a table cell in CSS. columnIndex - The index of the column, used to identify the rowspec associated to the cell. The rowspec can give information about the colsep. 1 based. Returns: true if a separator should be placed at its right, false otherwise. See Also:
        * [AuthorTableCellSepProvider.getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement, int)](../../../api/AuthorTableCellSepProvider.md#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int))

### isTableElement

protected boolean isTableElement([AuthorElement](../../../api/node/AuthorElement.md) element)
 Description copied from class: [CALSTableCellInfoProvider](CALSTableCellInfoProvider.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement))
Check if this element is a table element.
  Overrides: [isTableElement](CALSTableCellInfoProvider.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [CALSTableCellInfoProvider](CALSTableCellInfoProvider.md) Parameters: element - The analyzed element. Returns: true if this element is a CALS table element. See Also:
        * [CALSTableCellInfoProvider.isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement)](CALSTableCellInfoProvider.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTgroupElement

protected boolean isTgroupElement([AuthorElement](../../../api/node/AuthorElement.md) element)
 Description copied from class: [CALSTableCellInfoProvider](CALSTableCellInfoProvider.md#isTgroupElement(ro.sync.ecss.extensions.api.node.AuthorElement))
Check if this element is a tgroup element.
  Overrides: [isTgroupElement](CALSTableCellInfoProvider.md#isTgroupElement(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [CALSTableCellInfoProvider](CALSTableCellInfoProvider.md) Parameters: element - The analyzed element. Returns: true if this element is a CALS tgroup element. See Also:
        * [CALSTableCellInfoProvider.isTgroupElement(ro.sync.ecss.extensions.api.node.AuthorElement)](CALSTableCellInfoProvider.md#isTgroupElement(ro.sync.ecss.extensions.api.node.AuthorElement))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
