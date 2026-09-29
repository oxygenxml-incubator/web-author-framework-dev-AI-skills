Package [ro.sync.ecss.extensions.api.review](package-summary.md)

# Class ReviewActionsProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.review.ReviewActionsProvider
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ReviewActionsProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Provides a set of custom actions for a certain highlight. The actions will be mounted on the contextual menu when right clicking a review entry.
  Since: 17.1
## Constructor Summary
 Constructors
Constructor

Description
 [ReviewActionsProvider](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [customizeContextualMenuActions](#customizeContextualMenuActions(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight%5B%5D,java.lang.Object))([AuthorAccess](../AuthorAccess.md) authorAccess, [AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)[] selectedHighlights, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popupMenu)
Get the list of actions to show for a review entry.
  void [customizeHoverActions](#customizeHoverActions(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight,java.util.List))([AuthorAccess](../AuthorAccess.md) authorAccess, [AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) authorPersistentHighlight, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) actions)
Customize the list of actions which are shown when hovering the item.
  boolean [performCustomActionOnDelete](#performCustomActionOnDelete(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight%5B%5D))([AuthorAccess](../AuthorAccess.md) authorAccess, [AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)[] selectedHighlights)
This method is called when the DEL button is pressed in the review panel.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ReviewActionsProvider

public ReviewActionsProvider()

## Method Details

### customizeContextualMenuActions

public void customizeContextualMenuActions([AuthorAccess](../AuthorAccess.md) authorAccess, [AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)[] selectedHighlights, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popupMenu)

Get the list of actions to show for a review entry.
  Parameters: authorAccess - The Author access. selectedHighlights - The list of selected highlights popupMenu - The popup menu with default actions. (implementation of JPopupMenu on Swing or MenuManager on Eclipse).
### performCustomActionOnDelete

public boolean performCustomActionOnDelete([AuthorAccess](../AuthorAccess.md) authorAccess, [AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)[] selectedHighlights)

This method is called when the DEL button is pressed in the review panel.
  Parameters: authorAccess - The Author access. selectedHighlights - The list of selected highlights Returns: true if the API implementor will perform a custom delete action using for example methods in the AuthorChangeTrackingController API.
### customizeHoverActions

public void customizeHoverActions([AuthorAccess](../AuthorAccess.md) authorAccess, [AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) authorPersistentHighlight, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) actions)

Customize the list of actions which are shown when hovering the item. The actions are either Swing actions or SWT actions. For Swing actions you can use the API "ro.sync.exml.workspace.api.standalone.StandalonePluginWorkspace.getOxygenActionID(Action)" to query each action's ID.
  Parameters: authorAccess - The author access. authorPersistentHighlight - The current highlight. actions - The list of hover actions which appear by default when hovering a change/comment in the Review panel. You can add more actions to it, wrap existing actions or remove actions. Since: 18.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
