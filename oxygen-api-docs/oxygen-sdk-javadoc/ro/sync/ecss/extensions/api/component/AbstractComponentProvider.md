Package [ro.sync.ecss.extensions.api.component](package-summary.md)

# Class AbstractComponentProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.component.InternalComponentProvider
        * ro.sync.ecss.extensions.api.component.AbstractComponentProvider
   All Implemented Interfaces: [ComponentProvider](ComponentProvider.md), [EditorComponentProvider](EditorComponentProvider.md), [DisplayModeConstants](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md)   Direct Known Subclasses: [AuthorComponentProvider](AuthorComponentProvider.md), [GenericEditorComponentProvider](GenericEditorComponentProvider.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public abstract class AbstractComponentProvider extends ro.sync.ecss.extensions.api.component.InternalComponentProvider implements [DisplayModeConstants](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md), [EditorComponentProvider](EditorComponentProvider.md)
A component encapsulating all the editing part. Developers can create an editor, and access the document through the [WSEditor](../../../../exml/workspace/api/editor/WSEditor.md) API.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected boolean [detectionFinished](#detectionFinished)
True if the detection finished
  protected static final org.slf4j.Logger [logger](#logger)
Logger for logging.
  protected static final ro.sync.i18n.MessageBundle [messages](#messages)
The messages resource bundle.

### Fields inherited from interface ro.sync.exml.workspace.api.editor.page.author.[DisplayModeConstants](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md)
 [DISPLAY_MODE_BLOCK_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_BLOCK_TAGS), [DISPLAY_MODE_BLOCK_TAGS_WITHOUT_TEXT](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_BLOCK_TAGS_WITHOUT_TEXT), [DISPLAY_MODE_FULL_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_FULL_TAGS), [DISPLAY_MODE_FULL_TAGS_WITH_ATTRS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_FULL_TAGS_WITH_ATTRS), [DISPLAY_MODE_INLINE_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_INLINE_TAGS), [DISPLAY_MODE_NO_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_NO_TAGS), [DISPLAY_MODE_PARTIAL_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_PARTIAL_TAGS)
### Fields inherited from interface ro.sync.ecss.extensions.api.component.[EditorComponentProvider](EditorComponentProvider.md)
 [ATTRIBUTES_PANEL_ID](EditorComponentProvider.md#ATTRIBUTES_PANEL_ID), [ELEMENTS_PANEL_ID](EditorComponentProvider.md#ELEMENTS_PANEL_ID), [ENTITIES_PANEL_ID](EditorComponentProvider.md#ENTITIES_PANEL_ID), [MODEL_PANEL_ID](EditorComponentProvider.md#MODEL_PANEL_ID), [OUTLINER_PANEL_ID](EditorComponentProvider.md#OUTLINER_PANEL_ID), [REVIEWS_PANEL_ID](EditorComponentProvider.md#REVIEWS_PANEL_ID)
## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addAuthorComponentListener](#addAuthorComponentListener(ro.sync.ecss.extensions.api.component.listeners.AuthorComponentListener))([AuthorComponentListener](listeners/AuthorComponentListener.md) listener)
Adds an author component listener.
  protected abstract ro.sync.exml.editor.AbstractEditor [createEditor](#createEditor(ro.sync.exml.workspace.impl.component.BaseComponentEditorManager,java.awt.Frame,java.lang.String%5B%5D,java.lang.String,java.lang.String))(ro.sync.exml.workspace.impl.component.BaseComponentEditorManager parentEditorManager, [Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) parentFrame, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
Create an editor
  [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) [createReader](#createReader())()
Create a reader over the editor's current page content
  [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) [getAdditionalEditHelper](#getAdditionalEditHelper(int))(int helperID)
Get an additional edit helper panel.
  [Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) [getEditorComponent](#getEditorComponent())()
Get the main editor panel.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getEditorKey](#getEditorKey())()

 [Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) [getStatusComponent](#getStatusComponent())()
Get the status panel which shows the status of the edited document.
  [WSEditor](../../../../exml/workspace/api/editor/WSEditor.md) [getWSEditorAccess](#getWSEditorAccess())()
Get the access to the WS Editor.
  boolean [isModified](#isModified())()
Check if the component is modified
  void [load](#load(java.net.URL,java.io.Reader))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)
Sets the content to edit.
  void [print](#print(boolean))(boolean preview)
Print the author component content.
  void [removeAuthorComponentListener](#removeAuthorComponentListener(ro.sync.ecss.extensions.api.component.listeners.AuthorComponentListener))([AuthorComponentListener](listeners/AuthorComponentListener.md) listener)
Removes an author component listener.
  void [save](#save())()
Save the content back to the original URL from where it was loaded using the internal support.
  void [setModified](#setModified(boolean))(boolean modified)
Sets the modified status.
  void [showLocation](#showLocation(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Show the location referenced by a given URL in the editor.
  void [showLocation](#showLocation(java.net.URL,java.io.Reader))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)
Show the location referenced by a given URL in the editor.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### logger

protected static final org.slf4j.Logger logger

Logger for logging.

### messages

protected static final ro.sync.i18n.MessageBundle messages

The messages resource bundle.

### detectionFinished

protected boolean detectionFinished

True if the detection finished

## Method Details

### save

public void save()

Save the content back to the original URL from where it was loaded using the internal support. Useful only when you provide an initial URL from which the component is loaded.

### load

public void load([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)throws [AuthorComponentException](AuthorComponentException.md)

Sets the content to edit.
This does not guarantee that the set content has been interpreted, you should set an [AuthorComponentListener](listeners/AuthorComponentListener.md) and listen for documentTypeChanged() before using the author extension actions.

  Specified by: [load](ComponentProvider.md#load(java.net.URL,java.io.Reader)) in interface [ComponentProvider](ComponentProvider.md) Parameters: url - URL to load, can be null if the reader is specified If no XML content reader is given, the URL will be used both to obtain the content and to solve relative references (eg: images). If the XML content reader is also given, the URL will only be used to solve relative references from the file. reader - The reader. Throws: [AuthorComponentException](AuthorComponentException.md) - When there was a load problem (eg: IOException).
### showLocation

public void showLocation([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)throws [AuthorComponentException](AuthorComponentException.md)
 Description copied from interface: [EditorComponentProvider](EditorComponentProvider.md#showLocation(java.net.URL,java.io.Reader))
Show the location referenced by a given URL in the editor. If the document pointed by this URL is different than the document currently loaded in the editor page, this URL will be used to set the content to edit, to solve relative references (eg: images) and to show the location pointed by the URL reference part. If the document pointed by this URL is currently loaded in the editor page, only the reference part of the given URL will be used to show the corresponding location in the editor.
  Specified by: [showLocation](EditorComponentProvider.md#showLocation(java.net.URL,java.io.Reader)) in interface [EditorComponentProvider](EditorComponentProvider.md) Parameters: url - The URL to show location for. reader - The reader over the URL, can be null. Throws: [AuthorComponentException](AuthorComponentException.md) - When there was a load problem (eg: IOException). See Also:
        * [EditorComponentProvider.showLocation(java.net.URL, java.io.Reader)](EditorComponentProvider.md#showLocation(java.net.URL,java.io.Reader))

### createEditor

protected abstract ro.sync.exml.editor.AbstractEditor createEditor(ro.sync.exml.workspace.impl.component.BaseComponentEditorManager parentEditorManager, [Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) parentFrame, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)throws [AuthorComponentException](AuthorComponentException.md)

Create an editor
  Parameters: parentEditorManager - The view manager. parentFrame - View's parent frame. allowedPages - The enumeration of allowed pages. initialPage - The initial page. Can be null contentType - The content type of the editor. Returns: The new created editor. Throws: [AuthorComponentException](AuthorComponentException.md)
### createReader

public [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) createReader()

Create a reader over the editor's current page content
  Returns: The reader over the current page's content
### addAuthorComponentListener

public void addAuthorComponentListener([AuthorComponentListener](listeners/AuthorComponentListener.md) listener)

Adds an author component listener.
  Specified by: [addAuthorComponentListener](EditorComponentProvider.md#addAuthorComponentListener(ro.sync.ecss.extensions.api.component.listeners.AuthorComponentListener)) in interface [EditorComponentProvider](EditorComponentProvider.md) Parameters: listener - The listener.
### removeAuthorComponentListener

public void removeAuthorComponentListener([AuthorComponentListener](listeners/AuthorComponentListener.md) listener)

Removes an author component listener.
  Specified by: [removeAuthorComponentListener](EditorComponentProvider.md#removeAuthorComponentListener(ro.sync.ecss.extensions.api.component.listeners.AuthorComponentListener)) in interface [EditorComponentProvider](EditorComponentProvider.md) Parameters: listener - The listener.
### getEditorComponent

public [Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) getEditorComponent()
 Description copied from interface: [ComponentProvider](ComponentProvider.md#getEditorComponent())
Get the main editor panel.
  Specified by: [getEditorComponent](ComponentProvider.md#getEditorComponent()) in interface [ComponentProvider](ComponentProvider.md) Returns: The editor panel.
### getStatusComponent

public [Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) getStatusComponent()
 Description copied from interface: [ComponentProvider](ComponentProvider.md#getStatusComponent())
Get the status panel which shows the status of the edited document.
  Specified by: [getStatusComponent](ComponentProvider.md#getStatusComponent()) in interface [ComponentProvider](ComponentProvider.md) Returns: The status panel.
### isModified

public boolean isModified()

Check if the component is modified
  Returns: true if the component is modified.
### setModified

public void setModified(boolean modified)

Sets the modified status.
  Parameters: modified - true to flag as modified. Since: 13
### getWSEditorAccess

public [WSEditor](../../../../exml/workspace/api/editor/WSEditor.md) getWSEditorAccess()

Get the access to the WS Editor.
  Specified by: [getWSEditorAccess](ComponentProvider.md#getWSEditorAccess()) in interface [ComponentProvider](ComponentProvider.md) Returns: The author access.
### getEditorKey

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getEditorKey()
  Specified by: getEditorKey in class ro.sync.ecss.extensions.api.component.InternalComponentProvider Returns: The editor.
### getAdditionalEditHelper

public [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) getAdditionalEditHelper(int helperID)

Get an additional edit helper panel. It can be the Attributes, Reviews, Outliner, Elements, Entities, Model component, depending on the ID. Note that the Elements, Entities and Model views are not available in the Author Reviewer edition.
  Specified by: [getAdditionalEditHelper](EditorComponentProvider.md#getAdditionalEditHelper(int)) in interface [EditorComponentProvider](EditorComponentProvider.md) Parameters: helperID - One of:
        * [EditorComponentProvider.ATTRIBUTES_PANEL_ID](EditorComponentProvider.md#ATTRIBUTES_PANEL_ID),
        * [EditorComponentProvider.REVIEWS_PANEL_ID](EditorComponentProvider.md#REVIEWS_PANEL_ID),
        * [EditorComponentProvider.OUTLINER_PANEL_ID](EditorComponentProvider.md#OUTLINER_PANEL_ID)
        * [EditorComponentProvider.ELEMENTS_PANEL_ID](EditorComponentProvider.md#ELEMENTS_PANEL_ID)
        * [EditorComponentProvider.ENTITIES_PANEL_ID](EditorComponentProvider.md#ENTITIES_PANEL_ID)
        * [EditorComponentProvider.MODEL_PANEL_ID](EditorComponentProvider.md#MODEL_PANEL_ID) constants.
 Returns: The additional component.
### print

public void print(boolean preview)

Print the author component content. Shows the Print dialog.
  Specified by: [print](ComponentProvider.md#print(boolean)) in interface [ComponentProvider](ComponentProvider.md) Parameters: preview - true to show the Print Preview dialog, false to show the Print dialog. Since: 13
### showLocation

public void showLocation([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)throws [AuthorComponentException](AuthorComponentException.md)

Show the location referenced by a given URL in the editor. If the document pointed by this URL is different than the document currently loaded in the editor page, this URL will be used to set the content to edit, to solve relative references (eg: images) and to show the location pointed by the URL reference part. If the document pointed by this URL is currently loaded in the editor page, only the reference part of the given URL will be used to show the corresponding location in the editor.
  Parameters: url - The URL to show location for. Throws: [AuthorComponentException](AuthorComponentException.md) - When there was a load problem (eg: IOException). Since: 14.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
