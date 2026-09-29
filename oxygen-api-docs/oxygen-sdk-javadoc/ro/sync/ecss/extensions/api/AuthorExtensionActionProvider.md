Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorExtensionActionProvider
    All Known Subinterfaces: [WebappActionsManager](webapp/WebappActionsManager.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorExtensionActionProvider
Provides an author extension action for a given action ID. These actions are configured in the associated document type of the current document.
  Since: 15.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [IAuthorExtensionAction](editor/IAuthorExtensionAction.md) [getExtensionAction](#getExtensionAction(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) actionID)
Gets the author extension action with the given action ID.
  [IAuthorExtensionAction](editor/IAuthorExtensionAction.md) [getExtensionAction](#getExtensionAction(ro.sync.ecss.css.functions.ActionLexicalUnit))(ro.sync.ecss.css.functions.ActionLexicalUnit actionLU)
Creates an action that comes from the CSS.

## Method Details

### getExtensionAction

[IAuthorExtensionAction](editor/IAuthorExtensionAction.md) getExtensionAction([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) actionID)

Gets the author extension action with the given action ID. These actions are configured in the associated document type of the current document.
  Parameters: actionID - Action ID. Returns: The extension action or null if not found.
### getExtensionAction

[IAuthorExtensionAction](editor/IAuthorExtensionAction.md) getExtensionAction(ro.sync.ecss.css.functions.ActionLexicalUnit actionLU)

Creates an action that comes from the CSS. These actions are defined directly into the CSS using the CSS oxy_action function.
  Parameters: actionLU - The Action lexical unit, containing all the properties. Returns: An new action, or null if the action cannot be built.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
