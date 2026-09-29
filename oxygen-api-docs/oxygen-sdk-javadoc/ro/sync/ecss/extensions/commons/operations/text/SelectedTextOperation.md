Package [ro.sync.ecss.extensions.commons.operations.text](package-summary.md)

# Class SelectedTextOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.operations.text.SelectedTextOperation
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   Direct Known Subclasses: [ToLowerCaseOperation](ToLowerCaseOperation.md), [ToUpperCaseOperation](ToUpperCaseOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class SelectedTextOperation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorOperation](../../../api/AuthorOperation.md)
Provides upper case and lower case operations over a selected text.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [SelectedTextOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) arguments)
Process the selected text and make it lower case or upper case.
  [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [processText](#processText(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text)
Process text.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../../api/Extension.md)
 [getDescription](../../../api/Extension.md#getDescription())
## Constructor Details

### SelectedTextOperation

public SelectedTextOperation()

## Method Details

### getArguments

public [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] getArguments()
  Specified by: [getArguments](../../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../../api/AuthorOperation.md) Returns: An array of [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments())

### doOperation

public void doOperation([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) arguments)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Process the selected text and make it lower case or upper case.
  Specified by: [doOperation](../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in interface [AuthorOperation](../../../api/AuthorOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. arguments - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AuthorOperation.doOperation(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### processText

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) processText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text)

Process text.
  Parameters: text - The text to be processed. Returns: The text after process.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
