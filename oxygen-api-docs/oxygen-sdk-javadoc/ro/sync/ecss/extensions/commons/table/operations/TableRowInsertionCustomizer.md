Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class TableRowInsertionCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.operations.TableRowInsertionCustomizer
   Direct Known Subclasses: [ECTableRowInsertionCustomizerInvoker](ECTableRowInsertionCustomizerInvoker.md), [SATableRowInsertionCustomizerInvoker](SATableRowInsertionCustomizerInvoker.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class TableRowInsertionCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Table row insertion customizer. Shows the dialog used for customization and gets the new information.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [TableRowsInfo](TableRowsInfo.md) [tableRowsInfo](#tableRowsInfo)
The last rows info specified by the user.

## Constructor Summary
 Constructors
Constructor

Description
 [TableRowInsertionCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 [TableRowsInfo](TableRowsInfo.md) [customizeTableRowInsertion](#customizeTableRowInsertion(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)
Customize a table row insertion.
  protected abstract [TableRowsInfo](TableRowsInfo.md) [showCustomTableRowInsertionDialog](#showCustomTableRowInsertionDialog(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)
Show table row insertion customizer dialog and return new row(s) information.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### tableRowsInfo

protected [TableRowsInfo](TableRowsInfo.md) tableRowsInfo

The last rows info specified by the user. Session level persistence.

## Constructor Details

### TableRowInsertionCustomizer

public TableRowInsertionCustomizer()

## Method Details

### customizeTableRowInsertion

public [TableRowsInfo](TableRowsInfo.md) customizeTableRowInsertion([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)

Customize a table row insertion. A table row insertion customizer dialog is shown, giving the possibility to choose the properties of the new row(s) to be inserted in the document. An object containing the new information is returned.
  Parameters: authorAccess - Access to Author operations. Returns: The row information provided by the user or nullif customization operation is canceled.
### showCustomTableRowInsertionDialog

protected abstract [TableRowsInfo](TableRowsInfo.md) showCustomTableRowInsertionDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)

Show table row insertion customizer dialog and return new row(s) information.
  Parameters: authorAccess - The Author access. Returns: The row(s) information provided by the user or null if customization operation is canceled.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
