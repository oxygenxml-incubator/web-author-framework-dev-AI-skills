Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Class RectangleHighlightPainter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.highlights.RectangleHighlightPainter
   All Implemented Interfaces: [HighlightPainter](HighlightPainter.md), [PrioritizableHighlightPainter](PrioritizableHighlightPainter.md)   @API(type=EXTENDABLE, src=PUBLIC) public class RectangleHighlightPainter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [HighlightPainter](HighlightPainter.md), [PrioritizableHighlightPainter](PrioritizableHighlightPainter.md)
Fill a rectangle for the given highlight.

## Nested Class Summary

## Nested classes/interfaces inherited from interface ro.sync.ecss.extensions.api.highlights.[PrioritizableHighlightPainter](PrioritizableHighlightPainter.md)
 [PrioritizableHighlightPainter.ZLayer](PrioritizableHighlightPainter.ZLayer.md)
## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [Color](../../../../exml/view/graphics/Color.md) [fillColor](#fillColor)
The fill color.

## Constructor Summary
 Constructors
Constructor

Description
 [RectangleHighlightPainter](#%3Cinit%3E(ro.sync.exml.view.graphics.Color))([Color](../../../../exml/view/graphics/Color.md) fillColor)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [PrioritizableHighlightPainter.ZLayer](PrioritizableHighlightPainter.ZLayer.md) [getZLayer](#getZLayer())()
Get the Z layer where this highlight painter paints all its highlights.
  void [paint](#paint(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo))([HighlightPainterInfo](HighlightPainterInfo.md) pi)
Renders the highlight.
  protected void [paintHighlight](#paintHighlight(ro.sync.exml.view.graphics.Graphics,int,int,int,int))([Graphics](../../../../exml/view/graphics/Graphics.md) g, int x, int y, int width, int height)
Paint highlight.
  void [setFillColor](#setFillColor(ro.sync.exml.view.graphics.Color))([Color](../../../../exml/view/graphics/Color.md) fillColor)

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### fillColor

protected [Color](../../../../exml/view/graphics/Color.md) fillColor

The fill color.

## Constructor Details

### RectangleHighlightPainter

public RectangleHighlightPainter([Color](../../../../exml/view/graphics/Color.md) fillColor)

Constructor.
  Parameters: fillColor - The fill color.
## Method Details

### getZLayer

public [PrioritizableHighlightPainter.ZLayer](PrioritizableHighlightPainter.ZLayer.md) getZLayer()
 Description copied from interface: [PrioritizableHighlightPainter](PrioritizableHighlightPainter.md#getZLayer())
Get the Z layer where this highlight painter paints all its highlights. One of [PrioritizableHighlightPainter.ZLayer.BASE_LAYER](PrioritizableHighlightPainter.ZLayer.md#BASE_LAYER), [PrioritizableHighlightPainter.ZLayer.MIDDLE_LAYER](PrioritizableHighlightPainter.ZLayer.md#MIDDLE_LAYER) or [PrioritizableHighlightPainter.ZLayer.TOP_LAYER](PrioritizableHighlightPainter.ZLayer.md#TOP_LAYER).
  Specified by: [getZLayer](PrioritizableHighlightPainter.md#getZLayer()) in interface [PrioritizableHighlightPainter](PrioritizableHighlightPainter.md) Returns: the Z layer where this highlight painter paints all its highlights. See Also:
        * [PrioritizableHighlightPainter.getZLayer()](PrioritizableHighlightPainter.md#getZLayer())

### paint

public void paint([HighlightPainterInfo](HighlightPainterInfo.md) pi)
 Description copied from interface: [HighlightPainter](HighlightPainter.md#paint(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo))
Renders the highlight.
  Specified by: [paint](HighlightPainter.md#paint(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo)) in interface [HighlightPainter](HighlightPainter.md) Parameters: pi - Information used by highlight See Also:
        * [HighlightPainter.paint(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo)](HighlightPainter.md#paint(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo))

### paintHighlight

protected void paintHighlight([Graphics](../../../../exml/view/graphics/Graphics.md) g, int x, int y, int width, int height)

Paint highlight.
  Parameters: g - The graphics used for paint. x - The x coordinate. y - The y coordinate. width - The rectangle width. height - The rectangle height.
### setFillColor

public void setFillColor([Color](../../../../exml/view/graphics/Color.md) fillColor)
  Parameters: fillColor - The fill color to set.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
