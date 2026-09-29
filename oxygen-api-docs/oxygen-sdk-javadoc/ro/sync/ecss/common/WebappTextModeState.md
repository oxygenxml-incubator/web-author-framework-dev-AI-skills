Package [ro.sync.ecss.common](package-summary.md)

# Class WebappTextModeState

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.common.WebappTextModeState
   @API(type=INTERNAL, src=PUBLIC) public class WebappTextModeState extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The state of the document that can be input to a text editor.

## Constructor Summary
 Constructors
Constructor

Description
 [WebappTextModeState](#%3Cinit%3E(java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlContent, int caretOffset)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getCaretOffset](#getCaretOffset())()
Returns caret position in the XML content that corresponds to the caret position in Author mode.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXmlContent](#getXmlContent())()
Returns the XML content in text format that can be saved on disk or edited in a normal text editor.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WebappTextModeState

public WebappTextModeState([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlContent, int caretOffset)

Constructor.
  Parameters: xmlContent - The text mode content. caretOffset - The caret offset.
## Method Details

### getXmlContent

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXmlContent()

Returns the XML content in text format that can be saved on disk or edited in a normal text editor.
  Returns: the XML content in text format that can be saved on disk or edited in a normal text editor.
### getCaretOffset

public int getCaretOffset()

Returns caret position in the XML content that corresponds to the caret position in Author mode.
  Returns: the offset of the caret in text mode.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
