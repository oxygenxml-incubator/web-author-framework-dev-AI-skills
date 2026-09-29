# Interface: Element

##  Element

Interface for the element nodes.

### Extends

* [Node](Node.md)

### Methods

#### compareDocumentPosition(other)

 Compares the reference node, i.e. the node on which this method is being called, with a node, i.e. the one passed as a parameter, with regard to their position in the document and according to the document order.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `other` |   [Node](Node.md)   | The node to compare to. |
    Inherited From:
*   [Node#compareDocumentPosition](Node.md#compareDocumentPosition)

##### Returns:

 A bitmask with the following values from the Node class:
*  DOCUMENT_POSITION_CONTAINED_BY - The node is contained by the reference node. A node which is contained is always following, too.
*  DOCUMENT_POSITION_CONTAINS - The node contains the reference node. A node which contains is always preceding, too.
* DOCUMENT_POSITION_DISCONNECTED - The two nodes are disconnected. Order between disconnected nodes is always implementation-specific.
* DOCUMENT_POSITION_FOLLOWING - The node follows the reference node.
* DOCUMENT_POSITION_IMPLEMENTATION_SPECIFIC - The determination of preceding versus following is implementation-specific.
* DOCUMENT_POSITION_PRECEDING - The second node precedes the reference node.

     Type     number
#### getAttribute(name)

 Returns the value of the attribute with a given name.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `name` |   string   | The qualified name of the attribute. |

##### Returns:

 The value of the attribute.
     Type     string
#### getAttributeNode(name)

 Returns the attribute with a given name.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `name` |   string   | The qualified name of the attribute. |

##### Returns:

 The attribute node.
     Type     [Attr](Attr.md)
#### getAttributeNodeNS(name, namespaceURI)

 Returns the attribute with a given name and namespace.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `name` |   string   | The name of the attribute. |
| `namespaceURI` |   string   | The namespace URI. |

##### Returns:

 The attribute node.
     Type     [Attr](Attr.md)
#### getAttributeNS(name, namespaceURI)

 Returns the value of the attribute with a given name and namespace.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `name` |   string   | The name of the attribute. |
| `namespaceURI` |   string   | The namespace URI. |

##### Returns:

 The value of the attribute.
     Type     string
#### getElementsByTagName(tagName)

 Returns a NodeList of all the Elements in document order with a given tag name and are contained in the document.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `tagName` |   string   | The tagName of the elements, or '\*' to match all elements. |

##### Returns:

 The list of elements.
     Type     [NodeList](NodeList.md)
#### getElementsByTagNameNS(localName, namespaceURI)

 Returns a NodeList of all the Elements in document order with a given name and namespace and are contained in the document.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `localName` |   string   | The localName of the elements, or '\*' to match all element names. |
| `namespaceURI` |   string   | The namespaceURI of the elements, or '\*' to match all namespaces. |

##### Returns:

 The list of elements.
     Type     [NodeList](NodeList.md)
#### hasAttribute(name)

 Returns true if the node has an attribute with a given qualified name.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `name` |   string   | The qualified name of the attribute. |

##### Returns:

 if the attribute exists.
     Type     true
#### hasAttributeNS(name, namespaceURI)

 Returns true if the node has an attribute with a given name and namespace.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `name` |   string   | The name of the attribute. |
| `namespaceURI` |   string   | The namespace URI. |

##### Returns:

 if the attribute exists.
     Type     true
#### hasAttributes()

 Returns true if the node has attributes.
    Inherited From:
*   [Node#hasAttributes](Node.md#hasAttributes)

##### Returns:

 if the node has attributes.
     Type     true
#### hasChildNodes()

 Returns whether this node has any children.
    Inherited From:
*   [Node#hasChildNodes](Node.md#hasChildNodes)
    Overrides:
*   [Node#hasChildNodes](Node.md#hasChildNodes)

##### Returns:

 true if the node has child nodes.
     Type     boolean
#### hasPseudoClass(name)

 Returns true if the node has a pseudo-class with a given name.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `name` |   string   | The name of the pseudo-class. |

##### Returns:

 if the pseudo-class is set.
     Type     true
#### isEqualNode(other)

 Test if two nodes have the same structure.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `other` |   [Node](Node.md)   | The node to compare to. |
    Inherited From:
*   [Node#isEqualNode](Node.md#isEqualNode)

##### Returns:

 true if the two nodes have the same structure.
     Type     boolean
#### isSameNode(other)

 The API may return different JS DOM objects for the same XML node - to detect this case, use this method.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `other` |   [Node](Node.md)   | The node to compare to. |
    Inherited From:
*   [Node#isSameNode](Node.md#isSameNode)

##### Returns:

 true if the two objects represent the same XML node.
     Type     boolean
#### lookupNamespaceURI(prefix)

 Look up the namespace URI associated to the given prefix, starting from this node.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `prefix` |   string   | The URI of the namespace. |
    Inherited From:
*   [Node#lookupNamespaceURI](Node.md#lookupNamespaceURI)

##### Returns:

 the mapped namespace URI.
     Type     string
#### lookupPrefix(namespaceURI)

 Look up the prefix associated to the given namespace URI, starting from this node. The default namespace declarations are ignored by this method.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `namespaceURI` |   string   | The URI of the namespace. |
    Inherited From:
*   [Node#lookupPrefix](Node.md#lookupPrefix)

##### Returns:

 the associated prefix, or null if there is no associated prefix. If there are multiple mappings, return the closest one to this node.
     Type     string

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
