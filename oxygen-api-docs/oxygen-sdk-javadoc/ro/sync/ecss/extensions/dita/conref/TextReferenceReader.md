Package [ro.sync.ecss.extensions.dita.conref](package-summary.md)

# Class TextReferenceReader

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.conref.TextReferenceReader
   All Implemented Interfaces: [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html)   @API(type=INTERNAL, src=PUBLIC) public class TextReferenceReader extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html)
A XMLReader implementation used to provide the content of a DITA reference as text. It also extracts the text inside a given line interval.

## Constructor Summary
 Constructors
Constructor

Description
 [TextReferenceReader](#%3Cinit%3E(java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.access.AuthorUtilAccess))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceSystemId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) encoding, [AuthorUtilAccess](../../api/access/AuthorUtilAccess.md) authorUtilAccess)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) [getContentHandler](#getContentHandler())()

 [DTDHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/DTDHandler.html) [getDTDHandler](#getDTDHandler())()

 [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) [getEntityResolver](#getEntityResolver())()

 [ErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ErrorHandler.html) [getErrorHandler](#getErrorHandler())()

 boolean [getFeature](#getFeature(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getProperty](#getProperty(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

 void [parse](#parse(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId)

 void [parse](#parse(org.xml.sax.InputSource))([InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html) input)

 void [setContentHandler](#setContentHandler(org.xml.sax.ContentHandler))([ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) handler)

 void [setDTDHandler](#setDTDHandler(org.xml.sax.DTDHandler))([DTDHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/DTDHandler.html) handler)

 void [setEntityResolver](#setEntityResolver(org.xml.sax.EntityResolver))([EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) resolver)

 void [setErrorHandler](#setErrorHandler(org.xml.sax.ErrorHandler))([ErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ErrorHandler.html) handler)

 void [setFeature](#setFeature(java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, boolean value)

 void [setProperty](#setProperty(java.lang.String,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TextReferenceReader

public TextReferenceReader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceSystemId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) encoding, [AuthorUtilAccess](../../api/access/AuthorUtilAccess.md) authorUtilAccess)

Constructor.
  Parameters: referenceSystemId - The referred file system ID. encoding - The encoding of the referred file. if null will use the EncodingDetectorSingleton.getInstance(). authorUtilAccess - Access to util methods.
## Method Details

### getContentHandler

public [ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) getContentHandler()
  Specified by: [getContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#getContentHandler()) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) See Also:
        * [XMLReader.getContentHandler()](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#getContentHandler())

### getDTDHandler

public [DTDHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/DTDHandler.html) getDTDHandler()
  Specified by: [getDTDHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#getDTDHandler()) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) See Also:
        * [XMLReader.getDTDHandler()](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#getDTDHandler())

### getEntityResolver

public [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) getEntityResolver()
  Specified by: [getEntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#getEntityResolver()) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) See Also:
        * [XMLReader.getEntityResolver()](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#getEntityResolver())

### getErrorHandler

public [ErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ErrorHandler.html) getErrorHandler()
  Specified by: [getErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#getErrorHandler()) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) See Also:
        * [XMLReader.getErrorHandler()](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#getErrorHandler())

### getFeature

public boolean getFeature([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)throws [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html), [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)
  Specified by: [getFeature](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#getFeature(java.lang.String)) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) Throws: [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html) [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html) See Also:
        * [XMLReader.getFeature(java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#getFeature(java.lang.String))

### getProperty

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)throws [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html), [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)
  Specified by: [getProperty](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#getProperty(java.lang.String)) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) Throws: [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html) [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html) See Also:
        * [XMLReader.getProperty(java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#getProperty(java.lang.String))

### parse

public void parse([InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html) input)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [parse](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#parse(org.xml.sax.InputSource)) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [XMLReader.parse(org.xml.sax.InputSource)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#parse(org.xml.sax.InputSource))

### parse

public void parse([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
  Specified by: [parse](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#parse(java.lang.String)) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) See Also:
        * [XMLReader.parse(java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#parse(java.lang.String))

### setContentHandler

public void setContentHandler([ContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ContentHandler.html) handler)
  Specified by: [setContentHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#setContentHandler(org.xml.sax.ContentHandler)) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) See Also:
        * [XMLReader.setContentHandler(org.xml.sax.ContentHandler)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#setContentHandler(org.xml.sax.ContentHandler))

### setDTDHandler

public void setDTDHandler([DTDHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/DTDHandler.html) handler)
  Specified by: [setDTDHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#setDTDHandler(org.xml.sax.DTDHandler)) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) See Also:
        * [XMLReader.setDTDHandler(org.xml.sax.DTDHandler)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#setDTDHandler(org.xml.sax.DTDHandler))

### setEntityResolver

public void setEntityResolver([EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) resolver)
  Specified by: [setEntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#setEntityResolver(org.xml.sax.EntityResolver)) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) See Also:
        * [XMLReader.setEntityResolver(org.xml.sax.EntityResolver)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#setEntityResolver(org.xml.sax.EntityResolver))

### setErrorHandler

public void setErrorHandler([ErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ErrorHandler.html) handler)
  Specified by: [setErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#setErrorHandler(org.xml.sax.ErrorHandler)) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) See Also:
        * [XMLReader.setErrorHandler(org.xml.sax.ErrorHandler)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#setErrorHandler(org.xml.sax.ErrorHandler))

### setFeature

public void setFeature([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, boolean value)throws [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html), [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)
  Specified by: [setFeature](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#setFeature(java.lang.String,boolean)) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) Throws: [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html) [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html) See Also:
        * [XMLReader.setFeature(java.lang.String, boolean)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#setFeature(java.lang.String,boolean))

### setProperty

public void setProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)throws [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html), [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)
  Specified by: [setProperty](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#setProperty(java.lang.String,java.lang.Object)) in interface [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) Throws: [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html) [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html) See Also:
        * [XMLReader.setProperty(java.lang.String, java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html#setProperty(java.lang.String,java.lang.Object))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
