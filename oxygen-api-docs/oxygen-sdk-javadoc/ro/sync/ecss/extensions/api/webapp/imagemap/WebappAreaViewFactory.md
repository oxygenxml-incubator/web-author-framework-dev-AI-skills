Package [ro.sync.ecss.extensions.api.webapp.imagemap](package-summary.md)

# Interface WebappAreaViewFactory
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WebappAreaViewFactory
Creates instances of WebappAreaView.
  Since: 25.0
## Method Summary
  Static Methods
Modifier and Type

Method

Description
 static [WebappAreaView](WebappAreaView.md) [createCircle](#createCircle(ro.sync.exml.view.graphics.Circle,int))([Circle](../../../../../exml/view/graphics/Circle.md) circle, int layer)
Create a circle.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[NewWebappAreaView](NewWebappAreaView.md)> [createFromSvg](#createFromSvg(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) svg)
Return the areas encoded in the SVG.
  static [WebappAreaView](WebappAreaView.md) [createPolygon](#createPolygon(ro.sync.exml.view.graphics.Polygon,int))([Polygon](../../../../../exml/view/graphics/Polygon.md) polygon, int layer)
Create a polygon.
  static [WebappAreaView](WebappAreaView.md) [createRectangle](#createRectangle(ro.sync.exml.view.graphics.Rectangle,int))([Rectangle](../../../../../exml/view/graphics/Rectangle.md) rectangle, int layer)
Create a rectangle.

## Method Details

### createRectangle

static [WebappAreaView](WebappAreaView.md) createRectangle([Rectangle](../../../../../exml/view/graphics/Rectangle.md) rectangle, int layer)

Create a rectangle.
  Parameters: rectangle - The shape. layer - The layer on which it is painted. Returns: The area view.
### createCircle

static [WebappAreaView](WebappAreaView.md) createCircle([Circle](../../../../../exml/view/graphics/Circle.md) circle, int layer)

Create a circle.
  Parameters: circle - The shape. layer - The layer on which it is painted. Returns: The area view.
### createPolygon

static [WebappAreaView](WebappAreaView.md) createPolygon([Polygon](../../../../../exml/view/graphics/Polygon.md) polygon, int layer)

Create a polygon.
  Parameters: polygon - The shape. layer - The layer on which it is painted. Returns: The area view.
### createFromSvg

static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[NewWebappAreaView](NewWebappAreaView.md)> createFromSvg([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) svg)

Return the areas encoded in the SVG.
  Parameters: svg - The SVG string. Returns: The list of areas. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if the areas could not be decoded.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
