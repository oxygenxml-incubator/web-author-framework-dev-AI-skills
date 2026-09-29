Package [ro.sync.exml.workspace.api.editor.page.author.css](package-summary.md)

# Class CSSResource

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.author.css.CSSResource
   All Implemented Interfaces: ro.sync.ecss.component.CSSSourceTypes   @API(type=EXTENDABLE, src=PUBLIC) public class CSSResource extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements ro.sync.ecss.component.CSSSourceTypes
The CSS resource contains an URI to the CSS resource and its origin.
  Since: 17
## Field Summary

### Fields inherited from interface ro.sync.ecss.component.CSSSourceTypes
 SOURCE_DOCUMENT, SOURCE_DOCUMENT_TYPE, SOURCE_XHTML_DOCUMENT
## Constructor Summary
 Constructors
Constructor

Description
 [CSSResource](#%3Cinit%3E(java.lang.String,byte))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cssURL, byte origin)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCssURL](#getCssURL())()

 byte [getOrigin](#getOrigin())()

 int [hashCode](#hashCode())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CSSResource

public CSSResource([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cssURL, byte origin)

Constructor.
  Parameters: cssURL - The CSS url. origin - The CSS origin. Can be SOURCE_DOCUMENT, SOURCE_DOCUMENT_TYPE or SOURCE_XHTML_DOCUMENT. See the "SOURCE_" constants.
## Method Details

### getCssURL

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCssURL()
  Returns: The CSS URL.
### getOrigin

public byte getOrigin()
  Returns: The stylesheet origin.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
