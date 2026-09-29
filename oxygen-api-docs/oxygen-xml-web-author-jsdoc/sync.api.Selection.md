# Class: Selection

##   [sync](sync.md)[.api](sync.api.md). Selection

#### new Selection()

 Author-specific selection.

### Methods

#### &lt;static&gt; createAroundNode(node)

 Create a selection around the given node.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `node` |   [Node](Node.md)   | The node which selection should wrap. |
    Deprecated:
* use [sync.api.SelectionManager#createAroundNode](sync.api.SelectionManager.md#createAroundNode)

##### Returns:

 The selection object.
     Type     [sync.api.Selection](sync.api.Selection.md)
#### &lt;static&gt; createEmptySelectionInNode(node, pos)

 Returns a selection that is empty and is located inside the given node, at the given position.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `node` |   [Node](Node.md)   | The element, comment or PI in which the selection is positioned. |
| `pos` |   string   | The position of the caret: * 'before' means before all children nodes * 'after' that means after all children nodes  |
    Deprecated:
* use [sync.api.SelectionManager#createEmptySelectionInNode](sync.api.SelectionManager.md#createEmptySelectionInNode)

##### Returns:

 The selection.
     Type     [sync.api.Selection](sync.api.Selection.md)
#### &lt;static&gt; createEmptySelectionRelativeToNode(node, offset [, opt_fromNodeEndTag])

 Creates an empty selection at a position that is "offset" steps to the right of the start/end tag of the given "node". A step means either a content character, a start tag of a node or an end tag of a node. For example, with this XML content:`&lt;p&gt;I &lt;b&gt;like&lt;/b&gt; XML.&lt;/p&gt;`The following call:`Selection.createEmptySelectionRelativeToNode(p, 5, true)`Creates a position in the word "like" as presented below:`&lt;p&gt;I &lt;b&gt;li|ke&lt;/b&gt; XML.&lt;/p&gt;`

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `node` |   [Node](Node.md)   |    | The element, comment or PI used as a reference for the selection position. |
| `offset` |   number   |    | The number of steps to the right of the start/end tag of the reference node. |
| `opt_fromNodeEndTag` |   boolean   |  &lt;optional&gt;   | true, to create the selection relative to the end tag of the given node rather than to its start. |
    Deprecated:
* use [sync.api.SelectionManager#createEmptySelectionRelativeToNode](sync.api.SelectionManager.md#createEmptySelectionRelativeToNode)

#### extendedTo(node, offset [, opt_fromNodeEndTag])

 Returns a new selection which is created by extending the current selection to the position that is "offset" steps to the right of the start/end tag of the given "node". A step means either a content character, a start tag of a node or an end tag of a node. For example, with this XML content, and the selection represented as a vertical line:`&lt;p&gt;I &lt;b&gt;|like&lt;/b&gt; XML.&lt;/p&gt;`The following call:`var extendedSel = sel.extendedTo(p, 7, true)`creates a new extended selection to select the word "like" as presented below:`&lt;p&gt;I &lt;b&gt;|like|&lt;/b&gt; XML.&lt;/p&gt;`

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `node` |   [Node](Node.md)   |    | The element, comment, or PI used as a reference for the selection position. |
| `offset` |   number   |    | The number of steps to the right of the start/end tag of the reference node. |
| `opt_fromNodeEndTag` |   boolean   |  &lt;optional&gt;   | true, to create the selection relative to the end tag of the given node rather than to its start. |

##### Returns:
     Type     [sync.api.Selection](sync.api.Selection.md)
#### getCaretPositionInformation()

 Retrieve information about the caret position.
The XML content is modeled as a sequence of items that can be either characters and XML (start or end ) tags. The caret is said to be positioned "on" a certain item if it is visually to the left of that item.

##### Returns:

 Information about caret position.
     Type     [sync.api.PositionInformation](sync.api.PositionInformation.md)
#### getFullySelectedNode()

 Returns the element, comment or PI that is fully selected.

##### Returns:

 The element, comment or PI which is fully selected.
     Type     [Node](Node.md)
#### getNodeAtCaret( [opt_includeTextNodes])

 Returns the node at caret if the selection is empty.
If the caret is "on" [sync.api.Selection#getCaretPositionInformation](sync.api.Selection.md#getCaretPositionInformation) a start tag of an element "X", it is considered to be outside the node "X", so the returned node is the parent of "X".

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `opt_includeTextNodes` |   boolean   |  &lt;optional&gt;   | If present and `true` will include text nodes. By default text nodes are ignored. |

##### Returns:

 The node at caret if the selection is empty.
     Type     [Node](Node.md) | null
#### getNodeAtSelection( [opt_includeTextNodes])

 Returns the node at the current selection.
If the current selection is empty, the node in which the selection resides is returned.

If the selection is around an entire node, that node will be returned.

If the selection spans multiple nodes, the node where the selection has ended is returned.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `opt_includeTextNodes` |   boolean   |  &lt;optional&gt;   | If present and `true` will include text nodes. By default text nodes are ignored. |

##### Returns:

 The node at the current selection.
     Type     [Node](Node.md)
#### getNodeAtSelectionEnd( [opt_includeTextNodes])

 Returns the node at the current selection.
If the current selection is empty, the node in which the selection resides is returned.

If the selection is around an entire node, that node will be returned.

If the selection spans multiple nodes, the node at the end of it.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `opt_includeTextNodes` |   boolean   |  &lt;optional&gt;   | If present and `true` will include text nodes. By default text nodes are ignored. |

##### Returns:

 The node at the current selection.
     Type     [Node](Node.md)
#### getNodeAtSelectionStart( [opt_includeTextNodes])

 Returns the node at the current selection.
If the current selection is empty, the node in which the selection resides is returned.

If the selection is around an entire node, that node will be returned.

If the selection spans multiple nodes, the node at the start of it.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `opt_includeTextNodes` |   boolean   |  &lt;optional&gt;   | If present and `true` will include text nodes. By default text nodes are ignored. |

##### Returns:

 The node at the current selection.
     Type     [Node](Node.md)

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
