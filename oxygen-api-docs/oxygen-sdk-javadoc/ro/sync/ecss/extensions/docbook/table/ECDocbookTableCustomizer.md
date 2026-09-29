Package [ro.sync.ecss.extensions.docbook.table](package-summary.md)

# Class ECDocbookTableCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.TableCustomizer](../../commons/table/operations/TableCustomizer.md)
        * ro.sync.ecss.extensions.docbook.table.ECDocbookTableCustomizer
   @API(type=INTERNAL, src=PUBLIC) public final class ECDocbookTableCustomizer extends [TableCustomizer](../../commons/table/operations/TableCustomizer.md)
Customize a Docbook table. It is used on Eclipse platform implementation.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[TableCustomizer](../../commons/table/operations/TableCustomizer.md)
 [tableInfo](../../commons/table/operations/TableCustomizer.md#tableInfo)
## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static [ECDocbookTableCustomizer](ECDocbookTableCustomizer.md) [getInstance](#getInstance())()
Get the singleton instance.
  protected [TableInfo](../../commons/table/operations/TableInfo.md) [showCustomizeTableDialog](#showCustomizeTableDialog(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, int predefinedRowsCount, int predefinedColumnsCount, int defaultTableModel)
Show table customizer dialog and return new table information.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[TableCustomizer](../../commons/table/operations/TableCustomizer.md)
 [customizeTable](../../commons/table/operations/TableCustomizer.md#customizeTable(ro.sync.ecss.extensions.api.AuthorAccess)), [customizeTable](../../commons/table/operations/TableCustomizer.md#customizeTable(ro.sync.ecss.extensions.api.AuthorAccess,int,int)), [customizeTable](../../commons/table/operations/TableCustomizer.md#customizeTable(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### getInstance

public static [ECDocbookTableCustomizer](ECDocbookTableCustomizer.md) getInstance()

Get the singleton instance.
  Returns: The singleton instance.
### showCustomizeTableDialog

protected [TableInfo](../../commons/table/operations/TableInfo.md) showCustomizeTableDialog([AuthorAccess](../../api/AuthorAccess.md) authorAccess, int predefinedRowsCount, int predefinedColumnsCount, int defaultTableModel)
 Description copied from class: [TableCustomizer](../../commons/table/operations/TableCustomizer.md#showCustomizeTableDialog(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int))
Show table customizer dialog and return new table information.
  Specified by: [showCustomizeTableDialog](../../commons/table/operations/TableCustomizer.md#showCustomizeTableDialog(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int)) in class [TableCustomizer](../../commons/table/operations/TableCustomizer.md) Parameters: authorAccess - The Author access. predefinedRowsCount - Predefined number of rows. predefinedColumnsCount - Predefined number of columns. defaultTableModel - The default model of the table that will be inserted. Returns: The table information provided by the user or null if customization operation is canceled. See Also:
        * [TableCustomizer.showCustomizeTableDialog(ro.sync.ecss.extensions.api.AuthorAccess, int, int, int)](../../commons/table/operations/TableCustomizer.md#showCustomizeTableDialog(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
