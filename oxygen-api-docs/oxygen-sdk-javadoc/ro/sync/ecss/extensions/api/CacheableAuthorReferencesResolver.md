Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface CacheableAuthorReferencesResolver
    All Known Implementing Classes: [DITAConRefResolver](../dita/conref/DITAConRefResolver.md), [DITAMapRefResolver](../dita/map/topicref/DITAMapRefResolver.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface CacheableAuthorReferencesResolver
Marker for cachable references resolvers.

## Method Summary
  All MethodsInstance MethodsDefault Methods
Modifier and Type

Method

Description
 default [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCacheKey](#getCacheKey(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) nodeWithReference)
Get an unique cache key for a node which references content which will be expanded.

## Method Details

### getCacheKey

default [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCacheKey([AuthorNode](node/AuthorNode.md) nodeWithReference)

Get an unique cache key for a node which references content which will be expanded.
  Parameters: nodeWithReference - The node. Returns: an unique cache key for a node which references expanded content. Can be null if the node should not be cached.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
