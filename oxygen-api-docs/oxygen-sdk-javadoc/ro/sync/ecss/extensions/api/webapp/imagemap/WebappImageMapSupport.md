Package [ro.sync.ecss.extensions.api.webapp.imagemap](package-summary.md)

# Interface WebappImageMapSupport
    All Known Implementing Classes: [XHTMLWebappImageMapSupport](../../../xhtml/imagemap/XHTMLWebappImageMapSupport.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface WebappImageMapSupport
Represents an instance of an image map embedded in a document.
  Since: 25.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WebappAreaView](WebappAreaView.md)> [getAreas](#getAreas(int))(int fontSize)

 [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Rectangle](../../../../../exml/view/graphics/Rectangle.md)> [getImageSize](#getImageSize(int))(int fontSize)
The image size, as specified by XML attributes.

## Method Details

### getAreas

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WebappAreaView](WebappAreaView.md)> getAreas(int fontSize)
  Parameters: fontSize - The font size of the image. Returns: The list of area views in the order that needs to be stacked vertically.
### getImageSize

[Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Rectangle](../../../../../exml/view/graphics/Rectangle.md)> getImageSize(int fontSize)

The image size, as specified by XML attributes. If the image size is not specified by XML attributes, the editor will determine it based on the natural size of the image file.
  Parameters: fontSize - The font size of the image map. Returns: A rectangle centered in origin with width and height equal to those of the image, or empty.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
