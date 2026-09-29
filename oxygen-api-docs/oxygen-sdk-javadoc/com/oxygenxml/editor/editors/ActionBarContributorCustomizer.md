Package [com.oxygenxml.editor.editors](package-summary.md)

# Class ActionBarContributorCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * com.oxygenxml.editor.editors.ActionBarContributorCustomizer
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ActionBarContributorCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Abstract class allowed as an extension point to customize the menu and toolbar buttons added by our editors. In your plugin in the plugin.xml you should reference it like:
```

  <extension point="oxygen.plugin.id.actionBarContributorCustomizer">
     <implementation class="my.package.CustomActionBarContributorCustomizer"/>;
    </extension>

```

  Since: 14.1
## Constructor Summary
 Constructors
Constructor

Description
 [ActionBarContributorCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> [customizeActionsContributedToDocumentMenu](#customizeActionsContributedToDocumentMenu(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> actions)
Customize the actions before they are contributed to the main Document menu (XML or XSL, or XSD, etc).
  abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> [customizeActionsContributedToDocumentToolbar](#customizeActionsContributedToDocumentToolbar(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> actions)
Customize the actions before they are contributed to the main Document toolbar.
  void [customizeAuthorBreadcrumbPopUpMenu](#customizeAuthorBreadcrumbPopUpMenu(org.eclipse.jface.action.IMenuManager,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode))(org.eclipse.jface.action.IMenuManager popUp, [AuthorAccess](../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) authorAccess, [AuthorNode](../../../../ro/sync/ecss/extensions/api/node/AuthorNode.md) currentNode)
Customize a pop-up menu about to be shown in the Author page Breadcrumb (current elements path) toolbar.
  void [customizeAuthorOutlinePopUpMenu](#customizeAuthorOutlinePopUpMenu(org.eclipse.jface.action.IMenuManager,ro.sync.ecss.extensions.api.AuthorAccess))(org.eclipse.jface.action.IMenuManager popUp, [AuthorAccess](../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) authorAccess)
Customize a pop-up menu about to be shown in the Author page Outline view.
  void [customizeAuthorPageExtensionMenu](#customizeAuthorPageExtensionMenu(org.eclipse.jface.action.IMenuManager,ro.sync.ecss.extensions.api.AuthorAccess))(org.eclipse.jface.action.IMenuManager extensionMenu, [AuthorAccess](../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) authorAccess)
Customize an extension main menu contributed by the Author page document type configuration.
  void [customizeAuthorPageExtensionToolbar](#customizeAuthorPageExtensionToolbar(org.eclipse.jface.action.IToolBarManager,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))(org.eclipse.jface.action.IToolBarManager extensionToolbar, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toolbarID, [AuthorAccess](../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) authorAccess)
Customize an extension toolbar contributed by the Author page document type configuration.
  abstract void [customizeAuthorPageInternalCoolbar](#customizeAuthorPageInternalCoolbar(org.eclipse.swt.widgets.CoolBar,ro.sync.exml.workspace.api.editor.page.author.WSAuthorEditorPage))(org.eclipse.swt.widgets.CoolBar coolbar, [WSAuthorEditorPage](../../../../ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPage.md) authorEditorPage)
Customize an internal coolbar for a cetain author page.
  void [customizeAuthorPopUpMenu](#customizeAuthorPopUpMenu(org.eclipse.jface.action.IMenuManager,ro.sync.ecss.extensions.api.AuthorAccess))(org.eclipse.jface.action.IMenuManager popUp, [AuthorAccess](../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) authorAccess)
Customize a pop-up menu in the Author page before showing it.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> [customizeDITAMapsManagerExtendedToolbar](#customizeDITAMapsManagerExtendedToolbar(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> toolbarActions)
Customize the DITA Maps Manager extended toolbar.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> [customizeDITAMapsManagerMainToolbar](#customizeDITAMapsManagerMainToolbar(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> toolbarActions)
Customize the DITA Maps Manager main toolbar.
  void [customizeTextPopUpMenu](#customizeTextPopUpMenu(org.eclipse.jface.action.IMenuManager,ro.sync.exml.workspace.api.editor.page.text.WSTextEditorPage))(org.eclipse.jface.action.IMenuManager popUp, [WSTextEditorPage](../../../../ro/sync/exml/workspace/api/editor/page/text/WSTextEditorPage.md) textPage)
Customize a pop-up menu in the Text page before showing it.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ActionBarContributorCustomizer

public ActionBarContributorCustomizer()

## Method Details

### customizeActionsContributedToDocumentMenu

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> customizeActionsContributedToDocumentMenu([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> actions)

Customize the actions before they are contributed to the main Document menu (XML or XSL, or XSD, etc).
  Parameters: actions - The list of original actions. Returns: The list of actions to be presented in the menu.
### customizeActionsContributedToDocumentToolbar

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> customizeActionsContributedToDocumentToolbar([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> actions)

Customize the actions before they are contributed to the main Document toolbar. Drop down actions implement the interface "com.oxygenxml.editor.editors.IDropDownMenuAction" in order to be able to set a customized for the drop down actions list.
  Parameters: actions - The list of original actions. Returns: The list of actions to be presented in the toolbar.
### customizeAuthorPageExtensionMenu

public void customizeAuthorPageExtensionMenu(org.eclipse.jface.action.IMenuManager extensionMenu, [AuthorAccess](../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) authorAccess)

Customize an extension main menu contributed by the Author page document type configuration. For example DITA, Docbook, etc...
  Parameters: extensionMenu - The extension menu. authorAccess - Access class to the author functions. Since: 17
### customizeAuthorPageExtensionToolbar

public void customizeAuthorPageExtensionToolbar(org.eclipse.jface.action.IToolBarManager extensionToolbar, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toolbarID, [AuthorAccess](../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) authorAccess)

Customize an extension toolbar contributed by the Author page document type configuration. The toolbar will be included in the Author internal coolbar. An extension toolbar contains actions belonging to the specific support the application offers for a certain vocabulary.
  Parameters: extensionToolbar - The extension toolbar. toolbarID - The toolbar ID. authorAccess - Access class to the author functions. Since: 17
### customizeAuthorPageInternalCoolbar

public abstract void customizeAuthorPageInternalCoolbar(org.eclipse.swt.widgets.CoolBar coolbar, [WSAuthorEditorPage](../../../../ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPage.md) authorEditorPage)

Customize an internal coolbar for a cetain author page. This callback may be received more than once for the same document so please make sure that you do not add the same action twice. Calling getData("OXYGEN_ID") on each widget in the coolbar should give you more information about the action it was created from.
```

 CoolItem[] items = coolbar.getItems();
 for (CoolItem coolItem : items) {
   Control control = coolItem.getControl();
   Object oxygenID = control.getData("OXYGEN_ID");
   System.out.println(oxygenID);
   if (control instanceof ToolBar) {
     ToolBar toolBar = (ToolBar) control;
     ToolItem[] tollbarItems = toolBar.getItems();
     for (ToolItem toolItem : tollbarItems) {
       System.out.println("   " + toolItem.getData("OXYGEN_ID"));
     }
   }
 }

```
If you want to remove an item from the coolbar you can use:
```

 CoolItem[] items = coolbar.getItems();
 CoolItem coolItem = items[1];

 coolItem.setControl(new Label(coolbar, SWT.NONE));

 coolItem.setMinimumSize(0, 0);
 coolItem.setSize(new Point(0, 0));

 coolbar.update();

```
If you want to remove actions from drop-down buttons you can cast them to a special interface "com.oxygenxml.editor.editors.xml.IDropDownToolItem" and add an actions filter to them. For example the following code removes the first two actions from the "Profiling" drop-down button:
```

          CoolItem[] items = coolbar.getItems();
          for (CoolItem coolItem : items) {
            Control control = coolItem.getControl();
            if (control instanceof ToolBar) {
              ToolBar toolBar = (ToolBar) control;
              ToolItem[] tollbarItems = toolBar.getItems();
              for (ToolItem toolItem : tollbarItems) {
                if("Profiling".equals(toolItem.getData("OXYGEN_ID"))){
                  //Remove it
                  if(toolItem instanceof IDropDownToolItem){
                    ((IDropDownToolItem)toolItem).addActionsListFilter(new ActionsListFilter() {
                     public void filterActions(List<IAction> actions) {
                       for (int i = actions.size() - 1; i >= 0; i--) {
                         IAction action = actions.get(i);
                         if(action != null){
                           if("Profiling_Condition_Sets/Apply_profiling_styles".equals(action.getId())
                               || "Profiling_Condition_Sets/Show_Profiling_Attributes".equals(action.getId())){
                             actions.remove(i);
                           }
                         }
                       }
                     }
                   });
                  }
                }
              }
            }
         }

```

  Parameters: coolbar - The internal coolbar after the fixed actions have been added. authorEditorPage - The current author editor page.
### customizeDITAMapsManagerExtendedToolbar

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> customizeDITAMapsManagerExtendedToolbar([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> toolbarActions)

Customize the DITA Maps Manager extended toolbar.
  Parameters: toolbarActions - The current list of actions which will be added. Returns: The list of actions to be presented in the toolbar. Since: 17
### customizeDITAMapsManagerMainToolbar

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> customizeDITAMapsManagerMainToolbar([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<org.eclipse.jface.action.IAction> toolbarActions)

Customize the DITA Maps Manager main toolbar.
  Parameters: toolbarActions - The current list of actions which will be added. Returns: The list of actions to present in the main toolbar. Since: 17
### customizeAuthorPopUpMenu

public void customizeAuthorPopUpMenu(org.eclipse.jface.action.IMenuManager popUp, [AuthorAccess](../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) authorAccess)

Customize a pop-up menu in the Author page before showing it. If everything is removed then the menu will not be shown.By default this method gets called for both the contextual menu shown in the main editing area, shown in the Outline view or shown in the Breadcrumb.
  Parameters: popUp - The pop-up Menu. authorAccess - Access class to the author functions. Since: 17
### customizeAuthorOutlinePopUpMenu

public void customizeAuthorOutlinePopUpMenu(org.eclipse.jface.action.IMenuManager popUp, [AuthorAccess](../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) authorAccess)

Customize a pop-up menu about to be shown in the Author page Outline view. If everything is removed then the menu will not be shown.
  Parameters: popUp - The pop-up Menu. authorAccess - Access class to the author functions. Since: 18.1
### customizeAuthorBreadcrumbPopUpMenu

public void customizeAuthorBreadcrumbPopUpMenu(org.eclipse.jface.action.IMenuManager popUp, [AuthorAccess](../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) authorAccess, [AuthorNode](../../../../ro/sync/ecss/extensions/api/node/AuthorNode.md) currentNode)

Customize a pop-up menu about to be shown in the Author page Breadcrumb (current elements path) toolbar. If everything is removed then the menu will not be shown.
  Parameters: popUp - The pop-up Menu. authorAccess - Access class to the author functions. currentNode - The current node on which the popup is shown. Since: 18.1
### customizeTextPopUpMenu

public void customizeTextPopUpMenu(org.eclipse.jface.action.IMenuManager popUp, [WSTextEditorPage](../../../../ro/sync/exml/workspace/api/editor/page/text/WSTextEditorPage.md) textPage)

Customize a pop-up menu in the Text page before showing it. If everything is removed then the menu will not be shown.
  Parameters: popUp - The pop-up Menu. textPage - The page over which the pop-up will be presented. Since: 17
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
