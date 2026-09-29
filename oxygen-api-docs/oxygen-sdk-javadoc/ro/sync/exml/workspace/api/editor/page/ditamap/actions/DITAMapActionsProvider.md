Package [ro.sync.exml.workspace.api.editor.page.ditamap.actions](package-summary.md)

# Interface DITAMapActionsProvider
    All Superinterfaces: [ActionsProvider](../../author/actions/ActionsProvider.md), [CommonActionsProvider](../../../../actions/CommonActionsProvider.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface DITAMapActionsProviderextends [ActionsProvider](../../author/actions/ActionsProvider.md)
Provides access to actions defined in the DITA Map editor page.
  Since: 15.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> [getActions](#getActions())()
Get the map of DITA Map common actions (undo, redo, cut, copy, paste, etc).

### Methods inherited from interface ro.sync.exml.workspace.api.actions.[CommonActionsProvider](../../../../actions/CommonActionsProvider.md)
 [addActionPerformedListener](../../../../actions/CommonActionsProvider.md#addActionPerformedListener(java.lang.Object,ro.sync.exml.workspace.api.editor.page.author.actions.ActionPerformedListener)), [getActionID](../../../../actions/CommonActionsProvider.md#getActionID(java.lang.Object)), [invokeAction](../../../../actions/CommonActionsProvider.md#invokeAction(java.lang.Object)), [removeActionPerformedListener](../../../../actions/CommonActionsProvider.md#removeActionPerformedListener(java.lang.Object,ro.sync.exml.workspace.api.editor.page.author.actions.ActionPerformedListener))
## Method Details

### getActions

[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> getActions()

Get the map of DITA Map common actions (undo, redo, cut, copy, paste, etc).
  Returns: The map with (action id, Action) pairs with the actions defined for working in the Author. If the standalone Oxygen implementation is used, the actions are instance of javax.swing.Action If the eclipse plugin Oxygen implementation is used, the actions are instance of org.eclipse.jface.action.Action
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
