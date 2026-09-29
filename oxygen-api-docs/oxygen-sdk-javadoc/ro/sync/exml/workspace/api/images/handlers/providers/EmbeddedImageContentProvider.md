Package [ro.sync.exml.workspace.api.images.handlers.providers](package-summary.md)

# Class EmbeddedImageContentProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.workspace.api.images.handlers.providers.ImageContentProvider](ImageContentProvider.md)
        * ro.sync.exml.workspace.api.images.handlers.providers.EmbeddedImageContentProvider
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class EmbeddedImageContentProvider extends [ImageContentProvider](ImageContentProvider.md)
Provides access to the XML image contents...
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [EmbeddedImageContentProvider](#%3Cinit%3E(java.net.URL,java.lang.String,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imageSerializedContent, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypeContent)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDoctype](#getDoctype())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getImageSerializedContent](#getImageSerializedContent())()
Get the image serialized content.
  [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) [getInputStream](#getInputStream())()
Return an UTF8-encoded representation of the image serialized content.

### Methods inherited from class ro.sync.exml.workspace.api.images.handlers.providers.[ImageContentProvider](ImageContentProvider.md)
 [getUrl](ImageContentProvider.md#getUrl())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### EmbeddedImageContentProvider

public EmbeddedImageContentProvider([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imageSerializedContent, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypeContent)

Constructor.
  Parameters: systemID - The system ID of the document which contains the XML image. imageSerializedContent - The image serialized content. doctypeContent - The doctype content.
## Method Details

### getImageSerializedContent

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getImageSerializedContent()

Get the image serialized content. Not null when the image is embedded in the document (SVG, MathML, etc).
  Returns: Returns the image serialized content. Not null when the image is embedded in the document (SVG, MathML, etc).
### getDoctype

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDoctype()
  Returns: Returns the doctype.
### getInputStream

public [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) getInputStream()

Return an UTF8-encoded representation of the image serialized content.
  Overrides: [getInputStream](ImageContentProvider.md#getInputStream()) in class [ImageContentProvider](ImageContentProvider.md) Returns: Returns an input stream which can be used to read the image contents. This is never null. See Also:
        * [ImageContentProvider.getInputStream()](ImageContentProvider.md#getInputStream())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
