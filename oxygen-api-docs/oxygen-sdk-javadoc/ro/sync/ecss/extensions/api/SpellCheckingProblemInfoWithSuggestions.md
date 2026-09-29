Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class SpellCheckingProblemInfoWithSuggestions

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.SpellCheckingProblemInfo](SpellCheckingProblemInfo.md)
        * ro.sync.ecss.extensions.api.SpellCheckingProblemInfoWithSuggestions
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class SpellCheckingProblemInfoWithSuggestions extends [SpellCheckingProblemInfo](SpellCheckingProblemInfo.md)
## Constructor Summary
 Constructors
Constructor

Description
 [SpellCheckingProblemInfoWithSuggestions](#%3Cinit%3E(int,int,java.lang.String,java.lang.String,java.util.List))(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> suggestions)
Create spell checking result information for a word.
  [SpellCheckingProblemInfoWithSuggestions](#%3Cinit%3E(int,int,java.lang.String,java.lang.String,java.util.List,ro.sync.ecss.extensions.api.webapp.WebAuthorSpellcheckErrorTypes,java.lang.String))(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> suggestions, [WebAuthorSpellcheckErrorTypes](webapp/WebAuthorSpellcheckErrorTypes.md) errorType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) errorMessage)
Create spell checking result information for a word.

## Method Summary

### Methods inherited from class ro.sync.ecss.extensions.api.[SpellCheckingProblemInfo](SpellCheckingProblemInfo.md)
 [getEndOffset](SpellCheckingProblemInfo.md#getEndOffset()), [getErrorCode](SpellCheckingProblemInfo.md#getErrorCode()), [getErrorMessage](SpellCheckingProblemInfo.md#getErrorMessage()), [getErrorType](SpellCheckingProblemInfo.md#getErrorType()), [getLanguageIsoName](SpellCheckingProblemInfo.md#getLanguageIsoName()), [getStartOffset](SpellCheckingProblemInfo.md#getStartOffset()), [getSuggestions](SpellCheckingProblemInfo.md#getSuggestions()), [getWord](SpellCheckingProblemInfo.md#getWord()), [toString](SpellCheckingProblemInfo.md#toString())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SpellCheckingProblemInfoWithSuggestions

public SpellCheckingProblemInfoWithSuggestions(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> suggestions)

Create spell checking result information for a word.
  Parameters: startOffset - The start offset of the word. endOffset - The end offset of the word. lang - ISO Name for the language of the word. word - The word found at the offsets. suggestions - List of suggestions, should not be null. Since: 21
### SpellCheckingProblemInfoWithSuggestions

public SpellCheckingProblemInfoWithSuggestions(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> suggestions, [WebAuthorSpellcheckErrorTypes](webapp/WebAuthorSpellcheckErrorTypes.md) errorType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) errorMessage)

Create spell checking result information for a word.
  Parameters: startOffset - The start offset of the word. endOffset - The end offset of the word. lang - ISO Name for the language of the word. word - The word found at the offsets. suggestions - List of suggestions, should not be null. errorType - The error type. errorMessage - Error message for the word. Since: 28\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
