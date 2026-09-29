Package [ro.sync.exml.workspace.api.standalone.project.textcompletions](package-summary.md)

# Class CompletionProposalsOptions.Builder

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.standalone.project.textcompletions.CompletionProposalsOptions.Builder
   Enclosing class: [CompletionProposalsOptions](CompletionProposalsOptions.md)   public static class CompletionProposalsOptions.Builder extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Builder.

## Constructor Summary
 Constructors
Constructor

Description
 [Builder](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [CompletionProposalsOptions](CompletionProposalsOptions.md) [build](#build())()
Builds the options.
  [CompletionProposalsOptions.Builder](CompletionProposalsOptions.Builder.md) [withMaximumCompletionSize](#withMaximumCompletionSize(int))(int maximumCompletionSize)
Sets the maximum completion size.
  [CompletionProposalsOptions.Builder](CompletionProposalsOptions.Builder.md) [withMaximumNumberOfCompletions](#withMaximumNumberOfCompletions(int))(int maximumNumberOfCompletions)
Sets the maximum number of completions.
  [CompletionProposalsOptions.Builder](CompletionProposalsOptions.Builder.md) [withMaximumPrefixSize](#withMaximumPrefixSize(int))(int maximumPrefixSize)
Sets the maximum prefix size.
  [CompletionProposalsOptions.Builder](CompletionProposalsOptions.Builder.md) [withMinimumPrefixSize](#withMinimumPrefixSize(int))(int minimumPrefixSize)
Sets the minimum prefix size.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### Builder

public Builder()

Constructor.

## Method Details

### withMaximumNumberOfCompletions

public [CompletionProposalsOptions.Builder](CompletionProposalsOptions.Builder.md) withMaximumNumberOfCompletions(int maximumNumberOfCompletions)

Sets the maximum number of completions.
  Parameters: maximumNumberOfCompletions - The maximum number of distinct completions. Returns: The builder reference.
### withMaximumCompletionSize

public [CompletionProposalsOptions.Builder](CompletionProposalsOptions.Builder.md) withMaximumCompletionSize(int maximumCompletionSize)

Sets the maximum completion size. The default is 10.
  Parameters: maximumCompletionSize - The maximum completion size. Returns: The builder reference.
### withMinimumPrefixSize

public [CompletionProposalsOptions.Builder](CompletionProposalsOptions.Builder.md) withMinimumPrefixSize(int minimumPrefixSize)

Sets the minimum prefix size.
  Parameters: minimumPrefixSize - The minimum prefix size. Returns: The builder reference.
### withMaximumPrefixSize

public [CompletionProposalsOptions.Builder](CompletionProposalsOptions.Builder.md) withMaximumPrefixSize(int maximumPrefixSize)

Sets the maximum prefix size.
  Parameters: maximumPrefixSize - The maximum prefix size. Returns: The builder reference.
### build

public [CompletionProposalsOptions](CompletionProposalsOptions.md) build()

Builds the options.
  Returns: A new completion options object.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
