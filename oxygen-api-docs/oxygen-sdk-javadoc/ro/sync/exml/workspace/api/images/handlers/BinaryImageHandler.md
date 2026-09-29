Package [ro.sync.exml.workspace.api.images.handlers](package-summary.md)

# Class BinaryImageHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.workspace.api.images.handlers.ImageHandler](ImageHandler.md)
        * ro.sync.exml.workspace.api.images.handlers.BinaryImageHandler
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class BinaryImageHandler extends [ImageHandler](ImageHandler.md)
Special handler for binary images like EPS or AI... The handler will receive an input stream for the image and it needs to state if it is interested in handling it...
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [BinaryImageHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract boolean [canHandle](#canHandle(java.io.InputStream))([InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) inputStream)
Check if can handle this input stream.

### Methods inherited from class ro.sync.exml.workspace.api.images.handlers.[ImageHandler](ImageHandler.md)
 [canHandleFileType](ImageHandler.md#canHandleFileType(java.lang.String)), [clearCache](ImageHandler.md#clearCache()), [getImage](ImageHandler.md#getImage(ro.sync.exml.workspace.api.images.handlers.providers.ImageContentProvider,ro.sync.exml.workspace.api.images.handlers.ImageRenderingContext)), [getImageLayoutInformation](ImageHandler.md#getImageLayoutInformation(ro.sync.exml.workspace.api.images.handlers.providers.ImageContentProvider,ro.sync.exml.workspace.api.images.handlers.ImageRenderingContext))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### BinaryImageHandler

public BinaryImageHandler()

## Method Details

### canHandle

public abstract boolean canHandle([InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) inputStream)

Check if can handle this input stream. Ideally will read only some metadata from the stream.
  Parameters: inputStream - The binary image input stream. Never NULL. Returns: true if can handle this document.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
