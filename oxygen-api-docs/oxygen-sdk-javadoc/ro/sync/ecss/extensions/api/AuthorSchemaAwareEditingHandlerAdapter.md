Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorSchemaAwareEditingHandlerAdapter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandlerAdapter
   All Implemented Interfaces: [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md)   Direct Known Subclasses: [DITASchemaAwareEditingHandler](../dita/DITASchemaAwareEditingHandler.md), [DocbookSchemaAwareEditingHandler](../docbook/DocbookSchemaAwareEditingHandler.md), [TEISchemaAwareEditingHandler](../tei/TEISchemaAwareEditingHandler.md)   @API(type=EXTENDABLE, src=PUBLIC) public class AuthorSchemaAwareEditingHandlerAdapter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md)
Adapter class.

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static class  [AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions](AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions.md)
One of the default smart paste strategies involves detecting an path o ancestors from the context element to the inserted one.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) [lastHandlerResult](#lastHandlerResult)
Last handler result.

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md)
 [ACTION_ID_BACKSPACE](AuthorSchemaAwareEditingHandler.md#ACTION_ID_BACKSPACE), [ACTION_ID_CUT](AuthorSchemaAwareEditingHandler.md#ACTION_ID_CUT), [ACTION_ID_DELETE](AuthorSchemaAwareEditingHandler.md#ACTION_ID_DELETE), [ACTION_ID_DND](AuthorSchemaAwareEditingHandler.md#ACTION_ID_DND), [ACTION_ID_INSERT_FRAGMENT](AuthorSchemaAwareEditingHandler.md#ACTION_ID_INSERT_FRAGMENT), [ACTION_ID_PASTE](AuthorSchemaAwareEditingHandler.md#ACTION_ID_PASTE), [ACTION_ID_TYPING](AuthorSchemaAwareEditingHandler.md#ACTION_ID_TYPING), [CREATE_FRAGMENT_PURPOSE_COPY](AuthorSchemaAwareEditingHandler.md#CREATE_FRAGMENT_PURPOSE_COPY), [CREATE_FRAGMENT_PURPOSE_CUT](AuthorSchemaAwareEditingHandler.md#CREATE_FRAGMENT_PURPOSE_CUT), [CREATE_FRAGMENT_PURPOSE_DND_COPY](AuthorSchemaAwareEditingHandler.md#CREATE_FRAGMENT_PURPOSE_DND_COPY), [CREATE_FRAGMENT_PURPOSE_DND_MOVE](AuthorSchemaAwareEditingHandler.md#CREATE_FRAGMENT_PURPOSE_DND_MOVE)
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorSchemaAwareEditingHandlerAdapter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 boolean [canBeReplaced](#canBeReplaced(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) nodeToReplace)
When pasting an element inside an empty element with the same name, a possible solution is to replace the empty node with the new one.
  boolean [changeElementsToMoveUpDown](#changeElementsToMoveUpDown(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](node/AuthorNode.md)> selectedElements)
Determine the elements that should be moved by the Move Up/Down operation.
  [AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions](AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions.md) [getAncestorDetectionOptions](#getAncestorDetectionOptions())()
One of the default smart paste strategies involves detecting an path o ancestors from the context element to the inserted one.
  [SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) [getLastResult](#getLastResult())()  Deprecated.
Will be removed in a future version
   [QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html) [getPreferredElement](#getPreferredElement(ro.sync.ecss.extensions.api.AuthorDocumentController,int))([AuthorDocumentController](AuthorDocumentController.md) ctrl, int offset)
Get the qualified name of the best element to be inserted at the caret position as a wrapper for the content that is being typed or pasted.
  [AuthorDocumentFragment](node/AuthorDocumentFragment.md) [handleCreateDocumentFragment](#handleCreateDocumentFragment(int,int,int,ro.sync.ecss.extensions.api.AuthorAccess))(int startOffset, int endOffset, int creationPurposeID, [AuthorAccess](AuthorAccess.md) authorAccess)
Create an AuthorDocumentFragment for a paste or DnD purpose
  boolean [handleDelete](#handleDelete(int,int,ro.sync.ecss.extensions.api.AuthorAccess,boolean))(int offset, int deleteType, [AuthorAccess](AuthorAccess.md) authorAccess, boolean wordLevel)
Handle a keyboard delete event at the given offset (using Delete or Backspace keys) in the Author edit area.
  boolean [handleDeleteElementTags](#handleDeleteElementTags(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](node/AuthorNode.md) nodeToUnwrap, [AuthorAccess](AuthorAccess.md) authorAccess)
Handle delete element tags event.
  boolean [handleDeleteNodes](#handleDeleteNodes(ro.sync.ecss.extensions.api.node.AuthorNode%5B%5D,int,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](node/AuthorNode.md)[] nodes, int deleteType, [AuthorAccess](AuthorAccess.md) authorAccess)
Handle a delete nodes event coming from the Outline or Bread crumb.
  boolean [handleDeleteSelection](#handleDeleteSelection(int,int,int,ro.sync.ecss.extensions.api.AuthorAccess))(int selectionStart, int selectionEnd, int generatedByActionId, [AuthorAccess](AuthorAccess.md) authorAccess)
Handle a delete selection event in the Author edit area.
  boolean [handleJoinElements](#handleJoinElements(ro.sync.ecss.extensions.api.node.AuthorNode,java.util.List,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](node/AuthorNode.md) targetNode, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](node/AuthorNode.md)> nodesToJoin, [AuthorAccess](AuthorAccess.md) authorAccess)
Handle a join event between the given nodes.
  boolean [handlePasteFragment](#handlePasteFragment(int,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,int,ro.sync.ecss.extensions.api.AuthorAccess))(int offset, [AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragmentsToInsert, int actionId, [AuthorAccess](AuthorAccess.md) authorAccess)
Handle an insert fragment event generated by: a Paste action.
  boolean [handleTyping](#handleTyping(int,char,ro.sync.ecss.extensions.api.AuthorAccess))(int offset, char ch, [AuthorAccess](AuthorAccess.md) authorAccess)
Handle a typing event.
  boolean [handleTypingFallback](#handleTypingFallback(int,char,ro.sync.ecss.extensions.api.AuthorAccess))(int offset, char ch, [AuthorAccess](AuthorAccess.md) authorAccess)
Give a fallback solution for a typing event.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md)
 [handleCodePointTyping](AuthorSchemaAwareEditingHandler.md#handleCodePointTyping(int,int,ro.sync.ecss.extensions.api.AuthorAccess)), [handleCodePointTypingFallback](AuthorSchemaAwareEditingHandler.md#handleCodePointTypingFallback(int,int,ro.sync.ecss.extensions.api.AuthorAccess))
## Field Details

### lastHandlerResult

protected [SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) lastHandlerResult

Last handler result.

## Constructor Details

### AuthorSchemaAwareEditingHandlerAdapter

public AuthorSchemaAwareEditingHandlerAdapter()

## Method Details

### handleDelete

public boolean handleDelete(int offset, int deleteType, [AuthorAccess](AuthorAccess.md) authorAccess, boolean wordLevel)throws [InvalidEditException](InvalidEditException.md)
 Description copied from interface: [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md#handleDelete(int,int,ro.sync.ecss.extensions.api.AuthorAccess,boolean))
Handle a keyboard delete event at the given offset (using Delete or Backspace keys) in the Author edit area.
  Specified by: [handleDelete](AuthorSchemaAwareEditingHandler.md#handleDelete(int,int,ro.sync.ecss.extensions.api.AuthorAccess,boolean)) in interface [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) Parameters: offset - Offset where the delete event happened. deleteType - ACTION_ID_DELETE if Delete key was used or ACTION_ID_BACKSPACE for Backspace. authorAccess - Access class to the author functions. wordLevel - true if the user requested a delete for a whole word. Returns: true if the event was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected. See Also:
        * [AuthorSchemaAwareEditingHandler.handleDelete(int, int, ro.sync.ecss.extensions.api.AuthorAccess, boolean)](AuthorSchemaAwareEditingHandler.md#handleDelete(int,int,ro.sync.ecss.extensions.api.AuthorAccess,boolean))

### handleDeleteElementTags

public boolean handleDeleteElementTags([AuthorNode](node/AuthorNode.md) nodeToUnwrap, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)
 Description copied from interface: [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md#handleDeleteElementTags(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))
Handle delete element tags event. (Unwrapping)
  Specified by: [handleDeleteElementTags](AuthorSchemaAwareEditingHandler.md#handleDeleteElementTags(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) Parameters: nodeToUnwrap - The node to delete element tags. authorAccess - Access class to the author functions. Returns: true if the event was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected. See Also:
        * [AuthorSchemaAwareEditingHandler.handleDeleteElementTags(ro.sync.ecss.extensions.api.node.AuthorNode, ro.sync.ecss.extensions.api.AuthorAccess)](AuthorSchemaAwareEditingHandler.md#handleDeleteElementTags(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))

### handleDeleteSelection

public boolean handleDeleteSelection(int selectionStart, int selectionEnd, int generatedByActionId, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)
 Description copied from interface: [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md#handleDeleteSelection(int,int,int,ro.sync.ecss.extensions.api.AuthorAccess))
Handle a delete selection event in the Author edit area. The event is generated when a selection exists inside the document and one of following actions takes place:
        * typing (insert a new character in document by typing);
        * cut;
        * DND move;
        * delete or backspace.

  Specified by: [handleDeleteSelection](AuthorSchemaAwareEditingHandler.md#handleDeleteSelection(int,int,int,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) Parameters: selectionStart - Selection start offset, inclusive. selectionEnd - Selection end offset, inclusive. generatedByActionId - An id identifying the action that generated this event. One of the following constants are possible: ACTION_ID_TYPING, ACTION_ID_DELETE, ACTION_ID_PASTE, ACTION_ID_CUT, ACTION_ID_DND, ACTION_ID_INSERT_FRAGMENT. authorAccess - Access class to the author functions. Returns: true if the event was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected. See Also:
        * [AuthorSchemaAwareEditingHandler.handleDeleteSelection(int, int, int, ro.sync.ecss.extensions.api.AuthorAccess)](AuthorSchemaAwareEditingHandler.md#handleDeleteSelection(int,int,int,ro.sync.ecss.extensions.api.AuthorAccess))

### handleJoinElements

public boolean handleJoinElements([AuthorNode](node/AuthorNode.md) targetNode, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](node/AuthorNode.md)> nodesToJoin, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)
 Description copied from interface: [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md#handleJoinElements(ro.sync.ecss.extensions.api.node.AuthorNode,java.util.List,ro.sync.ecss.extensions.api.AuthorAccess))
Handle a join event between the given nodes.
  Specified by: [handleJoinElements](AuthorSchemaAwareEditingHandler.md#handleJoinElements(ro.sync.ecss.extensions.api.node.AuthorNode,java.util.List,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) Parameters: targetNode - The node where the content of the other nodes must migrate. nodesToJoin - The nodes that must be joined in the target node. authorAccess - Access class to the author functions. Returns: true if the event was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected. See Also:
        * [AuthorSchemaAwareEditingHandler.handleJoinElements(ro.sync.ecss.extensions.api.node.AuthorNode, java.util.List, ro.sync.ecss.extensions.api.AuthorAccess)](AuthorSchemaAwareEditingHandler.md#handleJoinElements(ro.sync.ecss.extensions.api.node.AuthorNode,java.util.List,ro.sync.ecss.extensions.api.AuthorAccess))

### handlePasteFragment

public boolean handlePasteFragment(int offset, [AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragmentsToInsert, int actionId, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)
 Description copied from interface: [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md#handlePasteFragment(int,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,int,ro.sync.ecss.extensions.api.AuthorAccess))
Handle an insert fragment event generated by:
        * a Paste action. In this case, selection removal is handled before calling this method.
        * a DND action. In this case source removal is handled after calling this method (unless an exception was thrown).
        * an insert fragment event occurred as a result of an schema aware insert event, like [AuthorDocumentController.insertXMLFragmentSchemaAware(String, int)](AuthorDocumentController.md#insertXMLFragmentSchemaAware(java.lang.String,int)). Selection removal is handled before calling this method.

  Specified by: [handlePasteFragment](AuthorSchemaAwareEditingHandler.md#handlePasteFragment(int,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,int,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) Parameters: offset - Offset where the event occurred. fragmentsToInsert - Fragments to be inserted. actionId - ACTION_ID_PASTE if event was generated by paste action, ACTION_ID_DND if it was generated by a DND event or ACTION_ID_INSERT_FRAGMENT if the event was generated by an [AuthorDocumentController](AuthorDocumentController.md) schema aware insert method. authorAccess - Access class to the author functions. Returns: true if the insertion was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected. See Also:
        * [AuthorSchemaAwareEditingHandler.handlePasteFragment(int, ro.sync.ecss.extensions.api.node.AuthorDocumentFragment[], int, ro.sync.ecss.extensions.api.AuthorAccess)](AuthorSchemaAwareEditingHandler.md#handlePasteFragment(int,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,int,ro.sync.ecss.extensions.api.AuthorAccess))

### handleTyping

public boolean handleTyping(int offset, char ch, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)
 Description copied from interface: [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md#handleTyping(int,char,ro.sync.ecss.extensions.api.AuthorAccess))
Handle a typing event. If the event is not handled, the default implementation of a handler will be given a chance to handle the event. If that fails to provide a solution, [AuthorSchemaAwareEditingHandler.handleTypingFallback(int, char, AuthorAccess)](AuthorSchemaAwareEditingHandler.md#handleTypingFallback(int,char,ro.sync.ecss.extensions.api.AuthorAccess))will get called.
  Specified by: [handleTyping](AuthorSchemaAwareEditingHandler.md#handleTyping(int,char,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) Parameters: offset - Offset where the typing occurred. ch - The typed character. authorAccess - Access class to the author functions. Returns: true if the typing was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected. See Also:
        * [AuthorSchemaAwareEditingHandler.handleTyping(int, char, ro.sync.ecss.extensions.api.AuthorAccess)](AuthorSchemaAwareEditingHandler.md#handleTyping(int,char,ro.sync.ecss.extensions.api.AuthorAccess))

### getLastResult

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) getLastResult()
 Deprecated.
Will be removed in a future version
   Returns: The result generated by the last handler method invoked before this call. Is null if event was not handled.
### handleCreateDocumentFragment

public [AuthorDocumentFragment](node/AuthorDocumentFragment.md) handleCreateDocumentFragment(int startOffset, int endOffset, int creationPurposeID, [AuthorAccess](AuthorAccess.md) authorAccess)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create an AuthorDocumentFragment for a paste or DnD purpose
  Specified by: [handleCreateDocumentFragment](AuthorSchemaAwareEditingHandler.md#handleCreateDocumentFragment(int,int,int,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) Parameters: startOffset - Start offset of fragment endOffset - End offset of fragment creationPurposeID - One of the CREATE_FRAGMENT_\* constants in this class. authorAccess - Access to the Author API. Returns: The created fragment or null if the event was not handled. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) Since: 12.1 See Also:
        * [AuthorSchemaAwareEditingHandler.handleCreateDocumentFragment(int, int, int, ro.sync.ecss.extensions.api.AuthorAccess)](AuthorSchemaAwareEditingHandler.md#handleCreateDocumentFragment(int,int,int,ro.sync.ecss.extensions.api.AuthorAccess))

### handleDeleteNodes

public boolean handleDeleteNodes([AuthorNode](node/AuthorNode.md)[] nodes, int deleteType, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)
 Description copied from interface: [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md#handleDeleteNodes(ro.sync.ecss.extensions.api.node.AuthorNode%5B%5D,int,ro.sync.ecss.extensions.api.AuthorAccess))
Handle a delete nodes event coming from the Outline or Bread crumb.
  Specified by: [handleDeleteNodes](AuthorSchemaAwareEditingHandler.md#handleDeleteNodes(ro.sync.ecss.extensions.api.node.AuthorNode%5B%5D,int,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) Parameters: nodes - The nodes to delete. deleteType - ACTION_ID_DELETE if the nodes were deleted directly by the user or ACTION_ID_DND if the nodes were deleted as a result of a drag and drop move operation in the Outline. authorAccess - Access class to the author functions. Returns: true if the event was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected. See Also:
        * [AuthorSchemaAwareEditingHandler.handleDeleteNodes(ro.sync.ecss.extensions.api.node.AuthorNode[], int, ro.sync.ecss.extensions.api.AuthorAccess)](AuthorSchemaAwareEditingHandler.md#handleDeleteNodes(ro.sync.ecss.extensions.api.node.AuthorNode%5B%5D,int,ro.sync.ecss.extensions.api.AuthorAccess))

### handleTypingFallback

public boolean handleTypingFallback(int offset, char ch, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)
 Description copied from interface: [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md#handleTypingFallback(int,char,ro.sync.ecss.extensions.api.AuthorAccess))
Give a fallback solution for a typing event. This call comes when this object's [AuthorSchemaAwareEditingHandler.handleTyping(int, char, AuthorAccess)](AuthorSchemaAwareEditingHandler.md#handleTyping(int,char,ro.sync.ecss.extensions.api.AuthorAccess)) method did not handle the typing event and neither did the [AuthorSchemaAwareEditingHandler.handleTyping(int, char, AuthorAccess)](AuthorSchemaAwareEditingHandler.md#handleTyping(int,char,ro.sync.ecss.extensions.api.AuthorAccess)) from the default implementation.
As a fallback solution, a paragraph can be inserted at the given offset (if allowed) and then the typed character can be inserted inside it.

  Specified by: [handleTypingFallback](AuthorSchemaAwareEditingHandler.md#handleTypingFallback(int,char,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) Parameters: offset - Offset where the typing occurred. ch - The typed character. authorAccess - Access class to the author functions. Returns: true if the typing was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected. See Also:
        * [AuthorSchemaAwareEditingHandler.handleTypingFallback(int, char, ro.sync.ecss.extensions.api.AuthorAccess)](AuthorSchemaAwareEditingHandler.md#handleTypingFallback(int,char,ro.sync.ecss.extensions.api.AuthorAccess))

### changeElementsToMoveUpDown

public boolean changeElementsToMoveUpDown([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](node/AuthorNode.md)> selectedElements)

Determine the elements that should be moved by the Move Up/Down operation. For example if the current selected element is a title then the element that should actually be moved is its parent (e.g. section for DocBook).
  Parameters: selectedElements - the selected elements in the author page. This list should be altered depending on the framework specific structure. For example if the current selected element is a title then the element that should actually be present in this list is its parent (e.g. section for DocBook). Returns: true if the list of elements to be moved was altered by the framework specific handler. Since: 15.2
### getAncestorDetectionOptions

public [AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions](AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions.md) getAncestorDetectionOptions()

One of the default smart paste strategies involves detecting an path o ancestors from the context element to the inserted one. These are the preferences that control how these ancestors are chosen.
  Returns: Preferences for choosing the best possible ancestors while building a path. Since: 18
### canBeReplaced

public boolean canBeReplaced([AuthorNode](node/AuthorNode.md) nodeToReplace)

When pasting an element inside an empty element with the same name, a possible solution is to replace the empty node with the new one. This callback has a chance of rejecting this behavior when, for example, the node to replace has important attributes set on it.
  Parameters: nodeToReplace - The node to replace. Returns: true if this node can be replaced by the strategy with a similar one. false if this node is important and must be kept in the document. Since: 18
### getPreferredElement

public [QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html) getPreferredElement([AuthorDocumentController](AuthorDocumentController.md) ctrl, int offset)

Get the qualified name of the best element to be inserted at the caret position as a wrapper for the content that is being typed or pasted.
  Parameters: ctrl - Provides methods for modifying the Author document. offset - The caret offset where the insertion is performed. Returns: the qualified name of the preferred element or null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
