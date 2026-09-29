Package [ro.sync.ecss.extensions.commons.operations.text](package-summary.md)

# Class CapitalizeSentencesOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.operations.text.FormSelectedTextOperation](FormSelectedTextOperation.md)
        * ro.sync.ecss.extensions.commons.operations.text.CapitalizeSentencesOperation
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class CapitalizeSentencesOperation extends [FormSelectedTextOperation](FormSelectedTextOperation.md)
The class provides an operation for forming sentences over a selection. If the start character of a sentence is lower case, it will be changed to upper case.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [CapitalizeSentencesOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected boolean [isDelimiterBeforeTextNode](#isDelimiterBeforeTextNode(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, int contentOffset)
Decides if there is a sentence delimiter before the text node.
  protected char[] [processTextContent](#processTextContent(char%5B%5D,boolean))(char[] charArray, boolean isDelimiterBefore)
Process char array and upper case first letter of containing sentences.

### Methods inherited from class ro.sync.ecss.extensions.commons.operations.text.[FormSelectedTextOperation](FormSelectedTextOperation.md)
 [doOperation](FormSelectedTextOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](FormSelectedTextOperation.md#getArguments()), [isWordDelimiter](FormSelectedTextOperation.md#isWordDelimiter(char))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CapitalizeSentencesOperation

public CapitalizeSentencesOperation()

## Method Details

### isDelimiterBeforeTextNode

protected boolean isDelimiterBeforeTextNode([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, int contentOffset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from class: [FormSelectedTextOperation](FormSelectedTextOperation.md#isDelimiterBeforeTextNode(ro.sync.ecss.extensions.api.AuthorAccess,int))
Decides if there is a sentence delimiter before the text node.
  Specified by: [isDelimiterBeforeTextNode](FormSelectedTextOperation.md#isDelimiterBeforeTextNode(ro.sync.ecss.extensions.api.AuthorAccess,int)) in class [FormSelectedTextOperation](FormSelectedTextOperation.md) contentOffset - The offset where search is started. Returns: true if the there is a sentence delimiter before the text node or false if a non-delimiter character was found. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [AuthorOperationException](../../../api/AuthorOperationException.md) See Also:
        * [FormSelectedTextOperation.isDelimiterBeforeTextNode(ro.sync.ecss.extensions.api.AuthorAccess, int)](FormSelectedTextOperation.md#isDelimiterBeforeTextNode(ro.sync.ecss.extensions.api.AuthorAccess,int))

### processTextContent

protected char[] processTextContent(char[] charArray, boolean isDelimiterBefore)

Process char array and upper case first letter of containing sentences.
  Specified by: [processTextContent](FormSelectedTextOperation.md#processTextContent(char%5B%5D,boolean)) in class [FormSelectedTextOperation](FormSelectedTextOperation.md) Parameters: charArray - The character array that must be processed. isDelimiterBefore - true if we have a delimiter before the given char array, false otherwise.
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
