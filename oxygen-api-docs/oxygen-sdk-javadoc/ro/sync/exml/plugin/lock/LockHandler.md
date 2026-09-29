Package [ro.sync.exml.plugin.lock](package-summary.md)

# Interface LockHandler
    All Known Implementing Classes: [LockHandlerBase](LockHandlerBase.md), [LockHandlerWithContext](../../../ecss/extensions/api/webapp/plugin/LockHandlerWithContext.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface LockHandler
Manage locking and unlocking.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [unlock](#unlock(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource)
Unlock a specific resource
  void [updateLock](#updateLock(java.net.URL,int))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource, int timeoutSeconds)
Lock a specific resource if it has never been locked before or refresh the lock.

## Method Details

### unlock

void unlock([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource)throws [LockException](LockException.md)

Unlock a specific resource
  Parameters: resource - The URL to unlock Throws: [LockException](LockException.md) - When could not unlock properly.
### updateLock

void updateLock([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource, int timeoutSeconds)throws [LockException](LockException.md)

Lock a specific resource if it has never been locked before or refresh the lock. This will get called at the beginning to lock the resource and after that periodically.
  Parameters: resource - The URL to lock. timeoutSeconds - The timeout in seconds to set for the lock (so that the lock expires after the timeout passes). The refresh on the lock is called about every (timeout/2) seconds. Throws: [LockException](LockException.md) - When could not lock properly.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
