Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Class WebappAuthorDocumentFactory

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.WebappAuthorDocumentFactory
   All Implemented Interfaces: [WebappAuthorDocumentFactoryConstants](WebappAuthorDocumentFactoryConstants.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public final class WebappAuthorDocumentFactory extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [WebappAuthorDocumentFactoryConstants](WebappAuthorDocumentFactoryConstants.md)
Factory class that creates the document model to be used in the Web Reviewer.
  Since: 15.1
## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.webapp.[WebappAuthorDocumentFactoryConstants](WebappAuthorDocumentFactoryConstants.md)
 [EDITING_CONTEXT_MODEL_ATTR](WebappAuthorDocumentFactoryConstants.md#EDITING_CONTEXT_MODEL_ATTR), [ETAG_RECORD_LOADING_OPTION_KEY](WebappAuthorDocumentFactoryConstants.md#ETAG_RECORD_LOADING_OPTION_KEY), [SEND_ETAG_ON_SAVE_LOADING_OPTION_KEY](WebappAuthorDocumentFactoryConstants.md#SEND_ETAG_ON_SAVE_LOADING_OPTION_KEY)
## Method Summary
  All MethodsStatic MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 static [AuthorDocumentModel](AuthorDocumentModel.md) [createAuthorDocumentInfo](#createAuthorDocumentInfo(java.lang.String,java.io.Reader,java.util.Map))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) docReader, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),?> sessionAttributes)
Factory method that creates a document model for the document with the specified systemID.
  static [AuthorDocumentModel](AuthorDocumentModel.md) [createAuthorDocumentInfo](#createAuthorDocumentInfo(java.lang.String,java.util.Map))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),?> sessionAttributes)
Factory method that creates a document model for the document with the specified systemID.
  static [AuthorDocumentModel](AuthorDocumentModel.md) [createAuthorDocumentInfo](#createAuthorDocumentInfo(java.net.URL,java.io.Reader,java.util.List,java.util.Map))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemIdUrl, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) docReader, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) bomBytes, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),?> sessionAttributes)
Factory method that creates a document model for the document with the specified systemID.
  static [DITAMapDocumentModel](../../../webapp/ditamap/DITAMapDocumentModel.md) [createDITAMapDocumentInfo](#createDITAMapDocumentInfo(java.lang.String,java.io.Reader,java.util.Map))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) docReader, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),?> sessionAttributes)
Factory method that creates an editable DITA Map document model for the document with the specified systemID.
  static [DITAMapDocumentModel](../../../webapp/ditamap/DITAMapDocumentModel.md) [createDITAMapDocumentInfo](#createDITAMapDocumentInfo(java.lang.String,java.util.Map))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),?> sessionAttributes)
Factory method that creates an editable DITA Map document model for the document with the specified systemID.
  static [DITAMapDocumentModel](../../../webapp/ditamap/DITAMapDocumentModel.md) [createDITAMapDocumentInfo](#createDITAMapDocumentInfo(java.net.URL,java.io.Reader,java.util.List,java.util.Map))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemIdUrl, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) docReader, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) bomBytes, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),?> sessionAttributes)
Factory method that creates an editable DITA Map document model for the document with the specified systemID.
  static void [dispose](#dispose())()
Disposes any resources used by the document factory.
  static [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getInitializationFatalError](#getInitializationFatalError())()

 static [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) [getPluginsCSS](#getPluginsCSS())()
Returns a reader over the plugins WebappCSSResource files.
  static [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) [getPluginsJS](#getPluginsJS())()
Returns a reader over all JS files from the plugins.
  static void [init](#init())()
Initialize the web application.
  static void [setFrameworks](#setFrameworks(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworksDir)
Sets the folder that contains the frameworks.
  static void [setOptions](#setOptions(java.io.File,java.lang.String))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) workDir, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionsFileName)
Sets the file to be used to load the oxygen options.
  static void [setPlugins](#setPlugins(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) workDir)  Deprecated.
use {[setPlugins(File, File)](#setPlugins(java.io.File,java.io.File)).
   static void [setPlugins](#setPlugins(java.io.File,java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) pluginsDir, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) userUploadedPluginsDir)
Sets the folder that contains the plugins.
  static void [setUserFrameworks](#setUserFrameworks(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) userFrameworksDir)
Sets the folder that contains the frameworks the user has uploaded.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### createDITAMapDocumentInfo

public static [DITAMapDocumentModel](../../../webapp/ditamap/DITAMapDocumentModel.md) createDITAMapDocumentInfo([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemIdUrl, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) docReader, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) bomBytes, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),?> sessionAttributes)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)

Factory method that creates an editable DITA Map document model for the document with the specified systemID. It takes care of detecting the encoding, resolving DTD, etc.
  Parameters: systemIdUrl - The document URL. docReader - Reader over the document. bomBytes - BOM bytes. sessionAttributes - A map of session attributes. Returns: The author document. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) Since: 26.1
### createAuthorDocumentInfo

public static [AuthorDocumentModel](AuthorDocumentModel.md) createAuthorDocumentInfo([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemIdUrl, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) docReader, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) bomBytes, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),?> sessionAttributes)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)

Factory method that creates a document model for the document with the specified systemID. It takes care of detecting the encoding, resolving DTD, CSS resources, etc.
  Parameters: systemIdUrl - The document URL. docReader - Reader over the document. bomBytes - BOM bytes. sessionAttributes - A map of session attributes. Returns: The author document. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
### createAuthorDocumentInfo

public static [AuthorDocumentModel](AuthorDocumentModel.md) createAuthorDocumentInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),?> sessionAttributes)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)

Factory method that creates a document model for the document with the specified systemID. It takes care of detecting the encoding, resolving DTD, CSS resources, etc.
  Parameters: systemID - The document URL. sessionAttributes - The session attributes. Returns: The author document. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
### createAuthorDocumentInfo

public static [AuthorDocumentModel](AuthorDocumentModel.md) createAuthorDocumentInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) docReader, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),?> sessionAttributes)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)

Factory method that creates a document model for the document with the specified systemID. It takes care of detecting the encoding, resolving DTD, CSS resources, etc.
  Parameters: systemID - The document URL. docReader - Reader over the document. sessionAttributes - Session attributes. Returns: The author document. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
### setOptions

public static void setOptions([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) workDir, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionsFileName)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Sets the file to be used to load the oxygen options. This method should be called before any other use of the Options singleton.
  Parameters: workDir - The directory in which the options file resides. optionsFileName - The name of the options file. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - Unable to set the working dir.
### setFrameworks

public static void setFrameworks([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworksDir)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Sets the folder that contains the frameworks. This method should be called before creating any document models.
  Parameters: frameworksDir - The folder that contains the frameworks. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - If the framework's directory URL is malformed.
### setUserFrameworks

public static void setUserFrameworks([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) userFrameworksDir)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Sets the folder that contains the frameworks the user has uploaded. This method should be called before creating any document models.
  Parameters: userFrameworksDir - The folder that contains the user uploaded frameworks. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - If the framework's directory URL is malformed.
### setPlugins

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static void setPlugins([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) workDir)
 Deprecated.
use {[setPlugins(File, File)](#setPlugins(java.io.File,java.io.File)).

Sets the folder that contains the plugins. This method should be called before creating any document models.
  Parameters: workDir - The folder that contains the plugins.
### setPlugins

public static void setPlugins([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) pluginsDir, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) userUploadedPluginsDir)

Sets the folder that contains the plugins. This method should be called before creating any document models.
  Parameters: pluginsDir - The folder that contains the plugins. userUploadedPluginsDir - the directory holding the user uploaded plugins.
### getPluginsJS

public static [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) getPluginsJS()

Returns a reader over all JS files from the plugins. Beside plugins options it contains some server-side options.
  Returns: The reader over the concatenated JS files from plugins.
### getPluginsCSS

public static [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) getPluginsCSS()

Returns a reader over the plugins WebappCSSResource files.
  Returns: The reader over the concatenated CSS files from plugins.
### init

public static void init()

Initialize the web application.

### getInitializationFatalError

public static [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getInitializationFatalError()
  Returns: Fatal error that occurred during initialization. This can be presented in browser when trying to access Web Author.
### dispose

public static void dispose()

Disposes any resources used by the document factory.

### createDITAMapDocumentInfo

public static [DITAMapDocumentModel](../../../webapp/ditamap/DITAMapDocumentModel.md) createDITAMapDocumentInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) docReader, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),?> sessionAttributes)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)

Factory method that creates an editable DITA Map document model for the document with the specified systemID. It takes care of detecting the encoding, resolving DTD, etc.
  Parameters: systemID - The document URL. docReader - Reader over the document. sessionAttributes - Session attributes. Returns: The author document. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) Since: 26.1
### createDITAMapDocumentInfo

public static [DITAMapDocumentModel](../../../webapp/ditamap/DITAMapDocumentModel.md) createDITAMapDocumentInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),?> sessionAttributes)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)

Factory method that creates an editable DITA Map document model for the document with the specified systemID. It takes care of detecting the encoding, resolving DTD, etc.
  Parameters: systemID - The document URL. sessionAttributes - The session attributes. Returns: The author document. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) Since: 26.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
