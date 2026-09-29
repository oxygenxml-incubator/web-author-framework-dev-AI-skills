Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class EditPropertiesHandlerAdapter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.EditPropertiesHandlerAdapter
   All Implemented Interfaces: [EditPropertiesHandler](EditPropertiesHandler.md), [Extension](Extension.md)   @API(type=EXTENDABLE, src=PUBLIC) public class EditPropertiesHandlerAdapter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [EditPropertiesHandler](EditPropertiesHandler.md)
Adapter class. A custom implementation to handle editing properties for an author node. For example when a user double clicks on an element tag we will invoke this extension and a specific dialog can be presented. The user can edit different facets of that element, like attributes.
  Since: 17.1
## Constructor Summary
 Constructors
Constructor

Description
 [EditPropertiesHandlerAdapter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [canEditProperties](#canEditProperties(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) authorNode)
Checks if it can edit the properties for a given node.
  void [editProperties](#editProperties(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](node/AuthorNode.md) authorNode, [AuthorAccess](AuthorAccess.md) authorAccess)
Edit the properties for the given node.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### EditPropertiesHandlerAdapter

public EditPropertiesHandlerAdapter()

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](Extension.md#getDescription()) in interface [Extension](Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](Extension.md#getDescription())

### editProperties

public void editProperties([AuthorNode](node/AuthorNode.md) authorNode, [AuthorAccess](AuthorAccess.md) authorAccess)
 Description copied from interface: [EditPropertiesHandler](EditPropertiesHandler.md#editProperties(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))
Edit the properties for the given node.
  Specified by: [editProperties](EditPropertiesHandler.md#editProperties(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [EditPropertiesHandler](EditPropertiesHandler.md) Parameters: authorNode - Author node to edit the properties for. authorAccess - Author access. See Also:
        * [EditPropertiesHandler.editProperties(ro.sync.ecss.extensions.api.node.AuthorNode, ro.sync.ecss.extensions.api.AuthorAccess)](EditPropertiesHandler.md#editProperties(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))

### canEditProperties

public boolean canEditProperties([AuthorNode](node/AuthorNode.md) authorNode)
 Description copied from interface: [EditPropertiesHandler](EditPropertiesHandler.md#canEditProperties(ro.sync.ecss.extensions.api.node.AuthorNode))
Checks if it can edit the properties for a given node.
  Specified by: [canEditProperties](EditPropertiesHandler.md#canEditProperties(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [EditPropertiesHandler](EditPropertiesHandler.md) Parameters: authorNode - Author node to edit the properties for. Returns: true if it can edit the properties of the node and false if the properties of this node can't be edited. See Also:
        * [EditPropertiesHandler.canEditProperties(ro.sync.ecss.extensions.api.node.AuthorNode)](EditPropertiesHandler.md#canEditProperties(ro.sync.ecss.extensions.api.node.AuthorNode))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
