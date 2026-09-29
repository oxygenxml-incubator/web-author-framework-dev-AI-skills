Package [ro.sync.exml.workspace.api.actions](package-summary.md)

# Interface CommonActionsProvider
    All Known Subinterfaces: [ActionsProvider](../editor/page/author/actions/ActionsProvider.md), [ActionsProvider](../standalone/actions/ActionsProvider.md), [AuthorActionsProvider](../editor/page/author/actions/AuthorActionsProvider.md), [DITAMapActionsProvider](../editor/page/ditamap/actions/DITAMapActionsProvider.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface CommonActionsProvider
Provides access to actions.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addActionPerformedListener](#addActionPerformedListener(java.lang.Object,ro.sync.exml.workspace.api.editor.page.author.actions.ActionPerformedListener))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action, [ActionPerformedListener](../editor/page/author/actions/ActionPerformedListener.md) listener)
Add a listener which gets triggered before and after a certain action is triggered.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getActionID](#getActionID(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) actionOrUIObject)
Get an unique ID (which does not depend on the action name) for an action Oxygen has mounted on the main JMenuBar or on the toolbars or for an UI component like a JMenuItem or a JButton provided by Oxygen.
  void [invokeAction](#invokeAction(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action)
If an action was obtained using one of the methods in this interface this method provides means to invoke an action on AWT thread (for the standalone distribution) or SWT thread (for the eclipse distribution).
  void [removeActionPerformedListener](#removeActionPerformedListener(java.lang.Object,ro.sync.exml.workspace.api.editor.page.author.actions.ActionPerformedListener))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action, [ActionPerformedListener](../editor/page/author/actions/ActionPerformedListener.md) listener)
Remove the listener which gets triggered before and after a certain action is triggered.

## Method Details

### invokeAction

void invokeAction([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action)

If an action was obtained using one of the methods in this interface this method provides means to invoke an action on AWT thread (for the standalone distribution) or SWT thread (for the eclipse distribution). The action will be invoked only if it is enabled in the current context.
  Parameters: action - The action to invoke Since: 12.1
### getActionID

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getActionID([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) actionOrUIObject)

Get an unique ID (which does not depend on the action name) for an action Oxygen has mounted on the main JMenuBar or on the toolbars or for an UI component like a JMenuItem or a JButton provided by Oxygen. If the action appears on a contextual menu but is not installed on a main menu it will be prefixed with the constant "ACTION_WITH_NO_SHORTCUT/"
  Parameters: actionOrUIObject - The action or UI component for which to retrieve the ID. Returns: The unique human-readable ID which does not depend on the user interface language or null if the ID could not be determined. Since: 13.2
### addActionPerformedListener

void addActionPerformedListener([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action, [ActionPerformedListener](../editor/page/author/actions/ActionPerformedListener.md) listener)

Add a listener which gets triggered before and after a certain action is triggered.
  Parameters: action - The action on which to add the listener. listener - The listener. Since: 15
### removeActionPerformedListener

void removeActionPerformedListener([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) action, [ActionPerformedListener](../editor/page/author/actions/ActionPerformedListener.md) listener)

Remove the listener which gets triggered before and after a certain action is triggered.
  Parameters: action - The action. listener - The listener. Since: 15
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
