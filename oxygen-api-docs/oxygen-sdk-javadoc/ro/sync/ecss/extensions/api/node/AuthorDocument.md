Package [ro.sync.ecss.extensions.api.node](package-summary.md)

# Interface AuthorDocument
    All Superinterfaces: [AuthorNode](AuthorNode.md), [AuthorParentNode](AuthorParentNode.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorDocumentextends [AuthorParentNode](AuthorParentNode.md)
The Document interface represents the entire XML document. Conceptually, it is the root of the document tree, and provides the primary access to the document's data.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.node.[AuthorNode](AuthorNode.md)
 [NODE_NAME_CDATA](AuthorNode.md#NODE_NAME_CDATA), [NODE_NAME_COMMENT](AuthorNode.md#NODE_NAME_COMMENT), [NODE_NAME_DOCUMENT](AuthorNode.md#NODE_NAME_DOCUMENT), [NODE_NAME_PI](AuthorNode.md#NODE_NAME_PI), [NODE_NAME_REFERENCE](AuthorNode.md#NODE_NAME_REFERENCE), [NODE_TYPE_CDATA](AuthorNode.md#NODE_TYPE_CDATA), [NODE_TYPE_COMMENT](AuthorNode.md#NODE_TYPE_COMMENT), [NODE_TYPE_DOCUMENT](AuthorNode.md#NODE_TYPE_DOCUMENT), [NODE_TYPE_ELEMENT](AuthorNode.md#NODE_TYPE_ELEMENT), [NODE_TYPE_PI](AuthorNode.md#NODE_TYPE_PI), [NODE_TYPE_PSEUDO_DOCTYPE](AuthorNode.md#NODE_TYPE_PSEUDO_DOCTYPE), [NODE_TYPE_PSEUDO_ELEMENT](AuthorNode.md#NODE_TYPE_PSEUDO_ELEMENT), [NODE_TYPE_REFERENCE](AuthorNode.md#NODE_TYPE_REFERENCE), [NODE_TYPE_TEXT](AuthorNode.md#NODE_TYPE_TEXT)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorElementBaseInterface](../AuthorElementBaseInterface.md) [getElementById](#getElementById(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) id)
Gets the element that has the ID attribute with the specified value.
  int [getLength](#getLength())()
Get the length of the document.
  [AuthorElement](AuthorElement.md) [getRootElement](#getRootElement())()
Returns the child node that is the root element of the document.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSystemID](#getSystemID())()
Returns the systemID of the document.

### Methods inherited from interface ro.sync.ecss.extensions.api.node.[AuthorNode](AuthorNode.md)
 [getContentIterator](AuthorNode.md#getContentIterator()), [getDisplayName](AuthorNode.md#getDisplayName()), [getEndOffset](AuthorNode.md#getEndOffset()), [getName](AuthorNode.md#getName()), [getNamespace](AuthorNode.md#getNamespace()), [getNamespaceContext](AuthorNode.md#getNamespaceContext()), [getOwnerDocument](AuthorNode.md#getOwnerDocument()), [getParent](AuthorNode.md#getParent()), [getStartOffset](AuthorNode.md#getStartOffset()), [getTextContent](AuthorNode.md#getTextContent()), [getType](AuthorNode.md#getType()), [getXMLBaseURL](AuthorNode.md#getXMLBaseURL()), [isDescendentOf](AuthorNode.md#isDescendentOf(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from interface ro.sync.ecss.extensions.api.node.[AuthorParentNode](AuthorParentNode.md)
 [getContentNodes](AuthorParentNode.md#getContentNodes()), [getParentElement](AuthorParentNode.md#getParentElement())
## Method Details

### getRootElement

[AuthorElement](AuthorElement.md) getRootElement()

Returns the child node that is the root element of the document.
  Returns: The root element of the document. Might be null for documents with no children elements.
### getSystemID

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSystemID()

Returns the systemID of the document.
  Returns: The systemID of the document, or null if not provided.
### getLength

int getLength()

Get the length of the document.
  Returns: the length of the document in characters, including the sentinel characters that delimit each element. Since: 13.2
### getElementById

[AuthorElementBaseInterface](../AuthorElementBaseInterface.md) getElementById([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) id)

Gets the element that has the ID attribute with the specified value.
  Parameters: id - The ID of the searched element. Should not contain the # symbol. Returns: null if no elements with the specified ID exists.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
