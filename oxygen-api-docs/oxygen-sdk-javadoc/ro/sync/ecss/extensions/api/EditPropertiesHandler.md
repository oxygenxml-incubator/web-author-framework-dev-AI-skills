Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface EditPropertiesHandler
    All Superinterfaces: [Extension](Extension.md)   All Known Implementing Classes: [EditPropertiesHandlerAdapter](EditPropertiesHandlerAdapter.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface EditPropertiesHandlerextends [Extension](Extension.md)
A custom implementation to handle editing properties for an author node. For example when a user double clicks on an element tag we will invoke this extension and a specific dialog can be presented. The user can edit different facets of that element, like attributes.
It is recommended to extend class [EditPropertiesHandlerAdapter](EditPropertiesHandlerAdapter.md) in order to be protected from any API additions that may occur in interface [EditPropertiesHandler](EditPropertiesHandler.md).

  Since: 17.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [canEditProperties](#canEditProperties(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) authorNode)
Checks if it can edit the properties for a given node.
  void [editProperties](#editProperties(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](node/AuthorNode.md) authorNode, [AuthorAccess](AuthorAccess.md) authorAccess)
Edit the properties for the given node.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Method Details

### editProperties

void editProperties([AuthorNode](node/AuthorNode.md) authorNode, [AuthorAccess](AuthorAccess.md) authorAccess)

Edit the properties for the given node.
  Parameters: authorNode - Author node to edit the properties for. authorAccess - Author access.
### canEditProperties

boolean canEditProperties([AuthorNode](node/AuthorNode.md) authorNode)

Checks if it can edit the properties for a given node.
  Parameters: authorNode - Author node to edit the properties for. Returns: true if it can edit the properties of the node and false if the properties of this node can't be edited.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
