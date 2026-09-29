Package [ro.sync.ecss.extensions.api.node](package-summary.md)

# Interface AuthorParentNode
    All Superinterfaces: [AuthorNode](AuthorNode.md)   All Known Subinterfaces: [AuthorDocument](AuthorDocument.md), [AuthorElement](AuthorElement.md), [AuthorElementBaseInterface](../AuthorElementBaseInterface.md), [AuthorReferenceNode](AuthorReferenceNode.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorParentNodeextends [AuthorNode](AuthorNode.md)
An author parent node contains a list of children.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.node.[AuthorNode](AuthorNode.md)
 [NODE_NAME_CDATA](AuthorNode.md#NODE_NAME_CDATA), [NODE_NAME_COMMENT](AuthorNode.md#NODE_NAME_COMMENT), [NODE_NAME_DOCUMENT](AuthorNode.md#NODE_NAME_DOCUMENT), [NODE_NAME_PI](AuthorNode.md#NODE_NAME_PI), [NODE_NAME_REFERENCE](AuthorNode.md#NODE_NAME_REFERENCE), [NODE_TYPE_CDATA](AuthorNode.md#NODE_TYPE_CDATA), [NODE_TYPE_COMMENT](AuthorNode.md#NODE_TYPE_COMMENT), [NODE_TYPE_DOCUMENT](AuthorNode.md#NODE_TYPE_DOCUMENT), [NODE_TYPE_ELEMENT](AuthorNode.md#NODE_TYPE_ELEMENT), [NODE_TYPE_PI](AuthorNode.md#NODE_TYPE_PI), [NODE_TYPE_PSEUDO_DOCTYPE](AuthorNode.md#NODE_TYPE_PSEUDO_DOCTYPE), [NODE_TYPE_PSEUDO_ELEMENT](AuthorNode.md#NODE_TYPE_PSEUDO_ELEMENT), [NODE_TYPE_REFERENCE](AuthorNode.md#NODE_TYPE_REFERENCE), [NODE_TYPE_TEXT](AuthorNode.md#NODE_TYPE_TEXT)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> [getContentNodes](#getContentNodes())()
Returns the list with all children of this element.
  [AuthorElementBaseInterface](../AuthorElementBaseInterface.md) [getParentElement](#getParentElement())()
Get the parent element of the node.

### Methods inherited from interface ro.sync.ecss.extensions.api.node.[AuthorNode](AuthorNode.md)
 [getContentIterator](AuthorNode.md#getContentIterator()), [getDisplayName](AuthorNode.md#getDisplayName()), [getEndOffset](AuthorNode.md#getEndOffset()), [getName](AuthorNode.md#getName()), [getNamespace](AuthorNode.md#getNamespace()), [getNamespaceContext](AuthorNode.md#getNamespaceContext()), [getOwnerDocument](AuthorNode.md#getOwnerDocument()), [getParent](AuthorNode.md#getParent()), [getStartOffset](AuthorNode.md#getStartOffset()), [getTextContent](AuthorNode.md#getTextContent()), [getType](AuthorNode.md#getType()), [getXMLBaseURL](AuthorNode.md#getXMLBaseURL()), [isDescendentOf](AuthorNode.md#isDescendentOf(ro.sync.ecss.extensions.api.node.AuthorNode))
## Method Details

### getContentNodes

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> getContentNodes()

Returns the list with all children of this element.
  Returns: The list that contains all children of this node without text nodes. Warning: Used to iterate a node's children. Do not modify. Never null.
### getParentElement

[AuthorElementBaseInterface](../AuthorElementBaseInterface.md) getParentElement()

Get the parent element of the node. Skips nodes which should be considered as transparent when matching the CSS selectors like reference nodes.
  Returns: The parent element, or null. Since: 13.2
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
