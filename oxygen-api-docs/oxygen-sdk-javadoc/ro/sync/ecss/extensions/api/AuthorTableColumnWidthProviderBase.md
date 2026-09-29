Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorTableColumnWidthProviderBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorTableColumnWidthProviderBase
   All Implemented Interfaces: [AuthorTableColumnWidthProvider](AuthorTableColumnWidthProvider.md), [Extension](Extension.md)   Direct Known Subclasses: [CALSandHTMLTableCellInfoProvider](../commons/table/support/CALSandHTMLTableCellInfoProvider.md), [CALSTableCellInfoProvider](../commons/table/support/CALSTableCellInfoProvider.md), [DITATableCellInfoProvider](../commons/table/support/DITATableCellInfoProvider.md), [HTMLTableCellInfoProvider](../commons/table/support/HTMLTableCellInfoProvider.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorTableColumnWidthProviderBase extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorTableColumnWidthProvider](AuthorTableColumnWidthProvider.md)
This is an interface for classes which are responsible for providing information and handling modifications regarding table and column widths. It should be implemented when the author extension being developed offers support for editing data in tabular form.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [TableLayoutErrorsListener](../commons/table/support/errorscanner/TableLayoutErrorsListener.md) [errorsListener](#errorsListener)
Table layout errors listener.

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorTableColumnWidthProviderBase](#%3Cinit%3E())()
Constructor
  [AuthorTableColumnWidthProviderBase](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutErrorsListener))([TableLayoutErrorsListener](../commons/table/support/errorscanner/TableLayoutErrorsListener.md) errorsListener)
Constructor

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WidthRepresentation](WidthRepresentation.md)> [getAllColspecWidthRepresentations](#getAllColspecWidthRepresentations())()
Get all with representations defined in all colspecs.
  [TableLayoutErrorsListener](../commons/table/support/errorscanner/TableLayoutErrorsListener.md) [getErrorsListener](#getErrorsListener())()
Get table layout error listener
  boolean [isPreferPercentageColumnWidths](#isPreferPercentageColumnWidths(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)
Check if percentage column widths are preferred.
  void [setErrorsListener](#setErrorsListener(ro.sync.ecss.extensions.commons.table.support.errorscanner.TableLayoutErrorsListener))([TableLayoutErrorsListener](../commons/table/support/errorscanner/TableLayoutErrorsListener.md) errorsListener)
Set a table layout error listener.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProvider](AuthorTableColumnWidthProvider.md)
 [commitColumnWidthModifications](AuthorTableColumnWidthProvider.md#commitColumnWidthModifications(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.WidthRepresentation%5B%5D,java.lang.String)), [commitTableWidthModification](AuthorTableColumnWidthProvider.md#commitTableWidthModification(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.lang.String)), [getCellWidth](AuthorTableColumnWidthProvider.md#getCellWidth(ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getTableWidth](AuthorTableColumnWidthProvider.md#getTableWidth(java.lang.String)), [init](AuthorTableColumnWidthProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement)), [isAcceptingFixedColumnWidths](AuthorTableColumnWidthProvider.md#isAcceptingFixedColumnWidths(java.lang.String)), [isAcceptingPercentageColumnWidths](AuthorTableColumnWidthProvider.md#isAcceptingPercentageColumnWidths(java.lang.String)), [isAcceptingProportionalColumnWidths](AuthorTableColumnWidthProvider.md#isAcceptingProportionalColumnWidths(java.lang.String)), [isTableAcceptingWidth](AuthorTableColumnWidthProvider.md#isTableAcceptingWidth(java.lang.String)), [isTableAndColumnsResizable](AuthorTableColumnWidthProvider.md#isTableAndColumnsResizable(java.lang.String))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Field Details

### errorsListener

protected [TableLayoutErrorsListener](../commons/table/support/errorscanner/TableLayoutErrorsListener.md) errorsListener

Table layout errors listener.

## Constructor Details

### AuthorTableColumnWidthProviderBase

public AuthorTableColumnWidthProviderBase()

Constructor

### AuthorTableColumnWidthProviderBase

public AuthorTableColumnWidthProviderBase([TableLayoutErrorsListener](../commons/table/support/errorscanner/TableLayoutErrorsListener.md) errorsListener)

Constructor
  Parameters: errorsListener - Table layout errors listener Since: 18
## Method Details

### setErrorsListener

public void setErrorsListener([TableLayoutErrorsListener](../commons/table/support/errorscanner/TableLayoutErrorsListener.md) errorsListener)

Set a table layout error listener.
  Parameters: errorsListener - The table layout errors listener. Since: 18
### getAllColspecWidthRepresentations

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WidthRepresentation](WidthRepresentation.md)> getAllColspecWidthRepresentations()

Get all with representations defined in all colspecs. If a colspec does not specify a width, it is supposed to be 1\*. If the table group specifies more columns than colspecs, those widths are supposed to be 1\*.
  Returns: All width representations from the defined colspecs.
### getErrorsListener

public [TableLayoutErrorsListener](../commons/table/support/errorscanner/TableLayoutErrorsListener.md) getErrorsListener()

Get table layout error listener
  Returns: Returns the table layout errors listener .
### isPreferPercentageColumnWidths

public boolean isPreferPercentageColumnWidths([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tableCellsTagName)

Check if percentage column widths are preferred.
  Parameters: tableCellsTagName - The cell tag name Returns: false by default. Since: 20
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
