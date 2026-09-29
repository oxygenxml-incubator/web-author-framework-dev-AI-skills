Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class TableCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.operations.TableCustomizer
   Direct Known Subclasses: [ECDITARelTableCustomizer](../../../dita/map/table/ECDITARelTableCustomizer.md), [ECDITATableCustomizer](../../../dita/topic/table/ECDITATableCustomizer.md), [ECDocbookInnerTableCustomizer](../../../docbook/table/ECDocbookInnerTableCustomizer.md), [ECDocbookTableCustomizer](../../../docbook/table/ECDocbookTableCustomizer.md), [ECTEITableCustomizer](../../../tei/table/ECTEITableCustomizer.md), [ECXHTMLTableCustomizerInvoker](xhtml/ECXHTMLTableCustomizerInvoker.md), [SADITARelTableCustomizer](../../../dita/map/table/SADITARelTableCustomizer.md), [SADITATableCustomizer](../../../dita/topic/table/SADITATableCustomizer.md), [SADocbookInnerTableCustomizer](../../../docbook/table/SADocbookInnerTableCustomizer.md), [SADocbookTableCustomizer](../../../docbook/table/SADocbookTableCustomizer.md), [SATEITableCustomizer](../../../tei/table/SATEITableCustomizer.md), [SAXHTMLTableCustomizerInvoker](xhtml/SAXHTMLTableCustomizerInvoker.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class TableCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Base for frameworks table customizers. It is used on standalone implementation.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [TableInfo](TableInfo.md) [tableInfo](#tableInfo)
The last table info specified by the user.

## Constructor Summary
 Constructors
Constructor

Description
 [TableCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 [TableInfo](TableInfo.md) [customizeTable](#customizeTable(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)
Customize a table.
  [TableInfo](TableInfo.md) [customizeTable](#customizeTable(ro.sync.ecss.extensions.api.AuthorAccess,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, int predefinedRowsCount, int predefinedColumnsCount)
Customize a table.
  [TableInfo](TableInfo.md) [customizeTable](#customizeTable(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, int predefinedRowsCount, int predefinedColumnsCount, int defaultTableModel)
Customize a table.
  protected abstract [TableInfo](TableInfo.md) [showCustomizeTableDialog](#showCustomizeTableDialog(ro.sync.ecss.extensions.api.AuthorAccess,int,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, int predefinedRowsCount, int predefinedColumnsCount, int defaultTableModel)
Show table customizer dialog and return new table information.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### tableInfo

protected [TableInfo](TableInfo.md) tableInfo

The last table info specified by the user. Session level persistence.

## Constructor Details

### TableCustomizer

public TableCustomizer()

## Method Details

### customizeTable

public [TableInfo](TableInfo.md) customizeTable([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)

Customize a table. A table customizer dialog is shown, giving the possibility to choose the properties of a new table to be inserted in the document. An object containing the new table information is returned.
  Parameters: authorAccess - Access to Author operations. Returns: The table information provided by the user or nullif customization operation is canceled.
### customizeTable

public [TableInfo](TableInfo.md) customizeTable([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, int predefinedRowsCount, int predefinedColumnsCount)

Customize a table. A table customizer dialog is shown, giving the possibility to choose the properties of a new table to be inserted in the document. An object containing the new table information is returned.
  Parameters: authorAccess - Access to Author operations. predefinedRowsCount - The predefined number of rows, -1 if the user can control the number of inserted column. predefinedColumnsCount - The predefined number of columns, -1 if the user can control the number of inserted column. If predefined columns count and predefined rows count values are positive then the dialog will not contain any field for defining the table columns and rows count and the inserted table will use the predefined values. Returns: The table information provided by the user or nullif customization operation is canceled.
### showCustomizeTableDialog

protected abstract [TableInfo](TableInfo.md) showCustomizeTableDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, int predefinedRowsCount, int predefinedColumnsCount, int defaultTableModel)

Show table customizer dialog and return new table information.
  Parameters: authorAccess - The Author access. predefinedRowsCount - Predefined number of rows. predefinedColumnsCount - Predefined number of columns. defaultTableModel - The default model of the table that will be inserted. Returns: The table information provided by the user or null if customization operation is canceled.
### customizeTable

public [TableInfo](TableInfo.md) customizeTable([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, int predefinedRowsCount, int predefinedColumnsCount, int defaultTableModel)

Customize a table. A table customizer dialog is shown, giving the possibility to choose the properties of a new table to be inserted in the document. An object containing the new table information is returned.
  Parameters: authorAccess - Access to Author operations. predefinedRowsCount - The predefined number of rows, -1 if the user can control the number of inserted column. predefinedColumnsCount - The predefined number of columns, -1 if the user can control the number of inserted column. If predefined columns count and predefined rows count values are positive then the dialog will not contain any field for defining the table columns and rows count and the inserted table will use the predefined values. defaultTableModel - The default model of the table that will be inserted. Returns: The table information provided by the user or nullif customization operation is canceled.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
