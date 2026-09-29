Package [ro.sync.ecss.extensions.api.access](package-summary.md)

# Interface UnsavedReferenceNodeDescriptor
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface UnsavedReferenceNodeDescriptor
Descriptor for an [AuthorReferenceNode](../node/AuthorReferenceNode.md) that contains an unsaved reference.
  Since: 23
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getUrl](#getUrl())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXmlFragment](#getXmlFragment())()

## Method Details

### getUrl

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getUrl()
  Returns: The URL from which the referenced content was loaded.
### getXmlFragment

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXmlFragment()
  Returns: The reference node serialized as an XML fragment.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
