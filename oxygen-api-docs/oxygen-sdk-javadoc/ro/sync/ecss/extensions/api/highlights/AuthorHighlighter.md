Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Interface AuthorHighlighter
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorHighlighter
The highlighter which will be available to users to add, remove and check highlights. To have access to this highlighter use the following method: [WSAuthorEditorPageBase.getHighlighter()](../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getHighlighter())

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Highlight](Highlight.md) [addHighlight](#addHighlight(int,int,ro.sync.ecss.extensions.api.highlights.HighlightPainter,java.lang.Object))(int startOffset, int endOffset, [HighlightPainter](HighlightPainter.md) painter, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) additionalData)
Adds a highlight to the view.
  void [addListener](#addListener(ro.sync.ecss.extensions.api.highlights.AuthorHighlighterListener))([AuthorHighlighterListener](AuthorHighlighterListener.md) listener)
Adds a listener to be notified about changes regarding highlights.
  [Highlight](Highlight.md)[] [findNonPersistentHighlights](#findNonPersistentHighlights(int,int))(int startOffset, int endOffset)
Find all non-persistent highlights that intersect a range of content.
  [Highlight](Highlight.md)[] [getHighlights](#getHighlights())()
Fetches the current list of highlights.
  void [removeAllHighlights](#removeAllHighlights())()
Removes all highlights this highlighter is responsible for.
  void [removeHighlight](#removeHighlight(ro.sync.ecss.extensions.api.highlights.Highlight))([Highlight](Highlight.md) highlight)
Removes a highlight from the view.
  void [removeHighlights](#removeHighlights(ro.sync.ecss.extensions.api.highlights.Highlight%5B%5D))([Highlight](Highlight.md)[] highlights)
Removes multiple highlights from the view.

## Method Details

### addHighlight

[Highlight](Highlight.md) addHighlight(int startOffset, int endOffset, [HighlightPainter](HighlightPainter.md) painter, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) additionalData)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Adds a highlight to the view. Returns a tag that can be used to refer to the highlight.
  Parameters: startOffset - the beginning of the range >= 0 endOffset - the inclusive end of the range >= startOffset painter - the painter to use for the actual highlighting additionalData - The additional data which can be stored in the highlight. May be null. In Web Author, if the provided additional data is a map, all the keys/value pairs of String/String type are inserted as attributes in the generated HTML span element (excepting the "class" key, all keys are inserted as attributes names with a "data-" prefix). Returns: an object that refers to the highlight Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - for an invalid range specification
### removeHighlight

void removeHighlight([Highlight](Highlight.md) highlight)

Removes a highlight from the view.
  Parameters: highlight - which highlight to remove
### removeHighlights

void removeHighlights([Highlight](Highlight.md)[] highlights)

Removes multiple highlights from the view.
  Parameters: highlights - which highlights to be removed Since: 23.1
### removeAllHighlights

void removeAllHighlights()

Removes all highlights this highlighter is responsible for.

### getHighlights

[Highlight](Highlight.md)[] getHighlights()

Fetches the current list of highlights.
  Returns: the highlight list
### findNonPersistentHighlights

[Highlight](Highlight.md)[] findNonPersistentHighlights(int startOffset, int endOffset)

Find all non-persistent highlights that intersect a range of content.
  Parameters: startOffset - The start offset of the range. endOffset - The end offset of the range. Returns: The list of non-persistent highlights
### addListener

void addListener([AuthorHighlighterListener](AuthorHighlighterListener.md) listener)

Adds a listener to be notified about changes regarding highlights.
  Parameters: listener - The listener Since: 21.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
