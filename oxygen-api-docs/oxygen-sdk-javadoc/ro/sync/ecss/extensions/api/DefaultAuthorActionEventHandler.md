Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class DefaultAuthorActionEventHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorActionEventHandlerBase](AuthorActionEventHandlerBase.md)
        * ro.sync.ecss.extensions.api.DefaultAuthorActionEventHandler
   All Implemented Interfaces: [AuthorActionEventHandler](AuthorActionEventHandler.md), [Extension](Extension.md)   Direct Known Subclasses: [DITAAuthorActionEventHandler](DITAAuthorActionEventHandler.md), [DocbookAuthorActionEventHandler](DocbookAuthorActionEventHandler.md), [TEIAuthorActionEventHandler](TEIAuthorActionEventHandler.md), [XHTMLAuthorActionEventHandler](XHTMLAuthorActionEventHandler.md)   @API(type=EXTENDABLE, src=PUBLIC) public class DefaultAuthorActionEventHandler extends [AuthorActionEventHandlerBase](AuthorActionEventHandlerBase.md)
Intercepts TAB and SHIFT+TAB events inside a list item and promotes or demotes it.
  Since: 18
## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 protected static class  [DefaultAuthorActionEventHandler.CiElementAndOffset](DefaultAuthorActionEventHandler.CiElementAndOffset.md)
A simple structure to return from the method getInsertableFormForElement both the CIElement that can be inserted for a given element and the offset that should be applied to the insertion position in order to insert it.

## Nested classes/interfaces inherited from interface ro.sync.ecss.extensions.api.[AuthorActionEventHandler](AuthorActionEventHandler.md)
 [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md)
## Constructor Summary
 Constructors
Constructor

Description
 [DefaultAuthorActionEventHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [areCompatibleLists](#areCompatibleLists(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node1, [AuthorNode](node/AuthorNode.md) node2)
Check if two given nodes are compatible lists (i.e.
  boolean [canHandleEvent](#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType))([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) type)
Check if an Author action event can be handled.
  protected static void [deleteNodeChildren](#deleteNodeChildren(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorDocumentController](AuthorDocumentController.md) controller, [AuthorNode](node/AuthorNode.md) insertedNode)
Delete node contents.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[IAuthorExtensionAction](editor/IAuthorExtensionAction.md)> [getContentCompletionActions](#getContentCompletionActions(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](AuthorAccess.md) authorAccess, int caretOffset)
Intercepts action events in the Author mode and provides them in the content completion lists.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected [DefaultAuthorActionEventHandler.CiElementAndOffset](DefaultAuthorActionEventHandler.CiElementAndOffset.md) [getInsertableFormForElement](#getInsertableFormForElement(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorDocumentController](AuthorDocumentController.md) controller, [AuthorElement](node/AuthorElement.md) element, int insertPos)

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getParagraphElement](#getParagraphElement(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Get the preferred XML element content to be inserted.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPreferredXMLElementContent](#getPreferredXMLElementContent(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Get the preferred XML element content to be inserted.
  boolean [handleEvent](#handleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType))([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) eventType)
An event was generated.
  protected boolean [isList](#isList(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node)
Check if the given node is a list.
  protected boolean [isMovableListItem](#isMovableListItem(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorNode](node/AuthorNode.md) candidate)
Checks if this node represents a list item that can be promoted/demoted.
  protected [ContentInterval](ContentInterval.md) [promote](#promote(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.util.List,boolean))([AuthorDocumentController](AuthorDocumentController.md) controller, int offset, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](node/AuthorNode.md)> candidates, boolean hasSelection)
Unwraps these list items from the list.
  protected void [promoteSubListItems](#promoteSubListItems(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorDocumentController](AuthorDocumentController.md) controller, [AuthorNode](node/AuthorNode.md) theDemotedCandidate, [AuthorNode](node/AuthorNode.md) listElement)
Sometimes, when we demote a list item, we want it to become the sibling of its children.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorActionEventHandler](AuthorActionEventHandler.md)
 [canHandleEvent](AuthorActionEventHandler.md#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventDetails)), [getListItemAncestorToSplit](AuthorActionEventHandler.md#getListItemAncestorToSplit(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))
## Constructor Details

### DefaultAuthorActionEventHandler

public DefaultAuthorActionEventHandler()

## Method Details

### handleEvent

public boolean handleEvent([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) eventType)
 Description copied from interface: [AuthorActionEventHandler](AuthorActionEventHandler.md#handleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType))
An event was generated.
  Parameters: authorAccess - Author access. eventType - The type of the generated event. Returns: true if the event was handled and the default operation should be skipped, false to let the default operation execute. See Also:
        * [AuthorActionEventHandler.handleEvent(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType)](AuthorActionEventHandler.md#handleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType))

### getPreferredXMLElementContent

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPreferredXMLElementContent([AuthorAccess](AuthorAccess.md) authorAccess)

Get the preferred XML element content to be inserted. Can be null.
  Parameters: authorAccess - The author access. Returns: the preferred XML element content to be inserted. Can be null
### getParagraphElement

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getParagraphElement([AuthorAccess](AuthorAccess.md) authorAccess)

Get the preferred XML element content to be inserted. Can be null.
  Parameters: authorAccess - The author access. Returns: the preferred XML element content to be inserted.
### isMovableListItem

protected boolean isMovableListItem([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorNode](node/AuthorNode.md) candidate)

Checks if this node represents a list item that can be promoted/demoted.
  Parameters: authorAccess - The Author access. candidate - The node that candidates for promotion/demotion. Returns: true if the list item can be promoted/demoted.
### promote

protected [ContentInterval](ContentInterval.md) promote([AuthorDocumentController](AuthorDocumentController.md) controller, int offset, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](node/AuthorNode.md)> candidates, boolean hasSelection)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [AuthorOperationException](AuthorOperationException.md)

Unwraps these list items from the list. Moves them up one level in the hierarchy of nested lists.
  Parameters: controller - Author document controller. offset - If there is no selection, this is the offset where the action is invoked. Otherwise, this represents the end offset of the selection, needed for restoring caret position. candidates - The list items to promote. hasSelection - true if the promotion is performed on a selection. Returns: If there was no selection, return an interval from the next caret position to itself. Otherwise, if the selection was forward, return an interval from the lower offset to the higher one, or if the selection was backward, return an interval from the higher offset to the lower one. "From" means start offset and "to" means end offset. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [AuthorOperationException](AuthorOperationException.md)
### deleteNodeChildren

protected static void deleteNodeChildren([AuthorDocumentController](AuthorDocumentController.md) controller, [AuthorNode](node/AuthorNode.md) insertedNode)

Delete node contents.
  Parameters: controller - The controller. insertedNode - The inserted node.
### getInsertableFormForElement

protected [DefaultAuthorActionEventHandler.CiElementAndOffset](DefaultAuthorActionEventHandler.CiElementAndOffset.md) getInsertableFormForElement([AuthorDocumentController](AuthorDocumentController.md) controller, [AuthorElement](node/AuthorElement.md) element, int insertPos)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
  Parameters: controller - The document controller. element - The element. insertPos - The insertion position. Returns: a CIElement that represents the given element. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### promoteSubListItems

protected void promoteSubListItems([AuthorDocumentController](AuthorDocumentController.md) controller, [AuthorNode](node/AuthorNode.md) theDemotedCandidate, [AuthorNode](node/AuthorNode.md) listElement)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [AuthorOperationException](AuthorOperationException.md)

Sometimes, when we demote a list item, we want it to become the sibling of its children. To obtain this, after demoting the item along with its children, we promote the children. This method promotes the children.
  Parameters: controller - The Author document controller. theDemotedCandidate - The candidate which was demoted. listElement - The parent list of the demoted item. Throws: [AuthorOperationException](AuthorOperationException.md) [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### isList

protected boolean isList([AuthorNode](node/AuthorNode.md) node)

Check if the given node is a list.
  Parameters: node - The node. Returns: true if the node is a list.
### areCompatibleLists

protected boolean areCompatibleLists([AuthorNode](node/AuthorNode.md) node1, [AuthorNode](node/AuthorNode.md) node2)

Check if two given nodes are compatible lists (i.e. if we accept items from one list to migrate into the other one).
  Returns: true if the two given nodes are compatible lists.
### canHandleEvent

public boolean canHandleEvent([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) type)
 Description copied from interface: [AuthorActionEventHandler](AuthorActionEventHandler.md#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType))
Check if an Author action event can be handled.
  Parameters: authorAccess - Access to the Author API. type - The type of event generated. Returns: true if the Author action event can be handled. See Also:
        * [AuthorActionEventHandler.canHandleEvent(AuthorAccess, AuthorActionEventType)](AuthorActionEventHandler.md#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](Extension.md#getDescription())

### getContentCompletionActions

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[IAuthorExtensionAction](editor/IAuthorExtensionAction.md)> getContentCompletionActions([AuthorAccess](AuthorAccess.md) authorAccess, int caretOffset)

Intercepts action events in the Author mode and provides them in the content completion lists.
  Overrides: [getContentCompletionActions](AuthorActionEventHandlerBase.md#getContentCompletionActions(ro.sync.ecss.extensions.api.AuthorAccess,int)) in class [AuthorActionEventHandlerBase](AuthorActionEventHandlerBase.md) Parameters: authorAccess - The author access. caretOffset - The caret offset. Returns: The content completion actions.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
