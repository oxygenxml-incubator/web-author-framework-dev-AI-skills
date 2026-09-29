# Package ro.sync.ecss.extensions.api.node

package ro.sync.ecss.extensions.api.node

API which allows access to the internal Author hierarchical structure.
     Related Packages
Package

Description
 [ro.sync.ecss.extensions.api](../package-summary.md)
Main API package used for controlling the Author page (making modifications, adding listeners).
      All Classes and InterfacesInterfacesClasses
Class

Description
 [ArtificialNode](ArtificialNode.md)
Marker interface for artificial elements which wrap Processing Instructions, CData and Comments allowing access to the wrapped node.
  [AttrValue](AttrValue.md)
Contains informations about an attribute value.
  [AuthorDocument](AuthorDocument.md)
The Document interface represents the entire XML document.
  [AuthorDocumentFragment](AuthorDocumentFragment.md)
Represents a fragment of an XML document.
  [AuthorDocumentProvider](AuthorDocumentProvider.md)
Use this API to access an "in memory" representation of an author document over a resource and customize the document in a non visual way using the [AuthorDocumentController](../AuthorDocumentController.md) and [AuthorDocument](AuthorDocument.md) API.
  [AuthorElement](AuthorElement.md)
The Author Element represents an XML element.
  [AuthorNode](AuthorNode.md)
Base interface for all Author nodes.
  [AuthorNodeUtil](AuthorNodeUtil.md)
Utility functions for working with AuthorNodes.
  [AuthorParentNode](AuthorParentNode.md)
An author parent node contains a list of children.
  [AuthorReferenceNode](AuthorReferenceNode.md)
Interface for reference nodes that have a content expanded when displayed in the Author mode.
  [ContentIterator](ContentIterator.md)
Iterator over the content of a node.
  [NamespaceContext](NamespaceContext.md)
Useful interface which can be used to obtain mappings from prefix to namespace and from namespace to prefix in the context of the current element.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
