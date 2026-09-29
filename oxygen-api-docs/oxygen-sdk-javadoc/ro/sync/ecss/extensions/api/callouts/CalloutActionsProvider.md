Package [ro.sync.ecss.extensions.api.callouts](package-summary.md)

# Class CalloutActionsProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.callouts.CalloutActionsProvider
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class CalloutActionsProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Provides a set of custom actions for a certain highlight. The actions will be mounted on the contextual menu when right clicking a callout.
  Since: 17
## Constructor Summary
 Constructors
Constructor

Description
 [CalloutActionsProvider](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> [getActions](#getActions(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight,java.util.List))([AuthorAccess](../AuthorAccess.md) authorAccess, [AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) highlight, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> defaultActionsList)
Get the list of actions to show for a callout in the contextual menu.
  [AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html) [getDefaultAction](#getDefaultAction(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight,java.util.List))([AuthorAccess](../AuthorAccess.md) authorAccess, [AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) highlight, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> actionsList)
Get the default action which is invoked when the user double clicks the callout.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CalloutActionsProvider

public CalloutActionsProvider()

## Method Details

### getActions

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> getActions([AuthorAccess](../AuthorAccess.md) authorAccess, [AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) highlight, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> defaultActionsList)

Get the list of actions to show for a callout in the contextual menu.
  Parameters: authorAccess - The Author access. highlight - The highlight for which the actions will be presented. defaultActionsList - The default list of actions which would be contributed by the standard implementation. The default actions list can be null when used with custom highlights. Returns: The final list of actions to show when right clicking a callout or an attribute with change tracking in the Attributes view.
### getDefaultAction

public [AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html) getDefaultAction([AuthorAccess](../AuthorAccess.md) authorAccess, [AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) highlight, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> actionsList)

Get the default action which is invoked when the user double clicks the callout.
  Parameters: authorAccess - The Author access. highlight - The highlight for which the actions will be presented. actionsList - The default list of actions which would be contributed by the standard implementation. Returns: The action which is invoked when a callout is double clicked. If the action provided by user is null, it returns the built-in action. Since: 19
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
