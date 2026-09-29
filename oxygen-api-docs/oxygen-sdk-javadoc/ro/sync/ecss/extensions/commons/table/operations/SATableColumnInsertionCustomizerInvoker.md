Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class SATableColumnInsertionCustomizerInvoker

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.TableColumnInsertionCustomizer](TableColumnInsertionCustomizer.md)
        * ro.sync.ecss.extensions.commons.table.operations.SATableColumnInsertionCustomizerInvoker
   @API(type=INTERNAL, src=PUBLIC) public final class SATableColumnInsertionCustomizerInvoker extends [TableColumnInsertionCustomizer](TableColumnInsertionCustomizer.md)
Customize table column at insertion.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[TableColumnInsertionCustomizer](TableColumnInsertionCustomizer.md)
 [tableColumnsInfo](TableColumnInsertionCustomizer.md#tableColumnsInfo)
## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static [TableColumnInsertionCustomizer](TableColumnInsertionCustomizer.md) [getInstance](#getInstance())()
Get the singleton instance.
  static void [setInstance](#setInstance(ro.sync.ecss.extensions.commons.table.operations.TableColumnInsertionCustomizer))([TableColumnInsertionCustomizer](TableColumnInsertionCustomizer.md) anotherInstance)
Only for tests.
  protected [TableColumnsInfo](TableColumnsInfo.md) [showCustomTableColumnInsertionDialog](#showCustomTableColumnInsertionDialog(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)
Show the dialog for customizing column insertion.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[TableColumnInsertionCustomizer](TableColumnInsertionCustomizer.md)
 [customizeTableColumnInsertion](TableColumnInsertionCustomizer.md#customizeTableColumnInsertion(ro.sync.ecss.extensions.api.AuthorAccess))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### getInstance

public static [TableColumnInsertionCustomizer](TableColumnInsertionCustomizer.md) getInstance()

Get the singleton instance.
  Returns: The singleton instance.
### setInstance

public static void setInstance([TableColumnInsertionCustomizer](TableColumnInsertionCustomizer.md) anotherInstance)

Only for tests. Don't use it for other purposes.
  Parameters: anotherInstance - another instance
### showCustomTableColumnInsertionDialog

protected [TableColumnsInfo](TableColumnsInfo.md) showCustomTableColumnInsertionDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)

Show the dialog for customizing column insertion.
  Specified by: [showCustomTableColumnInsertionDialog](TableColumnInsertionCustomizer.md#showCustomTableColumnInsertionDialog(ro.sync.ecss.extensions.api.AuthorAccess)) in class [TableColumnInsertionCustomizer](TableColumnInsertionCustomizer.md) Parameters: authorAccess - The Author access. Returns: The column(s) information provided by the user or null if customization operation was canceled. See Also:
        * [TableColumnInsertionCustomizer.showCustomTableColumnInsertionDialog(ro.sync.ecss.extensions.api.AuthorAccess)](TableColumnInsertionCustomizer.md#showCustomTableColumnInsertionDialog(ro.sync.ecss.extensions.api.AuthorAccess))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
