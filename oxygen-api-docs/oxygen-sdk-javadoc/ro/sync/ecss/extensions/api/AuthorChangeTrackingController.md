Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorChangeTrackingController
    All Superinterfaces: [ChangeTrackingController](ChangeTrackingController.md)   All Known Subinterfaces: [AuthorReviewController](AuthorReviewController.md), [ReviewController](webapp/review/ReviewController.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorChangeTrackingControllerextends [ChangeTrackingController](ChangeTrackingController.md)
Controls the change tracking mode. Can toggle change tracking on and off and check its state.

## Method Summary

### Methods inherited from interface ro.sync.ecss.extensions.api.[ChangeTrackingController](ChangeTrackingController.md)
 [accept](ChangeTrackingController.md#accept(int,int)), [accept](ChangeTrackingController.md#accept(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight)), [acceptSelection](ChangeTrackingController.md#acceptSelection(int,int)), [getAttributeChangeHighlights](ChangeTrackingController.md#getAttributeChangeHighlights()), [getChangeHighlights](ChangeTrackingController.md#getChangeHighlights()), [getChangeHighlights](ChangeTrackingController.md#getChangeHighlights(int,int)), [isTrackingChanges](ChangeTrackingController.md#isTrackingChanges()), [reject](ChangeTrackingController.md#reject(int,int)), [reject](ChangeTrackingController.md#reject(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight)), [rejectSelection](ChangeTrackingController.md#rejectSelection(int,int)), [toggleTrackChanges](ChangeTrackingController.md#toggleTrackChanges())
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
