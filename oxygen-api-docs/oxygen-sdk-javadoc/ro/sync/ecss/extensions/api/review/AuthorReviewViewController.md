Package [ro.sync.ecss.extensions.api.review](package-summary.md)

# Interface AuthorReviewViewController
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorReviewViewController
The review view presents Track Changes insert and delete highlights and review comment highlights in the Author mode.
  Since: 17.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addReviewActionsProvider](#addReviewActionsProvider(ro.sync.ecss.extensions.api.review.ReviewActionsProvider))([ReviewActionsProvider](ReviewActionsProvider.md) actionsProvider)
Add a review actions provider, notified when a review is right clicked.
  void [removeReviewActionsProvider](#removeReviewActionsProvider(ro.sync.ecss.extensions.api.review.ReviewActionsProvider))([ReviewActionsProvider](ReviewActionsProvider.md) actionsProvider)
Remove a review actions provider.
  void [setReviewsRenderingInformationProvider](#setReviewsRenderingInformationProvider(ro.sync.ecss.extensions.api.review.ReviewsRenderingInformationProvider))([ReviewsRenderingInformationProvider](ReviewsRenderingInformationProvider.md) provider)
Set the provider for data that will be rendered in the review panel for a specific highlight.

## Method Details

### setReviewsRenderingInformationProvider

void setReviewsRenderingInformationProvider([ReviewsRenderingInformationProvider](ReviewsRenderingInformationProvider.md) provider)

Set the provider for data that will be rendered in the review panel for a specific highlight. The review entries are representations of Track Changes insert and delete highlights, review comment highlights and custom review highlights in Author mode.
  Parameters: provider - The highlights review rendering information provider. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - Thrown when a property name is not a valid XML attribute name.
### addReviewActionsProvider

void addReviewActionsProvider([ReviewActionsProvider](ReviewActionsProvider.md) actionsProvider)

Add a review actions provider, notified when a review is right clicked.
  Parameters: actionsProvider - The review actions provider.
### removeReviewActionsProvider

void removeReviewActionsProvider([ReviewActionsProvider](ReviewActionsProvider.md) actionsProvider)

Remove a review actions provider.
  Parameters: actionsProvider - The review actions provider.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
