Package [ro.sync.ecss.extensions.api.webapp.plugin](package-summary.md)

# Class LockHandlerWithContext

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.plugin.lock.LockHandlerBase](../../../../../exml/plugin/lock/LockHandlerBase.md)
        * ro.sync.ecss.extensions.api.webapp.plugin.LockHandlerWithContext
   All Implemented Interfaces: [LockHandler](../../../../../exml/plugin/lock/LockHandler.md)   @API(src=PRIVATE, type=EXTENDABLE) public abstract class LockHandlerWithContext extends [LockHandlerBase](../../../../../exml/plugin/lock/LockHandlerBase.md)
A base-class to be extended to implement lock/unlock functionality.

This class should be used with URLs, for whose protocol the [URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html) implements [URLStreamHandlerWithContext](URLStreamHandlerWithContext.md). It is this implementation which decides what contextId means.

It is intended to be used in Oxygen XML Web Author. It provides similar functionality to [LockHandlerBase](../../../../../exml/plugin/lock/LockHandlerBase.md), but is designed to work in a multi-user setting. Every method receives an extra parameter that identifies the user on behalf of which the resource should be locked. To make Web Author use this class, one should register a [LockHandlerFactoryPluginExtension](../../../../../exml/plugin/urlstreamhandler/LockHandlerFactoryPluginExtension.md).
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [LockHandlerWithContext](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract boolean [isSaveAllowed](#isSaveAllowed(java.lang.String,java.net.URL,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, int timeoutSeconds)
Checks if save is allowed for a resource identified by its URL.
  final boolean [isSaveAllowed](#isSaveAllowed(java.net.URL,int))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, int timeoutSeconds)
Checks if save is allowed for a resource identified by its URL.
  abstract void [unlock](#unlock(java.lang.String,java.net.URL))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource)
Unlock a specific resource
  final void [unlock](#unlock(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource)
Unlock a specific resource
  abstract void [updateLock](#updateLock(java.lang.String,java.net.URL,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource, int timeoutSeconds)
Lock a specific resource if it has never been locked before or refresh the lock.
  final void [updateLock](#updateLock(java.net.URL,int))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource, int timeoutSeconds)
Lock a specific resource if it has never been locked before or refresh the lock.

### Methods inherited from class ro.sync.exml.plugin.lock.[LockHandlerBase](../../../../../exml/plugin/lock/LockHandlerBase.md)
 [isLockEnabled](../../../../../exml/plugin/lock/LockHandlerBase.md#isLockEnabled())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### LockHandlerWithContext

public LockHandlerWithContext()

## Method Details

### isSaveAllowed

public final boolean isSaveAllowed([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, int timeoutSeconds)

Checks if save is allowed for a resource identified by its URL. **This method is used only by the Oxygen XML Editor, not by the Web Author editor.**
  Specified by: [isSaveAllowed](../../../../../exml/plugin/lock/LockHandlerBase.md#isSaveAllowed(java.net.URL,int)) in class [LockHandlerBase](../../../../../exml/plugin/lock/LockHandlerBase.md) Parameters: url - The URL for which the check is performed. timeoutSeconds - The timeout in seconds to set for the lock . Returns: true if saving is allowed.
### isSaveAllowed

public abstract boolean isSaveAllowed([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, int timeoutSeconds)

Checks if save is allowed for a resource identified by its URL. **This method is used only by the Oxygen XML Editor, not by the Web Author editor.**
  Parameters: contextId - The ID of the user context, as defined by the [URLStreamHandlerWithContext](URLStreamHandlerWithContext.md) implementation for the URL's protocol. url - The URL for which the check is performed. timeoutSeconds - The timeout in seconds to set for the lock . Returns: true if saving is allowed.
### unlock

public final void unlock([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource)throws [LockException](../../../../../exml/plugin/lock/LockException.md)

Unlock a specific resource
  Parameters: resource - The URL to unlock Throws: [LockException](../../../../../exml/plugin/lock/LockException.md) - When could not unlock properly.
### unlock

public abstract void unlock([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource)throws [LockException](../../../../../exml/plugin/lock/LockException.md)

Unlock a specific resource
  Parameters: contextId - The ID of the user context, as defined by the [URLStreamHandlerWithContext](URLStreamHandlerWithContext.md) implementation for the URL's protocol. resource - The URL to unlock Throws: [LockException](../../../../../exml/plugin/lock/LockException.md) - When could not unlock properly.
### updateLock

public final void updateLock([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource, int timeoutSeconds)throws [LockException](../../../../../exml/plugin/lock/LockException.md)

Lock a specific resource if it has never been locked before or refresh the lock. This will get called at the beginning to lock the resource and after that periodically.
  Parameters: resource - The URL to lock. timeoutSeconds - The timeout in seconds to set for the lock (so that the lock expires after the timeout passes). The refresh on the lock is called about every (timeout/2) seconds. Throws: [LockException](../../../../../exml/plugin/lock/LockException.md) - When could not lock properly.
### updateLock

public abstract void updateLock([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource, int timeoutSeconds)throws [LockException](../../../../../exml/plugin/lock/LockException.md)

Lock a specific resource if it has never been locked before or refresh the lock. This will get called at the beginning to lock the resource and after that periodically.
  Parameters: contextId - The ID of the user context, as defined by the [URLStreamHandlerWithContext](URLStreamHandlerWithContext.md) implementation for the URL's protocol. resource - The URL to lock. timeoutSeconds - The timeout in seconds to set for the lock (so that the lock expires after the timeout passes). The refresh on the lock is called about every (timeout/2) seconds. Throws: [LockException](../../../../../exml/plugin/lock/LockException.md) - When could not lock properly.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
