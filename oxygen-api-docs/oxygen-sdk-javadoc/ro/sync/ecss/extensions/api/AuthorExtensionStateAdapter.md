Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorExtensionStateAdapter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorExtensionStateAdapter
   All Implemented Interfaces: [AuthorExtensionStateListener](AuthorExtensionStateListener.md), [Extension](Extension.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorExtensionStateAdapter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorExtensionStateListener](AuthorExtensionStateListener.md)
Adapter class for [AuthorExtensionStateListener](AuthorExtensionStateListener.md).

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorExtensionStateAdapter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [activated](#activated(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Method called when the Author extension was activated.
  void [deactivated](#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Method called when the Author extension was deactivated.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorExtensionStateAdapter

public AuthorExtensionStateAdapter()

## Method Details

### activated

public void activated([AuthorAccess](AuthorAccess.md) authorAccess)
 Description copied from interface: [AuthorExtensionStateListener](AuthorExtensionStateListener.md#activated(ro.sync.ecss.extensions.api.AuthorAccess))
Method called when the Author extension was activated. This event is triggered when the Author extension where this listener is defined was activated in relation with a document opened in Author page. Listeners like [AuthorMouseListener](AuthorMouseListener.md) or [AuthorListener](AuthorListener.md) can be added at this point.
  Specified by: [activated](AuthorExtensionStateListener.md#activated(ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorExtensionStateListener](AuthorExtensionStateListener.md) Parameters: authorAccess - The [AuthorAccess](AuthorAccess.md) of the Author page where the listener was activated. See Also:
        * [AuthorExtensionStateListener.activated(ro.sync.ecss.extensions.api.AuthorAccess)](AuthorExtensionStateListener.md#activated(ro.sync.ecss.extensions.api.AuthorAccess))

### deactivated

public void deactivated([AuthorAccess](AuthorAccess.md) authorAccess)
 Description copied from interface: [AuthorExtensionStateListener](AuthorExtensionStateListener.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))
Method called when the Author extension was deactivated. This event is triggered when another Author extension corresponding to the the current document opened in Author page was activated, the user switches to another editor page or the editor is closed.
  Specified by: [deactivated](AuthorExtensionStateListener.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorExtensionStateListener](AuthorExtensionStateListener.md) Parameters: authorAccess - The [AuthorAccess](AuthorAccess.md) of the Author page where the listener was deactivated. See Also:
        * [AuthorExtensionStateListener.deactivated(ro.sync.ecss.extensions.api.AuthorAccess)](AuthorExtensionStateListener.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](Extension.md#getDescription()) in interface [Extension](Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
