Package [ro.sync.exml.view.graphics](package-summary.md)

# Class Ellipse

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.view.graphics.BaseShape](BaseShape.md)
        * ro.sync.exml.view.graphics.Ellipse
   All Implemented Interfaces: [Shape](Shape.md)   @API(type=EXTENDABLE, src=PRIVATE) public class Ellipse extends [BaseShape](BaseShape.md)
The class describes an ellipse that is defined by a bounding rectangle.

## Field Summary
 Fields
Modifier and Type

Field

Description
 final int [height](#height)
The overall height of this ellipse.
  final int [width](#width)
The overall width of this ellipse.
  final int [x](#x)
The x coordinate of the upper left corner of this ellipse.
  final int [y](#y)
The y coordinate of the upper left corner of thise llipse.

## Constructor Summary
 Constructors
Constructor

Description
 [Ellipse](#%3Cinit%3E(int,int,int,int))(int x, int y, int width, int height)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [contains](#contains(int,int))(int x, int y)
Warning ! This was not implemented !
  [Rectangle](Rectangle.md) [getBounds](#getBounds())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

 [Shape](Shape.md) [translate](#translate(int,int))(int tx, int ty)
Translate the shape into another one.

### Methods inherited from class ro.sync.exml.view.graphics.[BaseShape](BaseShape.md)
 [contains](BaseShape.md#contains(int,int,int,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### x

public final int x

The x coordinate of the upper left corner of this ellipse.

### y

public final int y

The y coordinate of the upper left corner of thise llipse.

### width

public final int width

The overall width of this ellipse.

### height

public final int height

The overall height of this ellipse.

## Constructor Details

### Ellipse

public Ellipse(int x, int y, int width, int height)

Constructor.
  Parameters: x - The bounding rectangle x pos. y - The bounding rectangle y pos. width - The bounding rectangle width. height - The bounding rectangle height.
## Method Details

### getBounds

public [Rectangle](Rectangle.md) getBounds()
  Returns: The bounds of this shape. See Also:
        * [Shape.getBounds()](Shape.md#getBounds())

### contains

public boolean contains(int x, int y)

Warning ! This was not implemented !
  Parameters: x - The horizontal coordinate. y - The vertical coordinate. Returns: true if the point is inside the shape. false otherwise. See Also:
        * [Shape.contains(int, int)](Shape.md#contains(int,int))

### translate

public [Shape](Shape.md) translate(int tx, int ty)
 Description copied from interface: [Shape](Shape.md#translate(int,int))
Translate the shape into another one.
  Parameters: tx - the distance by which coordinates are translated in the X axis direction ty - the distance by which coordinates are translated in the Y axis direction Returns: The newly translated shape See Also:
        * [Shape.translate(int, int)](Shape.md#translate(int,int))

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
