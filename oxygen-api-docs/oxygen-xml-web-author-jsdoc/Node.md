# Interface: Node

##  Node

Base interface for DOM nodes.

##### Properties:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `nodeName` |   string   | The name of this node, depending on its type. *  Attr - the attribute qualified name *  Comment - #comment *  Document - #document *  Element - the element's qualified name *  EntityReference - the name of the entity *  Processing Instruction - the target of the processing instruction *  Text - #text  |
| `nodeValue` |   string   | The value of this node, depending on its type *  Attr - the attribute value *  Comment - the comment's content *  Processing Instruction - the data of the processing instruction *  Text - the text content *  Otherwise, null  |
| `nodeType` |   number   | The type of the node. One of these values *  ELEMENT - 1 *  ATTRIBUTE - 2 *  TEXT - 3 *  ENTITY_REFERENCE - 5 *  PROCESSING_INSTRUCTION - 7 *  COMMENT - 8 *  DOCUMENT - 9  |
| `parentNode` |   [Node](Node.md)   | The parent of the current node, null for the #document node and for attributes. |
| `childNodes` |   [NodeList](NodeList.md)   | A NodeList that contains all children of this node. If there are no children, this is a NodeList containing no nodes |
| `firstChild` |   [Node](Node.md)   | The first child of this node. If there is no such node, this returns null. |
| `lastChild` |   [Node](Node.md)   | The last child of this node. If there is no such node, this returns null. |
| `previousSibling` |   [Node](Node.md)   | The node immediately preceding this node. If there is no such node, this returns null. |
| `nextSibling` |   [Node](Node.md)   | The node immediately following this node. If there is no such node, this returns null. |
| `attributes` |   [NamedNodeMap](NamedNodeMap.md)   | A NamedNodeMap containing the attributes of this node (if it is an Element) or null otherwise |
| `ownerDocument` |   [Document](Document.md)   | The Document object associated with this node. |
| `namespaceURI` |   string   | The namespace URI of this node - null if there is no namespace or if the node is not Element or Attribute. |
| `prefix` |   string   | The prefix of this node - null if there is no namespace or if the node is not Element or Attribute. |
| `localName` |   string   | The local name of this node, null if not attribute or element. |
| `baseURI` |   string   | The base URI for this node - it takes content references and xi:includes into account, but not the xml:base attribute. |
| `textContent` |   string   | The text content of the node - it ignores descendant comments and processing instructions. For attributes it returns the its value. |

### Methods

#### compareDocumentPosition(other)

 Compares the reference node, i.e. the node on which this method is being called, with a node, i.e. the one passed as a parameter, with regard to their position in the document and according to the document order.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `other` |   [Node](Node.md)   | The node to compare to. |

##### Returns:

 A bitmask with the following values from the Node class:
*  DOCUMENT_POSITION_CONTAINED_BY - The node is contained by the reference node. A node which is contained is always following, too.
*  DOCUMENT_POSITION_CONTAINS - The node contains the reference node. A node which contains is always preceding, too.
* DOCUMENT_POSITION_DISCONNECTED - The two nodes are disconnected. Order between disconnected nodes is always implementation-specific.
* DOCUMENT_POSITION_FOLLOWING - The node follows the reference node.
* DOCUMENT_POSITION_IMPLEMENTATION_SPECIFIC - The determination of preceding versus following is implementation-specific.
* DOCUMENT_POSITION_PRECEDING - The second node precedes the reference node.

     Type     number
#### hasAttributes()

 Returns true if the node has attributes.

##### Returns:

 if the node has attributes.
     Type     true
#### hasChildNodes()

 Returns whether this node has any children.

##### Returns:

 true if the node has child nodes.
     Type     boolean
#### hasChildNodes()

 Returns whether this node has any children.

##### Returns:

 true if the node has child nodes.
     Type     boolean
#### isEqualNode(other)

 Test if two nodes have the same structure.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `other` |   [Node](Node.md)   | The node to compare to. |

##### Returns:

 true if the two nodes have the same structure.
     Type     boolean
#### isSameNode(other)

 The API may return different JS DOM objects for the same XML node - to detect this case, use this method.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `other` |   [Node](Node.md)   | The node to compare to. |

##### Returns:

 true if the two objects represent the same XML node.
     Type     boolean
#### lookupNamespaceURI(prefix)

 Look up the namespace URI associated to the given prefix, starting from this node.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `prefix` |   string   | The URI of the namespace. |

##### Returns:

 the mapped namespace URI.
     Type     string
#### lookupPrefix(namespaceURI)

 Look up the prefix associated to the given namespace URI, starting from this node. The default namespace declarations are ignored by this method.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `namespaceURI` |   string   | The URI of the namespace. |

##### Returns:

 the associated prefix, or null if there is no associated prefix. If there are multiple mappings, return the closest one to this node.
     Type     string

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
