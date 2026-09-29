Package [ro.sync.exml.workspace.api.images.handlers](package-summary.md)

# Class ImageHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.images.handlers.ImageHandler
   Direct Known Subclasses: [BinaryImageHandler](BinaryImageHandler.md), [EditImageHandler](EditImageHandler.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ImageHandler extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Base class for all the image handlers.
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [ImageHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract boolean [canHandleFileType](#canHandleFileType(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) extension)
Checks if the handler can "deal with" a certain type of XML application, or other image.
  abstract void [clearCache](#clearCache())()
Clear the individual cache the image handler might store internally.
  abstract [Image](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Image.html) [getImage](#getImage(ro.sync.exml.workspace.api.images.handlers.providers.ImageContentProvider,ro.sync.exml.workspace.api.images.handlers.ImageRenderingContext))([ImageContentProvider](providers/ImageContentProvider.md) contentProvider, [ImageRenderingContext](ImageRenderingContext.md) renderingContext)
Get an image for the corresponding URL.
  abstract [ImageLayoutInformation](ImageLayoutInformation.md) [getImageLayoutInformation](#getImageLayoutInformation(ro.sync.exml.workspace.api.images.handlers.providers.ImageContentProvider,ro.sync.exml.workspace.api.images.handlers.ImageRenderingContext))([ImageContentProvider](providers/ImageContentProvider.md) contentProvider, [ImageRenderingContext](ImageRenderingContext.md) renderingContext)
Get the size of the image.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ImageHandler

public ImageHandler()

## Method Details

### getImage

public abstract [Image](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Image.html) getImage([ImageContentProvider](providers/ImageContentProvider.md) contentProvider, [ImageRenderingContext](ImageRenderingContext.md) renderingContext)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Get an image for the corresponding URL.
  Parameters: contentProvider - Provides access to the image contents. If the image is embedded in the content, the content provider is an instance of [EmbeddedImageContentProvider](providers/EmbeddedImageContentProvider.md) renderingContext - The rendering context. Never null. Should contain the font of the parent element where the equation/graphic resides. Can be ignored for raster graphics. Returns: the image, never null. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - When the image could not be loaded.
### canHandleFileType

public abstract boolean canHandleFileType([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) extension)

Checks if the handler can "deal with" a certain type of XML application, or other image.
  Parameters: extension - The extension of the file, or the type of the XML content to be rendered. The implementation should accept the string in a case insensitive manner. Examples: "mathml", "SVG", "svg".. Returns: True if the extension is known by the handler.
### getImageLayoutInformation

public abstract [ImageLayoutInformation](ImageLayoutInformation.md) getImageLayoutInformation([ImageContentProvider](providers/ImageContentProvider.md) contentProvider, [ImageRenderingContext](ImageRenderingContext.md) renderingContext)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Get the size of the image. Ideally the handler should compute it as fast as possible, without loading the entire image in memory.
  Parameters: contentProvider - Provides access to the image contents. If the image is embedded in the content, the content provider is an instance of [EmbeddedImageContentProvider](providers/EmbeddedImageContentProvider.md) renderingContext - The rendering context. Should contain the font of the parent element where the equation/graphic resides. Can be ignored for raster graphics. Returns: The size of the image. Never null. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - When the image size could not be determined.
### clearCache

public abstract void clearCache()

Clear the individual cache the image handler might store internally.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
