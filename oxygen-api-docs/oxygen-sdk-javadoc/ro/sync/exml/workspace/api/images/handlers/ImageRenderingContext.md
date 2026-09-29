Package [ro.sync.exml.workspace.api.images.handlers](package-summary.md)

# Class ImageRenderingContext

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.images.handlers.ImageRenderingContext
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class ImageRenderingContext extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Contains information about the context in which the image will be rendered..
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [ImageRenderingContext](#%3Cinit%3E(ro.sync.exml.view.graphics.Font))([Font](../../../../view/graphics/Font.md) font)
Constructor.
  [ImageRenderingContext](#%3Cinit%3E(ro.sync.exml.view.graphics.Font,int))([Font](../../../../view/graphics/Font.md) font, int dotsPerInch)
Constructor.
  [ImageRenderingContext](#%3Cinit%3E(ro.sync.exml.view.graphics.Font,int,ro.sync.exml.view.graphics.Rectangle))([Font](../../../../view/graphics/Font.md) font, int dotsPerInch, [Rectangle](../../../../view/graphics/Rectangle.md) imageInfo)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getDotsPerInch](#getDotsPerInch())()
Get the current monitor DPI settings.
  [Font](../../../../view/graphics/Font.md) [getFont](#getFont())()
Get the font used in the place where the image will be displayed.
  [Dimension](../../../../view/graphics/Dimension.md) [getImageDimensions](#getImageDimensions())()
Gets the final dimension of the image that will be painted.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ImageRenderingContext

public ImageRenderingContext([Font](../../../../view/graphics/Font.md) font)

Constructor.
  Parameters: font - The font.
### ImageRenderingContext

public ImageRenderingContext([Font](../../../../view/graphics/Font.md) font, int dotsPerInch)

Constructor.
  Parameters: font - The font. dotsPerInch - The current monitor DPI (Dots per Inch)
### ImageRenderingContext

public ImageRenderingContext([Font](../../../../view/graphics/Font.md) font, int dotsPerInch, [Rectangle](../../../../view/graphics/Rectangle.md) imageInfo)

Constructor.
  Parameters: font - The font. dotsPerInch - The current monitor DPI (Dots per Inch) imageInfo - Image's layout info. Since: 24.0
## Method Details

### getFont

public [Font](../../../../view/graphics/Font.md) getFont()

Get the font used in the place where the image will be displayed. Some image handlers (for example an SVG or a MathML image handler) might use this information to render and compute the image sizes...
  Returns: Returns the font used in the place where the image will be displayed.
### getDotsPerInch

public int getDotsPerInch()

Get the current monitor DPI settings. The default is 96.
  Returns: Returns the current monitor.
### getImageDimensions

public [Dimension](../../../../view/graphics/Dimension.md) getImageDimensions()

Gets the final dimension of the image that will be painted. Some image handlers (for example an SVG or a MathML image handler) might use this information to scale images without losing accuracy. If the handler does not use this information, the image is automatically scaled by the application to the display dimensions.
  Returns: Returns The final dimensions of the image, or null. Since: 24.0
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
