Package [ro.sync.ecss.extensions.api.review](package-summary.md)

# Class AuthorReviewRenderingInformation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.review.AuthorReviewRenderingInformation
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorReviewRenderingInformation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The review view entries are representations of Track Changes insert and delete highlights and review comment highlights highlights in Author mode.
  Since: 17.1
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorReviewRenderingInformation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAuthor](#getAuthor())()
Provides the reviewer author name that will be presented in the review view entry.
  [Color](../../../../exml/view/graphics/Color.md) [getColor](#getColor())()
Provides color for styling the associated review entry box.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getComment](#getComment(int))(int limit)
Provides the review comment that will be presented in the review entry.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContentFromTarget](#getContentFromTarget(int))(int limit)
Provides a section from the document content that is covered by this review entry.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getIconPath](#getIconPath())()
Provides the icon URL path for styling the associated review entry box.
  long [getTimestamp](#getTimestamp())()
Provides the review creation or modification time.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTooltip](#getTooltip())()
Get tooltip to show when hovering over the review entry.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorReviewRenderingInformation

public AuthorReviewRenderingInformation()

## Method Details

### getAuthor

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAuthor()

Provides the reviewer author name that will be presented in the review view entry.
  Returns: the reviewer author name. Can be null if the default author must be used
### getTimestamp

public long getTimestamp()

Provides the review creation or modification time.
  Returns: the review creation or modification time. Returns the number of milliseconds since January 1, 1970, 00:00:00 GMT
Can be -1 if the modification time was not set. In this case, the review view will present the default detected timestamp.

### getTooltip

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTooltip()

Get tooltip to show when hovering over the review entry. By default this shows the review creation or modification time.
  Returns: the tooltip to show when hovering over the review entry.
Can be null to use the default behavior.

### getComment

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getComment(int limit)

Provides the review comment that will be presented in the review entry. This could be a part of the real comment stored in the change or persistent highlight.
  Parameters: limit - the suggested text limit (in characters). Returns: the review comment. Can be null if you want the default processing to be performed.
### getContentFromTarget

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContentFromTarget(int limit)

Provides a section from the document content that is covered by this review entry. This will be presented in the content part of the review entry. Note that it is not necessary to provide the entire content related to the review entry.
  Parameters: limit - the suggested text limit (in characters). Returns: the limited document content. Can be null if the content should be processed using the default behavior.
### getColor

public [Color](../../../../exml/view/graphics/Color.md) getColor()

Provides color for styling the associated review entry box.
  Returns: The color to be used for rendering the review entry. Can be null for the default.
### getIconPath

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getIconPath()

Provides the icon URL path for styling the associated review entry box.
  Returns: The icon to be used for rendering the review entry. Can be null for the default.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
