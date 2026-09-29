Package [ro.sync.exml.view.graphics](package-summary.md)

# Class Rectangle

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.view.graphics.Rectangle
   All Implemented Interfaces: [Shape](Shape.md)   Direct Known Subclasses: [ImageLayoutInformation](../../workspace/api/images/handlers/ImageLayoutInformation.md)   @API(type=EXTENDABLE, src=PRIVATE) public class Rectangle extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Shape](Shape.md)
Rectangle.

## Field Summary
 Fields
Modifier and Type

Field

Description
 int [height](#height)
The height.
  int [width](#width)
The width.
  int [x](#x)
The x.
  int [y](#y)
The y.

## Constructor Summary
 Constructors
Constructor

Description
 [Rectangle](#%3Cinit%3E(int,int,int,int))(int x, int y, int width, int height)
Constructor.
  [Rectangle](#%3Cinit%3E(ro.sync.exml.view.graphics.Rectangle))([Rectangle](Rectangle.md) r)
Copy constructor.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [adjacent](#adjacent(ro.sync.exml.view.graphics.Rectangle))([Rectangle](Rectangle.md) r)

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()

 boolean [contains](#contains(int,int))(int x, int y)
Checks whether or not this Rectangle contains the point at the specified location (*x*, *y*).
  boolean [contains](#contains(int,int,int,int))(int X, int Y, int W, int H)
Checks whether this Rectangle entirely contains the Rectangle at the specified location ( *X* ,  *Y* ) with the specified dimensions ( *W* ,  *H* ).
  boolean [contains](#contains(ro.sync.exml.view.graphics.Rectangle))([Rectangle](Rectangle.md) r)
Checks whether or not this Rectangle entirely contains the specified Rectangle.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
Checks whether two rectangles are equal.
  [Rectangle](Rectangle.md) [getBounds](#getBounds())()

 int [getHeight](#getHeight())()

 int [getWidth](#getWidth())()

 int [getX](#getX())()

 int [getY](#getY())()

 int [hashCode](#hashCode())()

 [Rectangle](Rectangle.md) [intersection](#intersection(ro.sync.exml.view.graphics.Rectangle))([Rectangle](Rectangle.md) r)
Computes the intersection of this Rectangle with the specified Rectangle.
  final boolean [intersects](#intersects(int,int,int,int))(int rX, int rY, int rW, int rH)
Determines whether or not this Rectangle and the specified Rectangle intersect.
  final boolean [intersects](#intersects(ro.sync.exml.view.graphics.Rectangle))([Rectangle](Rectangle.md) r)
Determines whether or not this Rectangle and the specified Rectangle intersect.
  static void [main](#main(java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] args)
TC main.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()
Returns a String representing this Rectangle and its values.
  [Shape](Shape.md) [translate](#translate(int,int))(int tx, int ty)
Translate the shape into another one.
  [Rectangle](Rectangle.md) [union](#union(ro.sync.exml.view.graphics.Rectangle))([Rectangle](Rectangle.md) r)
Computes the union of this Rectangle with the specified Rectangle.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### width

public int width

The width.

### height

public int height

The height.

### x

public int x

The x.

### y

public int y

The y.

## Constructor Details

### Rectangle

public Rectangle(int x, int y, int width, int height)

Constructor.
  Parameters: x - The x coordinate. y - The y coordinate. width - The width. height - The height.
### Rectangle

public Rectangle([Rectangle](Rectangle.md) r)

Copy constructor.
  Parameters: r - The other rectangle to be used.
## Method Details

### intersects

public final boolean intersects([Rectangle](Rectangle.md) r)

Determines whether or not this Rectangle and the specified Rectangle intersect. Two rectangles intersect if their intersection is nonempty.
  Parameters: r - the specified Rectangle Returns: true if the specified Rectangle and this Rectangle intersect; false otherwise.
### intersects

public final boolean intersects(int rX, int rY, int rW, int rH)

Determines whether or not this Rectangle and the specified Rectangle intersect. Two rectangles intersect if their intersection is nonempty.
  Parameters: rX - X of rect rY - Y of rect rW - Width of rect rH - Height of rect Returns: true if the specified Rectangle and this Rectangle intersect; false otherwise.
### contains

public boolean contains([Rectangle](Rectangle.md) r)

Checks whether or not this Rectangle entirely contains the specified Rectangle.
  Parameters: r - the specified Rectangle Returns: true if the Rectangle is contained entirely inside this Rectangle;false otherwise.
### contains

public boolean contains(int X, int Y, int W, int H)

Checks whether this Rectangle entirely contains the Rectangle at the specified location ( *X* ,  *Y* ) with the specified dimensions ( *W* ,  *H* ).
  Specified by: [contains](Shape.md#contains(int,int,int,int)) in interface [Shape](Shape.md) Parameters: X - the specified x coordinate Y - the specified y coordinate W - the width of the Rectangle H - the height of the Rectangle Returns: true if the Rectangle specified by ( *X* ,  *Y* ,  *W* ,  *H* ) is entirely enclosed inside this Rectangle;false otherwise.
### contains

public boolean contains(int x, int y)

Checks whether or not this Rectangle contains the point at the specified location (*x*, *y*).
  Specified by: [contains](Shape.md#contains(int,int)) in interface [Shape](Shape.md) Parameters: x - the specified x coordinate y - the specified y coordinate Returns: true if the point (*x*, *y*) is inside this Rectangle; false otherwise.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()

Returns a String representing this Rectangle and its values.
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Returns: a String representing this Rectangle object's coordinate and size values.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

Checks whether two rectangles are equal.
The result is true if and only if the argument is not null and is a Rectangle object that has the same top-left corner, width, and height as this Rectangle.

  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Parameters: obj - the Object to compare with this Rectangle Returns: true if the objects are equal; false otherwise.
### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### union

public [Rectangle](Rectangle.md) union([Rectangle](Rectangle.md) r)

Computes the union of this Rectangle with the specified Rectangle. Returns a new Rectangle that represents the union of the two rectangles
  Parameters: r - the specified Rectangle Returns: the smallest Rectangle containing both the specified Rectangle and this Rectangle.
### getHeight

public int getHeight()
  Returns: The rectangle height.
### getWidth

public int getWidth()
  Returns: The rectangle width.
### getX

public int getX()
  Returns: The rectangle x coordinate.
### getY

public int getY()
  Returns: The rectangle y coordinate.
### adjacent

public boolean adjacent([Rectangle](Rectangle.md) r)
  Parameters: r - The rectangle to check for adjacency. Returns: True if the rectangles are neighbours around one margin and they do not intersect each other.
### intersection

public [Rectangle](Rectangle.md) intersection([Rectangle](Rectangle.md) r)

Computes the intersection of this Rectangle with the specified Rectangle. Returns a new Rectangle that represents the intersection of the two rectangles. If the two rectangles do not intersect, the result will be an empty rectangle.
  Parameters: r - the specified Rectangle Returns: the largest Rectangle contained in both the specified Rectangle and in this Rectangle; or if the rectangles do not intersect, an empty rectangle.
### main

public static void main([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] args)

TC main.
  Parameters: args - Main args
### getBounds

public [Rectangle](Rectangle.md) getBounds()
  Specified by: [getBounds](Shape.md#getBounds()) in interface [Shape](Shape.md) Returns: The bounds of this shape. See Also:
        * [Shape.getBounds()](Shape.md#getBounds())

### translate

public [Shape](Shape.md) translate(int tx, int ty)
 Description copied from interface: [Shape](Shape.md#translate(int,int))
Translate the shape into another one.
  Specified by: [translate](Shape.md#translate(int,int)) in interface [Shape](Shape.md) Parameters: tx - the distance by which coordinates are translated in the X axis direction ty - the distance by which coordinates are translated in the Y axis direction Returns: The newly translated shape See Also:
        * [Shape.translate(int, int)](Shape.md#translate(int,int))

### clone

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone()
  Overrides: [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.clone()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
