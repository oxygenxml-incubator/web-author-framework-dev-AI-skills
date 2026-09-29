Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class SpellSuggestionsInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.SpellSuggestionsInfo
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class SpellSuggestionsInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Container for spellchecking suggestions information.

## Constructor Summary
 Constructors
Constructor

Description
 [SpellSuggestionsInfo](#%3Cinit%3E(int,int,java.lang.String,java.lang.String%5B%5D))(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] suggestions)

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getEndOffset](#getEndOffset())()
Gets the end offset.
  int [getStartOffset](#getStartOffset())()
Gets the start offset.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getSuggestions](#getSuggestions())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getWord](#getWord())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SpellSuggestionsInfo

public SpellSuggestionsInfo(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] suggestions)
  Parameters: startOffset - Start offset of the word. endOffset - End offset of the word. word - The targeted word for suggestions. suggestions - List of suggestions.
## Method Details

### getStartOffset

public int getStartOffset()

Gets the start offset.
  Returns: Returns the start offset.
### getEndOffset

public int getEndOffset()

Gets the end offset.
  Returns: Returns the end offset.
### getWord

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getWord()
  Returns: Returns the word for which suggestions were provided.
### getSuggestions

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getSuggestions()
  Returns: Returns the suggestions.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
