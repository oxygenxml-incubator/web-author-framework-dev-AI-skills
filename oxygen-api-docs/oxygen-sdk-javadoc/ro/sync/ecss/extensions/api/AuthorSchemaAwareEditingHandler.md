Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorSchemaAwareEditingHandler
    All Known Implementing Classes: [AuthorSchemaAwareEditingHandlerAdapter](AuthorSchemaAwareEditingHandlerAdapter.md), [DITAMapSchemaAwareEditingHandler](../dita/map/DITAMapSchemaAwareEditingHandler.md), [DITASchemaAwareEditingHandler](../dita/DITASchemaAwareEditingHandler.md), [Docbook5SchemaAwareEditingHandler](../docbook/Docbook5SchemaAwareEditingHandler.md), [DocbookSchemaAwareEditingHandler](../docbook/DocbookSchemaAwareEditingHandler.md), [TEISchemaAwareEditingHandler](../tei/TEISchemaAwareEditingHandler.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorSchemaAwareEditingHandler
If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this handler. The handler can either resolve a specific case, let the default implementation take place or reject the edit entirely by throwing an [InvalidEditException](InvalidEditException.md).
It is recommended to extend class [AuthorSchemaAwareEditingHandlerAdapter](AuthorSchemaAwareEditingHandlerAdapter.md) in order to be protected from any API additions that may occur in interface [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md).

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [ACTION_ID_BACKSPACE](#ACTION_ID_BACKSPACE)
Delete action through backspace key.
  static final int [ACTION_ID_CUT](#ACTION_ID_CUT)
Cut action.
  static final int [ACTION_ID_DELETE](#ACTION_ID_DELETE)
Delete action through delete key.
  static final int [ACTION_ID_DND](#ACTION_ID_DND)
DND action.
  static final int [ACTION_ID_INSERT_FRAGMENT](#ACTION_ID_INSERT_FRAGMENT)
Insert document fragment action by an action other than PASTE or DND.
  static final int [ACTION_ID_PASTE](#ACTION_ID_PASTE)
Paste action.
  static final int [ACTION_ID_TYPING](#ACTION_ID_TYPING)
Typing action.
  static final int [CREATE_FRAGMENT_PURPOSE_COPY](#CREATE_FRAGMENT_PURPOSE_COPY)
Create a fragment for copy.
  static final int [CREATE_FRAGMENT_PURPOSE_CUT](#CREATE_FRAGMENT_PURPOSE_CUT)
Create a fragment for cut.
  static final int [CREATE_FRAGMENT_PURPOSE_DND_COPY](#CREATE_FRAGMENT_PURPOSE_DND_COPY)
Create a fragment for DND copy.
  static final int [CREATE_FRAGMENT_PURPOSE_DND_MOVE](#CREATE_FRAGMENT_PURPOSE_DND_MOVE)
Create a fragment for DND move.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 default boolean [handleCodePointTyping](#handleCodePointTyping(int,int,ro.sync.ecss.extensions.api.AuthorAccess))(int offset, int codePoint, [AuthorAccess](AuthorAccess.md) authorAccess)
Handle a typing event.
  default boolean [handleCodePointTypingFallback](#handleCodePointTypingFallback(int,int,ro.sync.ecss.extensions.api.AuthorAccess))(int offset, int codePoint, [AuthorAccess](AuthorAccess.md) authorAccess)
Give a fallback solution for a typing event.
  [AuthorDocumentFragment](node/AuthorDocumentFragment.md) [handleCreateDocumentFragment](#handleCreateDocumentFragment(int,int,int,ro.sync.ecss.extensions.api.AuthorAccess))(int startOffset, int endOffset, int creationPurposeID, [AuthorAccess](AuthorAccess.md) authorAccess)
Create an AuthorDocumentFragment for a purpose
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

## Field Details

### ACTION_ID_TYPING

static final int ACTION_ID_TYPING

Typing action.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandler.ACTION_ID_TYPING)

### ACTION_ID_DELETE

static final int ACTION_ID_DELETE

Delete action through delete key.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandler.ACTION_ID_DELETE)

### ACTION_ID_BACKSPACE

static final int ACTION_ID_BACKSPACE

Delete action through backspace key.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandler.ACTION_ID_BACKSPACE)

### ACTION_ID_PASTE

static final int ACTION_ID_PASTE

Paste action.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandler.ACTION_ID_PASTE)

### ACTION_ID_CUT

static final int ACTION_ID_CUT

Cut action.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandler.ACTION_ID_CUT)

### ACTION_ID_DND

static final int ACTION_ID_DND

DND action.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandler.ACTION_ID_DND)

### ACTION_ID_INSERT_FRAGMENT

static final int ACTION_ID_INSERT_FRAGMENT

Insert document fragment action by an action other than PASTE or DND.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandler.ACTION_ID_INSERT_FRAGMENT)

### CREATE_FRAGMENT_PURPOSE_COPY

static final int CREATE_FRAGMENT_PURPOSE_COPY

Create a fragment for copy.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandler.CREATE_FRAGMENT_PURPOSE_COPY)

### CREATE_FRAGMENT_PURPOSE_CUT

static final int CREATE_FRAGMENT_PURPOSE_CUT

Create a fragment for cut.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandler.CREATE_FRAGMENT_PURPOSE_CUT)

### CREATE_FRAGMENT_PURPOSE_DND_COPY

static final int CREATE_FRAGMENT_PURPOSE_DND_COPY

Create a fragment for DND copy.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandler.CREATE_FRAGMENT_PURPOSE_DND_COPY)

### CREATE_FRAGMENT_PURPOSE_DND_MOVE

static final int CREATE_FRAGMENT_PURPOSE_DND_MOVE

Create a fragment for DND move.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandler.CREATE_FRAGMENT_PURPOSE_DND_MOVE)

## Method Details

### handleDelete

boolean handleDelete(int offset, int deleteType, [AuthorAccess](AuthorAccess.md) authorAccess, boolean wordLevel)throws [InvalidEditException](InvalidEditException.md)

Handle a keyboard delete event at the given offset (using Delete or Backspace keys) in the Author edit area.
  Parameters: offset - Offset where the delete event happened. deleteType - ACTION_ID_DELETE if Delete key was used or ACTION_ID_BACKSPACE for Backspace. authorAccess - Access class to the author functions. wordLevel - true if the user requested a delete for a whole word. Returns: true if the event was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected.
### handleDeleteNodes

boolean handleDeleteNodes([AuthorNode](node/AuthorNode.md)[] nodes, int deleteType, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)

Handle a delete nodes event coming from the Outline or Bread crumb.
  Parameters: nodes - The nodes to delete. deleteType - ACTION_ID_DELETE if the nodes were deleted directly by the user or ACTION_ID_DND if the nodes were deleted as a result of a drag and drop move operation in the Outline. authorAccess - Access class to the author functions. Returns: true if the event was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected. Since: 12.1
### handleDeleteSelection

boolean handleDeleteSelection(int selectionStart, int selectionEnd, int generatedByActionId, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)

Handle a delete selection event in the Author edit area. The event is generated when a selection exists inside the document and one of following actions takes place:
        * typing (insert a new character in document by typing);
        * cut;
        * DND move;
        * delete or backspace.

  Parameters: selectionStart - Selection start offset, inclusive. selectionEnd - Selection end offset, inclusive. generatedByActionId - An id identifying the action that generated this event. One of the following constants are possible: ACTION_ID_TYPING, ACTION_ID_DELETE, ACTION_ID_PASTE, ACTION_ID_CUT, ACTION_ID_DND, ACTION_ID_INSERT_FRAGMENT. authorAccess - Access class to the author functions. Returns: true if the event was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected.
### handlePasteFragment

boolean handlePasteFragment(int offset, [AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragmentsToInsert, int actionId, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)

Handle an insert fragment event generated by:
        * a Paste action. In this case, selection removal is handled before calling this method.
        * a DND action. In this case source removal is handled after calling this method (unless an exception was thrown).
        * an insert fragment event occurred as a result of an schema aware insert event, like [AuthorDocumentController.insertXMLFragmentSchemaAware(String, int)](AuthorDocumentController.md#insertXMLFragmentSchemaAware(java.lang.String,int)). Selection removal is handled before calling this method.

  Parameters: offset - Offset where the event occurred. fragmentsToInsert - Fragments to be inserted. actionId - ACTION_ID_PASTE if event was generated by paste action, ACTION_ID_DND if it was generated by a DND event or ACTION_ID_INSERT_FRAGMENT if the event was generated by an [AuthorDocumentController](AuthorDocumentController.md) schema aware insert method. authorAccess - Access class to the author functions. Returns: true if the insertion was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected.
### handleTyping

boolean handleTyping(int offset, char ch, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)

Handle a typing event. If the event is not handled, the default implementation of a handler will be given a chance to handle the event. If that fails to provide a solution, [handleTypingFallback(int, char, AuthorAccess)](#handleTypingFallback(int,char,ro.sync.ecss.extensions.api.AuthorAccess))will get called.
  Parameters: offset - Offset where the typing occurred. ch - The typed character. authorAccess - Access class to the author functions. Returns: true if the typing was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected.
### handleCodePointTyping

default boolean handleCodePointTyping(int offset, int codePoint, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)

Handle a typing event. If the event is not handled, the default implementation of a handler will be given a chance to handle the event. If that fails to provide a solution, [handleCodePointTypingFallback(int, int, AuthorAccess)](#handleCodePointTypingFallback(int,int,ro.sync.ecss.extensions.api.AuthorAccess))will get called.
  Parameters: offset - Offset where the typing occurred. codePoint - The typed Unicode code point. authorAccess - Access class to the author functions. Returns: true if the typing was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected. Since: 26.1
### handleTypingFallback

boolean handleTypingFallback(int offset, char ch, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)

Give a fallback solution for a typing event. This call comes when this object's [handleTyping(int, char, AuthorAccess)](#handleTyping(int,char,ro.sync.ecss.extensions.api.AuthorAccess)) method did not handle the typing event and neither did the [handleTyping(int, char, AuthorAccess)](#handleTyping(int,char,ro.sync.ecss.extensions.api.AuthorAccess)) from the default implementation.
As a fallback solution, a paragraph can be inserted at the given offset (if allowed) and then the typed character can be inserted inside it.

  Parameters: offset - Offset where the typing occurred. ch - The typed character. authorAccess - Access class to the author functions. Returns: true if the typing was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected. Since: 13.2
### handleCodePointTypingFallback

default boolean handleCodePointTypingFallback(int offset, int codePoint, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)

Give a fallback solution for a typing event. This call comes when this object's [handleCodePointTyping(int, int, AuthorAccess)](#handleCodePointTyping(int,int,ro.sync.ecss.extensions.api.AuthorAccess)) method did not handle the typing event and neither did the [handleCodePointTyping(int, int, AuthorAccess)](#handleCodePointTyping(int,int,ro.sync.ecss.extensions.api.AuthorAccess)) from the default implementation.
As a fallback solution, a paragraph can be inserted at the given offset (if allowed) and then the typed character can be inserted inside it.

  Parameters: offset - Offset where the typing occurred. codePoint - The typed Unicode code point. authorAccess - Access class to the author functions. Returns: true if the typing was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected. Since: 26.1
### handleDeleteElementTags

boolean handleDeleteElementTags([AuthorNode](node/AuthorNode.md) nodeToUnwrap, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)

Handle delete element tags event. (Unwrapping)
  Parameters: nodeToUnwrap - The node to delete element tags. authorAccess - Access class to the author functions. Returns: true if the event was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected.
### handleJoinElements

boolean handleJoinElements([AuthorNode](node/AuthorNode.md) targetNode, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](node/AuthorNode.md)> nodesToJoin, [AuthorAccess](AuthorAccess.md) authorAccess)throws [InvalidEditException](InvalidEditException.md)

Handle a join event between the given nodes.
  Parameters: targetNode - The node where the content of the other nodes must migrate. nodesToJoin - The nodes that must be joined in the target node. authorAccess - Access class to the author functions. Returns: true if the event was handled. Throws: [InvalidEditException](InvalidEditException.md) - This is an invalid edit and must be rejected.
### handleCreateDocumentFragment

[AuthorDocumentFragment](node/AuthorDocumentFragment.md) handleCreateDocumentFragment(int startOffset, int endOffset, int creationPurposeID, [AuthorAccess](AuthorAccess.md) authorAccess)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create an AuthorDocumentFragment for a purpose
  Parameters: authorAccess - Access to the Author API. startOffset - Start offset of fragment endOffset - End offset of fragment creationPurposeID - One of the CREATE_FRAGMENT_\* constants in this class. Returns: The created fragment or null if the event was not handled. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) Since: 12.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
