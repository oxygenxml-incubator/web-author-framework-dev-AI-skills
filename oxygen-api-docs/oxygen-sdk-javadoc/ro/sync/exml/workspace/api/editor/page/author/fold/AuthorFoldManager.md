Package [ro.sync.exml.workspace.api.editor.page.author.fold](package-summary.md)

# Interface AuthorFoldManager
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorFoldManager
Interface which can be used to expand/collapse foldable nodes. The CSS is used to mark nodes as foldable: https://www.oxygenxml.com/doc/ug-oxygen/#topics/dg-folding-elements.html
  Since: 17
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [collapseFold](#collapseFold(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) node)
If the node's fold is expanded, collapse it.
  void [expandFold](#expandFold(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) node)
If the node is folded, expand it.
  boolean [isFoldable](#isFoldable(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) node)
Check if a particular node is foldable.
  boolean [isFolded](#isFolded(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) node)
Check if a particular node is folded.

## Method Details

### isFoldable

boolean isFoldable([AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) node)

Check if a particular node is foldable.
  Parameters: node - The Author Node. Returns: true if the node can be folded.
### isFolded

boolean isFolded([AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) node)

Check if a particular node is folded.
  Parameters: node - The Author Node. Returns: true if the node is folded.
### expandFold

void expandFold([AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) node)

If the node is folded, expand it.
  Parameters: node - The Author Node.
### collapseFold

void collapseFold([AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) node)

If the node's fold is expanded, collapse it.
  Parameters: node - The Author Node.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
