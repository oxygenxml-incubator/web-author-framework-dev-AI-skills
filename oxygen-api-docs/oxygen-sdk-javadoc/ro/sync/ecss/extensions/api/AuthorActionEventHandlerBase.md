Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorActionEventHandlerBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorActionEventHandlerBase
   All Implemented Interfaces: [AuthorActionEventHandler](AuthorActionEventHandler.md), [Extension](Extension.md)   Direct Known Subclasses: [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorActionEventHandlerBase extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorActionEventHandler](AuthorActionEventHandler.md)
Adds various API methods, for example it adds a method which intercepts action events in the Author mode and can handle them in a special manner.
  Since: 19
## Nested Class Summary

## Nested classes/interfaces inherited from interface ro.sync.ecss.extensions.api.[AuthorActionEventHandler](AuthorActionEventHandler.md)
 [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md)
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorActionEventHandlerBase](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[IAuthorExtensionAction](editor/IAuthorExtensionAction.md)> [getContentCompletionActions](#getContentCompletionActions(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](AuthorAccess.md) authorAccess, int caretOffset)
Provides a list of actions that will be contributed in the content completion lists.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorActionEventHandler](AuthorActionEventHandler.md)
 [canHandleEvent](AuthorActionEventHandler.md#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventDetails)), [canHandleEvent](AuthorActionEventHandler.md#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType)), [getListItemAncestorToSplit](AuthorActionEventHandler.md#getListItemAncestorToSplit(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess)), [handleEvent](AuthorActionEventHandler.md#handleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Constructor Details

### AuthorActionEventHandlerBase

public AuthorActionEventHandlerBase()

## Method Details

### getContentCompletionActions

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[IAuthorExtensionAction](editor/IAuthorExtensionAction.md)> getContentCompletionActions([AuthorAccess](AuthorAccess.md) authorAccess, int caretOffset)

Provides a list of actions that will be contributed in the content completion lists.
  Parameters: authorAccess - Access to the Author API. caretOffset - The caret offset. Returns: A list of actions that will be contributed in the content completion lists. Can be null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
