Package [ro.sync.exml.plugin.openredirect](package-summary.md)

# Class OpenRedirectInformation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.plugin.openredirect.OpenRedirectInformation
   All Implemented Interfaces: ro.sync.basic.contenttypes.ContentTypes   @API(type=EXTENDABLE, src=PUBLIC) public class OpenRedirectInformation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements ro.sync.basic.contenttypes.ContentTypes
Information about redirecting an URL

## Field Summary

### Fields inherited from interface ro.sync.basic.contenttypes.ContentTypes
 ANT_CONTENT_TYPE, ANY_CONTENT_TYPE, BATCH_CONTENT_TYPE, C_CONTENT_TYPE, CPLUSPLUS_CONTENT_TYPE, CSS_CONTENT_TYPE, DITAMAP_CONTENT_TYPE, DOCKERFILE_CONTENT_TYPE, DTD_CONTENT_TYPE, EXF_CONTENT_TYPE, HTML_CONTENT_TYPE, IMAGE_CONTENT_TYPE, JAVA_CONTENT_TYPE, JAVASCRIPT_CONTENT_TYPE, JSON_CONTENT_TYPE, JSON_SCHEMA_CONTENT_TYPE, JSON5_CONTENT_TYPE, JSONL_CONTENT_TYPE, LESS_CONTENT_TYPE, MD_CONTENT_TYPE, NVDL_CONTENT_TYPE, PERL_CONTENT_TYPE, PHP_CONTENT_TYPE, PLAIN_TEXT_CONTENT_TYPE, POWER_SHELL_CONTENT_TYPE, PROPERTIES_CONTENT_TYPE, PYTHON_CONTENT_TYPE, RNC_CONTENT_TYPE, RNG_CONTENT_TYPE, SCHEMATRON_CONTENT_TYPE, SHELL_CONTENT_TYPE, SQL_CONTENT_TYPE, SVG_CONTENT_TYPE, WSDL_CONTENT_TYPE, XHTML_CONTENT_TYPE, XML_CONTENT_TYPE, XPATH_CONTENT_TYPE, XPROC_CONTENT_TYPE, XQUERY_CONTENT_TYPE, XSD_CONTENT_TYPE, XSL_CONTENT_TYPE, XSPEC_CONTENT_TYPE, YAML_CONTENT_TYPE, ZIP_CONTENT_TYPE
## Constructor Summary
 Constructors
Constructor

Description
 [OpenRedirectInformation](#%3Cinit%3E(java.net.URL,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContentType](#getContentType())()

 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getUrl](#getUrl())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### OpenRedirectInformation

public OpenRedirectInformation([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)

Constructor.
  Parameters: url - The URL to open contentType - The content type to open as. Can be null for auto open. The content type can either be null (and Oxygen will do the default detection) or one of the constant values defined in this class like:
        * application/zip - To open in the Archive Browser
        * application/ditamap - To open in the DITA Maps Manager
        * application/image - To open in the Image Previewer
        * text/xml - To open in the XML editor
        * text/css - To open in the CSS editor
        * ...

## Method Details

### getContentType

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContentType()
  Returns: Returns the contentType.
### getUrl

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getUrl()
  Returns: Returns the url.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
