Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Interface HighlightPainter
    All Known Subinterfaces: [TextForegroundHighlighterPainter](TextForegroundHighlighterPainter.md)   All Known Implementing Classes: [ColorHighlightPainter](ColorHighlightPainter.md), [RectangleHighlightPainter](RectangleHighlightPainter.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface HighlightPainter
Highlight renderer.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [paint](#paint(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo))([HighlightPainterInfo](HighlightPainterInfo.md) pi)
Renders the highlight.

## Method Details

### paint

void paint([HighlightPainterInfo](HighlightPainterInfo.md) pi)

Renders the highlight.
  Parameters: pi - Information used by highlight
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
