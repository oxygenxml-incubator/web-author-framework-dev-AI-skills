Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class SATableRowInsertionCustomizerInvoker

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.TableRowInsertionCustomizer](TableRowInsertionCustomizer.md)
        * ro.sync.ecss.extensions.commons.table.operations.SATableRowInsertionCustomizerInvoker
   @API(type=INTERNAL, src=PUBLIC) public final class SATableRowInsertionCustomizerInvoker extends [TableRowInsertionCustomizer](TableRowInsertionCustomizer.md)
Customize table rows at insertion.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[TableRowInsertionCustomizer](TableRowInsertionCustomizer.md)
 [tableRowsInfo](TableRowInsertionCustomizer.md#tableRowsInfo)
## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static [TableRowInsertionCustomizer](TableRowInsertionCustomizer.md) [getInstance](#getInstance())()
Get the singleton instance.
  static void [setInstance](#setInstance(ro.sync.ecss.extensions.commons.table.operations.TableRowInsertionCustomizer))([TableRowInsertionCustomizer](TableRowInsertionCustomizer.md) anotherInstance)
Only for tests.
  protected [TableRowsInfo](TableRowsInfo.md) [showCustomTableRowInsertionDialog](#showCustomTableRowInsertionDialog(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)
Show the dialog for customizing row insertion.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[TableRowInsertionCustomizer](TableRowInsertionCustomizer.md)
 [customizeTableRowInsertion](TableRowInsertionCustomizer.md#customizeTableRowInsertion(ro.sync.ecss.extensions.api.AuthorAccess))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### getInstance

public static [TableRowInsertionCustomizer](TableRowInsertionCustomizer.md) getInstance()

Get the singleton instance.
  Returns: The singleton instance.
### setInstance

public static void setInstance([TableRowInsertionCustomizer](TableRowInsertionCustomizer.md) anotherInstance)

Only for tests. Don't use it for other purposes.
  Parameters: anotherInstance - another instance
### showCustomTableRowInsertionDialog

protected [TableRowsInfo](TableRowsInfo.md) showCustomTableRowInsertionDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)

Show the dialog for customizing row insertion.
  Specified by: [showCustomTableRowInsertionDialog](TableRowInsertionCustomizer.md#showCustomTableRowInsertionDialog(ro.sync.ecss.extensions.api.AuthorAccess)) in class [TableRowInsertionCustomizer](TableRowInsertionCustomizer.md) Parameters: authorAccess - The Author access. Returns: The row(s) information provided by the user or null if customization operation is canceled. See Also:
        * [TableRowInsertionCustomizer.showCustomTableRowInsertionDialog(ro.sync.ecss.extensions.api.AuthorAccess)](TableRowInsertionCustomizer.md#showCustomTableRowInsertionDialog(ro.sync.ecss.extensions.api.AuthorAccess))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
