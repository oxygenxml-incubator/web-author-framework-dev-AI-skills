Package [ro.sync.ecss.extensions.commons.table.support](package-summary.md)

# Class DITACALSTableCellInfoProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
        * [ro.sync.ecss.extensions.commons.table.support.CALSTableCellInfoProvider](CALSTableCellInfoProvider.md)
            * ro.sync.ecss.extensions.commons.table.support.DITACALSTableCellInfoProvider
   All Implemented Interfaces: [AuthorTableCellSepProvider](../../../api/AuthorTableCellSepProvider.md), [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md), [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md), [Extension](../../../api/Extension.md), [CALSConstants](../operations/cals/CALSConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class DITACALSTableCellInfoProvider extends [CALSTableCellInfoProvider](CALSTableCellInfoProvider.md)
DITA CALS table cell info provider, should work with specializations.

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
 [DITACALSTableCellInfoProvider](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [isColspec](#isColspec(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) child)
Check if the child is a column specification.
  protected boolean [isTableCell](#isTableCell(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Check if the name of an element is a table cell.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.support.[CALSTableCellInfoProvider](CALSTableCellInfoProvider.md)
 [commitColumnWidthModifications](CALSTableCellInfoProvider.md#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String)), [commitTableWidthModification](CALSTableCellInfoProvider.md#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String)), [getAllColspecWidthRepresentations](CALSTableCellInfoProvider.md#getAllColspecWidthRepresentations()), [getCellSpanSpec](CALSTableCellInfoProvider.md#getCellSpanSpec(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement)), [getCellWidth](CALSTableCellInfoProvider.md#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getColSep](CALSTableCellInfoProvider.md#getColSep(ro.sync.ecss.extensions.api.node.AuthorElement,int)), [getColSpan](CALSTableCellInfoProvider.md#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement)), [getColSpanInterval](CALSTableCellInfoProvider.md#getColSpanInterval(ro.sync.ecss.extensions.api.node.AuthorElement)), [getColSpec](CALSTableCellInfoProvider.md#getColSpec(int)), [getColSpec](CALSTableCellInfoProvider.md#getColSpec(java.lang.String)), [getColSpecElement](CALSTableCellInfoProvider.md#getColSpecElement(ro.sync.ecss.extensions.commons.table.support.CALSColSpec)), [getColSpecs](CALSTableCellInfoProvider.md#getColSpecs()), [getDescription](CALSTableCellInfoProvider.md#getDescription()), [getRowSep](CALSTableCellInfoProvider.md#getRowSep(ro.sync.ecss.extensions.api.node.AuthorElement,int)), [getRowSpan](CALSTableCellInfoProvider.md#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTableWidth](CALSTableCellInfoProvider.md#getTableWidth(java.lang.String)), [hasColumnSpecifications](CALSTableCellInfoProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement)), [init](CALSTableCellInfoProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement)), [isAcceptingFixedColumnWidths](CALSTableCellInfoProvider.md#isAcceptingFixedColumnWidths(java.lang.String)), [isAcceptingPercentageColumnWidths](CALSTableCellInfoProvider.md#isAcceptingPercentageColumnWidths(java.lang.String)), [isAcceptingProportionalColumnWidths](CALSTableCellInfoProvider.md#isAcceptingProportionalColumnWidths(java.lang.String)), [isTableAcceptingWidth](CALSTableCellInfoProvider.md#isTableAcceptingWidth(java.lang.String)), [isTableAndColumnsResizable](CALSTableCellInfoProvider.md#isTableAndColumnsResizable(java.lang.String)), [isTableElement](CALSTableCellInfoProvider.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTgroupElement](CALSTableCellInfoProvider.md#isTgroupElement(ro.sync.ecss.extensions.api.node.AuthorElement))
### Methods inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
 [getErrorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#getErrorsListener()), [isPreferPercentageColumnWidths](../../../api/AuthorTableColumnWidthProviderBase.md#isPreferPercentageColumnWidths(java.lang.String)), [setErrorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#setErrorsListener(ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutErrorsListener))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITACALSTableCellInfoProvider

public DITACALSTableCellInfoProvider()

## Method Details

### isTableCell

protected boolean isTableCell([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
 Description copied from class: [CALSTableCellInfoProvider](CALSTableCellInfoProvider.md#isTableCell(java.lang.String))
Check if the name of an element is a table cell.
  Overrides: [isTableCell](CALSTableCellInfoProvider.md#isTableCell(java.lang.String)) in class [CALSTableCellInfoProvider](CALSTableCellInfoProvider.md) Parameters: tableCellsTagName - The name of an element. Returns: true if the name of an element is a table cell. See Also:
        * [CALSTableCellInfoProvider.isTableCell(java.lang.String)](CALSTableCellInfoProvider.md#isTableCell(java.lang.String))

### isColspec

protected boolean isColspec([AuthorElement](../../../api/node/AuthorElement.md) child)
 Description copied from class: [CALSTableCellInfoProvider](CALSTableCellInfoProvider.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorElement))
Check if the child is a column specification.
  Overrides: [isColspec](CALSTableCellInfoProvider.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [CALSTableCellInfoProvider](CALSTableCellInfoProvider.md) Parameters: child - The child Returns: true if the child is a column specification. See Also:
        * [CALSTableCellInfoProvider.isColspec(ro.sync.ecss.extensions.api.node.AuthorElement)](CALSTableCellInfoProvider.md#isColspec(ro.sync.ecss.extensions.api.node.AuthorElement))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
