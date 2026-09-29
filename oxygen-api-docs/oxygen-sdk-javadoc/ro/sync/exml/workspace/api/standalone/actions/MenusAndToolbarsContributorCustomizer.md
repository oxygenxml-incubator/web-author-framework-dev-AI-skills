Package [ro.sync.exml.workspace.api.standalone.actions](package-summary.md)

# Class MenusAndToolbarsContributorCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.standalone.actions.MenusAndToolbarsContributorCustomizer
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class MenusAndToolbarsContributorCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Abstract class allowed as an extension point to customize the menu and toolbar buttons added by our editors.
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [MenusAndToolbarsContributorCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [customizeAuthorBreadcrumbPopUpMenu](#customizeAuthorBreadcrumbPopUpMenu(javax.swing.JPopupMenu,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode))([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUp, [AuthorAccess](../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess, [AuthorNode](../../../../../ecss/extensions/api/node/AuthorNode.md) currentNode)
Customize a pop-up menu about to be shown in the Author page Breadcrumb (current elements path) toolbar.
  void [customizeAuthorOutlinePopUpMenu](#customizeAuthorOutlinePopUpMenu(javax.swing.JPopupMenu,ro.sync.ecss.extensions.api.AuthorAccess))([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUp, [AuthorAccess](../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess)
Customize a pop-up menu about to be shown in the Author page Outline view.
  void [customizeAuthorPageExtensionMenu](#customizeAuthorPageExtensionMenu(javax.swing.JMenu,ro.sync.ecss.extensions.api.AuthorAccess))([JMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JMenu.html) extensionMenu, [AuthorAccess](../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess)
Customize an extension main menu contributed by the Author page document type configuration.
  void [customizeAuthorPageExtensionToolbar](#customizeAuthorPageExtensionToolbar(ro.sync.exml.workspace.api.standalone.ToolbarInfo,ro.sync.ecss.extensions.api.AuthorAccess))([ToolbarInfo](../ToolbarInfo.md) toolbarInfo, [AuthorAccess](../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess)
Customize an extension toolbar contributed by the Author page document type configuration.
  void [customizeAuthorPopUpMenu](#customizeAuthorPopUpMenu(javax.swing.JPopupMenu,ro.sync.ecss.extensions.api.AuthorAccess))([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUp, [AuthorAccess](../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess)
Customize a pop-up menu in the Author page before showing it.
  void [customizeDITAMapPopUpMenu](#customizeDITAMapPopUpMenu(javax.swing.JPopupMenu,ro.sync.exml.workspace.api.editor.page.ditamap.WSDITAMapEditorPage))([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUp, [WSDITAMapEditorPage](../../editor/page/ditamap/WSDITAMapEditorPage.md) ditaMapEditorPage)
Customize a pop-up menu in the DITA Maps Manager page before showing it.
  void [customizeDITAMapsManagerExtendedToolbar](#customizeDITAMapsManagerExtendedToolbar(ro.sync.exml.workspace.api.standalone.ToolbarInfo))([ToolbarInfo](../ToolbarInfo.md) toolbarInfo)
Customize the DITA Maps Manager extended toolbar.
  void [customizeDITAMapsManagerMainToolbar](#customizeDITAMapsManagerMainToolbar(ro.sync.exml.workspace.api.standalone.ToolbarInfo))([ToolbarInfo](../ToolbarInfo.md) toolbarInfo)
Customize the DITA Maps Manager main toolbar.
  void [customizeEditorTabPopUpMenu](#customizeEditorTabPopUpMenu(javax.swing.JPopupMenu,ro.sync.exml.workspace.api.editor.WSEditor))([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUpMenu, [WSEditor](../../editor/WSEditor.md) editor)
Customize the pop-up menu shown when right-clicking the tab of an editor (where the filename is presented).
  void [customizeTextPopUpMenu](#customizeTextPopUpMenu(javax.swing.JPopupMenu,ro.sync.exml.workspace.api.editor.page.text.WSTextEditorPage))([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUp, [WSTextEditorPage](../../editor/page/text/WSTextEditorPage.md) textPage)
Customize a pop-up menu in the Text page before showing it.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### MenusAndToolbarsContributorCustomizer

public MenusAndToolbarsContributorCustomizer()

## Method Details

### customizeAuthorPageExtensionMenu

public void customizeAuthorPageExtensionMenu([JMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JMenu.html) extensionMenu, [AuthorAccess](../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess)

Customize an extension main menu contributed by the Author page document type configuration. For example DITA, Docbook, etc...
  Parameters: extensionMenu - The extension menu. authorAccess - Access class to the author functions.
### customizeAuthorPageExtensionToolbar

public void customizeAuthorPageExtensionToolbar([ToolbarInfo](../ToolbarInfo.md) toolbarInfo, [AuthorAccess](../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess)

Customize an extension toolbar contributed by the Author page document type configuration. The toolbar will be included in the Author-specific toolbar. An extension toolbar contains actions belonging to the specific support the application offers for a certain vocabulary.
  Parameters: toolbarInfo - Information about toolbar components. authorAccess - Access class to the author functions.
### customizeDITAMapsManagerExtendedToolbar

public void customizeDITAMapsManagerExtendedToolbar([ToolbarInfo](../ToolbarInfo.md) toolbarInfo)

Customize the DITA Maps Manager extended toolbar.
  Parameters: toolbarInfo - The toolbar information.
### customizeDITAMapsManagerMainToolbar

public void customizeDITAMapsManagerMainToolbar([ToolbarInfo](../ToolbarInfo.md) toolbarInfo)

Customize the DITA Maps Manager main toolbar.
  Parameters: toolbarInfo - The toolbar components information.
### customizeAuthorPopUpMenu

public void customizeAuthorPopUpMenu([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUp, [AuthorAccess](../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess)

Customize a pop-up menu in the Author page before showing it. By default this method gets called for both the contextual menu shown in the main editing area, shown in the Outline view or shown in the Breadcrumb. If everything is removed then the menu will not be shown.
  Parameters: popUp - The pop-up Menu. authorAccess - Access class to the author functions.
### customizeAuthorOutlinePopUpMenu

public void customizeAuthorOutlinePopUpMenu([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUp, [AuthorAccess](../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess)

Customize a pop-up menu about to be shown in the Author page Outline view. If everything is removed then the menu will not be shown.
  Parameters: popUp - The pop-up Menu. authorAccess - Access class to the author functions. Since: 18.1
### customizeAuthorBreadcrumbPopUpMenu

public void customizeAuthorBreadcrumbPopUpMenu([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUp, [AuthorAccess](../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess, [AuthorNode](../../../../../ecss/extensions/api/node/AuthorNode.md) currentNode)

Customize a pop-up menu about to be shown in the Author page Breadcrumb (current elements path) toolbar. If everything is removed then the menu will not be shown.
  Parameters: popUp - The pop-up Menu. authorAccess - Access class to the author functions. currentNode - The current node on which the popup is shown. Since: 18.1
### customizeTextPopUpMenu

public void customizeTextPopUpMenu([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUp, [WSTextEditorPage](../../editor/page/text/WSTextEditorPage.md) textPage)

Customize a pop-up menu in the Text page before showing it. If everything is removed then the menu will not be shown.
  Parameters: popUp - The pop-up Menu. textPage - The page over which the pop-up will be presented.
### customizeDITAMapPopUpMenu

public void customizeDITAMapPopUpMenu([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUp, [WSDITAMapEditorPage](../../editor/page/ditamap/WSDITAMapEditorPage.md) ditaMapEditorPage)

Customize a pop-up menu in the DITA Maps Manager page before showing it. If everything is removed then the menu will not be shown.
  Parameters: popUp - The pop-up Menu. ditaMapEditorPage - The DITA Map editor page access.
### customizeEditorTabPopUpMenu

public void customizeEditorTabPopUpMenu([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUpMenu, [WSEditor](../../editor/WSEditor.md) editor)

Customize the pop-up menu shown when right-clicking the tab of an editor (where the filename is presented). Editor tabs from both the main editing area and the DITA Maps Manager are taken into account.
  Parameters: popUpMenu - The pop-up menu to customize. editor - The current editor, on whose tab the pop-up menu has been invoked. Since: 19.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
