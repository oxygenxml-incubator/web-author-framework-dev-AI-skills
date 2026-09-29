Package [ro.sync.ecss.extensions.commons.table.operations.xhtml](package-summary.md)

# Class ECXHTMLTableCustomizerInvoker

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.TableCustomizer](../TableCustomizer.md)
        * ro.sync.ecss.extensions.commons.table.operations.xhtml.ECXHTMLTableCustomizerInvoker
   @API(type=INTERNAL, src=PUBLIC) public final class ECXHTMLTableCustomizerInvoker extends [TableCustomizer](../TableCustomizer.md)
Customize a XHTML table for Eclipse application.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[TableCustomizer](../TableCustomizer.md)
 [tableInfo](../TableCustomizer.md#tableInfo)
## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static [ECXHTMLTableCustomizerInvoker](ECXHTMLTableCustomizerInvoker.md) [getInstance](#getInstance())()
Get the singleton instance.
  protected [TableInfo](../TableInfo.md) [showCustomizeTableDialog](#showCustomizeTableDialog(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, int predefinedRowsCount, int predefinedColumnsCount, int defaultTableModel)
Show table customizer dialog and return new table information.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[TableCustomizer](../TableCustomizer.md)
 [customizeTable](../TableCustomizer.md#customizeTable(ro.sync.ecss.extensions.api.AuthorAccess)), [customizeTable](../TableCustomizer.md#customizeTable(ro.sync.ecss.extensions.api.AuthorAccess,int,int)), [customizeTable](../TableCustomizer.md#customizeTable(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### getInstance

public static [ECXHTMLTableCustomizerInvoker](ECXHTMLTableCustomizerInvoker.md) getInstance()

Get the singleton instance.
  Returns: The singleton instance.
### showCustomizeTableDialog

protected [TableInfo](../TableInfo.md) showCustomizeTableDialog([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, int predefinedRowsCount, int predefinedColumnsCount, int defaultTableModel)
 Description copied from class: [TableCustomizer](../TableCustomizer.md#showCustomizeTableDialog(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int))
Show table customizer dialog and return new table information.
  Specified by: [showCustomizeTableDialog](../TableCustomizer.md#showCustomizeTableDialog(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int)) in class [TableCustomizer](../TableCustomizer.md) Parameters: authorAccess - The Author access. predefinedRowsCount - Predefined number of rows. predefinedColumnsCount - Predefined number of columns. defaultTableModel - The default model of the table that will be inserted. Returns: The table information provided by the user or null if customization operation is canceled. See Also:
        * [TableCustomizer.showCustomizeTableDialog(ro.sync.ecss.extensions.api.AuthorAccess, int, int, int)](../TableCustomizer.md#showCustomizeTableDialog(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
