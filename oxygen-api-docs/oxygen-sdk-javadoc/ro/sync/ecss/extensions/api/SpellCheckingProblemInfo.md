Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class SpellCheckingProblemInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.SpellCheckingProblemInfo
   Direct Known Subclasses: [SpellCheckingProblemInfoWithSuggestions](SpellCheckingProblemInfoWithSuggestions.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class SpellCheckingProblemInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
## Constructor Summary
 Constructors
Constructor

Description
 [SpellCheckingProblemInfo](#%3Cinit%3E(int,int,int,java.lang.String,java.lang.String))(int startOffset, int endOffset, int errorCode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word)

 [SpellCheckingProblemInfo](#%3Cinit%3E(int,int,int,java.lang.String,java.lang.String,java.util.List))(int startOffset, int endOffset, int errorCode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> suggestions)

 [SpellCheckingProblemInfo](#%3Cinit%3E(int,int,int,java.lang.String,java.lang.String,java.util.List,ro.sync.ecss.extensions.api.webapp.WebAuthorSpellcheckErrorTypes,java.lang.String))(int startOffset, int endOffset, int errorCode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> suggestions, [WebAuthorSpellcheckErrorTypes](webapp/WebAuthorSpellcheckErrorTypes.md) errorType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) errorMessage)

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getEndOffset](#getEndOffset())()

 int [getErrorCode](#getErrorCode())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getErrorMessage](#getErrorMessage())()

 [WebAuthorSpellcheckErrorTypes](webapp/WebAuthorSpellcheckErrorTypes.md) [getErrorType](#getErrorType())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLanguageIsoName](#getLanguageIsoName())()

 int [getStartOffset](#getStartOffset())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getSuggestions](#getSuggestions())()
Get the suggestions for a word.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getWord](#getWord())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SpellCheckingProblemInfo

public SpellCheckingProblemInfo(int startOffset, int endOffset, int errorCode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word)
  Parameters: startOffset - Word start position. endOffset - Word end position. errorCode - Error code result from spellchecking. lang - ISO Name for the language of the word. word - Word between the offsets.
### SpellCheckingProblemInfo

public SpellCheckingProblemInfo(int startOffset, int endOffset, int errorCode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> suggestions)
  Parameters: startOffset - Word start position. endOffset - Word end position. errorCode - Error code result from spellchecking. lang - ISO Name for the language of the word. word - Word between the offsets. suggestions - The suggestions for the word.
### SpellCheckingProblemInfo

public SpellCheckingProblemInfo(int startOffset, int endOffset, int errorCode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> suggestions, [WebAuthorSpellcheckErrorTypes](webapp/WebAuthorSpellcheckErrorTypes.md) errorType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) errorMessage)
  Parameters: startOffset - Word start position. endOffset - Word end position. errorCode - Error code result from spellchecking. lang - ISO Name for the language of the word. word - Word between the offsets. suggestions - The suggestions for the word. errorType - The error type. errorMessage - Error message for the word. Since: 27.1\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

## Method Details

### getStartOffset

public int getStartOffset()
  Returns: Returns the start.
### getEndOffset

public int getEndOffset()
  Returns: Returns the end.
### getErrorCode

public int getErrorCode()
  Returns: Returns the err.
### getLanguageIsoName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLanguageIsoName()
  Returns: Returns the languageIsoName.
### getWord

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getWord()
  Returns: Returns the word.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### getSuggestions

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getSuggestions()

Get the suggestions for a word. Custom spell checking engines may provide suggestions on detection.
  Returns: Returns the suggestions for the word. Since: 21
### getErrorMessage

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getErrorMessage()
  Returns: Returns the error message for the word. Since: 28\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

### getErrorType

public [WebAuthorSpellcheckErrorTypes](webapp/WebAuthorSpellcheckErrorTypes.md) getErrorType()
  Returns: Returns the error type. Since: 28\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
