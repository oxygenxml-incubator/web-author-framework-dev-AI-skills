Package [ro.sync.ecss.extensions.api.node](package-summary.md)

# Interface ArtificialNode
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ArtificialNode
Marker interface for artificial elements which wrap Processing Instructions, CData and Comments allowing access to the wrapped node. Call backs with implementations of the interface are made on the [StylesFilter](../StylesFilter.md) when requesting styles for processing instructions, comments and CData.
  Since: 13
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorNode](AuthorNode.md) [getWrappedNode](#getWrappedNode())()
Get the real node wrapped by this interface.

## Method Details

### getWrappedNode

[AuthorNode](AuthorNode.md) getWrappedNode()

Get the real node wrapped by this interface.
  Returns: The wrapped node.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
