Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AttributeChangedEvent
    All Superinterfaces: [AuthorDocumentEvent](AuthorDocumentEvent.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AttributeChangedEventextends [AuthorDocumentEvent](AuthorDocumentEvent.md)
Event received by the [AuthorListener](AuthorListener.md) when an Author attribute has been changed.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeName](#getAttributeName())()
Returns the name of the attribute that was changed.
  [AuthorNode](node/AuthorNode.md) [getOwnerAuthorNode](#getOwnerAuthorNode())()
Returns the owner [AuthorNode](node/AuthorNode.md) of the attribute.

## Method Details

### getOwnerAuthorNode

[AuthorNode](node/AuthorNode.md) getOwnerAuthorNode()

Returns the owner [AuthorNode](node/AuthorNode.md) of the attribute.
  Returns: The owner node.
### getAttributeName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeName()

Returns the name of the attribute that was changed.
  Returns: The name of the attribute that was changed.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
