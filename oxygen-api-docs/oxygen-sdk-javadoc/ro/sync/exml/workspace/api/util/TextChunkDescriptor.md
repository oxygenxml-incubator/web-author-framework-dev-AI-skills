Package [ro.sync.exml.workspace.api.util](package-summary.md)

# Interface TextChunkDescriptor
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface TextChunkDescriptor
Descriptor for a text chunk from a document.
  Since: 18.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html) [getCharSequence](#getCharSequence())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLang](#getLang())()

 int [getStartOffset](#getStartOffset())()

## Method Details

### getCharSequence

[CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html) getCharSequence()
  Returns: The char sequence.
### getLang

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLang()
  Returns: The language code, may be null, respects the xml:lang encoding (http://www.w3.org/TR/REC-xml/) Ex: "en", "en-GB", "en-US"
### getStartOffset

int getStartOffset()
  Returns: Returns the start offset of the sequence in document.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
