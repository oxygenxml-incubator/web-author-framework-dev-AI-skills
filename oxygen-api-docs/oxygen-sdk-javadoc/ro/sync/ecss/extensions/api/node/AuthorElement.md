Package [ro.sync.ecss.extensions.api.node](package-summary.md)

# Interface AuthorElement
    All Superinterfaces: [AuthorElementBaseInterface](../AuthorElementBaseInterface.md), [AuthorNode](AuthorNode.md), [AuthorParentNode](AuthorParentNode.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorElementextends [AuthorElementBaseInterface](../AuthorElementBaseInterface.md)
The Author Element represents an XML element. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.node.[AuthorNode](AuthorNode.md)
 [NODE_NAME_CDATA](AuthorNode.md#NODE_NAME_CDATA), [NODE_NAME_COMMENT](AuthorNode.md#NODE_NAME_COMMENT), [NODE_NAME_DOCUMENT](AuthorNode.md#NODE_NAME_DOCUMENT), [NODE_NAME_PI](AuthorNode.md#NODE_NAME_PI), [NODE_NAME_REFERENCE](AuthorNode.md#NODE_NAME_REFERENCE), [NODE_TYPE_CDATA](AuthorNode.md#NODE_TYPE_CDATA), [NODE_TYPE_COMMENT](AuthorNode.md#NODE_TYPE_COMMENT), [NODE_TYPE_DOCUMENT](AuthorNode.md#NODE_TYPE_DOCUMENT), [NODE_TYPE_ELEMENT](AuthorNode.md#NODE_TYPE_ELEMENT), [NODE_TYPE_PI](AuthorNode.md#NODE_TYPE_PI), [NODE_TYPE_PSEUDO_DOCTYPE](AuthorNode.md#NODE_TYPE_PSEUDO_DOCTYPE), [NODE_TYPE_PSEUDO_ELEMENT](AuthorNode.md#NODE_TYPE_PSEUDO_ELEMENT), [NODE_TYPE_REFERENCE](AuthorNode.md#NODE_TYPE_REFERENCE), [NODE_TYPE_TEXT](AuthorNode.md#NODE_TYPE_TEXT)
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 [AttrValue](AttrValue.md) [getAttribute](#getAttribute(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the value of an attribute with the given name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeAtIndex](#getAttributeAtIndex(int))(int index)
Returns the name of the attribute at the specified index.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeNamespace](#getAttributeNamespace(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributePrefix)
Get an attribute's namespace.
  int [getAttributesCount](#getAttributesCount())()
Returns the number of the element attributes.
  [AuthorNode](AuthorNode.md) [getChild](#getChild(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) childLocalName)  Deprecated.
Use [getElementsByLocalName(String)](#getElementsByLocalName(java.lang.String))[0] instead.
   [AuthorElement](AuthorElement.md)[] [getElementsByLocalName](#getElementsByLocalName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName)
Gets the children elements having the specified local name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLocalName](#getLocalName())()
Returns the local part of the qualified name of this element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNamespace](#getNamespace())()

 [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getPseudoClassNames](#getPseudoClassNames())()
Get the names of the pseudo-classes set on this element.
  void [removeAttribute](#removeAttribute(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName)
Removes the given attribute from the element list of attributes. **Warning:** Use this only when the element is from an [AuthorDocumentFragment](AuthorDocumentFragment.md) and not from the current [AuthorDocument](AuthorDocument.md) content.All operations on nodes from the document model must be done using the [AuthorDocumentController](../AuthorDocumentController.md) methods.
  void [setAttribute](#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName, [AttrValue](AttrValue.md) attributeValue)
Sets the value of an attribute for this element. **Warning:** Use this only when the element is from an [AuthorDocumentFragment](AuthorDocumentFragment.md) and not from the current [AuthorDocument](AuthorDocument.md) content.All operations on nodes from the document model must be done using the [AuthorDocumentController](../AuthorDocumentController.md) methods.
  void [setAttributesNoNSUpdate](#setAttributesNoNSUpdate(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](AttrValue.md)> attrs)
Sets an attribute, but without performing the update of the namespace mappings updates.
  void [setName](#setName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newName)
Sets the qualified name of this element. **Warning:** Use this only when the element is from an [AuthorDocumentFragment](AuthorDocumentFragment.md) and not from the current [AuthorDocument](AuthorDocument.md) content.All operations on nodes from the document model must be done using the [AuthorDocumentController](../AuthorDocumentController.md) methods.

### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorElementBaseInterface](../AuthorElementBaseInterface.md)
 [getBeforeElement](../AuthorElementBaseInterface.md#getBeforeElement()), [hasPseudoClass](../AuthorElementBaseInterface.md#hasPseudoClass(java.lang.String)), [isEmptyCSS3](../AuthorElementBaseInterface.md#isEmptyCSS3()), [isFirstChildElement](../AuthorElementBaseInterface.md#isFirstChildElement()), [removePseudoClass](../AuthorElementBaseInterface.md#removePseudoClass(java.lang.String)), [setPseudoClass](../AuthorElementBaseInterface.md#setPseudoClass(java.lang.String))
### Methods inherited from interface ro.sync.ecss.extensions.api.node.[AuthorNode](AuthorNode.md)
 [getContentIterator](AuthorNode.md#getContentIterator()), [getDisplayName](AuthorNode.md#getDisplayName()), [getEndOffset](AuthorNode.md#getEndOffset()), [getName](AuthorNode.md#getName()), [getNamespaceContext](AuthorNode.md#getNamespaceContext()), [getOwnerDocument](AuthorNode.md#getOwnerDocument()), [getParent](AuthorNode.md#getParent()), [getStartOffset](AuthorNode.md#getStartOffset()), [getTextContent](AuthorNode.md#getTextContent()), [getType](AuthorNode.md#getType()), [getXMLBaseURL](AuthorNode.md#getXMLBaseURL()), [isDescendentOf](AuthorNode.md#isDescendentOf(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from interface ro.sync.ecss.extensions.api.node.[AuthorParentNode](AuthorParentNode.md)
 [getContentNodes](AuthorParentNode.md#getContentNodes()), [getParentElement](AuthorParentNode.md#getParentElement())
## Method Details

### getAttribute

[AttrValue](AttrValue.md) getAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the value of an attribute with the given name. If no such attribute exists, returns null.
  Parameters: name - Name of the attribute. Returns: The [AttrValue](AttrValue.md), or null if the attribute does not exist.
### getNamespace

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNamespace()
  Specified by: [getNamespace](AuthorNode.md#getNamespace()) in interface [AuthorNode](AuthorNode.md) Returns: The namespace of this element. Empty string is returned if element has no namespace.
### getLocalName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLocalName()

Returns the local part of the qualified name of this element.
  Specified by: [getLocalName](../AuthorElementBaseInterface.md#getLocalName()) in interface [AuthorElementBaseInterface](../AuthorElementBaseInterface.md) Returns: The local name of the element.
### getChild

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [AuthorNode](AuthorNode.md) getChild([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) childLocalName)
 Deprecated.
Use [getElementsByLocalName(String)](#getElementsByLocalName(java.lang.String))[0] instead.

Search into the list of the children the first node that has specified local name.
  Parameters: childLocalName - The local name of the searched children. Returns: The searched node or null if not found.
### getElementsByLocalName

[AuthorElement](AuthorElement.md)[] getElementsByLocalName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName)

Gets the children elements having the specified local name.
  Parameters: localName - The local name of the searched children. Returns: The list of children (AuthorElements) having the specified local name or an empty array if none found. if not found.
### getAttributesCount

int getAttributesCount()

Returns the number of the element attributes.
  Returns: The number of the element attributes..
### getAttributeAtIndex

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeAtIndex(int index)throws [ArrayIndexOutOfBoundsException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ArrayIndexOutOfBoundsException.html)

Returns the name of the attribute at the specified index.
  Parameters: index - The index of the searched attribute, 0 based. Returns: The name of the attribute at the specified index, or null if the attribute was not set correctly. Throws: [ArrayIndexOutOfBoundsException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ArrayIndexOutOfBoundsException.html) - if the specified index is not in range.
### setAttribute

void setAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName, [AttrValue](AttrValue.md) attributeValue)

Sets the value of an attribute for this element. **Warning:** Use this only when the element is from an [AuthorDocumentFragment](AuthorDocumentFragment.md) and not from the current [AuthorDocument](AuthorDocument.md) content.All operations on nodes from the document model must be done using the [AuthorDocumentController](../AuthorDocumentController.md) methods. If the element is part of the edited document, an java.lang.UnsupportedOperationException is thrown.
  Parameters: qName - The qualified name of the attribute to be set. attributeValue - The [AttrValue](AttrValue.md) to set. Must not be null.
### setName

void setName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newName)throws [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html)

Sets the qualified name of this element. **Warning:** Use this only when the element is from an [AuthorDocumentFragment](AuthorDocumentFragment.md) and not from the current [AuthorDocument](AuthorDocument.md) content.All operations on nodes from the document model must be done using the [AuthorDocumentController](../AuthorDocumentController.md) methods. If the element is part of the edited document, an java.lang.UnsupportedOperationException is thrown.
  Parameters: newName - The new qualified name to be set. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - When the given name is not a valid qualified name. Since: 16
### removeAttribute

void removeAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName)

Removes the given attribute from the element list of attributes. **Warning:** Use this only when the element is from an [AuthorDocumentFragment](AuthorDocumentFragment.md) and not from the current [AuthorDocument](AuthorDocument.md) content.All operations on nodes from the document model must be done using the [AuthorDocumentController](../AuthorDocumentController.md) methods. If the element is part of the edited document, an java.lang.UnsupportedOperationException is thrown.
  Parameters: qName - The qualified name of the attribute to remove.
### getAttributeNamespace

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeNamespace([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributePrefix)

Get an attribute's namespace.
  Parameters: attributePrefix - Prefix of attribute. Returns: The attribute's namespace. Since: 13.2
### setAttributesNoNSUpdate

void setAttributesNoNSUpdate([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](AttrValue.md)> attrs)

Sets an attribute, but without performing the update of the namespace mappings updates.
 **Warning:** Use this only when the element is from an [AuthorDocumentFragment](AuthorDocumentFragment.md) and not from the current [AuthorDocument](AuthorDocument.md) content.All operations on nodes from the document model must be done using the [AuthorDocumentController](../AuthorDocumentController.md) methods. If the element is part of the edited document, an java.lang.UnsupportedOperationException is thrown.
  Parameters: attrs - The map containing attribute qNames and their attributeValues.
### getPseudoClassNames

[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getPseudoClassNames()

Get the names of the pseudo-classes set on this element.
  Returns: a set of pseudo-classes or an empty set. Never null. Since: 22.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
