Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface ChangeTrackingController
    All Known Subinterfaces: [AuthorChangeTrackingController](AuthorChangeTrackingController.md), [AuthorReviewController](AuthorReviewController.md), [DITAMapReviewController](../../../exml/workspace/api/editor/page/ditamap/review/DITAMapReviewController.md), [ReviewController](webapp/review/ReviewController.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ChangeTrackingController
Controls the change tracking mode. Can toggle change tracking on and off and check its state.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 void [accept](#accept(int,int))(int startOffset, int endOffset)  Deprecated.
Replaced by "ro.sync.ecss.extensions.api.ChangeTrackingController.acceptSelection(int, int)"
   void [accept](#accept(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) highlight)
Accept the given change tracking highlight.
  void [acceptSelection](#acceptSelection(int,int))(int startOffset, int endOffset)
Accept all change tracking highlights that intersect the interval between the given start and end offset.
  [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md)[] [getAttributeChangeHighlights](#getAttributeChangeHighlights())()
Get the full list of attribute changes.
  [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md)[] [getChangeHighlights](#getChangeHighlights())()
Fetches the list of change tracking highlights.
  [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md)[] [getChangeHighlights](#getChangeHighlights(int,int))(int startOffset, int endOffset)
Fetches the list of change tracking highlight that intersects the interval between the given start offset and end offset.
  boolean [isTrackingChanges](#isTrackingChanges())()
Return true if the current editor is in change tracking mode.
  void [reject](#reject(int,int))(int startOffset, int endOffset)  Deprecated.
Replaced by "ro.sync.ecss.extensions.api.ChangeTrackingController.rejectSelection(int, int)"
   void [reject](#reject(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) highlight)
Reject the given change tracking highlight.
  void [rejectSelection](#rejectSelection(int,int))(int startOffset, int endOffset)
Reject all change tracking highlights that intersect the interval between the given start and end offset.
  void [toggleTrackChanges](#toggleTrackChanges())()
Toggle the track changes mode.

## Method Details

### isTrackingChanges

boolean isTrackingChanges()

Return true if the current editor is in change tracking mode.
  Returns: true if the current editor is in change tracking mode.
### toggleTrackChanges

void toggleTrackChanges()

Toggle the track changes mode. Each opened document has a separate track changes state. The initial state is provided by the default values set in the user preferences: https://www.oxygenxml.com/doc/ug-oxygen/index.html?q=/doc/ug-oxygen/topics/preferences-track-changes.html So after a document is opened, this method can be used to change its track changes state.
  See Also:
        * [isTrackingChanges()](#isTrackingChanges())

### getChangeHighlights

[AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md)[] getChangeHighlights()

Fetches the list of change tracking highlights.
  Returns: The change tracking highlights array. Since: 12
### getAttributeChangeHighlights

[AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md)[] getAttributeChangeHighlights()

Get the full list of attribute changes.
  Returns: The list of attribute changes in the entire document. Since: 17
### getChangeHighlights

[AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md)[] getChangeHighlights(int startOffset, int endOffset)

Fetches the list of change tracking highlight that intersects the interval between the given start offset and end offset.
  Parameters: startOffset - The start offset(inclusive). endOffset - The end offset (inclusive). Returns: The change tracking highlights array. Can be null if no change tracking highlight intersects the given offsets interval. Since: 14.1
### accept

void accept(int startOffset, int endOffset)
 Deprecated.
Replaced by "ro.sync.ecss.extensions.api.ChangeTrackingController.acceptSelection(int, int)"

Accept all change tracking highlights that intersect the interval between the given start and end offset.
  Parameters: startOffset - The interval start offset, inclusive. endOffset - The interval end offset, inclusive. Since: 14.1
### acceptSelection

void acceptSelection(int startOffset, int endOffset)

Accept all change tracking highlights that intersect the interval between the given start and end offset. The difference from the "ro.sync.ecss.extensions.api.ChangeTrackingController.accept(int, int)" method is that the end offset is exclusive and you can accept the selection even if you select only one character.
  Parameters: startOffset - The interval start offset, inclusive. endOffset - The interval end offset, exclusive. Since: 20
### accept

void accept([AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) highlight)

Accept the given change tracking highlight.
  Parameters: highlight - The change tracking highlight to be accepted. Since: 14.1
### reject

void reject(int startOffset, int endOffset)
 Deprecated.
Replaced by "ro.sync.ecss.extensions.api.ChangeTrackingController.rejectSelection(int, int)"

Reject all change tracking highlights that intersect the interval between the given start and end offset.
  Parameters: startOffset - The interval start offset, inclusive. endOffset - The interval end offset, inclusive. Since: 14.1
### rejectSelection

void rejectSelection(int startOffset, int endOffset)

Reject all change tracking highlights that intersect the interval between the given start and end offset. The difference from the "ro.sync.ecss.extensions.api.ChangeTrackingController.reject(int, int)" method is that the end offset is exclusive and you can accept the selection even if you select only one character.
  Parameters: startOffset - The interval start offset, inclusive. endOffset - The interval end offset, exclusive. Since: 20
### reject

void reject([AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) highlight)

Reject the given change tracking highlight.
  Parameters: highlight - The change tracking highlight to be accepted. Since: 14.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
