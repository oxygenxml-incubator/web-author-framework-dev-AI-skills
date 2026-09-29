Package [ro.sync.ecss.dita.reference.reltable](package-summary.md)

# Interface RelLink
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface RelLink
Defines a relationship between two topic URLs. The source URL refers to the target URL.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getSourceURL](#getSourceURL())()

 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getTargetDefinitionLocation](#getTargetDefinitionLocation())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTargetFormat](#getTargetFormat())()
Get the format of the target resource.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTargetScope](#getTargetScope())()
Get the scope of the target resource.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getTargetURL](#getTargetURL())()

## Method Details

### getSourceURL

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getSourceURL()
  Returns: Returns the source URL.
### getTargetURL

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getTargetURL()
  Returns: Returns the target URL.
### getTargetScope

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTargetScope()

Get the scope of the target resource.
  Returns: The scope of the target resource.
### getTargetFormat

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTargetFormat()

Get the format of the target resource.
  Returns: The format of the target resource.
### getTargetDefinitionLocation

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getTargetDefinitionLocation()
  Returns: Returns the target definition location.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
