Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface DocumentContentDeletedEvent
    All Superinterfaces: [AuthorDocumentEvent](AuthorDocumentEvent.md), [DocumentContentChangedEvent](DocumentContentChangedEvent.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface DocumentContentDeletedEventextends [DocumentContentChangedEvent](DocumentContentChangedEvent.md)
Event received by an [AuthorListener](AuthorListener.md) when a deletion has been made in the content of the [AuthorDocument](node/AuthorDocument.md). It can have one of the types: [DocumentContentChangedEvent.DELETE_TEXT_EVENT](DocumentContentChangedEvent.md#DELETE_TEXT_EVENT) [DocumentContentChangedEvent.DELETE_FRAGMENT_EVENT](DocumentContentChangedEvent.md#DELETE_FRAGMENT_EVENT)

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[DocumentContentChangedEvent](DocumentContentChangedEvent.md)
 [DELETE_FRAGMENT_EVENT](DocumentContentChangedEvent.md#DELETE_FRAGMENT_EVENT), [DELETE_TEXT_EVENT](DocumentContentChangedEvent.md#DELETE_TEXT_EVENT), [INSERT_FRAGMENT_EVENT](DocumentContentChangedEvent.md#INSERT_FRAGMENT_EVENT), [INSERT_NODE_EVENT](DocumentContentChangedEvent.md#INSERT_NODE_EVENT), [INSERT_TEXT_EVENT](DocumentContentChangedEvent.md#INSERT_TEXT_EVENT)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorDocumentFragment](node/AuthorDocumentFragment.md) [getDeletedFragment](#getDeletedFragment())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDeletedText](#getDeletedText())()

### Methods inherited from interface ro.sync.ecss.extensions.api.[DocumentContentChangedEvent](DocumentContentChangedEvent.md)
 [getLength](DocumentContentChangedEvent.md#getLength()), [getOffset](DocumentContentChangedEvent.md#getOffset()), [getParentNode](DocumentContentChangedEvent.md#getParentNode()), [getType](DocumentContentChangedEvent.md#getType()), [isSimpleTextEdit](DocumentContentChangedEvent.md#isSimpleTextEdit())
## Method Details

### getDeletedText

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDeletedText()
  Returns: The deleted text if it is a simple text delete, [DocumentContentChangedEvent.DELETE_TEXT_EVENT](DocumentContentChangedEvent.md#DELETE_TEXT_EVENT). Null otherwise.
### getDeletedFragment

[AuthorDocumentFragment](node/AuthorDocumentFragment.md) getDeletedFragment()
  Returns: The deleted fragment if it is a fragment delete, [DocumentContentChangedEvent.DELETE_FRAGMENT_EVENT](DocumentContentChangedEvent.md#DELETE_FRAGMENT_EVENT). Null otherwise.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
