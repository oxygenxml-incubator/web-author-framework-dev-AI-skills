Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class ReferenceErrorResolverExt

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.ReferenceErrorResolverExt
   All Implemented Interfaces: [ReferenceErrorResolver](ReferenceErrorResolver.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ReferenceErrorResolverExt extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ReferenceErrorResolver](ReferenceErrorResolver.md)
Resolver for errors concerning references. It will offer solutions for solving the current reference error.

## Constructor Summary
 Constructors
Constructor

Description
 [ReferenceErrorResolverExt](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 final void [resolveError](#resolveError(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Offers solutions to the current reference error.
  void [resolveError](#resolveError(ro.sync.ecss.extensions.api.ErrorResolverContextInfo))([ErrorResolverContextInfo](ErrorResolverContextInfo.md) contextInfo)
Offers solutions to the current reference error.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ReferenceErrorResolverExt

public ReferenceErrorResolverExt()

## Method Details

### resolveError

public final void resolveError([AuthorAccess](AuthorAccess.md) authorAccess)
 Description copied from interface: [ReferenceErrorResolver](ReferenceErrorResolver.md#resolveError(ro.sync.ecss.extensions.api.AuthorAccess))
Offers solutions to the current reference error.
  Specified by: [resolveError](ReferenceErrorResolver.md#resolveError(ro.sync.ecss.extensions.api.AuthorAccess)) in interface [ReferenceErrorResolver](ReferenceErrorResolver.md) Parameters: authorAccess - Access to the author page. See Also:
        * [ReferenceErrorResolver.resolveError(ro.sync.ecss.extensions.api.AuthorAccess)](ReferenceErrorResolver.md#resolveError(ro.sync.ecss.extensions.api.AuthorAccess))

### resolveError

public void resolveError([ErrorResolverContextInfo](ErrorResolverContextInfo.md) contextInfo)

Offers solutions to the current reference error.
  Parameters: contextInfo - The current error context information.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
