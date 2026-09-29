Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorElementBaseInterface
    All Superinterfaces: [AuthorNode](node/AuthorNode.md), [AuthorParentNode](node/AuthorParentNode.md)   All Known Subinterfaces: [AuthorElement](node/AuthorElement.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorElementBaseInterfaceextends [AuthorParentNode](node/AuthorParentNode.md)
Element represents a tag in an XML document. The element is mapped into the content by two sentinel characters (the node positions point to them), having the '\0' character code. This is needed for easily moving the caret between two adjacent elements.
  Since: 13.2
## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.node.[AuthorNode](node/AuthorNode.md)
 [NODE_NAME_CDATA](node/AuthorNode.md#NODE_NAME_CDATA), [NODE_NAME_COMMENT](node/AuthorNode.md#NODE_NAME_COMMENT), [NODE_NAME_DOCUMENT](node/AuthorNode.md#NODE_NAME_DOCUMENT), [NODE_NAME_PI](node/AuthorNode.md#NODE_NAME_PI), [NODE_NAME_REFERENCE](node/AuthorNode.md#NODE_NAME_REFERENCE), [NODE_TYPE_CDATA](node/AuthorNode.md#NODE_TYPE_CDATA), [NODE_TYPE_COMMENT](node/AuthorNode.md#NODE_TYPE_COMMENT), [NODE_TYPE_DOCUMENT](node/AuthorNode.md#NODE_TYPE_DOCUMENT), [NODE_TYPE_ELEMENT](node/AuthorNode.md#NODE_TYPE_ELEMENT), [NODE_TYPE_PI](node/AuthorNode.md#NODE_TYPE_PI), [NODE_TYPE_PSEUDO_DOCTYPE](node/AuthorNode.md#NODE_TYPE_PSEUDO_DOCTYPE), [NODE_TYPE_PSEUDO_ELEMENT](node/AuthorNode.md#NODE_TYPE_PSEUDO_ELEMENT), [NODE_TYPE_REFERENCE](node/AuthorNode.md#NODE_TYPE_REFERENCE), [NODE_TYPE_TEXT](node/AuthorNode.md#NODE_TYPE_TEXT)
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 [AuthorElementBaseInterface](AuthorElementBaseInterface.md) [getBeforeElement](#getBeforeElement())()  Deprecated.
This functionality is needed from the CSS style matcher, so it will eventually move there.
   [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLocalName](#getLocalName())()

 boolean [hasPseudoClass](#hasPseudoClass(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Checks if a pseudo class is set on the element.
  boolean [isEmptyCSS3](#isEmptyCSS3())()
Checks if the element is empty (no content, or elements, may have PIs and Comments).
  boolean [isFirstChildElement](#isFirstChildElement())()  Deprecated.  void [removePseudoClass](#removePseudoClass(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Removes a pseudo class from the element.
  void [setPseudoClass](#setPseudoClass(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Sets a pseudo class on the element.

### Methods inherited from interface ro.sync.ecss.extensions.api.node.[AuthorNode](node/AuthorNode.md)
 [getContentIterator](node/AuthorNode.md#getContentIterator()), [getDisplayName](node/AuthorNode.md#getDisplayName()), [getEndOffset](node/AuthorNode.md#getEndOffset()), [getName](node/AuthorNode.md#getName()), [getNamespace](node/AuthorNode.md#getNamespace()), [getNamespaceContext](node/AuthorNode.md#getNamespaceContext()), [getOwnerDocument](node/AuthorNode.md#getOwnerDocument()), [getParent](node/AuthorNode.md#getParent()), [getStartOffset](node/AuthorNode.md#getStartOffset()), [getTextContent](node/AuthorNode.md#getTextContent()), [getType](node/AuthorNode.md#getType()), [getXMLBaseURL](node/AuthorNode.md#getXMLBaseURL()), [isDescendentOf](node/AuthorNode.md#isDescendentOf(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from interface ro.sync.ecss.extensions.api.node.[AuthorParentNode](node/AuthorParentNode.md)
 [getContentNodes](node/AuthorParentNode.md#getContentNodes()), [getParentElement](node/AuthorParentNode.md#getParentElement())
## Method Details

### getBeforeElement

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [AuthorElementBaseInterface](AuthorElementBaseInterface.md) getBeforeElement()
 Deprecated.
This functionality is needed from the CSS style matcher, so it will eventually move there. Will be removed in 17.0 or later.
   Returns: The before sibling if any.
### isFirstChildElement

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) boolean isFirstChildElement()
 Deprecated.
Check if this element is the first child element of the parent.
  Returns: Returns true if element is the first child in parent.
### getLocalName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLocalName()
  Returns: The element local name.
### hasPseudoClass

boolean hasPseudoClass([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Checks if a pseudo class is set on the element.
  Parameters: name - The name of the pseudo class. Let say :hover, :active, etc.. Returns: true if the pseudo class is set on the element.
### setPseudoClass

void setPseudoClass([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Sets a pseudo class on the element. **Warning:** Use this only when the element is from an [AuthorDocumentFragment](node/AuthorDocumentFragment.md) and not from the current [AuthorDocument](node/AuthorDocument.md) content.All operations on nodes from the document model must be done using the [AuthorDocumentController](AuthorDocumentController.md) methods.If the element is part of the edited document, an java.lang.UnsupportedOperationException is thrown.
  Parameters: name - The name of the pseudo class. Let say :hover, :active, etc..
### removePseudoClass

void removePseudoClass([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Removes a pseudo class from the element. **Warning:** Use this only when the element is from an [AuthorDocumentFragment](node/AuthorDocumentFragment.md) and not from the current [AuthorDocument](node/AuthorDocument.md) content.All operations on nodes from the document model must be done using the [AuthorDocumentController](AuthorDocumentController.md) methods.If the element is part of the edited document, an java.lang.UnsupportedOperationException is thrown.
  Parameters: name - The name of the pseudo class. Let say :hover, :active, etc..
### isEmptyCSS3

boolean isEmptyCSS3()

Checks if the element is empty (no content, or elements, may have PIs and Comments).
  Returns: true if the element is empty as defined here: http://www.w3.org/TR/css3-selectors/#empty-pseudo
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
