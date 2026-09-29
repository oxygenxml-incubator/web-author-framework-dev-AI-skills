Package [ro.sync.exml.workspace.api.editor.page.author.actions](package-summary.md)

# Interface AuthorActionsProvider
    All Superinterfaces: [ActionsProvider](ActionsProvider.md), [CommonActionsProvider](../../../../actions/CommonActionsProvider.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorActionsProviderextends [ActionsProvider](ActionsProvider.md)
Provides access to actions defined in the Author page.
  Since: 12.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> [getAuthorCommonActions](#getAuthorCommonActions())()
Get the map of author common actions (undo, redo, cut, copy, paste, etc).
  [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> [getAuthorExtensionActions](#getAuthorExtensionActions())()
Get the map of author extension actions.
  void [invokeAuthorExtensionActionInContext](#invokeAuthorExtensionActionInContext(java.lang.Object,int))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action, int offset)
If an Author extension action which was contributed in the document type configuration was obtained using one of the methods in this interface this method provides means to invoke an action on AWT thread (for the standalone distribution) or SWT thread (for the eclipse distribution) and have it executed at a certain offset.

### Methods inherited from interface ro.sync.exml.workspace.api.actions.[CommonActionsProvider](../../../../actions/CommonActionsProvider.md)
 [addActionPerformedListener](../../../../actions/CommonActionsProvider.md#addActionPerformedListener(java.lang.Object,ro.sync.exml.workspace.api.editor.page.author.actions.ActionPerformedListener)), [getActionID](../../../../actions/CommonActionsProvider.md#getActionID(java.lang.Object)), [invokeAction](../../../../actions/CommonActionsProvider.md#invokeAction(java.lang.Object)), [removeActionPerformedListener](../../../../actions/CommonActionsProvider.md#removeActionPerformedListener(java.lang.Object,ro.sync.exml.workspace.api.editor.page.author.actions.ActionPerformedListener))
## Method Details

### getAuthorCommonActions

[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> getAuthorCommonActions()

Get the map of author common actions (undo, redo, cut, copy, paste, etc).
  Returns: The map with (action id, Action) pairs with the actions defined for working in the Author. If the standalone Oxygen implementation is used, the actions are instance of javax.swing.Action If the eclipse plugin Oxygen implementation is used, the actions are instance of org.eclipse.jface.action.Action
### getAuthorExtensionActions

[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> getAuthorExtensionActions()

Get the map of author extension actions. Can be null if the author page does not have an associated document type. This should get called after each load as the extension actions depend on the loaded document type.
  Returns: The map with (action id, Action) pairs with the actions defined in the Author framework. Can be null if no actions available. If the standalone Oxygen implementation is used, the actions are instance of javax.swing.Action If the eclipse plugin Oxygen implementation is used, the actions are instance of org.eclipse.jface.action.Action Since: 12.1
### invokeAuthorExtensionActionInContext

void invokeAuthorExtensionActionInContext([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action, int offset)

If an Author extension action which was contributed in the document type configuration was obtained using one of the methods in this interface this method provides means to invoke an action on AWT thread (for the standalone distribution) or SWT thread (for the eclipse distribution) and have it executed at a certain offset. If the action is not an extension action, the method runs it without a context offset. The action will be invoked only if it is enabled in the execution context offset.
  Parameters: action - The action to invoke offset - The offset in the document where to invoke the action. Since: 16
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
