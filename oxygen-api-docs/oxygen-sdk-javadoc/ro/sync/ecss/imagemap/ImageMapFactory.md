Package [ro.sync.ecss.imagemap](package-summary.md)

# Class ImageMapFactory

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.imagemap.ImageMapFactory
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class ImageMapFactory extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Factory for image map implementations. Builds the necessary classes from the provided texts accordingly with the specified framework.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static ro.sync.ecss.imagemap.ImageMapWrapper [buildDITAWrapper](#buildDITAWrapper(java.lang.String,java.net.URL,ro.sync.ecss.extensions.api.AuthorAccess,int,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imageMapString, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int nodeFontSize, boolean validate)
Build the DITA wrapper.
  [IImageMapWrapper](IImageMapWrapper.md) [getImageMap](#getImageMap(ro.sync.ecss.imagemap.SupportedFrameworks,ro.sync.ecss.extensions.api.AuthorAccess,int,java.net.URL,java.util.Map,boolean,java.lang.String...))([SupportedFrameworks](SupportedFrameworks.md) supportedFramework, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int nodeFontSize, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> uri2ProxyMappings, boolean validate, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... sources)
Get the image map.
  [IImageMapWrapper](IImageMapWrapper.md) [getImageMap](#getImageMap(ro.sync.ecss.imagemap.SupportedFrameworks,ro.sync.ecss.extensions.api.AuthorAccess,int,java.net.URL,java.util.Map,java.lang.String...))([SupportedFrameworks](SupportedFrameworks.md) supportedFramework, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int nodeFontSize, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> uri2ProxyMappings, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... sources)
Get the image map.
  static [ImageMapFactory](ImageMapFactory.md) [getInstance](#getInstance())()
Get the image map factory instance.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### getInstance

public static [ImageMapFactory](ImageMapFactory.md) getInstance()

Get the image map factory instance.
  Returns: Returns the instance.
### getImageMap

public [IImageMapWrapper](IImageMapWrapper.md) getImageMap([SupportedFrameworks](SupportedFrameworks.md) supportedFramework, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int nodeFontSize, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> uri2ProxyMappings, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... sources)throws javax.xml.bind.JAXBException, [ImageMapNotSuportedException](ImageMapNotSuportedException.md), [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Get the image map.
  Parameters: supportedFramework - The supported framework. authorAccess - The author access. nodeFontSize - The size of the node's font as it is used in the author page that needs the image map to be rendered. baseURL - The base URL. uri2ProxyMappings - The URI to proxy mappings. sources - The sources for the image map components. Usually a single one, excepting XHTML which has two elements, one for image, one for map. Returns: The image map wrapper. Throws: javax.xml.bind.JAXBException - If the UnMarshall-ing fails. [ImageMapNotSuportedException](ImageMapNotSuportedException.md) - If the image map has some arguments that are not supported by us. [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - If the image URL cannot be computed.
### getImageMap

public [IImageMapWrapper](IImageMapWrapper.md) getImageMap([SupportedFrameworks](SupportedFrameworks.md) supportedFramework, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int nodeFontSize, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> uri2ProxyMappings, boolean validate, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... sources)throws javax.xml.bind.JAXBException, [ImageMapNotSuportedException](ImageMapNotSuportedException.md), [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Get the image map.
  Parameters: supportedFramework - The supported framework. authorAccess - The author access. nodeFontSize - The size of the node's font as it is used in the author page that needs the image map to be rendered. baseURL - The base URL. uri2ProxyMappings - The URI to proxy mappings. validate - true to validate the XMl structure which is loaded. if any unknown elements are encountered an exception will be thrown. sources - The sources for the image map components. Usually a single one, excepting XHTML which has two elements, one for image, one for map. Returns: The image map wrapper. Throws: javax.xml.bind.JAXBException - If the UnMarshall-ing fails. [ImageMapNotSuportedException](ImageMapNotSuportedException.md) - If the image map has some arguments that are not supported by us. [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - If the image URL cannot be computed.
### buildDITAWrapper

public static ro.sync.ecss.imagemap.ImageMapWrapper buildDITAWrapper([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imageMapString, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, int nodeFontSize, boolean validate)throws javax.xml.bind.JAXBException, [ImageMapNotSuportedException](ImageMapNotSuportedException.md), [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Build the DITA wrapper.
  Parameters: imageMapString - The string with the image map, in XML format. baseURL - The base URL (URL of the document usually). authorAccess - The author access. nodeFontSize - The size of the node's font as it is used in the author page that needs the image map to be rendered. validate - true to validate the input map. Returns: The DITA wrapper Throws: javax.xml.bind.JAXBException - If the UnMarshall-ing fails. [ImageMapNotSuportedException](ImageMapNotSuportedException.md) - If the image map has some arguments that are not supported by us. [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - If the image URL cannot be computed.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
