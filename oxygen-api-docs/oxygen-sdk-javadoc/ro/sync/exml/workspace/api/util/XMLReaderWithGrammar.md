Package [ro.sync.exml.workspace.api.util](package-summary.md)

# Class XMLReaderWithGrammar

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.util.XMLReaderWithGrammar
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class XMLReaderWithGrammar extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
XML Reader + grammar cache
  Since: 11.2
## Constructor Summary
 Constructors
Constructor

Description
 [XMLReaderWithGrammar](#%3Cinit%3E(org.xml.sax.XMLReader,java.lang.Object))([XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) xmlReader, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) grammarCache)
Constructor

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getGrammarCache](#getGrammarCache())()

 [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [getXmlReader](#getXmlReader())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XMLReaderWithGrammar

public XMLReaderWithGrammar([XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) xmlReader, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) grammarCache)

Constructor
  Parameters: xmlReader - The XML Reader grammarCache - The grammar cache token
## Method Details

### getXmlReader

public [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) getXmlReader()
  Returns: Returns the xmlReader.
### getGrammarCache

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getGrammarCache()
  Returns: Returns the grammarCache.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
