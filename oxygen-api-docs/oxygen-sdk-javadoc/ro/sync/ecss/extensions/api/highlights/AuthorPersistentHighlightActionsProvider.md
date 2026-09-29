Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Interface AuthorPersistentHighlightActionsProvider
    @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorPersistentHighlightActionsProvider
The provider for contextual actions that are shown on the contextual menu of the persistent highlight (in the main editor area - not yet supported) and on the associated callout. You can set such a provider by using the [AuthorPersistentHighlighter.setHighlightsActionsProvider(AuthorPersistentHighlightActionsProvider)](AuthorPersistentHighlighter.md#setHighlightsActionsProvider(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightActionsProvider))method.
  Since: 14
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> [getActions](#getActions(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)
Gets the available actions for a persistent highlight.
  [AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html) [getDefaultAction](#getDefaultAction(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)
Gets the action that will be invoked when the user double clicks a callout representation, or a persistent highlight in the main editing area (not yet supported).

## Method Details

### getActions

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html)> getActions([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)

Gets the available actions for a persistent highlight. This method is called only for the highlights that have a a callout associated. Only the following action properties are used in oXygen Eclipse plugin: [Action.SMALL_ICON](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#SMALL_ICON) is used as action image in the menu and [Action.NAME](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#NAME) is used as action name (label). In the future, this will be called also for the custom persistent highlights that are displayed in the main editing area. To associate callout information to custom persistent highlights use the method [AuthorCalloutsController.setCalloutsRenderingInformationProvider(ro.sync.ecss.extensions.api.callouts.CalloutsRenderingInformationProvider)](../callouts/AuthorCalloutsController.md#setCalloutsRenderingInformationProvider(ro.sync.ecss.extensions.api.callouts.CalloutsRenderingInformationProvider))
  Parameters: highlight - The highlight for which the actions are requested. Never null. Returns: The list of actions available for the highlight, or null if there is no action available for the context highlight. The list can contain null entries for separators.
### getDefaultAction

[AbstractAction](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractAction.html) getDefaultAction([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)

Gets the action that will be invoked when the user double clicks a callout representation, or a persistent highlight in the main editing area (not yet supported).
Is not necessary that this action to be included in the ones returned by [getActions(AuthorPersistentHighlight)](#getActions(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight)).

  Parameters: highlight - The highlight for which the default action is requested. Never null. Returns: The default action available for the highlight, or null if there is no action available for the context highlight.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
