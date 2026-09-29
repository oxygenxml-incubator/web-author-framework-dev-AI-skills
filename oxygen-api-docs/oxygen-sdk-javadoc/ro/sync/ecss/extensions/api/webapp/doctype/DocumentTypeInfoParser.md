Package [ro.sync.ecss.extensions.api.webapp.doctype](package-summary.md)

# Class DocumentTypeInfoParser

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.doctype.DocumentTypeInfoParser
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class DocumentTypeInfoParser extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Can parse framework files in memory.
  Since: 26.1
## Constructor Summary
 Constructors
Constructor

Description
 [DocumentTypeInfoParser](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [DocumentTypeInfo](DocumentTypeInfo.md) [parseExfFile](#parseExfFile(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) exfFile)
Loads a DocumentTypeInfo from a given exf file.
  static [DocumentTypeInfo](DocumentTypeInfo.md) [parseFrameworkFile](#parseFrameworkFile(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworkFile)
Loads a DocumentTypeInfo from a given framework file.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DocumentTypeInfoParser

public DocumentTypeInfoParser()

## Method Details

### parseFrameworkFile

public static [DocumentTypeInfo](DocumentTypeInfo.md) parseFrameworkFile([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworkFile)throws [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

Loads a DocumentTypeInfo from a given framework file.
  Parameters: frameworkFile - The framework file. Returns: the DocumentTypeInfo object. Throws: [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) - If fails to load the DocumentTypeInfo object.
### parseExfFile

public static [DocumentTypeInfo](DocumentTypeInfo.md) parseExfFile([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) exfFile)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html), [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html), net.sf.saxon.trans.XPathException, [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

Loads a DocumentTypeInfo from a given exf file.
  Parameters: exfFile - the .exf file. Returns: the DocumentTypeInfo object. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If fails to load the DocumentTypeInfo object. [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) - If fails to load the DocumentTypeInfo object. net.sf.saxon.trans.XPathException - If fails to load the DocumentTypeInfo object. [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html) - If fails to load the DocumentTypeInfo object. [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) - Generic exception.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
