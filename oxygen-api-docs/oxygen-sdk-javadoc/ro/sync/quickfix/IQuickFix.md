Package [ro.sync.quickfix](package-summary.md)

# Interface IQuickFix
    public interface IQuickFix
The interface describing a quick fix.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()
A human readable description for the quick fix.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFixedProblemDescription](#getFixedProblemDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFixId](#getFixId())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
A quick fix name.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.quickfix.SystemIDXMLOperationPair> [getOperations](#getOperations())()
The list with the operations associated with this quick fix.
  [QuickFixType](QuickFixType.md) [getQuickFixType](#getQuickFixType())()

## Method Details

### getName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

A quick fix name. For example it may be: Insert element 'person', Set attribute id.
  Returns: Returns a quick fix name.
### getDescription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()

A human readable description for the quick fix.
  Returns: Returns a human readable description for the quick fix.
### getOperations

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.quickfix.SystemIDXMLOperationPair> getOperations()

The list with the operations associated with this quick fix. They will be executed when applying this quick fix.
  Returns: The list with the commands associated with this script.
### getQuickFixType

[QuickFixType](QuickFixType.md) getQuickFixType()
  Returns: The type ID of the quick fix.
### getFixedProblemDescription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFixedProblemDescription()
  Returns: A description about the original problem. It is preferable to be a small because it could be used in the UI for grouping.
### getFixId

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFixId()
  Returns: An unique ID of the quick fix.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
