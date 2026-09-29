Package [ro.sync.exml.workspace.api.editor.page.ditamap.keys](package-summary.md)

# Interface KeyDefinitionManagerProvider
    @API(type=EXTENDABLE, src=PUBLIC) public interface KeyDefinitionManagerProvider
Provides the keys manager for an opened document.
  Since: 19.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [KeyDefinitionManager](KeyDefinitionManager.md) [getKeyDefinitionManager](#getKeyDefinitionManager(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess)
Returns the keys manager for an opened document.

## Method Details

### getKeyDefinitionManager

[KeyDefinitionManager](KeyDefinitionManager.md) getKeyDefinitionManager([AuthorAccess](../../../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess)

Returns the keys manager for an opened document.
  Parameters: authorAccess - The author access for an opened document. Returns: a [KeyDefinitionManager](KeyDefinitionManager.md) instance.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
