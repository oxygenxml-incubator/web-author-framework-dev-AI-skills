Package [ro.sync.exml.workspace.api.componentscollector](package-summary.md)

# Interface IComponentInfo
    All Known Subinterfaces: [IXSLComponentInfo](IXSLComponentInfo.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface IComponentInfo
Component information interface.
  Since: 27
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAnnotation](#getAnnotation())()

 int [getEndOffset](#getEndOffset())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()

 int [getStartOffset](#getStartOffset())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSystemId](#getSystemId())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getType](#getType())()

## Method Details

### getName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()
  Returns: Returns the name of the component.
### getSystemId

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSystemId()
  Returns: Returns the system ID of the current file in an URL format.
### getType

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getType()
  Returns: Returns the type of the component.
### getAnnotation

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAnnotation()
  Returns: Returns the annotation of the component.
### getStartOffset

int getStartOffset()
  Returns: Returns the start offset from the document . It returns 0 if the location cannot be determined.
### getEndOffset

int getEndOffset()
  Returns: Returns the end offset from the current document. It returns 0 if the location cannot be determined.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
