Package [ro.sync.ecss.extensions.api.webapp.findreplace](package-summary.md)

# Interface FindReplaceSupport
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface FindReplaceSupport
Support object for the Find/Replace related actions.
  Since: 16.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorHighlighter](../../highlights/AuthorHighlighter.md) [getSearchHighlightsProvider](#getSearchHighlightsProvider(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) searchFor)

 [AuthorHighlighter](../../highlights/AuthorHighlighter.md) [getSearchHighlightsProvider](#getSearchHighlightsProvider(java.lang.String,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) searchFor, boolean matchCase, boolean wholeWords)
Returns the highlights of the occurrences of the current string.
  [AuthorHighlighter](../../highlights/AuthorHighlighter.md) [getSearchHighlightsProvider](#getSearchHighlightsProvider(java.lang.String,ro.sync.ecss.extensions.api.webapp.findreplace.WebappFindOptions))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) searchFor, [WebappFindOptions](WebappFindOptions.md) options)
Returns the highlights of the occurrences of the current string.
  void [replace](#replace(int%5B%5D,java.lang.String))(int[] selectionOffsets, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textToReplaceWith)
Replace the occurrence found between the specified offsets.
  void [replaceAll](#replaceAll(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textToFind, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textToReplaceWith)
Replaces all the occurrences of some text with another.
  void [replaceAll](#replaceAll(java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.webapp.findreplace.WebappFindOptions))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textToFind, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textToReplaceWith, [WebappFindOptions](WebappFindOptions.md) options)
Replaces all the occurrences of some text with another.

## Method Details

### getSearchHighlightsProvider

[AuthorHighlighter](../../highlights/AuthorHighlighter.md) getSearchHighlightsProvider([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) searchFor, boolean matchCase, boolean wholeWords)

Returns the highlights of the occurrences of the current string.
  Parameters: searchFor - The string to search for. matchCase - Flag for matching case on the search string. wholeWords - Find whole words only. Returns: The highlights of the occurrences of the current string.
### getSearchHighlightsProvider

[AuthorHighlighter](../../highlights/AuthorHighlighter.md) getSearchHighlightsProvider([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) searchFor, [WebappFindOptions](WebappFindOptions.md) options)

Returns the highlights of the occurrences of the current string.
  Parameters: searchFor - The string to search for. options - The search options. Returns: The highlights of the occurrences of the current string. Since: 19.1
### replaceAll

void replaceAll([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textToFind, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textToReplaceWith)

Replaces all the occurrences of some text with another.
  Parameters: textToFind - The text to search for. textToReplaceWith - The text to replace with.
### replaceAll

void replaceAll([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textToFind, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textToReplaceWith, [WebappFindOptions](WebappFindOptions.md) options)

Replaces all the occurrences of some text with another. Also considers the options.
  Parameters: textToFind - The text to search for. textToReplaceWith - The text to replace with. options - The search options. Since: 19.1
### replace

void replace(int[] selectionOffsets, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textToReplaceWith)

Replace the occurrence found between the specified offsets.
  Parameters: selectionOffsets - The offsets. textToReplaceWith - The replacement text.
### getSearchHighlightsProvider

[AuthorHighlighter](../../highlights/AuthorHighlighter.md) getSearchHighlightsProvider([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) searchFor)
  Parameters: searchFor - The string to search for. Returns: The highlights of the occurrences of the current string.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
