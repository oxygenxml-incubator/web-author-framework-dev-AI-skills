Package [ro.sync.ecss.extensions.commons.sort](package-summary.md)

# Interface KeysController
    All Known Implementing Classes: [ECSortCustomizerDialog](ECSortCustomizerDialog.md), [SASortCustomizerDialog](SASortCustomizerDialog.md)   @API(type=INTERNAL, src=PUBLIC) public interface KeysController
Used for handling with a change of the keys selection.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [selectionChanged](#selectionChanged(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newSelection, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) oldSelection)
Method which controls the change of the selected key.

## Method Details

### selectionChanged

void selectionChanged([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newSelection, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) oldSelection)

Method which controls the change of the selected key.
  Parameters: newSelection - The new selected key. oldSelection - The old selected key.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
