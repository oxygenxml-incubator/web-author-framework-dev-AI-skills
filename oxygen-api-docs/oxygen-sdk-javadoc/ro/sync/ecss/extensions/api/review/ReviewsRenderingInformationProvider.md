Package [ro.sync.ecss.extensions.api.review](package-summary.md)

# Class ReviewsRenderingInformationProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.review.ReviewsRenderingInformationProvider
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ReviewsRenderingInformationProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Provider for data that will be rendered in the review view, in Author mode for highlights.
  Since: 17.1
## Constructor Summary
 Constructors
Constructor

Description
 [ReviewsRenderingInformationProvider](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract [AuthorReviewRenderingInformation](AuthorReviewRenderingInformation.md) [getReviewRenderingInformation](#getReviewRenderingInformation(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) highlight)
Get the review rendering information associated with a highlight.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ReviewsRenderingInformationProvider

public ReviewsRenderingInformationProvider()

## Method Details

### getReviewRenderingInformation

public abstract [AuthorReviewRenderingInformation](AuthorReviewRenderingInformation.md) getReviewRenderingInformation([AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) highlight)

Get the review rendering information associated with a highlight. The review entries are representations of Track Changes insert and delete highlights and review comment highlights in Author mode.
  Parameters: highlight - The Author persistent highlight. You can use the [AuthorPersistentHighlight.getType()](../highlights/AuthorPersistentHighlight.md#getType()) method to obtain its type. Returns: The review rendering information associated with a persistent highlight.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
