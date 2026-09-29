Package [ro.sync.exml.view.graphics](package-summary.md)

# Interface Shape
    All Known Implementing Classes: [BaseShape](BaseShape.md), [Circle](Circle.md), [Ellipse](Ellipse.md), [ImageLayoutInformation](../../workspace/api/images/handlers/ImageLayoutInformation.md), [Polygon](Polygon.md), [Rectangle](Rectangle.md)   @API(type=EXTENDABLE, src=PRIVATE) public interface Shape
Common shape

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [contains](#contains(int,int))(int x, int y)
Check if the specified coordinates are inside the shape.
  boolean [contains](#contains(int,int,int,int))(int x, int y, int w, int h)
Check if the specified coordinates are inside the shape.
  [Rectangle](Rectangle.md) [getBounds](#getBounds())()

 [Shape](Shape.md) [translate](#translate(int,int))(int tx, int ty)
Translate the shape into another one.

## Method Details

### getBounds

[Rectangle](Rectangle.md) getBounds()
  Returns: The bounds of this shape.
### translate

[Shape](Shape.md) translate(int tx, int ty)

Translate the shape into another one.
  Parameters: tx - the distance by which coordinates are translated in the X axis direction ty - the distance by which coordinates are translated in the Y axis direction Returns: The newly translated shape
### contains

boolean contains(int x, int y)

Check if the specified coordinates are inside the shape.
  Parameters: x - The horizontal coordinate. y - The vertical coordinate. Returns: true if the point is inside the shape. false otherwise.
### contains

boolean contains(int x, int y, int w, int h)

Check if the specified coordinates are inside the shape.
  Parameters: x - The horizontal coordinate. y - The vertical coordinate. w - The width. h - The height. Returns: true if the point is inside the shape. false otherwise.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
