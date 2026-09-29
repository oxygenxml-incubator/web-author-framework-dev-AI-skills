Package [ro.sync.ecss.extensions.commons.operations.text](package-summary.md)

# Class ToLowerCaseOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.operations.text.SelectedTextOperation](SelectedTextOperation.md)
        * ro.sync.ecss.extensions.commons.operations.text.ToLowerCaseOperation
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class ToLowerCaseOperation extends [SelectedTextOperation](SelectedTextOperation.md)
Provides an operation to convert the text from a selection into lower case text.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [ToLowerCaseOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()
No arguments necessary.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [processText](#processText(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text)
Processes text and makes it lower cased.

### Methods inherited from class ro.sync.ecss.extensions.commons.operations.text.[SelectedTextOperation](SelectedTextOperation.md)
 [doOperation](SelectedTextOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ToLowerCaseOperation

public ToLowerCaseOperation()

## Method Details

### processText

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) processText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text)

Processes text and makes it lower cased.
  Specified by: [processText](SelectedTextOperation.md#processText(java.lang.String)) in class [SelectedTextOperation](SelectedTextOperation.md) Parameters: text - The text to be processed. Returns: The text after process.
### getArguments

public [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] getArguments()

No arguments necessary.
  Specified by: [getArguments](../../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../../api/AuthorOperation.md) Overrides: [getArguments](SelectedTextOperation.md#getArguments()) in class [SelectedTextOperation](SelectedTextOperation.md) Returns: An array of [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments())

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
