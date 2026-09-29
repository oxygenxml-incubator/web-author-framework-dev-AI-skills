Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorOperationWithCustomUndoBehavior
    All Known Implementing Classes: [ReloadContentOperation](../commons/operations/ReloadContentOperation.md), [TopicContentViewModeOperation](../dita/map/topicref/TopicContentViewModeOperation.md), [TopicReferencesViewModeOperation](../dita/map/topicref/TopicReferencesViewModeOperation.md), [TopicTitlesViewModeOperation](../dita/map/topicref/TopicTitlesViewModeOperation.md), [WebappMarkAsSavedOperation](../commons/operations/WebappMarkAsSavedOperation.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorOperationWithCustomUndoBehavior
Marker interface that specifies that a particular operation should not be wrapped in a compound undoable edit. This is useful if the operation wants a custom undo behavior.
  Since: 21.1.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
