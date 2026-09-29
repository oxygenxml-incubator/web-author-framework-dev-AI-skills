Package [ro.sync.ecss.extensions.api.callouts](package-summary.md)

# Class AuthorCalloutRenderingInformation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.callouts.AuthorCalloutRenderingInformation
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorCalloutRenderingInformation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The callouts are representations of Track Changes insert and delete highlights, review comment highlights and custom review highlights in Author mode. By default, the callouts visibility in Author mode is controlled from Oxygen Preferences but it can be changed by using the [AuthorCalloutsController](AuthorCalloutsController.md) methods. The AuthorReviewCalloutInformation object holds the data that will be rendered as a callout, in Author mode. To render a custom highlight as a callout in Author mode, a callouts information provider must be set from [AuthorCalloutsController.setCalloutsRenderingInformationProvider(CalloutsRenderingInformationProvider)](AuthorCalloutsController.md#setCalloutsRenderingInformationProvider(ro.sync.ecss.extensions.api.callouts.CalloutsRenderingInformationProvider)) method.
  Since: 14
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorCalloutRenderingInformation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getAdditionalData](#getAdditionalData())()
Provides the review additional data that will be presented in the callout content part.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAuthor](#getAuthor())()
Provides the reviewer author name that will be presented in the callout header part, if [getHeaderInformation()](#getHeaderInformation()) method returns null.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCalloutType](#getCalloutType())()
Provides a human readable string representing the callout type that will be rendered as a description of the callout, in the header part, if [getHeaderInformation()](#getHeaderInformation()) method returns null.
  abstract [Color](../../../../exml/view/graphics/Color.md) [getColor](#getColor())()
Provides color for styling the associated callout box.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getComment](#getComment(int))(int limit)
Provides the review comment that will be presented in the callout content part.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContentFromTarget](#getContentFromTarget(int))(int limit)
Provides a section from the document content that is covered by this callout.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHeaderInformation](#getHeaderInformation())()
Provides a human readable string representing the callout description that will be rendered in the header part.
  abstract long [getTimestamp](#getTimestamp())()
Provides the review creation or modification time.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorCalloutRenderingInformation

public AuthorCalloutRenderingInformation()

## Method Details

### getAuthor

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAuthor()

Provides the reviewer author name that will be presented in the callout header part, if [getHeaderInformation()](#getHeaderInformation()) method returns null.
  Returns: the reviewer author name. Can be null if the author is not relevant.
### getTimestamp

public abstract long getTimestamp()

Provides the review creation or modification time.
  Returns: the review creation or modification time. Returns the number of milliseconds since January 1, 1970, 00:00:00 GMT
Can be -1 if the modification time was not set. In this case, the callout will not present any information regarding the review creation or modification time.

### getComment

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getComment(int limit)

Provides the review comment that will be presented in the callout content part. This could be a part of the real comment stored in the change or persistent highlight.
  Parameters: limit - the suggested text limit (in characters). This value comes from the Callouts Options (user preferences). Examples: 80 or 160 characters. Returns: the review comment. Can be null if a comment is not available for this callout.
### getContentFromTarget

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContentFromTarget(int limit)

Provides a section from the document content that is covered by this callout. This will be presented in the content part of the callout. Note that it is not necessary to provide the entire content related to the callout.
  Parameters: limit - the suggested text limit (in characters). This value comes from the Callouts Options (user preferences). Examples: 80 or 160 characters. Returns: the limited document content. Can be null if the content is not relevant for the callout.
### getAdditionalData

public abstract [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getAdditionalData()

Provides the review additional data that will be presented in the callout content part. The callout additional data must be provided as a map between data type and actual callout data. It will be rendered inside the callout as "data_type: data" strings, separated by new lines.
  Returns: The review additional data. Can be null if there is no additional information available for this review.
### getCalloutType

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCalloutType()

Provides a human readable string representing the callout type that will be rendered as a description of the callout, in the header part, if [getHeaderInformation()](#getHeaderInformation()) method returns null.
  Returns: The human readable string representing the callout type or nullif the type is not relevant.
### getHeaderInformation

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHeaderInformation()

Provides a human readable string representing the callout description that will be rendered in the header part.
  Returns: The callout description to be rendered in the header part. If this is null, the header will render the type (provided by [getCalloutType()](#getCalloutType()) method) and the author (provided by [getAuthor()](#getAuthor()) method) Since: 18
### getColor

public abstract [Color](../../../../exml/view/graphics/Color.md) getColor()

Provides color for styling the associated callout box.
  Returns: The color to be used for rendering the callout. Can be null for the default.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
