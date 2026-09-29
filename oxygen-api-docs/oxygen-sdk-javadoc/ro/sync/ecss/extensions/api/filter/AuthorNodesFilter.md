Package [ro.sync.ecss.extensions.api.filter](package-summary.md)

# Interface AuthorNodesFilter
    @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorNodesFilter
Provides information about the Author nodes that should be filtered.
  Since: 12.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [shouldFilterNode](#shouldFilterNode(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../node/AuthorNode.md) authorNode)
Checks if an Author Node should be filtered.

## Method Details

### shouldFilterNode

boolean shouldFilterNode([AuthorNode](../node/AuthorNode.md) authorNode)

Checks if an Author Node should be filtered.
  Parameters: authorNode - The Author node. Returns: True if the author node should be filtered.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
