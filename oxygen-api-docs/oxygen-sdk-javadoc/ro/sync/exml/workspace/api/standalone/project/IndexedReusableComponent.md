Package [ro.sync.exml.workspace.api.standalone.project](package-summary.md)

# Interface IndexedReusableComponent
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface IndexedReusableComponent
Represents information about an indexed reusable component

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getQName](#getQName())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTopicElementIDPath](#getTopicElementIDPath())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getURL](#getURL())()

## Method Details

### getQName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getQName()
  Returns: The XML tag name of the reusable component.
### getTopicElementIDPath

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTopicElementIDPath()
  Returns: a path like "topicID/elementID" to identify the reusable component inside the topic.
### getDescription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: a text description of the reusable component.
### getURL

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getURL()
  Returns: The URL path of the topic in which the component is defined
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
