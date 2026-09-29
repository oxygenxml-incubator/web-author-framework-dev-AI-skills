Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Interface WebappSpellchecker
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WebappSpellchecker
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[SpellCheckingProblemInfo](../SpellCheckingProblemInfo.md)> [check](#check(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TextChunkDescriptor](../../../../exml/workspace/api/util/TextChunkDescriptor.md)> textDescriptors)
Performs a spellcheck of the given text descriptors.
  [SpellSuggestionsInfo](../SpellSuggestionsInfo.md) [getSuggestionsForWordAtPosition](#getSuggestionsForWordAtPosition(int))(int position)
Gets the suggestions for the word at a certain position.
  [Dictionary](../../../../exml/workspace/api/spell/Dictionary.md) [getTermsDictionary](#getTermsDictionary())()
Get the current custom terms dictionary to be applied when doing spell checking actions.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TextChunkDescriptor](../../../../exml/workspace/api/util/TextChunkDescriptor.md)> [getTextDescriptors](#getTextDescriptors(int,int))(int startOffset, int endOffset)
Returns the list of descriptors for chunks of text between the given offsets.
  void [replaceWithSuggestion](#replaceWithSuggestion(int,int,java.lang.String))(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newWord)
Replaces word at a certain position.
  void [setDefaultLanguage](#setDefaultLanguage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang)
Sets the default language to be used for spell checking if an xml:lang attribute is not specified.
  void [setSpellcheckingEngine](#setSpellcheckingEngine(java.lang.String,ro.sync.ecss.extensions.api.webapp.SpellcheckingEngine))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [SpellcheckingEngine](SpellcheckingEngine.md) checker)
Sets the default spellchecker for a language.
  void [setTermsDictionary](#setTermsDictionary(ro.sync.exml.workspace.api.spell.Dictionary))([Dictionary](../../../../exml/workspace/api/spell/Dictionary.md) apiDict)
Set a custom terms dictionary to be used on spell checking actions.

## Method Details

### getSuggestionsForWordAtPosition

[SpellSuggestionsInfo](../SpellSuggestionsInfo.md) getSuggestionsForWordAtPosition(int position)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Gets the suggestions for the word at a certain position.
  Parameters: position - Position in the document. Returns: List of spellchecking suggestions for the word. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### replaceWithSuggestion

void replaceWithSuggestion(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newWord)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Replaces word at a certain position.
  Parameters: startOffset - Start offset for replacement. endOffset - End offset for replacement. newWord - Word to be inserted. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### getTextDescriptors

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TextChunkDescriptor](../../../../exml/workspace/api/util/TextChunkDescriptor.md)> getTextDescriptors(int startOffset, int endOffset)

Returns the list of descriptors for chunks of text between the given offsets.
  Parameters: startOffset - The start offset. endOffset - The end offset. Returns: The list of text descriptors.
### check

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[SpellCheckingProblemInfo](../SpellCheckingProblemInfo.md)> check([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TextChunkDescriptor](../../../../exml/workspace/api/util/TextChunkDescriptor.md)> textDescriptors)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Performs a spellcheck of the given text descriptors. This method is thread-safe. Can be called on multiple threads and can also be called while other threads are modifying the document.
  Parameters: textDescriptors - The text descriptors. Returns: The list of spelling problems. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If there is a problem reading the dictionaries.
### getTermsDictionary

[Dictionary](../../../../exml/workspace/api/spell/Dictionary.md) getTermsDictionary()

Get the current custom terms dictionary to be applied when doing spell checking actions.
  Returns: Returns the custom terms dictionary. Since: 21
### setTermsDictionary

void setTermsDictionary([Dictionary](../../../../exml/workspace/api/spell/Dictionary.md) apiDict)

Set a custom terms dictionary to be used on spell checking actions.
  Parameters: apiDict - The terms dictionary to set. Since: 21
### setDefaultLanguage

void setDefaultLanguage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang)

Sets the default language to be used for spell checking if an xml:lang attribute is not specified. Examples of format: **en_US**, **fr_FR**, **de_DE**, **jp_JP**, **it_IT**, **nl_NL**
  Parameters: lang - The language used to be used for spell checking. Since: 21
### setSpellcheckingEngine

void setSpellcheckingEngine([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lang, [SpellcheckingEngine](SpellcheckingEngine.md) checker)

Sets the default spellchecker for a language. Examples of language format: **en_US**, **fr_FR**, **de_DE**, **jp_JP**, **it_IT**, **nl_NL**
  Parameters: lang - The language to be handled by the spell checking engine. checker - The spell checking engine to be used for the language. Since: 21
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
