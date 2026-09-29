Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Interface AuthorHighlighterListener
    @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorHighlighterListener
Listener for the author highlighter events. To add this listener use the following method: [AuthorHighlighter.addListener(AuthorHighlighterListener)](AuthorHighlighter.md#addListener(ro.sync.ecss.extensions.api.highlights.AuthorHighlighterListener)).
  Since: 21.1
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 void [allHighlightsRemoved](#allHighlightsRemoved(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Highlight](Highlight.md)> removedHighlights)
All highlights were removed.
  void [highlightAdded](#highlightAdded(ro.sync.ecss.extensions.api.highlights.Highlight))([Highlight](Highlight.md) highlight)
A highlight was added.
  void [highlightRemoved](#highlightRemoved(ro.sync.ecss.extensions.api.highlights.Highlight))([Highlight](Highlight.md) highlight)
A highlight was removed.
  default void [highlightsRemoved](#highlightsRemoved(ro.sync.ecss.extensions.api.highlights.Highlight%5B%5D))([Highlight](Highlight.md)[] highlights)
A group of highlights was removed.

## Method Details

### highlightAdded

void highlightAdded([Highlight](Highlight.md) highlight)

A highlight was added.
  Parameters: highlight - The added highlight.
### highlightRemoved

void highlightRemoved([Highlight](Highlight.md) highlight)

A highlight was removed.
  Parameters: highlight - The removed highlight.
### highlightsRemoved

default void highlightsRemoved([Highlight](Highlight.md)[] highlights)

A group of highlights was removed.
  Parameters: highlights - The removed highlights.
### allHighlightsRemoved

void allHighlightsRemoved([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Highlight](Highlight.md)> removedHighlights)

All highlights were removed.
  Parameters: removedHighlights - The list of removed highlights.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
