Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class DITAAuthorActionEventHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorActionEventHandlerBase](AuthorActionEventHandlerBase.md)
        * [ro.sync.ecss.extensions.api.DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md)
            * ro.sync.ecss.extensions.api.DITAAuthorActionEventHandler
   All Implemented Interfaces: [AuthorActionEventHandler](AuthorActionEventHandler.md), [Extension](Extension.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class DITAAuthorActionEventHandler extends [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md)
Author action event handler for DITA. IMPORTANT, THIS CLASS SHOULD HAVE BEEN CREATED IN THE FRAMEWORK SPECIFIC PACKAGE. BUT IT WAS NOT, TOO LATE, WE KEEP IT HERE FOR BACKWARD COMPATIBILITY

## Nested Class Summary

## Nested classes/interfaces inherited from class ro.sync.ecss.extensions.api.[DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md)
 [DefaultAuthorActionEventHandler.CiElementAndOffset](DefaultAuthorActionEventHandler.CiElementAndOffset.md)
## Nested classes/interfaces inherited from interface ro.sync.ecss.extensions.api.[AuthorActionEventHandler](AuthorActionEventHandler.md)
 [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md)
## Constructor Summary
 Constructors
Constructor

Description
 [DITAAuthorActionEventHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [areCompatibleLists](#areCompatibleLists(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node1, [AuthorNode](node/AuthorNode.md) node2)
Check if two given nodes are compatible lists (i.e.
  boolean [canHandleEvent](#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventDetails))([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventDetails](AuthorActionEventDetails.md) eventDetails)
Check if an Author action event can be handled.
  [AuthorElement](node/AuthorElement.md) [getListItemAncestorToSplit](#getListItemAncestorToSplit(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](node/AuthorNode.md) node, [AuthorAccess](AuthorAccess.md) access)
Return the list item ancestor of the current node that needs to be split on Enter.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getParagraphElement](#getParagraphElement(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Get the preferred XML element content to be inserted.
  boolean [handleEvent](#handleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType))([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) eventType)
An event was generated.
  protected boolean [isList](#isList(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node)
Check if the given node is a list.
  protected boolean [isMovableListItem](#isMovableListItem(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorNode](node/AuthorNode.md) candidate)
Checks if this node represents a list item that can be promoted/demoted.

### Methods inherited from class ro.sync.ecss.extensions.api.[DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md)
 [canHandleEvent](DefaultAuthorActionEventHandler.md#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType)), [deleteNodeChildren](DefaultAuthorActionEventHandler.md#deleteNodeChildren(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorNode)), [getContentCompletionActions](DefaultAuthorActionEventHandler.md#getContentCompletionActions(ro.sync.ecss.extensions.api.AuthorAccess,int)), [getDescription](DefaultAuthorActionEventHandler.md#getDescription()), [getInsertableFormForElement](DefaultAuthorActionEventHandler.md#getInsertableFormForElement(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorElement,int)), [getPreferredXMLElementContent](DefaultAuthorActionEventHandler.md#getPreferredXMLElementContent(ro.sync.ecss.extensions.api.AuthorAccess)), [promote](DefaultAuthorActionEventHandler.md#promote(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.util.List,boolean)), [promoteSubListItems](DefaultAuthorActionEventHandler.md#promoteSubListItems(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAAuthorActionEventHandler

public DITAAuthorActionEventHandler()

## Method Details

### isMovableListItem

protected boolean isMovableListItem([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorNode](node/AuthorNode.md) candidate)
 Description copied from class: [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md#isMovableListItem(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode))
Checks if this node represents a list item that can be promoted/demoted.
  Overrides: [isMovableListItem](DefaultAuthorActionEventHandler.md#isMovableListItem(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode)) in class [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md) Parameters: authorAccess - The Author access. candidate - The node that candidates for promotion/demotion. Returns: true if the list item can be promoted/demoted. See Also:
        * [DefaultAuthorActionEventHandler.isMovableListItem(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorNode)](DefaultAuthorActionEventHandler.md#isMovableListItem(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode))

### isList

protected boolean isList([AuthorNode](node/AuthorNode.md) node)
 Description copied from class: [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md#isList(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if the given node is a list.
  Overrides: [isList](DefaultAuthorActionEventHandler.md#isList(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md) Parameters: node - The node. Returns: true if the node is a list. See Also:
        * [DefaultAuthorActionEventHandler.isList(ro.sync.ecss.extensions.api.node.AuthorNode)](DefaultAuthorActionEventHandler.md#isList(ro.sync.ecss.extensions.api.node.AuthorNode))

### getParagraphElement

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getParagraphElement([AuthorAccess](AuthorAccess.md) authorAccess)
 Description copied from class: [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md#getParagraphElement(ro.sync.ecss.extensions.api.AuthorAccess))
Get the preferred XML element content to be inserted. Can be null.
  Overrides: [getParagraphElement](DefaultAuthorActionEventHandler.md#getParagraphElement(ro.sync.ecss.extensions.api.AuthorAccess)) in class [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md) Parameters: authorAccess - The author access. Returns: the preferred XML element content to be inserted.
### areCompatibleLists

protected boolean areCompatibleLists([AuthorNode](node/AuthorNode.md) node1, [AuthorNode](node/AuthorNode.md) node2)
 Description copied from class: [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md#areCompatibleLists(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorNode))
Check if two given nodes are compatible lists (i.e. if we accept items from one list to migrate into the other one).
  Overrides: [areCompatibleLists](DefaultAuthorActionEventHandler.md#areCompatibleLists(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorNode)) in class [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md) Returns: true if the two given nodes are compatible lists. See Also:
        * [DefaultAuthorActionEventHandler.areCompatibleLists(ro.sync.ecss.extensions.api.node.AuthorNode, ro.sync.ecss.extensions.api.node.AuthorNode)](DefaultAuthorActionEventHandler.md#areCompatibleLists(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorNode))

### getListItemAncestorToSplit

public [AuthorElement](node/AuthorElement.md) getListItemAncestorToSplit([AuthorNode](node/AuthorNode.md) node, [AuthorAccess](AuthorAccess.md) access)
 Description copied from interface: [AuthorActionEventHandler](AuthorActionEventHandler.md#getListItemAncestorToSplit(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))
Return the list item ancestor of the current node that needs to be split on Enter.
  Parameters: node - The node. access - Access object to the Author API. Returns: the list item ancestor of the current node that needs to be split on Enter, or null. See Also:
        * [AuthorActionEventHandler.getListItemAncestorToSplit(ro.sync.ecss.extensions.api.node.AuthorNode, ro.sync.ecss.extensions.api.AuthorAccess)](AuthorActionEventHandler.md#getListItemAncestorToSplit(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))

### handleEvent

public boolean handleEvent([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) eventType)
 Description copied from interface: [AuthorActionEventHandler](AuthorActionEventHandler.md#handleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType))
An event was generated.
  Specified by: [handleEvent](AuthorActionEventHandler.md#handleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType)) in interface [AuthorActionEventHandler](AuthorActionEventHandler.md) Overrides: [handleEvent](DefaultAuthorActionEventHandler.md#handleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType)) in class [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md) Parameters: authorAccess - Author access. eventType - The type of the generated event. Returns: true if the event was handled and the default operation should be skipped, false to let the default operation execute. See Also:
        * [DefaultAuthorActionEventHandler.handleEvent(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType)](DefaultAuthorActionEventHandler.md#handleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType))

### canHandleEvent

public boolean canHandleEvent([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventDetails](AuthorActionEventDetails.md) eventDetails)
 Description copied from interface: [AuthorActionEventHandler](AuthorActionEventHandler.md#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventDetails))
Check if an Author action event can be handled.
  Parameters: authorAccess - Access to the Author API. eventDetails - The details of the event generated. Returns: true if the Author action event can be handled. See Also:
        * [AuthorActionEventHandler.canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorActionEventDetails)](AuthorActionEventHandler.md#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventDetails))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
