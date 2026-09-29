Package [ro.sync.exml.workspace.api.spell](package-summary.md)

# Interface Dictionary
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface Dictionary
This interface can be used to set an extra terms dictionary to be used on spell checking actions.
  Since: 21
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getSuggestions](#getSuggestions(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word)
Get suggestions for the word from the dictionaries of a certain user.
  boolean [isForbidden](#isForbidden(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word)
Check whether the word is forbidden considering dictionaries of a certain user.
  boolean [isLearned](#isLearned(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word)
Check whether the word is learned considering dictionaries of a certain user.

## Method Details

### isLearned

boolean isLearned([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word)

Check whether the word is learned considering dictionaries of a certain user.
  Parameters: lang - The language code, may be null. The language will be determined from the nearest ancestor with xml:lang attribute, otherwise will default to the user's interface language. Respects the xml:lang encoding (http://www.w3.org/TR/REC-xml/) Ex: "en", "en-GB", "en-US" word - The word to check. Returns: Whether the word is learned for a certain user.
### isForbidden

boolean isForbidden([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word)

Check whether the word is forbidden considering dictionaries of a certain user.
  Parameters: lang - The language code, may be null. The language will be determined from the nearest ancestor with xml:lang attribute, otherwise will default to the user's interface language. Respects the xml:lang encoding (http://www.w3.org/TR/REC-xml/) Ex: "en", "en-GB", "en-US" word - The word to check. Returns: Whether the word is forbidden for a certain user.
### getSuggestions

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getSuggestions([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) word)

Get suggestions for the word from the dictionaries of a certain user.
  Parameters: lang - The language code, may be null. The language will be determined from the nearest ancestor with xml:lang attribute, otherwise will default to the user's interface language. Respects the xml:lang encoding (http://www.w3.org/TR/REC-xml/) Ex: "en", "en-GB", "en-US" word - The word to check. Returns: A list of suggestions for the word, sorted by relevance.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
