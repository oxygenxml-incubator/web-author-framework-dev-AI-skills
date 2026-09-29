Package [ro.sync.exml.workspace.api.editor.page.author](package-summary.md)

# Interface AuthorNodeRendererCustomizerContext
    All Known Subinterfaces: [DITAMapNodeRendererCustomizerContext](../ditamap/DITAMapNodeRendererCustomizerContext.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorNodeRendererCustomizerContext
Offers access to the current Author node (the one for which we are customizing the renderer).
  Since: 20.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) [getAuthorNode](#getAuthorNode())()
Get the current Author node, i.e.

## Method Details

### getAuthorNode

[AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) getAuthorNode()

Get the current Author node, i.e. the node for which we are customizing the rendering.
  Returns: the current Author node.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
