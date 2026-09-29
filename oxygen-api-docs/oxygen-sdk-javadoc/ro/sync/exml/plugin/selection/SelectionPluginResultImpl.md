Package [ro.sync.exml.plugin.selection](package-summary.md)

# Class SelectionPluginResultImpl

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.plugin.selection.SelectionPluginResultImpl
   All Implemented Interfaces: [SelectionPluginResult](SelectionPluginResult.md)   @API(type=EXTENDABLE, src=PUBLIC) public class SelectionPluginResultImpl extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [SelectionPluginResult](SelectionPluginResult.md)
Support implementation of the PluginResult interface.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [selection](#selection)
The processed selection.

## Constructor Summary
 Constructors
Constructor

Description
 [SelectionPluginResultImpl](#%3Cinit%3E())()
Creates a no data plugin result.
  [SelectionPluginResultImpl](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) selection)
Creates the plugin result.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getProcessedSelection](#getProcessedSelection())()
Get the content which will replace the current selection.
  void [setProcessedSelection](#setProcessedSelection(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) selection)
Set the current selection.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### selection

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) selection

The processed selection.

## Constructor Details

### SelectionPluginResultImpl

public SelectionPluginResultImpl()

Creates a no data plugin result.

### SelectionPluginResultImpl

public SelectionPluginResultImpl([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) selection)

Creates the plugin result.
  Parameters: selection - The processed selection. The string can also contain editor variables available also to Oxygen code templates like ${caret} to position the caret at a certain location or ${selection} to surround the current selection with the processed string.
## Method Details

### setProcessedSelection

public void setProcessedSelection([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) selection)

Set the current selection. The string can also contain editor variables available also to Oxygen code templates like ${caret} to position the caret at a certain location or ${selection} to surround the current selection with the processed string.
  Parameters: selection - The current selection.
### getProcessedSelection

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getProcessedSelection()

Get the content which will replace the current selection. The string can also contain editor variables available also to Oxygen code templates like ${caret} to position the caret at a certain location or ${selection} to surround the current selection with the processed string.
  Specified by: [getProcessedSelection](SelectionPluginResult.md#getProcessedSelection()) in interface [SelectionPluginResult](SelectionPluginResult.md) Returns: the content which will replace the current selection.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
