Package [ro.sync.exml.workspace.api.images.handlers.providers](package-summary.md)

# Class ImageContentProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.images.handlers.providers.ImageContentProvider
   Direct Known Subclasses: [EmbeddedImageContentProvider](EmbeddedImageContentProvider.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class ImageContentProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Provides access to the image contents...
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [ImageContentProvider](#%3Cinit%3E(java.net.URL,java.io.InputStream))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) inputStream)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) [getInputStream](#getInputStream())()
Get an input stream which can be used to read the image contents.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getUrl](#getUrl())()
Get an URL pointing to the place where the image is located.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ImageContentProvider

public ImageContentProvider([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) inputStream)

Constructor.
  Parameters: url - The image URL. inputStream - The input stream.
## Method Details

### getUrl

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getUrl()

Get an URL pointing to the place where the image is located. If the image is embedded, this returns null.
  Returns: Returns an URL pointing to the place where the image is located. If the image is embedded, this returns null.
### getInputStream

public [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) getInputStream()

Get an input stream which can be used to read the image contents.
  Returns: Returns an input stream which can be used to read the image contents. This is never null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
