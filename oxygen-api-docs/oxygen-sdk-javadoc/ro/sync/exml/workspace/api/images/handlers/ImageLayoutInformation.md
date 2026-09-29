Package [ro.sync.exml.workspace.api.images.handlers](package-summary.md)

# Class ImageLayoutInformation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.view.graphics.Rectangle](../../../../view/graphics/Rectangle.md)
        * ro.sync.exml.workspace.api.images.handlers.ImageLayoutInformation
   All Implemented Interfaces: [Shape](../../../../view/graphics/Shape.md)   @API(type=EXTENDABLE, src=PUBLIC) public class ImageLayoutInformation extends [Rectangle](../../../../view/graphics/Rectangle.md)
Information about an image's dimensions and baseline.
  Since: 18
## Field Summary

### Fields inherited from class ro.sync.exml.view.graphics.[Rectangle](../../../../view/graphics/Rectangle.md)
 [height](../../../../view/graphics/Rectangle.md#height), [width](../../../../view/graphics/Rectangle.md#width), [x](../../../../view/graphics/Rectangle.md#x), [y](../../../../view/graphics/Rectangle.md#y)
## Constructor Summary
 Constructors
Constructor

Description
 [ImageLayoutInformation](#%3Cinit%3E(int,int,int,int))(int x, int y, int width, int height)
Information about an image.
  [ImageLayoutInformation](#%3Cinit%3E(int,int,int,int,int))(int x, int y, int width, int height, int ascend)
Information about an image.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
Checks whether two rectangles are equal.
  int [getAscend](#getAscend())()
Get the image ascend.
  int [hashCode](#hashCode())()

 void [setAscend](#setAscend(int))(int ascend)
Set the ascend.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()
Returns a String representing this Rectangle and its values.

### Methods inherited from class ro.sync.exml.view.graphics.[Rectangle](../../../../view/graphics/Rectangle.md)
 [adjacent](../../../../view/graphics/Rectangle.md#adjacent(ro.sync.exml.view.graphics.Rectangle)), [clone](../../../../view/graphics/Rectangle.md#clone()), [contains](../../../../view/graphics/Rectangle.md#contains(int,int)), [contains](../../../../view/graphics/Rectangle.md#contains(int,int,int,int)), [contains](../../../../view/graphics/Rectangle.md#contains(ro.sync.exml.view.graphics.Rectangle)), [getBounds](../../../../view/graphics/Rectangle.md#getBounds()), [getHeight](../../../../view/graphics/Rectangle.md#getHeight()), [getWidth](../../../../view/graphics/Rectangle.md#getWidth()), [getX](../../../../view/graphics/Rectangle.md#getX()), [getY](../../../../view/graphics/Rectangle.md#getY()), [intersection](../../../../view/graphics/Rectangle.md#intersection(ro.sync.exml.view.graphics.Rectangle)), [intersects](../../../../view/graphics/Rectangle.md#intersects(int,int,int,int)), [intersects](../../../../view/graphics/Rectangle.md#intersects(ro.sync.exml.view.graphics.Rectangle)), [main](../../../../view/graphics/Rectangle.md#main(java.lang.String%5B%5D)), [translate](../../../../view/graphics/Rectangle.md#translate(int,int)), [union](../../../../view/graphics/Rectangle.md#union(ro.sync.exml.view.graphics.Rectangle))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ImageLayoutInformation

public ImageLayoutInformation(int x, int y, int width, int height)

Information about an image. No base line information is given.
  Parameters: x - The x coordinate. y - The y coordinate. width - The width. height - The height.
### ImageLayoutInformation

public ImageLayoutInformation(int x, int y, int width, int height, int ascend)

Information about an image.
  Parameters: x - The x coordinate. y - The y coordinate. width - The width. height - The height. ascend - The image ascend, -1 if unknown.
## Method Details

### getAscend

public int getAscend()

Get the image ascend.
  Returns: Returns the ascend.
### setAscend

public void setAscend(int ascend)

Set the ascend.
  Parameters: ascend - The image ascend.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
 Description copied from class: [Rectangle](../../../../view/graphics/Rectangle.md#toString())
Returns a String representing this Rectangle and its values.
  Overrides: [toString](../../../../view/graphics/Rectangle.md#toString()) in class [Rectangle](../../../../view/graphics/Rectangle.md) Returns: a String representing this Rectangle object's coordinate and size values. See Also:
        * [Rectangle.toString()](../../../../view/graphics/Rectangle.md#toString())

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
 Description copied from class: [Rectangle](../../../../view/graphics/Rectangle.md#equals(java.lang.Object))
Checks whether two rectangles are equal.
The result is true if and only if the argument is not null and is a Rectangle object that has the same top-left corner, width, and height as this Rectangle.

  Overrides: [equals](../../../../view/graphics/Rectangle.md#equals(java.lang.Object)) in class [Rectangle](../../../../view/graphics/Rectangle.md) Parameters: obj - the Object to compare with this Rectangle Returns: true if the objects are equal; false otherwise. See Also:
        * [Rectangle.equals(java.lang.Object)](../../../../view/graphics/Rectangle.md#equals(java.lang.Object))

### hashCode

public int hashCode()
  Overrides: [hashCode](../../../../view/graphics/Rectangle.md#hashCode()) in class [Rectangle](../../../../view/graphics/Rectangle.md) See Also:
        * [Rectangle.hashCode()](../../../../view/graphics/Rectangle.md#hashCode())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
