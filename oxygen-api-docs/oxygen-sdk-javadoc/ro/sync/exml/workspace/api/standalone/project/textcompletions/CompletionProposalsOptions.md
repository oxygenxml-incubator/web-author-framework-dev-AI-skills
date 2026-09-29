Package [ro.sync.exml.workspace.api.standalone.project.textcompletions](package-summary.md)

# Class CompletionProposalsOptions

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.standalone.project.textcompletions.CompletionProposalsOptions
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public final class CompletionProposalsOptions extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
A set of options for the completion selection algorithm.

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static class  [CompletionProposalsOptions.Builder](CompletionProposalsOptions.Builder.md)
Builder.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getMaximumCompletionSize](#getMaximumCompletionSize())()

 int [getMaximumNumberOfCompletions](#getMaximumNumberOfCompletions())()

 int [getMaximumPrefixSize](#getMaximumPrefixSize())()

 int [getMinimumPrefixSize](#getMinimumPrefixSize())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### getMaximumNumberOfCompletions

public int getMaximumNumberOfCompletions()
  Returns: The maximum number of continuations.
### getMaximumCompletionSize

public int getMaximumCompletionSize()
  Returns: The maximum number of continuations.
### getMinimumPrefixSize

public int getMinimumPrefixSize()
  Returns: The minimum prefix size.
### getMaximumPrefixSize

public int getMaximumPrefixSize()
  Returns: The maximum prefix size.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
