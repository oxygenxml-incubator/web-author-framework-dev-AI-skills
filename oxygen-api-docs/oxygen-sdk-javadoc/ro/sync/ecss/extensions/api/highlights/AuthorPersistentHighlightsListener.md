Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Class AuthorPersistentHighlightsListener

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorPersistentHighlightsListener extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Listener for all the events related to the [AuthorPersistentHighlight](AuthorPersistentHighlight.md). You can register such a listener using [AuthorReviewController.addAuthorPersistentHighlightListener(AuthorPersistentHighlightsListener)](../AuthorReviewController.md#addAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener)),
  Since: 14
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorPersistentHighlightsListener](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract void [highlightAdded](#highlightAdded(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)
Notified when a [AuthorPersistentHighlight](AuthorPersistentHighlight.md) is added to the document.
  void [highlightRangeReconfiguredUpdated](#highlightRangeReconfiguredUpdated(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight,int,int))([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight, int oldStartOffset, int oldEndOffset)
Notified when the range of a [AuthorPersistentHighlight](AuthorPersistentHighlight.md) is updated, for example the start or end offsets might have changed.
  abstract void [highlightRemoved](#highlightRemoved(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)
Notified when a [AuthorPersistentHighlight](AuthorPersistentHighlight.md) is removed from the document.
  void [highlightsAdded](#highlightsAdded(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](AuthorPersistentHighlight.md)> highlights)
Notified when a list of [AuthorPersistentHighlight](AuthorPersistentHighlight.md) are added to the document.
  abstract void [highlightsChanged](#highlightsChanged())()
Event which notifies that the list of highlights (change tracking, comments or custom) has changed in an unpredictable way.
  void [highlightsRemoved](#highlightsRemoved(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](AuthorPersistentHighlight.md)> highlights)
Notified when a list of [AuthorPersistentHighlight](AuthorPersistentHighlight.md) are removed from the document.
  abstract void [highlightUpdated](#highlightUpdated(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)
Notified when a property of a [AuthorPersistentHighlight](AuthorPersistentHighlight.md) is updated, for example changing the comment of a change tracking marker.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorPersistentHighlightsListener

public AuthorPersistentHighlightsListener()

## Method Details

### highlightAdded

public abstract void highlightAdded([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)

Notified when a [AuthorPersistentHighlight](AuthorPersistentHighlight.md) is added to the document.
  Parameters: highlight - Added highlight.
### highlightsAdded

public void highlightsAdded([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](AuthorPersistentHighlight.md)> highlights)

Notified when a list of [AuthorPersistentHighlight](AuthorPersistentHighlight.md) are added to the document.
  Parameters: highlights - Added highlights.
### highlightRemoved

public abstract void highlightRemoved([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)

Notified when a [AuthorPersistentHighlight](AuthorPersistentHighlight.md) is removed from the document.
  Parameters: highlight - The removed highlight.
### highlightsRemoved

public void highlightsRemoved([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](AuthorPersistentHighlight.md)> highlights)

Notified when a list of [AuthorPersistentHighlight](AuthorPersistentHighlight.md) are removed from the document.
  Parameters: highlights - The list of highlights to be removed.
### highlightUpdated

public abstract void highlightUpdated([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight)

Notified when a property of a [AuthorPersistentHighlight](AuthorPersistentHighlight.md) is updated, for example changing the comment of a change tracking marker.
  Parameters: highlight - The updated highlight.
### highlightRangeReconfiguredUpdated

public void highlightRangeReconfiguredUpdated([AuthorPersistentHighlight](AuthorPersistentHighlight.md) highlight, int oldStartOffset, int oldEndOffset)

Notified when the range of a [AuthorPersistentHighlight](AuthorPersistentHighlight.md) is updated, for example the start or end offsets might have changed.
  Parameters: highlight - The updated highlight. oldStartOffset - The old start range for the highlight. oldEndOffset - The old end range for the highlight Since: 23
### highlightsChanged

public abstract void highlightsChanged()

Event which notifies that the list of highlights (change tracking, comments or custom) has changed in an unpredictable way. API code which inserts or deletes multiple fragments in one operation like:ro.sync.ecss.extensions.api.AuthorDocumentController.insertMultipleFragments(AuthorElement, AuthorDocumentFragment[], int[])ro.sync.ecss.extensions.api.AuthorDocumentController.insertMultipleElements(AuthorElement, String[], int[], String)ro.sync.ecss.extensions.api.AuthorDocumentController.multipleDelete(AuthorElement, int[], int[])will not fire atomic events each time a highlight is reconfigured.Instead, they will fire a single event after the operation has finished notifying the listener to reconfigure all its highlight data.This event will follow an:ro.sync.ecss.dom.AuthorDocumentListener.authorNodeStructureChanged(AuthorNodeStructureChangedEvent)event.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
