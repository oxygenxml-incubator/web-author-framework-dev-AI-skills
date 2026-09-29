Package [ro.sync.exml.workspace.api.standalone.project.textcompletions](package-summary.md)

# Class CompletionProposal

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.standalone.project.textcompletions.CompletionProposal
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public final class CompletionProposal extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Represents a text completion proposal.
  Since: 24.1
## Constructor Summary
 Constructors
Constructor

Description
 [CompletionProposal](#%3Cinit%3E(float,java.lang.String%5B%5D))(float score, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] tokens)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 float [getScore](#getScore())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTokens](#getTokens())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CompletionProposal

public CompletionProposal(float score, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] tokens)

Constructor.
  Parameters: score - The score of the proposal. tokens - The tokens that can follow the prefix.
## Method Details

### getTokens

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTokens()
  Returns: The tokens that can follow the prefix. Since: 24.1
### getScore

public float getScore()
  Returns: Returns the score of the proposal.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
