Package [ro.sync.ecss.extensions.commons.table.spansupport](package-summary.md)

# Class HTMLTableCellSpanProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
        * [ro.sync.ecss.extensions.commons.table.support.HTMLTableCellInfoProvider](../support/HTMLTableCellInfoProvider.md)
            * ro.sync.ecss.extensions.commons.table.spansupport.HTMLTableCellSpanProvider
   All Implemented Interfaces: [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md), [AuthorTableColumnWidthProvider](../../../api/AuthorTableColumnWidthProvider.md), [Extension](../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class HTMLTableCellSpanProvider extends [HTMLTableCellInfoProvider](../support/HTMLTableCellInfoProvider.md)
Empty implementation for backward compatibility. The HTML table cell span and column width provider.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.support.[HTMLTableCellInfoProvider](../support/HTMLTableCellInfoProvider.md)
 [ATTR_NAME_SPAN](../support/HTMLTableCellInfoProvider.md#ATTR_NAME_SPAN)
### Fields inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
 [errorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#errorsListener)
## Constructor Summary
 Constructors
Constructor

Description
 [HTMLTableCellSpanProvider](#%3Cinit%3E())()

## Method Summary

### Methods inherited from class ro.sync.ecss.extensions.commons.table.support.[HTMLTableCellInfoProvider](../support/HTMLTableCellInfoProvider.md)
 [commitColumnWidthModifications](../support/HTMLTableCellInfoProvider.md#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String)), [commitTableWidthModification](../support/HTMLTableCellInfoProvider.md#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String)), [getAllColspecWidthRepresentations](../support/HTMLTableCellInfoProvider.md#getAllColspecWidthRepresentations()), [getCellWidth](../support/HTMLTableCellInfoProvider.md#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getColSpan](../support/HTMLTableCellInfoProvider.md#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement)), [getColSpec](../support/HTMLTableCellInfoProvider.md#getColSpec(int)), [getDescription](../support/HTMLTableCellInfoProvider.md#getDescription()), [getRowSpan](../support/HTMLTableCellInfoProvider.md#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement)), [getTableWidth](../support/HTMLTableCellInfoProvider.md#getTableWidth(java.lang.String)), [hasColumnSpecifications](../support/HTMLTableCellInfoProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement)), [init](../support/HTMLTableCellInfoProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement)), [isAcceptingFixedColumnWidths](../support/HTMLTableCellInfoProvider.md#isAcceptingFixedColumnWidths(java.lang.String)), [isAcceptingPercentageColumnWidths](../support/HTMLTableCellInfoProvider.md#isAcceptingPercentageColumnWidths(java.lang.String)), [isAcceptingProportionalColumnWidths](../support/HTMLTableCellInfoProvider.md#isAcceptingProportionalColumnWidths(java.lang.String)), [isHTMLTableCellTagName](../support/HTMLTableCellInfoProvider.md#isHTMLTableCellTagName(java.lang.String)), [isPreferPercentageColumnWidths](../support/HTMLTableCellInfoProvider.md#isPreferPercentageColumnWidths(java.lang.String)), [isTableAcceptingWidth](../support/HTMLTableCellInfoProvider.md#isTableAcceptingWidth(java.lang.String)), [isTableAndColumnsResizable](../support/HTMLTableCellInfoProvider.md#isTableAndColumnsResizable(java.lang.String))
### Methods inherited from class ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../../api/AuthorTableColumnWidthProviderBase.md)
 [getErrorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#getErrorsListener()), [setErrorsListener](../../../api/AuthorTableColumnWidthProviderBase.md#setErrorsListener(ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutErrorsListener))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### HTMLTableCellSpanProvider

public HTMLTableCellSpanProvider()

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
