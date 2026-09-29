Package [ro.sync.ecss.extensions.api.webapp.ce](package-summary.md)

# Interface PeerContext
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface PeerContext
Context information about a document model that is part of a [Room](Room.md).
  Since: 23
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html) [getAttribute](#getAttribute(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
Method used to retrieve session attributes from [EditingSessionContext](../../access/EditingSessionContext.md)that were present when the document model joined the [Room](Room.md).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAuthorName](#getAuthorName())()

## Method Details

### getAuthorName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAuthorName()
  Returns: The author name used for example when adding review comments.
### getAttribute

[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html) getAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)

Method used to retrieve session attributes from [EditingSessionContext](../../access/EditingSessionContext.md)that were present when the document model joined the [Room](Room.md). Only attributes with a [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html) value can be retrieved.
  Parameters: attributeName - The attribute name. Returns: The attribute value.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
