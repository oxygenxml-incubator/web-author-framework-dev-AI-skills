Package [ro.sync.ecss.extensions.commons.operations](package-summary.md)

# Class MoveCaretUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.operations.MoveCaretUtil
   @API(type=INTERNAL, src=PUBLIC) public final class MoveCaretUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Utility to detect an editor variable in the Author page and move the caret to that place.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static boolean [hasImposedEditorVariableCaretOffset](#hasImposedEditorVariableCaretOffset(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment)
Check if the imposed editor variable caret offset can be found in the XML fragment.
  static void [moveCaretToImposedEditorVariableOffset](#moveCaretToImposedEditorVariableOffset(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, int insertionOffset)
Move the caret to the offset imposed by a certain editor variable present in the Author page.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### hasImposedEditorVariableCaretOffset

public static boolean hasImposedEditorVariableCaretOffset([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment)

Check if the imposed editor variable caret offset can be found in the XML fragment.
  Parameters: xmlFragment - The XML fragment. Returns: true if the imposed editor variable caret offset can be found in the XML fragment.
### moveCaretToImposedEditorVariableOffset

public static void moveCaretToImposedEditorVariableOffset([AuthorAccess](../../api/AuthorAccess.md) authorAccess, int insertionOffset)

Move the caret to the offset imposed by a certain editor variable present in the Author page.
  Parameters: authorAccess - The author access. insertionOffset - The offset where the operation inserted the XML fragment.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
