Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface DocumentContentChangedEvent
    All Superinterfaces: [AuthorDocumentEvent](AuthorDocumentEvent.md)   All Known Subinterfaces: [DocumentContentDeletedEvent](DocumentContentDeletedEvent.md), [DocumentContentInsertedEvent](DocumentContentInsertedEvent.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface DocumentContentChangedEventextends [AuthorDocumentEvent](AuthorDocumentEvent.md)
Event received by an [AuthorListener](AuthorListener.md) when changes have been made in the content of the [AuthorDocument](node/AuthorDocument.md).

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [DELETE_FRAGMENT_EVENT](#DELETE_FRAGMENT_EVENT)
Delete fragment event type.
  static final int [DELETE_TEXT_EVENT](#DELETE_TEXT_EVENT)
Delete simple text event type.
  static final int [INSERT_FRAGMENT_EVENT](#INSERT_FRAGMENT_EVENT)
Insert fragment event type.
  static final int [INSERT_NODE_EVENT](#INSERT_NODE_EVENT)
Insert node event type.
  static final int [INSERT_TEXT_EVENT](#INSERT_TEXT_EVENT)
Insert simple text event type.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 int [getLength](#getLength())()
Returns the length of the change.
  int [getOffset](#getOffset())()
Returns the start offset at which the change occurred.
  [AuthorNode](node/AuthorNode.md) [getParentNode](#getParentNode())()
Returns the [AuthorNode](node/AuthorNode.md) containing the change.
  int [getType](#getType())()
Returns the type of this event.
  boolean [isSimpleTextEdit](#isSimpleTextEdit())()  Deprecated.
Use [getType()](#getType()) to determine the type of edit.

## Field Details

### INSERT_TEXT_EVENT

static final int INSERT_TEXT_EVENT

Insert simple text event type.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.DocumentContentChangedEvent.INSERT_TEXT_EVENT)

### INSERT_NODE_EVENT

static final int INSERT_NODE_EVENT

Insert node event type.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.DocumentContentChangedEvent.INSERT_NODE_EVENT)

### INSERT_FRAGMENT_EVENT

static final int INSERT_FRAGMENT_EVENT

Insert fragment event type.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.DocumentContentChangedEvent.INSERT_FRAGMENT_EVENT)

### DELETE_TEXT_EVENT

static final int DELETE_TEXT_EVENT

Delete simple text event type.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.DocumentContentChangedEvent.DELETE_TEXT_EVENT)

### DELETE_FRAGMENT_EVENT

static final int DELETE_FRAGMENT_EVENT

Delete fragment event type.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.DocumentContentChangedEvent.DELETE_FRAGMENT_EVENT)

## Method Details

### getLength

int getLength()

Returns the length of the change.
  Returns: the length of the change. Zero in case of an attribute change.
### getOffset

int getOffset()

Returns the start offset at which the change occurred.
  Returns: the offset at which the change occurred. 0 in case of an attribute change.
### getParentNode

[AuthorNode](node/AuthorNode.md) getParentNode()

Returns the [AuthorNode](node/AuthorNode.md) containing the change.
  Returns: The node containing the change.
### isSimpleTextEdit

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) boolean isSimpleTextEdit()
 Deprecated.
Use [getType()](#getType()) to determine the type of edit.

Needed to verify if the change was a simple text edit and no node structure was affected.
  Returns: true if the edit was a simple text edit, no node structure was affected.
### getType

int getType()

Returns the type of this event. It can be one of the constants: [INSERT_TEXT_EVENT](#INSERT_TEXT_EVENT), [INSERT_FRAGMENT_EVENT](#INSERT_FRAGMENT_EVENT), [INSERT_NODE_EVENT](#INSERT_NODE_EVENT) [DELETE_TEXT_EVENT](#DELETE_TEXT_EVENT), [DELETE_FRAGMENT_EVENT](#DELETE_FRAGMENT_EVENT)
  Returns: The document changed event type.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
