Package [ro.sync.ecss.extensions.xhtml.imagemap](package-summary.md)

# Class XHTMLWebappImageMapSupport

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.xhtml.imagemap.XHTMLWebappImageMapSupport
   All Implemented Interfaces: [WebappImageMapSupport](../../api/webapp/imagemap/WebappImageMapSupport.md)   @API(type=INTERNAL, src=PUBLIC) public class XHTMLWebappImageMapSupport extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [WebappImageMapSupport](../../api/webapp/imagemap/WebappImageMapSupport.md)
Image map support for XHTML.

## Constructor Summary
 Constructors
Constructor

Description
 [XHTMLWebappImageMapSupport](#%3Cinit%3E(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) map)

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WebappAreaView](../../api/webapp/imagemap/WebappAreaView.md)> [getAreas](#getAreas(int))(int fontSize)

 [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Rectangle](../../../../exml/view/graphics/Rectangle.md)> [getImageSize](#getImageSize(int))(int fontSize)
The image size, as specified by XML attributes.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XHTMLWebappImageMapSupport

public XHTMLWebappImageMapSupport([AuthorElement](../../api/node/AuthorElement.md) map)throws [ImageMapFormatException](../../api/webapp/imagemap/ImageMapFormatException.md)
  Parameters: map - The  element. Throws: [ImageMapFormatException](../../api/webapp/imagemap/ImageMapFormatException.md) - If the image map does not have the correct format.
## Method Details

### getAreas

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WebappAreaView](../../api/webapp/imagemap/WebappAreaView.md)> getAreas(int fontSize)
  Specified by: [getAreas](../../api/webapp/imagemap/WebappImageMapSupport.md#getAreas(int)) in interface [WebappImageMapSupport](../../api/webapp/imagemap/WebappImageMapSupport.md) Parameters: fontSize - The font size of the image. Returns: The list of area views in the order that needs to be stacked vertically. See Also:
        * [WebappImageMapSupport.getAreas(int)](../../api/webapp/imagemap/WebappImageMapSupport.md#getAreas(int))

### getImageSize

public [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Rectangle](../../../../exml/view/graphics/Rectangle.md)> getImageSize(int fontSize)
 Description copied from interface: [WebappImageMapSupport](../../api/webapp/imagemap/WebappImageMapSupport.md#getImageSize(int))
The image size, as specified by XML attributes. If the image size is not specified by XML attributes, the editor will determine it based on the natural size of the image file.
  Specified by: [getImageSize](../../api/webapp/imagemap/WebappImageMapSupport.md#getImageSize(int)) in interface [WebappImageMapSupport](../../api/webapp/imagemap/WebappImageMapSupport.md) Parameters: fontSize - The font size of the image map. Returns: A rectangle centered in origin with width and height equal to those of the image, or empty. See Also:
        * [WebappImageMapSupport.getImageSize(int)](../../api/webapp/imagemap/WebappImageMapSupport.md#getImageSize(int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
