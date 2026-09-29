Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Interface TextForegroundHighlighterPainter
    All Superinterfaces: [HighlightPainter](HighlightPainter.md)   All Known Implementing Classes: [ColorHighlightPainter](ColorHighlightPainter.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface TextForegroundHighlighterPainterextends [HighlightPainter](HighlightPainter.md)
Can also draw the text foreground with a certain color.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Color](../../../../exml/view/graphics/Color.md) [getTextForegroundColor](#getTextForegroundColor())()
Get the color for the text foreground.

### Methods inherited from interface ro.sync.ecss.extensions.api.highlights.[HighlightPainter](HighlightPainter.md)
 [paint](HighlightPainter.md#paint(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo))
## Method Details

### getTextForegroundColor

[Color](../../../../exml/view/graphics/Color.md) getTextForegroundColor()

Get the color for the text foreground. NULL for inhibiting this feature.
  Returns: the color for the text foreground. NULL for inhibiting this feature.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
