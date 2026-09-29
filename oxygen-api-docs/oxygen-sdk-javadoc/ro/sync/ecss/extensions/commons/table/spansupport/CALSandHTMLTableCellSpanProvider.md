Package [ro.sync.ecss.extensions.commons.table.spansupport](package-summary.md)

# Class CALSandHTMLTableCellSpanProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
        * [ro.sync.ecss.extensions.commons.table.support.CALSandHTMLTableCellInfoProvider](../support/CALSandHTMLTableCellInfoProvider.md)
            * ro.sync.ecss.extensions.commons.table.spansupport.CALSandHTMLTableCellSpanProvider
   All Implemented Interfaces: [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md), [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md), [Extension](../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class CALSandHTMLTableCellSpanProvider extends [CALSandHTMLTableCellInfoProvider](../support/CALSandHTMLTableCellInfoProvider.md)
Empty implementation for backward compatibility . A table cell span info provider used for frameworks that have both CALS and HTML tables.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
 [errorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#errorsListener)
## Constructor Summary
 Constructors
Constructor

Description
 [CALSandHTMLTableCellSpanProvider](#%3Cinit%3E())()

## Method Summary

### Methods inherited from class ro.sync.ecss.extensions.commons.table.support.[CALSandHTMLTableCellInfoProvider](../support/CALSandHTMLTableCellInfoProvider.md)
 [commitColumnWidthModifications](../support/CALSandHTMLTableCellInfoProvider.md#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String)), [commitTableWidthModification](../support/CALSandHTMLTableCellInfoProvider.md#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String)), [getAllColspecWidthRepresentations](../support/CALSandHTMLTableCellInfoProvider.md#getAllColspecWidthRepresentations()), [getCALSTableCellSpanProvider](../support/CALSandHTMLTableCellInfoProvider.md#getCALSTableCellSpanProvider()), [getCellWidth](../support/CALSandHTMLTableCellInfoProvider.md#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getColSpan](../support/CALSandHTMLTableCellInfoProvider.md#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement)), [getDescription](../support/CALSandHTMLTableCellInfoProvider.md#getDescription()), [getRowSpan](../support/CALSandHTMLTableCellInfoProvider.md#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTableWidth](../support/CALSandHTMLTableCellInfoProvider.md#getTableWidth(java.lang.String)), [getXHTMLTableCellSpanProvider](../support/CALSandHTMLTableCellInfoProvider.md#getXHTMLTableCellSpanProvider()), [hasColumnSpecifications](../support/CALSandHTMLTableCellInfoProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement)), [init](../support/CALSandHTMLTableCellInfoProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement)), [isAcceptingFixedColumnWidths](../support/CALSandHTMLTableCellInfoProvider.md#isAcceptingFixedColumnWidths(java.lang.String)), [isAcceptingPercentageColumnWidths](../support/CALSandHTMLTableCellInfoProvider.md#isAcceptingPercentageColumnWidths(java.lang.String)), [isAcceptingProportionalColumnWidths](../support/CALSandHTMLTableCellInfoProvider.md#isAcceptingProportionalColumnWidths(java.lang.String)), [isPreferPercentageColumnWidths](../support/CALSandHTMLTableCellInfoProvider.md#isPreferPercentageColumnWidths(java.lang.String)), [isTableAcceptingWidth](../support/CALSandHTMLTableCellInfoProvider.md#isTableAcceptingWidth(java.lang.String)), [isTableAndColumnsResizable](../support/CALSandHTMLTableCellInfoProvider.md#isTableAndColumnsResizable(java.lang.String))
### Methods inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
 [getErrorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#getErrorsListener()), [setErrorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#setErrorsListener(ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutErrorsListener))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CALSandHTMLTableCellSpanProvider

public CALSandHTMLTableCellSpanProvider()

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
