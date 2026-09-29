Package [ro.sync.exml.view.graphics](package-summary.md)

# Class BaseShape

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.view.graphics.BaseShape
   All Implemented Interfaces: [Shape](Shape.md)   Direct Known Subclasses: [Circle](Circle.md), [Ellipse](Ellipse.md), [Polygon](Polygon.md)   @API(type=EXTENDABLE, src=PRIVATE) public abstract class BaseShape extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Shape](Shape.md)
Base for shapes.

## Constructor Summary
 Constructors
Constructor

Description
 [BaseShape](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [contains](#contains(int,int,int,int))(int x, int y, int w, int h)
Check if the specified coordinates are inside the shape.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.exml.view.graphics.[Shape](Shape.md)
 [contains](Shape.md#contains(int,int)), [getBounds](Shape.md#getBounds()), [translate](Shape.md#translate(int,int))
## Constructor Details

### BaseShape

public BaseShape()

## Method Details

### contains

public boolean contains(int x, int y, int w, int h)
 Description copied from interface: [Shape](Shape.md#contains(int,int,int,int))
Check if the specified coordinates are inside the shape.
  Specified by: [contains](Shape.md#contains(int,int,int,int)) in interface [Shape](Shape.md) Parameters: x - The horizontal coordinate. y - The vertical coordinate. w - The width. h - The height. Returns: true if the point is inside the shape. false otherwise. See Also:
        * [Shape.contains(int, int, int, int)](Shape.md#contains(int,int,int,int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
