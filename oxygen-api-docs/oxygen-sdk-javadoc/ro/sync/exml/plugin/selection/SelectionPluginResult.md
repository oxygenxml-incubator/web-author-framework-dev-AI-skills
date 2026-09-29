Package [ro.sync.exml.plugin.selection](package-summary.md)

# Interface SelectionPluginResult
    All Known Implementing Classes: [SelectionPluginResultImpl](SelectionPluginResultImpl.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface SelectionPluginResult
Plugin result interface. Provides the plugin processed data.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getProcessedSelection](#getProcessedSelection())()
Get the processed selection.

## Method Details

### getProcessedSelection

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getProcessedSelection()

Get the processed selection. The string can also contain editor variables available also to Oxygen code templates like ${caret} to position the caret at a certain location or ${selection} to surround the current selection with the processed string.
  Returns: The string which will replace the selection.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
