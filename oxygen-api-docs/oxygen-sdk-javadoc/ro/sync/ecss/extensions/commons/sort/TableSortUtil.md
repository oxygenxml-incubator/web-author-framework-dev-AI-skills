Package [ro.sync.ecss.extensions.commons.sort](package-summary.md)

# Class TableSortUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.sort.TableSortUtil
   @API(type=INTERNAL, src=PUBLIC) public final class TableSortUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Util class for table sort operations.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static boolean [isColumnOrTableSelection](#isColumnOrTableSelection(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Checks if the current selection from the table is a [SelectionInterpretationMode.TABLE_COLUMN](../../api/SelectionInterpretationMode.md#TABLE_COLUMN) selection or a [SelectionInterpretationMode.TABLE](../../api/SelectionInterpretationMode.md#TABLE) selection.
  static boolean [isEntirelySelected](#isEntirelySelected(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../api/node/AuthorElement.md) element)
Checks if the given element is entirely included in the current selection.
  static boolean [isIncludedInSelectionInterval](#isIncludedInSelectionInterval(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../api/node/AuthorElement.md) element)
Checks if the given element is included in the selection.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### isEntirelySelected

public static boolean isEntirelySelected([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../api/node/AuthorElement.md) element)

Checks if the given element is entirely included in the current selection.
  Parameters: authorAccess - The author access. element - The element to be checked. Returns: true if the given element is entirely included in the current selection. The check is done only if the table has COLUMN selection or TABLE selection.
### isIncludedInSelectionInterval

public static boolean isIncludedInSelectionInterval([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../api/node/AuthorElement.md) element)

Checks if the given element is included in the selection.
  Parameters: authorAccess - The author access. element - The element to be checked. Returns: true if it is entirely included in the selection, false otherwise.
### isColumnOrTableSelection

public static boolean isColumnOrTableSelection([AuthorAccess](../../api/AuthorAccess.md) authorAccess)

Checks if the current selection from the table is a [SelectionInterpretationMode.TABLE_COLUMN](../../api/SelectionInterpretationMode.md#TABLE_COLUMN) selection or a [SelectionInterpretationMode.TABLE](../../api/SelectionInterpretationMode.md#TABLE) selection.
  Parameters: authorAccess - The author access. Returns: true if the current selection is a [SelectionInterpretationMode.TABLE_COLUMN](../../api/SelectionInterpretationMode.md#TABLE_COLUMN) selection or a [SelectionInterpretationMode.TABLE](../../api/SelectionInterpretationMode.md#TABLE) selection.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
