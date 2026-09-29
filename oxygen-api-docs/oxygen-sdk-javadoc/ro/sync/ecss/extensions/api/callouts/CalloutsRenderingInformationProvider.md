Package [ro.sync.ecss.extensions.api.callouts](package-summary.md)

# Class CalloutsRenderingInformationProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.callouts.CalloutsRenderingInformationProvider
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class CalloutsRenderingInformationProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Provider for data that will be rendered as callouts, in Author mode. By default it only handles custom persistent highlights but you can override the method [handlesAlsoDefaultHighlights()](#handlesAlsoDefaultHighlights()) to handle also built-in persistent highlights (comment, insertion or deletion change). The callouts are representations of Track Changes insert and delete highlights, review comment highlights and custom review highlights in Author mode. By default, the callouts visibility in Author mode is controlled from Oxygen Preferences but it can be changed by using the [AuthorCalloutsController](AuthorCalloutsController.md) methods. The callouts rendering provider can be set from [AuthorCalloutsController.setCalloutsRenderingInformationProvider(CalloutsRenderingInformationProvider)](AuthorCalloutsController.md#setCalloutsRenderingInformationProvider(ro.sync.ecss.extensions.api.callouts.CalloutsRenderingInformationProvider))
  Since: 14
## Constructor Summary
 Constructors
Constructor

Description
 [CalloutsRenderingInformationProvider](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract [AuthorCalloutRenderingInformation](AuthorCalloutRenderingInformation.md) [getCalloutRenderingInformation](#getCalloutRenderingInformation(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) highlight)
Get the callout rendering information associated with a persistent highlight.
  boolean [handlesAlsoDefaultHighlights](#handlesAlsoDefaultHighlights())()
Return true if you want the rendering information provider to be also called for built-in persistent highlights (comment, insertion or deletion change).
  abstract boolean [shouldRenderAsCallout](#shouldRenderAsCallout(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) highlight)
Asks if a custom persistent highlight should be rendered as a callout in the Author mode.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CalloutsRenderingInformationProvider

public CalloutsRenderingInformationProvider()

## Method Details

### getCalloutRenderingInformation

public abstract [AuthorCalloutRenderingInformation](AuthorCalloutRenderingInformation.md) getCalloutRenderingInformation([AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) highlight)

Get the callout rendering information associated with a persistent highlight. For **custom highlights** the callout rendering information is requested only for that custom persistent highlights for which the [shouldRenderAsCallout(AuthorPersistentHighlight)](#shouldRenderAsCallout(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight)) For **built-in persistent highlights** (comment, insertion or deletion change) the rendering can be requested only you override the [handlesAlsoDefaultHighlights()](#handlesAlsoDefaultHighlights()) method to return true. The callouts are representations of Track Changes insert and delete highlights, review comment highlights and custom review highlights in Author mode.
  Parameters: highlight - The Author persistent highlight. The type of the highlight can be obtained by using the [AuthorPersistentHighlight.getType()](../highlights/AuthorPersistentHighlight.md#getType()) Returns: The callout rendering information associated with a custom persistent highlight or null if the highlight must not be rendered in Author as a callout.
### shouldRenderAsCallout

public abstract boolean shouldRenderAsCallout([AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) highlight)

Asks if a custom persistent highlight should be rendered as a callout in the Author mode. The callouts are representations of Track Changes insert and delete highlights, review comment highlights and custom persistent highlights in Author mode. If this method returns true, the callout rendering information for this callout must be provided by [getCalloutRenderingInformation(AuthorPersistentHighlight)](#getCalloutRenderingInformation(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))method. The implementation of this method must be fast, being called frequently.
  Parameters: highlight - The Author custom persistent highlight. Returns: true if the highlight can be rendered as a callout in Author mode.
### handlesAlsoDefaultHighlights

public boolean handlesAlsoDefaultHighlights()

Return true if you want the rendering information provider to be also called for built-in persistent highlights (comment, insertion or deletion change). The callout rendering information is requested only if the application preferences are configured to show callouts for these highlight types. By default the rendering information provider is called only for custom highlights. The callouts are representations of Track Changes insert and delete highlights, review comment highlights and custom review highlights in Author mode.
  Returns: true if the [getCalloutRenderingInformation(AuthorPersistentHighlight)](#getCalloutRenderingInformation(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight)) method should be called also for built-in persistent highlights (comment, insertion or deletion change). Since: 17.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
