Package [ro.sync.ecss.extensions.api.component](package-summary.md)

# Class AuthorComponentProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.component.InternalComponentProvider
        * [ro.sync.ecss.extensions.api.component.AbstractComponentProvider](AbstractComponentProvider.md)
            * ro.sync.ecss.extensions.api.component.AuthorComponentProvider
   All Implemented Interfaces: [ComponentProvider](ComponentProvider.md), [EditorComponentProvider](EditorComponentProvider.md), [DisplayModeConstants](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class AuthorComponentProvider extends [AbstractComponentProvider](AbstractComponentProvider.md)
A component encapsulating all the visual editing part. Developers can set the XML and CSS files, and access the document through the [AuthorAccess](../AuthorAccess.md) API.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.api.component.[AbstractComponentProvider](AbstractComponentProvider.md)
 [detectionFinished](AbstractComponentProvider.md#detectionFinished), [logger](AbstractComponentProvider.md#logger), [messages](AbstractComponentProvider.md#messages)
### Fields inherited from interface ro.sync.exml.workspace.api.editor.page.author.[DisplayModeConstants](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md)
 [DISPLAY_MODE_BLOCK_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_BLOCK_TAGS), [DISPLAY_MODE_BLOCK_TAGS_WITHOUT_TEXT](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_BLOCK_TAGS_WITHOUT_TEXT), [DISPLAY_MODE_FULL_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_FULL_TAGS), [DISPLAY_MODE_FULL_TAGS_WITH_ATTRS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_FULL_TAGS_WITH_ATTRS), [DISPLAY_MODE_INLINE_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_INLINE_TAGS), [DISPLAY_MODE_NO_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_NO_TAGS), [DISPLAY_MODE_PARTIAL_TAGS](../../../../exml/workspace/api/editor/page/author/DisplayModeConstants.md#DISPLAY_MODE_PARTIAL_TAGS)
### Fields inherited from interface ro.sync.ecss.extensions.api.component.[EditorComponentProvider](EditorComponentProvider.md)
 [ATTRIBUTES_PANEL_ID](EditorComponentProvider.md#ATTRIBUTES_PANEL_ID), [ELEMENTS_PANEL_ID](EditorComponentProvider.md#ELEMENTS_PANEL_ID), [ENTITIES_PANEL_ID](EditorComponentProvider.md#ENTITIES_PANEL_ID), [MODEL_PANEL_ID](EditorComponentProvider.md#MODEL_PANEL_ID), [OUTLINER_PANEL_ID](EditorComponentProvider.md#OUTLINER_PANEL_ID), [REVIEWS_PANEL_ID](EditorComponentProvider.md#REVIEWS_PANEL_ID)
## Method Summary
  All MethodsInstance MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 protected ro.sync.exml.editor.AbstractEditor [createEditor](#createEditor(ro.sync.exml.workspace.impl.component.BaseComponentEditorManager,java.awt.Frame,java.lang.String%5B%5D,java.lang.String,java.lang.String))(ro.sync.exml.workspace.impl.component.BaseComponentEditorManager parentEditorManager, [Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) parentFrame, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedPages, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) initialPage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
Create an editor
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[JToolBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolBar.html)> [createExtensionActionsToolbars](#createExtensionActionsToolbars())()  Deprecated.
Please use instead the method ((WSAuthorComponentEditorPage)getWSEditorAccess().getCurrentPage()).createExtensionActionsToolbars();
   [AuthorAccess](../AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()  Deprecated.
Please use instead the method ((WSAuthorEditorPage)getWSEditorAccess().getCurrentPage()).getAuthorAccess().
   [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> [getAuthorCommonActions](#getAuthorCommonActions())()  Deprecated.
Please use instead the method ((WSAuthorEditorPage)getWSEditorAccess().getCurrentPage()).getActionsProvider().getAuthorCommonActions().
   [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> [getAuthorExtensionActions](#getAuthorExtensionActions())()  Deprecated.
Please use instead the method ((WSAuthorEditorPage)getWSEditorAccess().getCurrentPage()).getActionsProvider().getAuthorExtensionActions().
   void [setBreadCrumbPopUpCustomizer](#setBreadCrumbPopUpCustomizer(ro.sync.ecss.extensions.api.component.PopupMenuCustomizer))([PopupMenuCustomizer](PopupMenuCustomizer.md) popUpCustomizer)  Deprecated.
Please use instead the method ((WSAuthorComponentEditorPage)getWSEditorAccess().getCurrentPage()).setBreadCrumbPopUpCustomizer();
   void [setEditorPopUpCustomizer](#setEditorPopUpCustomizer(ro.sync.ecss.extensions.api.component.PopupMenuCustomizer))([PopupMenuCustomizer](PopupMenuCustomizer.md) popUpCustomizer)  Deprecated.
Please use instead the method ((WSAuthorEditorPage)getWSEditorAccess().getCurrentPage())addPopUpMenuCustomizer(AuthorPopupMenuCustomizer popUpCustomizer)
   void [setOutlinerPopUpCustomizer](#setOutlinerPopUpCustomizer(ro.sync.ecss.extensions.api.component.PopupMenuCustomizer))([PopupMenuCustomizer](PopupMenuCustomizer.md) popUpCustomizer)  Deprecated.
Please use instead the method ((WSAuthorComponentEditorPage)getWSEditorAccess().getCurrentPage()).setOutlinerPopUpCustomizer();
   void [showBreadCrumb](#showBreadCrumb(boolean))(boolean showBreadCrumb)  Deprecated.
Please use instead the method ((WSAuthorComponentEditorPage)getWSEditorAccess().getCurrentPage()).showBreadCrumbPanel();

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

### setEditorPopUpCustomizer

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public void setEditorPopUpCustomizer([PopupMenuCustomizer](PopupMenuCustomizer.md) popUpCustomizer)
 Deprecated.
Please use instead the method ((WSAuthorEditorPage)getWSEditorAccess().getCurrentPage())addPopUpMenuCustomizer(AuthorPopupMenuCustomizer popUpCustomizer)

The Pop-up customizer can be used to add/remove actions from the pop-up menu in the Author page editor before showing it. If everything is removed then the menu will not be shown.
  Parameters: popUpCustomizer - The pop Up Customizer.
### setOutlinerPopUpCustomizer

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public void setOutlinerPopUpCustomizer([PopupMenuCustomizer](PopupMenuCustomizer.md) popUpCustomizer)
 Deprecated.
Please use instead the method ((WSAuthorComponentEditorPage)getWSEditorAccess().getCurrentPage()).setOutlinerPopUpCustomizer();

The Pop-up customizer can be used to add/remove actions from the pop-up menu in the Author Outliner view before showing it. If everything is removed then the menu will not be shown.
  Parameters: popUpCustomizer - The pop Up Customizer.
### showBreadCrumb

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public void showBreadCrumb(boolean showBreadCrumb)
 Deprecated.
Please use instead the method ((WSAuthorComponentEditorPage)getWSEditorAccess().getCurrentPage()).showBreadCrumbPanel();

Show or hide the Bread Crumb panel in Author component.
  Parameters: showBreadCrumb - true to show the Bread Crumb. Since: 14.1
### setBreadCrumbPopUpCustomizer

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public void setBreadCrumbPopUpCustomizer([PopupMenuCustomizer](PopupMenuCustomizer.md) popUpCustomizer)
 Deprecated.
Please use instead the method ((WSAuthorComponentEditorPage)getWSEditorAccess().getCurrentPage()).setBreadCrumbPopUpCustomizer();

The Pop-up customizer can be used to add/remove actions from the pop-up menu in the Author bread crumb before showing it. If everything is removed then the menu will not be shown.
  Parameters: popUpCustomizer - The pop Up Customizer.
### createExtensionActionsToolbars

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[JToolBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolBar.html)> createExtensionActionsToolbars()
 Deprecated.
Please use instead the method ((WSAuthorComponentEditorPage)getWSEditorAccess().getCurrentPage()).createExtensionActionsToolbars();

Create toolbars with all the actions defined at the framework level in exactly the same order in which they have been added to the toolbars from the Document Type Edit dialog. The toolbars will look almost identical with the ones which appear when the XML is opened in an Oxygen standalone version.
  Returns: toolbars with all the actions defined at the framework level. Since: 14.1
### getAuthorExtensionActions

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> getAuthorExtensionActions()
 Deprecated.
Please use instead the method ((WSAuthorEditorPage)getWSEditorAccess().getCurrentPage()).getActionsProvider().getAuthorExtensionActions().

Gets the map of author extension actions.
This should get called after each load as the extension actions depend on the loaded document type.

  Returns: The map with (action id, AbstractAction) pairs with the actions defined in the Author framework. Can be null if no actions available.
### getAuthorCommonActions

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> getAuthorCommonActions()
 Deprecated.
Please use instead the method ((WSAuthorEditorPage)getWSEditorAccess().getCurrentPage()).getActionsProvider().getAuthorCommonActions().

Get the map of author common actions (undo, redo, cut, copy, paste, etc).
  Returns: The map with (action id, AbstractAction) pairs with the actions defined for working in the Author.
### getAuthorAccess

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [AuthorAccess](../AuthorAccess.md) getAuthorAccess()
 Deprecated.
Please use instead the method ((WSAuthorEditorPage)getWSEditorAccess().getCurrentPage()).getAuthorAccess().

Get the author access used to perform various operations on the Author Page.
  Returns: The author access.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
