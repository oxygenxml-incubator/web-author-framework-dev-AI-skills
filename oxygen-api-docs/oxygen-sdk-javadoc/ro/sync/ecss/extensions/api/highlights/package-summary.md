# Package ro.sync.ecss.extensions.api.highlights

package ro.sync.ecss.extensions.api.highlights

API used to interact with persistent (change tracking, comments, user persistent highlights) and non persistent highlights in the Author page
     Related Packages
Package

Description
 [ro.sync.ecss.extensions.api](../package-summary.md)
Main API package used for controlling the Author page (making modifications, adding listeners).
      All Classes and InterfacesInterfacesClassesEnum Classes
Class

Description
 [AuthorHighlighter](AuthorHighlighter.md)
The highlighter which will be available to users to add, remove and check highlights.
  [AuthorHighlighterListener](AuthorHighlighterListener.md)
Listener for the author highlighter events.
  [AuthorPersistentHighlight](AuthorPersistentHighlight.md)
Defines the Author Persistent Highlight which get serialized in the XML as processing instruction.
  [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md)
The Author Persistent Highlight type.
  [AuthorPersistentHighlightActionsProvider](AuthorPersistentHighlightActionsProvider.md)
The provider for contextual actions that are shown on the contextual menu of the persistent highlight (in the main editor area - not yet supported) and on the associated callout.
  [AuthorPersistentHighlightConstants](AuthorPersistentHighlightConstants.md)
Constants used in the serialization process of the Author Persistent Highlights.
  [AuthorPersistentHighlighter](AuthorPersistentHighlighter.md)
Manage the user custom persistent highlights which get serialized in the XML as processing instructions with the form:  <?oxy_custom_start prop1="val1"....?> xml content <?oxy_custom_end?> The Highlighter is accessible from [WSAuthorEditorPageBase.getPersistentHighlighter()](../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getPersistentHighlighter()).
  [AuthorPersistentHighlightsFilter](AuthorPersistentHighlightsFilter.md)
Filter for the [AuthorPersistentHighlight](AuthorPersistentHighlight.md) presented in the author page, callouts section and review panel.
  [AuthorPersistentHighlightsListener](AuthorPersistentHighlightsListener.md)
Listener for all the events related to the [AuthorPersistentHighlight](AuthorPersistentHighlight.md).
  [ColorHighlightPainter](ColorHighlightPainter.md)
Painter that can be used to customize the way that a highlight is displayed by setting custom text decoration, text decoration stroke, background color or stroke color.
  [ColorHighlightPainter.TextDecoration](ColorHighlightPainter.TextDecoration.md)
The decoration added to text.
  [Highlight](Highlight.md)
The highlight interface.
  [HighlightActionsProvider](HighlightActionsProvider.md)
Provider for the actions available for a highlight.
  [HighlightActionsRenderingStyle](HighlightActionsRenderingStyle.md)
The rendering style of the actions associated with a highlight.
  [HighlightPainter](HighlightPainter.md)
Highlight renderer.
  [HighlightPainterInfo](HighlightPainterInfo.md)
Information needed by the painter.
  [PersistentHighlightRenderer](PersistentHighlightRenderer.md)
Customize the way that the author persistent highlights are displayed.
  [PrioritizableHighlightPainter](PrioritizableHighlightPainter.md)
A highlight painter that can be prioritized, by telling it to paint all its highlight on a specific layer.
  [PrioritizableHighlightPainter.ZLayer](PrioritizableHighlightPainter.ZLayer.md)
Layers where a painter can paint its highlights.
  [RectangleHighlightPainter](RectangleHighlightPainter.md)
Fill a rectangle for the given highlight.
  [TextForegroundHighlighterPainter](TextForegroundHighlighterPainter.md)
Can also draw the text foreground with a certain color.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
