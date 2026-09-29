Package [ro.sync.exml.workspace.api.editor.page.author.tooltip](package-summary.md)

# Interface AuthorTooltipCustomizerProvider
    All Known Subinterfaces: [AuthorEditorAccess](../../../../../../../ecss/extensions/api/access/AuthorEditorAccess.md), [IWebappAuthorEditorAccess](../../../../../../../ecss/extensions/api/webapp/access/IWebappAuthorEditorAccess.md), [WSAuthorComponentEditorPage](../WSAuthorComponentEditorPage.md), [WSAuthorEditorPage](../WSAuthorEditorPage.md), [WSAuthorEditorPageBase](../WSAuthorEditorPageBase.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorTooltipCustomizerProvider
Allow developers to add tooltip customizers for customizing the tooltips which appear when hovering in the visual Author editing mode.
  Since: 18
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addTooltipCustomizer](#addTooltipCustomizer(ro.sync.exml.workspace.api.editor.page.author.tooltip.AuthorTooltipCustomizer))([AuthorTooltipCustomizer](AuthorTooltipCustomizer.md) tooltipCustomizer)
Add a tooltip customizer.
  void [removeTooltipCustomizer](#removeTooltipCustomizer(ro.sync.exml.workspace.api.editor.page.author.tooltip.AuthorTooltipCustomizer))([AuthorTooltipCustomizer](AuthorTooltipCustomizer.md) tooltipCustomizer)
Remove a tooltip customizer.

## Method Details

### addTooltipCustomizer

void addTooltipCustomizer([AuthorTooltipCustomizer](AuthorTooltipCustomizer.md) tooltipCustomizer)

Add a tooltip customizer. The customizer can be used to customize the description shown when hovering the Author page.
  Parameters: tooltipCustomizer - The tooltip customizer.
### removeTooltipCustomizer

void removeTooltipCustomizer([AuthorTooltipCustomizer](AuthorTooltipCustomizer.md) tooltipCustomizer)

Remove a tooltip customizer.
  Parameters: tooltipCustomizer - The tooltip customizer.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
