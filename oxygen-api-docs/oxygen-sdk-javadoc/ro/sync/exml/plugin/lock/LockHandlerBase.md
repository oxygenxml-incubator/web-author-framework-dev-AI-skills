Package [ro.sync.exml.plugin.lock](package-summary.md)

# Class LockHandlerBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.plugin.lock.LockHandlerBase
   All Implemented Interfaces: [LockHandler](LockHandler.md)   Direct Known Subclasses: [LockHandlerWithContext](../../../ecss/extensions/api/webapp/plugin/LockHandlerWithContext.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class LockHandlerBase extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [LockHandler](LockHandler.md)
Base for classes used for managing locking and unlocking.
  Since: 17
## Constructor Summary
 Constructors
Constructor

Description
 [LockHandlerBase](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract boolean [isLockEnabled](#isLockEnabled())()
Checks if locking is enabled.
  abstract boolean [isSaveAllowed](#isSaveAllowed(java.net.URL,int))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, int timeoutSeconds)
Checks if save is allowed for a resource identified by its URL.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.exml.plugin.lock.[LockHandler](LockHandler.md)
 [unlock](LockHandler.md#unlock(java.net.URL)), [updateLock](LockHandler.md#updateLock(java.net.URL,int))
## Constructor Details

### LockHandlerBase

public LockHandlerBase()

## Method Details

### isLockEnabled

public abstract boolean isLockEnabled()

Checks if locking is enabled.
  Returns: true if locking is enabled
### isSaveAllowed

public abstract boolean isSaveAllowed([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, int timeoutSeconds)

Checks if save is allowed for a resource identified by its URL.
  Parameters: url - The URL for which the check is performed. timeoutSeconds - The timeout in seconds to set for the lock . Returns: true if saving is allowed.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
