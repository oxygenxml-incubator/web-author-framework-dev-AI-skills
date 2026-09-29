Package [ro.sync.ecss.extensions.api.component](package-summary.md)

# Class GenericEditorComponentProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.component.InternalComponentProvider
        * [ro.sync.ecss.extensions.api.component.AbstractComponentProvider](AbstractComponentProvider.md)
            * ro.sync.ecss.extensions.api.component.GenericEditorComponentProvider
   All Implemented Interfaces: [ComponentProvider](ComponentProvider.md), [EditorComponentProvider](EditorComponentProvider.md), [DisplayModeConstants](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public final class GenericEditorComponentProvider extends [AbstractComponentProvider](AbstractComponentProvider.md)
A component encapsulating all the editing part. Developers can create an editor, and access the document through the [WSEditor](../../../../exml/workspace/api/editor/WSEditor.md) API.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.api.component.[AbstractComponentProvider](AbstractComponentProvider.md)
 [detectionFinished](AbstractComponentProvider.md#detectionFinished), [logger](AbstractComponentProvider.md#logger), [messages](AbstractComponentProvider.md#messages)
### Fields inherited from interface ro.sync.exml.workspace.api.editor.page.author.[DisplayModeConstants](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md)
 [DISPLAY_MODE_BLOCK_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_BLOCK_TAGS), [DISPLAY_MODE_BLOCK_TAGS_WITHOUT_TEXT](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_BLOCK_TAGS_WITHOUT_TEXT), [DISPLAY_MODE_FULL_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_FULL_TAGS), [DISPLAY_MODE_FULL_TAGS_WITH_ATTRS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_FULL_TAGS_WITH_ATTRS), [DISPLAY_MODE_INLINE_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_INLINE_TAGS), [DISPLAY_MODE_NO_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_NO_TAGS), [DISPLAY_MODE_PARTIAL_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_PARTIAL_TAGS)
### Fields inherited from interface ro.sync.ecss.extensions.api.component.[EditorComponentProvider](EditorComponentProvider.md)
 [ATTRIBUTES_PANEL_ID](EditorComponentProvider.md#ATTRIBUTES_PANEL_ID), [ELEMENTS_PANEL_ID](EditorComponentProvider.md#ELEMENTS_PANEL_ID), [ENTITIES_PANEL_ID](EditorComponentProvider.md#ENTITIES_PANEL_ID), [MODEL_PANEL_ID](EditorComponentProvider.md#MODEL_PANEL_ID), [OUTLINER_PANEL_ID](EditorComponentProvider.md#OUTLINER_PANEL_ID), [REVIEWS_PANEL_ID](EditorComponentProvider.md#REVIEWS_PANEL_ID)
## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected ro.sync.exml.editor.AbstractEditor [createEditor](#createEditor(ro.sync.exml.workspace.impl.component.BaseComponentEditorManager,java.awt.Frame,java.lang.String%5B%5D,java.lang.String,java.lang.String))(ro.sync.exml.workspace.impl.component.BaseComponentEditorManager parentEditorManager, [Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) parentFrame, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
Create an editor

### Methods inherited from class ro.sync.ecss.extensions.api.component.[AbstractComponentProvider](AbstractComponentProvider.md)
 [addAuthorComponentListener](AbstractComponentProvider.md#addAuthorComponentListener(ro.sync.ecss.extensions.api.component.listeners.AuthorComponentListener)), [createReader](AbstractComponentProvider.md#createReader()), [getAdditionalEditHelper](AbstractComponentProvider.md#getAdditionalEditHelper(int)), [getEditorComponent](AbstractComponentProvider.md#getEditorComponent()), [getEditorKey](AbstractComponentProvider.md#getEditorKey()), [getStatusComponent](AbstractComponentProvider.md#getStatusComponent()), [getWSEditorAccess](AbstractComponentProvider.md#getWSEditorAccess()), [isModified](AbstractComponentProvider.md#isModified()), [load](AbstractComponentProvider.md#load(java.net.URL,java.io.Reader)), [print](AbstractComponentProvider.md#print(boolean)), [removeAuthorComponentListener](AbstractComponentProvider.md#removeAuthorComponentListener(ro.sync.ecss.extensions.api.component.listeners.AuthorComponentListener)), [save](AbstractComponentProvider.md#save()), [setModified](AbstractComponentProvider.md#setModified(boolean)), [showLocation](AbstractComponentProvider.md#showLocation(java.net.URL)), [showLocation](AbstractComponentProvider.md#showLocation(java.net.URL,java.io.Reader))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### createEditor

protected ro.sync.exml.editor.AbstractEditor createEditor(ro.sync.exml.workspace.impl.component.BaseComponentEditorManager parentEditorManager, [Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) parentFrame, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)throws [AuthorComponentException](AuthorComponentException.md)
 Description copied from class: [AbstractComponentProvider](AbstractComponentProvider.md#createEditor(ro.sync.exml.workspace.impl.component.BaseComponentEditorManager,java.awt.Frame,java.lang.String%5B%5D,java.lang.String,java.lang.String))
Create an editor
  Specified by: [createEditor](AbstractComponentProvider.md#createEditor(ro.sync.exml.workspace.impl.component.BaseComponentEditorManager,java.awt.Frame,java.lang.String%5B%5D,java.lang.String,java.lang.String)) in class [AbstractComponentProvider](AbstractComponentProvider.md) Parameters: parentEditorManager - The view manager. parentFrame - View's parent frame. allowedPages - The enumeration of allowed pages. initialPage - The initial page. Can be null contentType - The content type of the editor. Returns: The new created editor. Throws: [AuthorComponentException](AuthorComponentException.md) See Also:
        * [AbstractComponentProvider.createEditor(ro.sync.exml.workspace.impl.component.BaseComponentEditorManager, java.awt.Frame, java.lang.String[], java.lang.String, java.lang.String)](AbstractComponentProvider.md#createEditor(ro.sync.exml.workspace.impl.component.BaseComponentEditorManager,java.awt.Frame,java.lang.String%5B%5D,java.lang.String,java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
