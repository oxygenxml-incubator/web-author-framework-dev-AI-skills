Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Interface PersistentHighlightRenderer
    @API(type=EXTENDABLE, src=PUBLIC) public interface PersistentHighlightRenderer
Customize the way that the author persistent highlights are displayed. Persistent highlights get serialized as processing instructions in the XML content.
  Since: 12
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [HighlightPainter](HighlightPainter.md) [getHighlightPainter](#getHighlightPainter(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)
Get the painter associated with the given persistent highlight.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTooltip](#getTooltip(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)
Get the display tooltip text for a persistent highlight.

## Method Details

### getHighlightPainter

[HighlightPainter](HighlightPainter.md) getHighlightPainter([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)

Get the painter associated with the given persistent highlight. If a null value is returned the default highlight painter will be used. You can use or customize instances of the default [ColorHighlightPainter](ColorHighlightPainter.md).
  Parameters: highlight - The [AuthorPersistentHighlight](AuthorPersistentHighlight.md) to get the painter for. Returns: The painter.
### getTooltip

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTooltip([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)

Get the display tooltip text for a persistent highlight. If a null value is returned the default tooltip text will be used.
  Parameters: highlight - The [AuthorPersistentHighlight](AuthorPersistentHighlight.md) to get the tooltip for. Returns: The tool tip for the highlight.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
