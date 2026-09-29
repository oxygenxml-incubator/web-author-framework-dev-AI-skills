Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Interface PrioritizableHighlightPainter
    All Known Implementing Classes: [ColorHighlightPainter](ColorHighlightPainter.md), [RectangleHighlightPainter](RectangleHighlightPainter.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface PrioritizableHighlightPainter
A highlight painter that can be prioritized, by telling it to paint all its highlight on a specific layer.

## Nested Class Summary
 Nested Classes
Modifier and Type

Interface

Description
 static enum  [PrioritizableHighlightPainter.ZLayer](PrioritizableHighlightPainter.ZLayer.md)
Layers where a painter can paint its highlights.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [PrioritizableHighlightPainter.ZLayer](PrioritizableHighlightPainter.ZLayer.md) [getZLayer](#getZLayer())()
Get the Z layer where this highlight painter paints all its highlights.

## Method Details

### getZLayer

[PrioritizableHighlightPainter.ZLayer](PrioritizableHighlightPainter.ZLayer.md) getZLayer()

Get the Z layer where this highlight painter paints all its highlights. One of [PrioritizableHighlightPainter.ZLayer.BASE_LAYER](PrioritizableHighlightPainter.ZLayer.md#BASE_LAYER), [PrioritizableHighlightPainter.ZLayer.MIDDLE_LAYER](PrioritizableHighlightPainter.ZLayer.md#MIDDLE_LAYER) or [PrioritizableHighlightPainter.ZLayer.TOP_LAYER](PrioritizableHighlightPainter.ZLayer.md#TOP_LAYER).
  Returns: the Z layer where this highlight painter paints all its highlights. Since: 18.0
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
