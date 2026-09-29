Package [ro.sync.exml.view.graphics](package-summary.md)

# Class Polygon

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.view.graphics.BaseShape](BaseShape.md)
        * ro.sync.exml.view.graphics.Polygon
   All Implemented Interfaces: [Shape](Shape.md), ro.sync.exml.view.graphics.ShapePointContributor   @API(type=EXTENDABLE, src=PRIVATE) public class Polygon extends [BaseShape](BaseShape.md)implements ro.sync.exml.view.graphics.ShapePointContributor
The Polygon class encapsulates a description of a closed, two-dimensional region within a coordinate space.

## Field Summary
 Fields
Modifier and Type

Field

Description
 int [npoints](#npoints)
The total number of points.
  int[] [xpoints](#xpoints)
The array of *x* coordinates.
  int[] [ypoints](#ypoints)
The array of *y* coordinates.

## Constructor Summary
 Constructors
Constructor

Description
 [Polygon](#%3Cinit%3E())()
Creates an empty polygon.
  [Polygon](#%3Cinit%3E(int%5B%5D,int%5B%5D,int))(int[] xpoints, int[] ypoints, int npoints)
Constructs and initializes a Polygon from the specified parameters.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addPoint](#addPoint(int,int))(int x, int y)
Appends the specified coordinates to this Polygon.
  boolean [contains](#contains(int,int))(int x, int y)
Check if this complicated shape contains the requested point.
  [Rectangle](Rectangle.md) [getBounds](#getBounds())()

 [Shape](Shape.md) [translate](#translate(int,int))(int tx, int ty)
Translate the shape into another one.

### Methods inherited from class ro.sync.exml.view.graphics.[BaseShape](BaseShape.md)
 [contains](BaseShape.md#contains(int,int,int,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### npoints

public int npoints

The total number of points. The value of npointsrepresents the number of valid points in this Polygonand might be less than the number of elements in [xpoints](#xpoints) or [ypoints](#ypoints). This value can be NULL.
  See Also:
        * [addPoint(int, int)](#addPoint(int,int))

### xpoints

public int[] xpoints

The array of *x* coordinates. The number of elements in this array might be more than the number of *x* coordinates in this Polygon. The extra elements allow new points to be added to this Polygon without re-creating this array. The value of [npoints](#npoints) is equal to the number of valid points in this Polygon.
  See Also:
        * [addPoint(int, int)](#addPoint(int,int))

### ypoints

public int[] ypoints

The array of *y* coordinates. The number of elements in this array might be more than the number of *y* coordinates in this Polygon. The extra elements allow new points to be added to this Polygon without re-creating this array. The value of npoints is equal to the number of valid points in this Polygon.
  See Also:
        * [addPoint(int, int)](#addPoint(int,int))

## Constructor Details

### Polygon

public Polygon()

Creates an empty polygon.

### Polygon

public Polygon(int[] xpoints, int[] ypoints, int npoints)

Constructs and initializes a Polygon from the specified parameters.
  Parameters: xpoints - an array of *x* coordinates ypoints - an array of *y* coordinates npoints - the total number of points in the Polygon Throws: [NegativeArraySizeException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NegativeArraySizeException.html) - if the value of npoints is negative. [IndexOutOfBoundsException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IndexOutOfBoundsException.html) - if npoints is greater than the length of xpointsor the length of ypoints. [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if xpoints or ypoints is null.
## Method Details

### addPoint

public void addPoint(int x, int y)

Appends the specified coordinates to this Polygon.
If an operation that calculates the bounding box of this Polygon has already been performed, such as getBounds or contains, then this method updates the bounding box.

  Specified by: addPoint in interface ro.sync.exml.view.graphics.ShapePointContributor Parameters: x - the specified x coordinate y - the specified y coordinate See Also:
        * [Polygon.getBounds()](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Polygon.html#getBounds())

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

### contains

public boolean contains(int x, int y)

Check if this complicated shape contains the requested point.
  Specified by: [contains](Shape.md#contains(int,int)) in interface [Shape](Shape.md) Parameters: x - The X of the point. y - The Y of the point. Returns: true if the point is inside of the shape. false otherwise.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
