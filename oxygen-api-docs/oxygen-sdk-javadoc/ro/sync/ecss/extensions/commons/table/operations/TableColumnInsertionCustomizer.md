Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class TableColumnInsertionCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.operations.TableColumnInsertionCustomizer
   Direct Known Subclasses: [ECTableColumnInsertionCustomizerInvoker](ECTableColumnInsertionCustomizerInvoker.md), [SATableColumnInsertionCustomizerInvoker](SATableColumnInsertionCustomizerInvoker.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class TableColumnInsertionCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Table column insertion customizer. Shows the dialog used for customization and gets the new information.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [TableColumnsInfo](TableColumnsInfo.md) [tableColumnsInfo](#tableColumnsInfo)
The last columns info specified by the user.

## Constructor Summary
 Constructors
Constructor

Description
 [TableColumnInsertionCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 [TableColumnsInfo](TableColumnsInfo.md) [customizeTableColumnInsertion](#customizeTableColumnInsertion(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)
Customize a table column insertion.
  protected abstract [TableColumnsInfo](TableColumnsInfo.md) [showCustomTableColumnInsertionDialog](#showCustomTableColumnInsertionDialog(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)
Show table column insertion customizer dialog and return new column(s) information.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### tableColumnsInfo

protected [TableColumnsInfo](TableColumnsInfo.md) tableColumnsInfo

The last columns info specified by the user. Session level persistence.

## Constructor Details

### TableColumnInsertionCustomizer

public TableColumnInsertionCustomizer()

## Method Details

### customizeTableColumnInsertion

public [TableColumnsInfo](TableColumnsInfo.md) customizeTableColumnInsertion([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)

Customize a table column insertion. A table column insertion customizer dialog is shown, giving the possibility to choose the properties of the new column(s) to be inserted in the document. An object containing the new information is returned.
  Parameters: authorAccess - Access to Author operations. Returns: The column(s) information provided by the user or nullif customization operation is canceled.
### showCustomTableColumnInsertionDialog

protected abstract [TableColumnsInfo](TableColumnsInfo.md) showCustomTableColumnInsertionDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)

Show table column insertion customizer dialog and return new column(s) information.
  Parameters: authorAccess - The Author access. Returns: The column(s) information provided by the user or null if customization operation was canceled.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
