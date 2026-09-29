Package [ro.sync.ecss.extensions.api.component](package-summary.md)

# Interface ComponentProvider
    All Known Subinterfaces: [EditorComponentProvider](EditorComponentProvider.md)   All Known Implementing Classes: [AbstractComponentProvider](AbstractComponentProvider.md), [AuthorComponentProvider](AuthorComponentProvider.md), [DITAMapTreeComponentProvider](ditamap/DITAMapTreeComponentProvider.md), [GenericEditorComponentProvider](GenericEditorComponentProvider.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ComponentProvider
Base interface for Editor and for DITA Map component providers with common methods.
  Since: 15
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) [getEditorComponent](#getEditorComponent())()
Get the main editor panel.
  [Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) [getStatusComponent](#getStatusComponent())()
Get the status panel which shows the status of the edited document.
  [WSEditor](../../../../exml/workspace/api/editor/WSEditor.md) [getWSEditorAccess](#getWSEditorAccess())()
Get the access to the WS Editor.
  void [load](#load(java.net.URL,java.io.Reader))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)
Sets the content to edit.
  void [print](#print(boolean))(boolean preview)
Print the component content.

## Method Details

### load

void load([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)throws [AuthorComponentException](AuthorComponentException.md)

Sets the content to edit.
This does not guarantee that the set content has been interpreted, you should set an [AuthorComponentListener](listeners/AuthorComponentListener.md) and listen for documentTypeChanged() before using the author extension actions.

  Parameters: url - URL to load, can be null if the reader is specified If no XML content reader is given, the URL will be used both to obtain the content and to solve relative references (eg: images). If the XML content reader is also given, the URL will only be used to solve relative references from the file. reader - The reader. Throws: [AuthorComponentException](AuthorComponentException.md) - When there was a load problem (eg: IOException).
### getEditorComponent

[Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) getEditorComponent()

Get the main editor panel.
  Returns: The editor panel.
### getStatusComponent

[Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) getStatusComponent()

Get the status panel which shows the status of the edited document.
  Returns: The status panel.
### print

void print(boolean preview)

Print the component content. Shows the Print dialog.
  Parameters: preview - true to show the Print Preview dialog, false to show the Print dialog.
### getWSEditorAccess

[WSEditor](../../../../exml/workspace/api/editor/WSEditor.md) getWSEditorAccess()

Get the access to the WS Editor.
  Returns: The author access.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
