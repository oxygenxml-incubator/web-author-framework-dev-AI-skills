Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface DocumentContentInsertedEvent
    All Superinterfaces: [AuthorDocumentEvent](AuthorDocumentEvent.md), [DocumentContentChangedEvent](DocumentContentChangedEvent.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface DocumentContentInsertedEventextends [DocumentContentChangedEvent](DocumentContentChangedEvent.md)
Event received by an [AuthorListener](AuthorListener.md) when insertion have been made in the content of the [AuthorDocument](node/AuthorDocument.md). It can have one of the types: [DocumentContentChangedEvent.INSERT_TEXT_EVENT](DocumentContentChangedEvent.md#INSERT_TEXT_EVENT) [DocumentContentChangedEvent.INSERT_NODE_EVENT](DocumentContentChangedEvent.md#INSERT_NODE_EVENT) [DocumentContentChangedEvent.INSERT_FRAGMENT_EVENT](DocumentContentChangedEvent.md#INSERT_FRAGMENT_EVENT)

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[DocumentContentChangedEvent](DocumentContentChangedEvent.md)
 [DELETE_FRAGMENT_EVENT](DocumentContentChangedEvent.md#DELETE_FRAGMENT_EVENT), [DELETE_TEXT_EVENT](DocumentContentChangedEvent.md#DELETE_TEXT_EVENT), [INSERT_FRAGMENT_EVENT](DocumentContentChangedEvent.md#INSERT_FRAGMENT_EVENT), [INSERT_NODE_EVENT](DocumentContentChangedEvent.md#INSERT_NODE_EVENT), [INSERT_TEXT_EVENT](DocumentContentChangedEvent.md#INSERT_TEXT_EVENT)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorDocumentFragment](node/AuthorDocumentFragment.md) [getInsertedFragment](#getInsertedFragment())()

 [AuthorNode](node/AuthorNode.md) [getInsertedNode](#getInsertedNode())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getInsertedText](#getInsertedText())()

### Methods inherited from interface ro.sync.ecss.extensions.api.[DocumentContentChangedEvent](DocumentContentChangedEvent.md)
 [getLength](DocumentContentChangedEvent.md#getLength()), [getOffset](DocumentContentChangedEvent.md#getOffset()), [getParentNode](DocumentContentChangedEvent.md#getParentNode()), [getType](DocumentContentChangedEvent.md#getType()), [isSimpleTextEdit](DocumentContentChangedEvent.md#isSimpleTextEdit())
## Method Details

### getInsertedText

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getInsertedText()
  Returns: The inserted text if it is a simple text insert, [DocumentContentChangedEvent.INSERT_TEXT_EVENT](DocumentContentChangedEvent.md#INSERT_TEXT_EVENT). Null otherwise.
### getInsertedNode

[AuthorNode](node/AuthorNode.md) getInsertedNode()
  Returns: The inserted node if a node is inserted, [DocumentContentChangedEvent.INSERT_NODE_EVENT](DocumentContentChangedEvent.md#INSERT_NODE_EVENT). Null otherwise.
### getInsertedFragment

[AuthorDocumentFragment](node/AuthorDocumentFragment.md) getInsertedFragment()
  Returns: The inserted fragment if a fragment was inserted, [DocumentContentChangedEvent.INSERT_FRAGMENT_EVENT](DocumentContentChangedEvent.md#INSERT_FRAGMENT_EVENT). Null otherwise.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
