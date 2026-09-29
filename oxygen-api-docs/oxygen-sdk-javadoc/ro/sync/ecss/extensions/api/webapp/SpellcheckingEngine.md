Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Interface SpellcheckingEngine
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface SpellcheckingEngine
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[SpellCheckingProblemInfoWithSuggestions](../SpellCheckingProblemInfoWithSuggestions.md)> [check](#check(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TextChunkDescriptor](../../../../exml/workspace/api/util/TextChunkDescriptor.md)> text)
Check a list of text chunks for spell checking errors.

## Method Details

### check

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[SpellCheckingProblemInfoWithSuggestions](../SpellCheckingProblemInfoWithSuggestions.md)> check([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TextChunkDescriptor](../../../../exml/workspace/api/util/TextChunkDescriptor.md)> text)

Check a list of text chunks for spell checking errors.
  Parameters: text - The list of text descriptors to check. Returns: The list of identified spell checking problems. Since: 21
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
