Package [ro.sync.exml.workspace.api.editor.page.author.actions](package-summary.md)

# Interface ActionsProvider
    All Superinterfaces: [CommonActionsProvider](../../../../actions/CommonActionsProvider.md)   All Known Subinterfaces: [AuthorActionsProvider](AuthorActionsProvider.md), [DITAMapActionsProvider](../../ditamap/actions/DITAMapActionsProvider.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ActionsProviderextends [CommonActionsProvider](../../../../actions/CommonActionsProvider.md)
Provides access to actions defined in the Author page. You can obtain an action with a certain ID, invoke it or add before or after listeners to it.

## Method Summary

### Methods inherited from interface ro.sync.exml.workspace.api.actions.[CommonActionsProvider](../../../../actions/CommonActionsProvider.md)
 [addActionPerformedListener](../../../../actions/CommonActionsProvider.md#addActionPerformedListener(java.lang.Object,ro.sync.exml.workspace.api.editor.page.author.actions.ActionPerformedListener)), [getActionID](../../../../actions/CommonActionsProvider.md#getActionID(java.lang.Object)), [invokeAction](../../../../actions/CommonActionsProvider.md#invokeAction(java.lang.Object)), [removeActionPerformedListener](../../../../actions/CommonActionsProvider.md#removeActionPerformedListener(java.lang.Object,ro.sync.exml.workspace.api.editor.page.author.actions.ActionPerformedListener))
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
