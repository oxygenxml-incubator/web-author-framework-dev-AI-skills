Package [ro.sync.exml.plugin.document](package-summary.md)

# Interface DocumentPluginContext
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface DocumentPluginContext
Plugin context interface. Provides information for the plugin about the context it was invoked in.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html) [getDocument](#getDocument())()
Get the current document.
  [Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) [getFrame](#getFrame())()
Get the editing frame.
  [StandalonePluginWorkspace](../../workspace/api/standalone/StandalonePluginWorkspace.md) [getPluginWorkspace](#getPluginWorkspace())()
Get access to the entire workspace of Oxygen.
  [WSTextEditorPage](../../workspace/api/editor/page/text/WSTextEditorPage.md) [getTextPage](#getTextPage())()
Get access to the current text page on which this action will be invoked as a contextual menu action.

## Method Details

### getDocument

[Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html) getDocument()

Get the current document.
  Returns: the current document.
### getFrame

[Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) getFrame()

Get the editing frame.
  Returns: the frame in which is done the editing.
### getPluginWorkspace

[StandalonePluginWorkspace](../../workspace/api/standalone/StandalonePluginWorkspace.md) getPluginWorkspace()

Get access to the entire workspace of Oxygen.
  Returns: The access to the entire workspace of Oxygen Since: 12.1
### getTextPage

[WSTextEditorPage](../../workspace/api/editor/page/text/WSTextEditorPage.md) getTextPage()

Get access to the current text page on which this action will be invoked as a contextual menu action.
  Returns: Access to the text page API. Since: 15.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
