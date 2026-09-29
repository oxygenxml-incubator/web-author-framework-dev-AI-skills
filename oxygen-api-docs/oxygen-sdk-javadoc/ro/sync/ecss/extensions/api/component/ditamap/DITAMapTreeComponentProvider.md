Package [ro.sync.ecss.extensions.api.component.ditamap](package-summary.md)

# Class DITAMapTreeComponentProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.component.InternalComponentProvider
        * ro.sync.ecss.extensions.api.component.ditamap.DITAMapTreeComponentProvider
   All Implemented Interfaces: [ComponentProvider](../ComponentProvider.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class DITAMapTreeComponentProvider extends ro.sync.ecss.extensions.api.component.InternalComponentProvider implements [ComponentProvider](../ComponentProvider.md)
A component encapsulating editing a DITA Map in a DITA Maps Manager tree-like structure.
  Since: 14
## Field Summary
 Fields
Modifier and Type

Field

Description
 protected boolean [detectionFinished](#detectionFinished)
True if the detection finished
  protected static final ro.sync.i18n.MessageBundle [messages](#messages)
The messages resource bundle.

## Constructor Summary
 Constructors
Constructor

Description
 [DITAMapTreeComponentProvider](#%3Cinit%3E(ro.sync.exml.workspace.impl.component.DITAMapComponentEditorManager,ro.sync.exml.editor.EditorManager,java.awt.Frame))(ro.sync.exml.workspace.impl.component.DITAMapComponentEditorManager parentEditorManager, ro.sync.exml.editor.EditorManager mainFileOpener, [Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) parentFrame)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 void [addDITAMapTreeComponentListener](#addDITAMapTreeComponentListener(ro.sync.ecss.extensions.api.component.listeners.DITAMapTreeComponentListener))([DITAMapTreeComponentListener](../listeners/DITAMapTreeComponentListener.md) listener)
Adds a component listener.
  [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) [createReader](#createReader())()
Create a reader over the editor's current page content
  [WSDITAMapEditorPage](../../../../../exml/workspace/api/editor/page/ditamap/WSDITAMapEditorPage.md) [getDITAAccess](#getDITAAccess())()
Get the page access used to perform various operations on the DITA Map tree.
  [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> [getDITACommonActions](#getDITACommonActions())()  Deprecated.
Please use instead the method getDITAAccess().getActionsProvider().getActions().
   [Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) [getEditorComponent](#getEditorComponent())()
Get the main editor panel.
  ro.sync.exml.editor.AbstractEditor [getEditorKey](#getEditorKey())()

 [Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) [getStatusComponent](#getStatusComponent())()
Get the status panel which shows the status of the edited document.
  [WSEditor](../../../../../exml/workspace/api/editor/WSEditor.md) [getWSEditorAccess](#getWSEditorAccess())()
Get the access to the WS Editor.
  boolean [isModified](#isModified())()

 void [load](#load(java.net.URL,java.io.Reader))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)
Sets the content to edit.
  void [print](#print(boolean))(boolean preview)
Print the DITA Map component content.
  void [removeAuthorComponentListener](#removeAuthorComponentListener(ro.sync.ecss.extensions.api.component.listeners.DITAMapTreeComponentListener))([DITAMapTreeComponentListener](../listeners/DITAMapTreeComponentListener.md) listener)
Removes a component listener.
  void [save](#save())()
Save the content back to the original URL from where it was loaded using the internal support.
  void [setEditorPopUpCustomizer](#setEditorPopUpCustomizer(ro.sync.exml.workspace.api.editor.page.ditamap.DITAMapPopupMenuCustomizer))([DITAMapPopupMenuCustomizer](../../../../../exml/workspace/api/editor/page/ditamap/DITAMapPopupMenuCustomizer.md) popUpCustomizer)
The Pop-up customizer can be used to add/remove actions from the pop-up menu in the DITA Map tree editor before showing it.
  void [setModified](#setModified(boolean))(boolean modified)
Sets the modified status.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### messages

protected static final ro.sync.i18n.MessageBundle messages

The messages resource bundle.

### detectionFinished

protected boolean detectionFinished

True if the detection finished

## Constructor Details

### DITAMapTreeComponentProvider

public DITAMapTreeComponentProvider(ro.sync.exml.workspace.impl.component.DITAMapComponentEditorManager parentEditorManager, ro.sync.exml.editor.EditorManager mainFileOpener, [Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) parentFrame)throws [AuthorComponentException](../AuthorComponentException.md)

Constructor.
  Parameters: parentEditorManager - The parent editor manager mainFileOpener - The main file opener parentFrame - The parent frame. Throws: [AuthorComponentException](../AuthorComponentException.md)
## Method Details

### save

public void save()

Save the content back to the original URL from where it was loaded using the internal support. Useful only when you provide an initial URL from which the component is loaded.

### load

public void load([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)throws [AuthorComponentException](../AuthorComponentException.md)

Sets the content to edit.
This does not guarantee that the set content has been interpreted, you should set an [AuthorComponentListener](../listeners/AuthorComponentListener.md) and listen for documentTypeChanged() before using the author extension actions.

  Specified by: [load](../ComponentProvider.md#load(java.net.URL,java.io.Reader)) in interface [ComponentProvider](../ComponentProvider.md) Parameters: url - URL to load, can be null if the reader is specified If no XML content reader is given, the URL will be used both to obtain the content and to solve relative references (eg: images). If the XML content reader is also given, the URL will only be used to solve relative references from the file. reader - The reader. Throws: [AuthorComponentException](../AuthorComponentException.md) - When there was a load problem (eg: IOException).
### createReader

public [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) createReader()

Create a reader over the editor's current page content
  Returns: The reader over the current page's content
### addDITAMapTreeComponentListener

public void addDITAMapTreeComponentListener([DITAMapTreeComponentListener](../listeners/DITAMapTreeComponentListener.md) listener)

Adds a component listener.
  Parameters: listener - The listener.
### removeAuthorComponentListener

public void removeAuthorComponentListener([DITAMapTreeComponentListener](../listeners/DITAMapTreeComponentListener.md) listener)

Removes a component listener.
  Parameters: listener - The listener.
### getEditorComponent

public [Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) getEditorComponent()
 Description copied from interface: [ComponentProvider](../ComponentProvider.md#getEditorComponent())
Get the main editor panel.
  Specified by: [getEditorComponent](../ComponentProvider.md#getEditorComponent()) in interface [ComponentProvider](../ComponentProvider.md) Returns: The editor panel.
### getStatusComponent

public [Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) getStatusComponent()
 Description copied from interface: [ComponentProvider](../ComponentProvider.md#getStatusComponent())
Get the status panel which shows the status of the edited document.
  Specified by: [getStatusComponent](../ComponentProvider.md#getStatusComponent()) in interface [ComponentProvider](../ComponentProvider.md) Returns: The status panel.
### getDITACommonActions

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> getDITACommonActions()
 Deprecated.
Please use instead the method getDITAAccess().getActionsProvider().getActions().

Get the map of DITA Map common actions (undo, redo, cut, copy, paste, etc).
  Returns: The map with (action id, AbstractAction) pairs with the actions defined for working in the DITA Map.
### isModified

public boolean isModified()
  Returns: true if the component is modified.
### setModified

public void setModified(boolean modified)

Sets the modified status.
  Parameters: modified - true to flag as modified.
### getWSEditorAccess

public [WSEditor](../../../../../exml/workspace/api/editor/WSEditor.md) getWSEditorAccess()

Get the access to the WS Editor.
  Specified by: [getWSEditorAccess](../ComponentProvider.md#getWSEditorAccess()) in interface [ComponentProvider](../ComponentProvider.md) Returns: The editor access.
### getEditorKey

public ro.sync.exml.editor.AbstractEditor getEditorKey()
  Specified by: getEditorKey in class ro.sync.ecss.extensions.api.component.InternalComponentProvider Returns: The editor.
### getDITAAccess

public [WSDITAMapEditorPage](../../../../../exml/workspace/api/editor/page/ditamap/WSDITAMapEditorPage.md) getDITAAccess()

Get the page access used to perform various operations on the DITA Map tree.
  Returns: The page access.
### setEditorPopUpCustomizer

public void setEditorPopUpCustomizer([DITAMapPopupMenuCustomizer](../../../../../exml/workspace/api/editor/page/ditamap/DITAMapPopupMenuCustomizer.md) popUpCustomizer)

The Pop-up customizer can be used to add/remove actions from the pop-up menu in the DITA Map tree editor before showing it. If everything is removed then the menu will not be shown.
  Parameters: popUpCustomizer - The pop Up Customizer.
### print

public void print(boolean preview)

Print the DITA Map component content. Shows the Print dialog.
  Specified by: [print](../ComponentProvider.md#print(boolean)) in interface [ComponentProvider](../ComponentProvider.md) Parameters: preview - true to show the Print Preview dialog, false to show the Print dialog.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
