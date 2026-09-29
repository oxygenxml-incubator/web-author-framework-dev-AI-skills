Package [ro.sync.ecss.extensions.dita.conref](package-summary.md)

# Class DITAFilteringContentHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.conref.DITAFilteringContentHandler
   All Implemented Interfaces: [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html), [LexicalHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html)   @API(type=INTERNAL, src=PUBLIC) public class DITAFilteringContentHandler extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html), [LexicalHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html)
Content and lexical handler used to filter parser events outside the given topic IDs path.

## Constructor Summary
 Constructors
Constructor

Description
 [DITAFilteringContentHandler](#%3Cinit%3E(java.lang.String%5B%5D,java.lang.String%5B%5D,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] topicPath, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] endRangePath, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sourceClass, boolean isKeyReference)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [characters](#characters(char%5B%5D,int,int))(char[] ch, int start, int length)

 void [comment](#comment(char%5B%5D,int,int))(char[] ch, int start, int length)

 void [endCDATA](#endCDATA())()

 void [endDocument](#endDocument())()

 void [endDTD](#endDTD())()

 void [endElement](#endElement(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

 void [endEntity](#endEntity(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

 void [endPrefixMapping](#endPrefixMapping(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix)

 void [ignorableWhitespace](#ignorableWhitespace(char%5B%5D,int,int))(char[] ch, int start, int length)

 void [processingInstruction](#processingInstruction(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) target, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) data)

 void [setContentHandler](#setContentHandler(org.xml.sax.ContentHandler))([ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) contentHandler)
Set the wrapped content handler.
  void [setDocumentLocator](#setDocumentLocator(org.xml.sax.Locator))([Locator](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Locator.html) locator)

 void [setLexicalHandler](#setLexicalHandler(org.xml.sax.ext.LexicalHandler))([LexicalHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html) lexicalHandler)
Set the wrapped lexical handler.
  void [skippedEntity](#skippedEntity(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

 void [startCDATA](#startCDATA())()

 void [startDocument](#startDocument())()

 void [startDTD](#startDTD(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) publicId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId)

 void [startElement](#startElement(java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) atts)

 void [startEntity](#startEntity(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

 void [startPrefixMapping](#startPrefixMapping(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri)

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface org.xml.sax.[ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html)
 [declaration](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#declaration(java.lang.String,java.lang.String,java.lang.String))
## Constructor Details

### DITAFilteringContentHandler

public DITAFilteringContentHandler([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] topicPath, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] endRangePath, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sourceClass, boolean isKeyReference)

Constructor.
  Parameters: topicPath - The topic IDs path. If null, the first encountered topic will be used. endRangePath - If a "conrefend" is specified, this is the end range path sourceClass - The class attribute value of the element which makes the conref... isKeyReference - true if the reference is a key reference.
## Method Details

### setContentHandler

public void setContentHandler([ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) contentHandler)

Set the wrapped content handler.
  Parameters: contentHandler - The contentHandler to set.
### setLexicalHandler

public void setLexicalHandler([LexicalHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html) lexicalHandler)

Set the wrapped lexical handler.
  Parameters: lexicalHandler - The lexicalHandler to set.
### characters

public void characters(char[] ch, int start, int length)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [characters](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#characters(char%5B%5D,int,int)) in interface [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [ContentHandler.characters(char[], int, int)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#characters(char%5B%5D,int,int))

### endDocument

public void endDocument() throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [endDocument](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#endDocument()) in interface [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [ContentHandler.endDocument()](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#endDocument())

### endElement

public void endElement([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [endElement](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#endElement(java.lang.String,java.lang.String,java.lang.String)) in interface [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [ContentHandler.endElement(java.lang.String, java.lang.String, java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#endElement(java.lang.String,java.lang.String,java.lang.String))

### endPrefixMapping

public void endPrefixMapping([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [endPrefixMapping](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#endPrefixMapping(java.lang.String)) in interface [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [ContentHandler.endPrefixMapping(java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#endPrefixMapping(java.lang.String))

### ignorableWhitespace

public void ignorableWhitespace(char[] ch, int start, int length)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [ignorableWhitespace](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#ignorableWhitespace(char%5B%5D,int,int)) in interface [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [ContentHandler.ignorableWhitespace(char[], int, int)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#ignorableWhitespace(char%5B%5D,int,int))

### processingInstruction

public void processingInstruction([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) target, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) data)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [processingInstruction](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#processingInstruction(java.lang.String,java.lang.String)) in interface [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [ContentHandler.processingInstruction(java.lang.String, java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#processingInstruction(java.lang.String,java.lang.String))

### setDocumentLocator

public void setDocumentLocator([Locator](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Locator.html) locator)
  Specified by: [setDocumentLocator](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#setDocumentLocator(org.xml.sax.Locator)) in interface [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) See Also:
        * [ContentHandler.setDocumentLocator(org.xml.sax.Locator)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#setDocumentLocator(org.xml.sax.Locator))

### skippedEntity

public void skippedEntity([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [skippedEntity](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#skippedEntity(java.lang.String)) in interface [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [ContentHandler.skippedEntity(java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#skippedEntity(java.lang.String))

### startDocument

public void startDocument() throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [startDocument](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#startDocument()) in interface [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [ContentHandler.startDocument()](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#startDocument())

### startElement

public void startElement([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) atts)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [startElement](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#startElement(java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes)) in interface [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [ContentHandler.startElement(java.lang.String, java.lang.String, java.lang.String, org.xml.sax.Attributes)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#startElement(java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes))

### startPrefixMapping

public void startPrefixMapping([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [startPrefixMapping](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#startPrefixMapping(java.lang.String,java.lang.String)) in interface [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [ContentHandler.startPrefixMapping(java.lang.String, java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html#startPrefixMapping(java.lang.String,java.lang.String))

### comment

public void comment(char[] ch, int start, int length)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [comment](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#comment(char%5B%5D,int,int)) in interface [LexicalHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [LexicalHandler.comment(char[], int, int)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#comment(char%5B%5D,int,int))

### endCDATA

public void endCDATA() throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [endCDATA](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#endCDATA()) in interface [LexicalHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [LexicalHandler.endCDATA()](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#endCDATA())

### endDTD

public void endDTD() throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [endDTD](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#endDTD()) in interface [LexicalHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [LexicalHandler.endDTD()](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#endDTD())

### endEntity

public void endEntity([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [endEntity](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#endEntity(java.lang.String)) in interface [LexicalHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [LexicalHandler.endEntity(java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#endEntity(java.lang.String))

### startCDATA

public void startCDATA() throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [startCDATA](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#startCDATA()) in interface [LexicalHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [LexicalHandler.startCDATA()](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#startCDATA())

### startDTD

public void startDTD([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) publicId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [startDTD](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#startDTD(java.lang.String,java.lang.String,java.lang.String)) in interface [LexicalHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [LexicalHandler.startDTD(java.lang.String, java.lang.String, java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#startDTD(java.lang.String,java.lang.String,java.lang.String))

### startEntity

public void startEntity([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [startEntity](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#startEntity(java.lang.String)) in interface [LexicalHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html) Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [LexicalHandler.startEntity(java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ext/LexicalHandler.html#startEntity(java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
