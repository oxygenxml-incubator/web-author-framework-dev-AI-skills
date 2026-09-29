Package [ro.sync.exml.workspace.api.standalone.actions](package-summary.md)

# Interface ActionsProvider
    All Superinterfaces: [CommonActionsProvider](../../actions/CommonActionsProvider.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ActionsProviderextends [CommonActionsProvider](../../actions/CommonActionsProvider.md)
Provides access to global actions in the entire workbench.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> [getGlobalActions](#getGlobalActions())()
Get the map of global actions usually mounted on the main menu.
  void [registerAction](#registerAction(java.lang.String,java.lang.Object,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) actionID, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultKeyStroke)
Register a new global action.
  void [unregisterAction](#unregisterAction(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) actionID)
Unregister a global action.

### Methods inherited from interface ro.sync.exml.workspace.api.actions.[CommonActionsProvider](../../actions/CommonActionsProvider.md)
 [addActionPerformedListener](../../actions/CommonActionsProvider.md#addActionPerformedListener(java.lang.Object,ro.sync.exml.workspace.api.editor.page.author.actions.ActionPerformedListener)), [getActionID](../../actions/CommonActionsProvider.md#getActionID(java.lang.Object)), [invokeAction](../../actions/CommonActionsProvider.md#invokeAction(java.lang.Object)), [removeActionPerformedListener](../../actions/CommonActionsProvider.md#removeActionPerformedListener(java.lang.Object,ro.sync.exml.workspace.api.editor.page.author.actions.ActionPerformedListener))
## Method Details

### getGlobalActions

[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> getGlobalActions()

Get the map of global actions usually mounted on the main menu.
  Returns: The map with (action id, Action) pairs. Since: 18
### registerAction

void registerAction([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) actionID, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultKeyStroke)

Register a new global action. The action shortcut will be visible in the Oxygen menu shortcut keys table. If the action uses a shortcut which is not used by other Oxygen actions, the shortcut will work even if you do not add the action to an existing menu.
  Parameters: actionID - The action ID. An unique ID which you provide for your action... action - The action. It must be an instance of javax.swing.Action. It can have a default keystroke... defaultKeyStroke - The default action key stroke string representation. You can use platform-dependent strokes like "Ctrl Alt X" or platform-independent strokes like "M1 M3 X" where:
        * M1 represents the Command key on MacOS X, and the Ctrl key on other platforms.
        * M2 represents the Shift key.
        * M3 represents the Option key on MacOS X, and the Alt key on other platforms.
        * M4 represents the Ctrl key on MacOS X, and is undefined on other platforms.
 Since: 18
### unregisterAction

void unregisterAction([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) actionID)

Unregister a global action.
  Parameters: actionID - The action ID. Since: 18
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
