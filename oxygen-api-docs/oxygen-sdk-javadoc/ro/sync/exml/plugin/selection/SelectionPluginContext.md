Package [ro.sync.exml.plugin.selection](package-summary.md)

# Interface SelectionPluginContext
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface SelectionPluginContext
Plugin context interface. Provides information for the plugin about the context it was invoked in.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getDocumentURL](#getDocumentURL())()
Get the URL of the edited document.
  [Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) [getFrame](#getFrame())()
Get the editing frame.
  [StandalonePluginWorkspace](../../workspace/api/standalone/StandalonePluginWorkspace.md) [getPluginWorkspace](#getPluginWorkspace())()
Get access to the entire workspace of Oxygen.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSelection](#getSelection())()
Get the current selection.

## Method Details

### getSelection

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSelection()

Get the current selection.
  Returns: the current selection or an empty string if there is no selection.
### getFrame

[Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) getFrame()

Get the editing frame.
  Returns: the frame in which is done the editing.
### getDocumentURL

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getDocumentURL()

Get the URL of the edited document.
  Returns: The URL of the edited document.
### getPluginWorkspace

[StandalonePluginWorkspace](../../workspace/api/standalone/StandalonePluginWorkspace.md) getPluginWorkspace()

Get access to the entire workspace of Oxygen.
  Returns: The access to the entire workspace of Oxygen Since: 12.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
