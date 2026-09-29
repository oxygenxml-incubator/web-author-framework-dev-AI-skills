Package [ro.sync.exml.workspace.api.editor.page.text.actions](package-summary.md)

# Interface TextActionsProvider
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface TextActionsProvider
Provides access to actions defined in the Text page.
  Since: 14.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getActionID](#getActionID(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action)
Get an unique ID (which does not depend on the action name) for an action Oxygen has mounted on the main JMenuBar or on the toolbars.
  [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> [getTextActions](#getTextActions())()
Get the map of Text actions (undo, redo, cut, copy, paste, etc).
  void [invokeAction](#invokeAction(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action)
If an action was obtained using one of the methods in this interface this method provides means to invoke an action on AWT thread (for the standalone distribution) or SWT thread (for the eclipse distribution).

## Method Details

### getTextActions

[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> getTextActions()

Get the map of Text actions (undo, redo, cut, copy, paste, etc).
  Returns: The map with (action id, Action) pairs with the actions defined for working in the Text page. If the standalone Oxygen implementation is used, the actions are instance of javax.swing.Action If the eclipse plugin Oxygen implementation is used, the actions are instance of org.eclipse.jface.action.Action
### invokeAction

void invokeAction([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action)

If an action was obtained using one of the methods in this interface this method provides means to invoke an action on AWT thread (for the standalone distribution) or SWT thread (for the eclipse distribution).
  Parameters: action - The action to invoke
### getActionID

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getActionID([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action)

Get an unique ID (which does not depend on the action name) for an action Oxygen has mounted on the main JMenuBar or on the toolbars. If the action appears on a contextual menu but is not installed on a main menu it will pe prefixed with the constant "ACTION_WITH_NO_SHORTCUT/"
  Parameters: action - The action for which to retrieve the ID. Returns: The unique ID or null if the action is not one provided by Oxygen.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
