Package [ro.sync.net.protocol.http](package-summary.md)

# Class WebdavLockHelper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.net.protocol.http.WebdavLockHelper
   @API(src=PRIVATE, type=NOT_EXTENDABLE) public class WebdavLockHelper extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Helper class that allows one to implement locking for a WebDAV server in a multi-user scenario.

## Constructor Summary
 Constructors
Constructor

Description
 [WebdavLockHelper](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addLockHeader](#addLockHeader(java.lang.String,java.net.HttpURLConnection))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [HttpURLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/HttpURLConnection.html) conn)
Adds the lock header so that we can perform write operations on a resource that we locked ourselves.
  long [getServerPreferredTimeout](#getServerPreferredTimeout())()

 boolean [isLockEnabled](#isLockEnabled())()
Checks if locking is enabled.
  boolean [isSaveAllowed](#isSaveAllowed(java.lang.String,java.net.URL,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, int timeoutSeconds)
Checks if save is allowed for a resource identified by its URL.
  void [setLockOwner](#setLockOwner(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lockOwnerName)
Sets the lock owner for the specified session Id.
  void [unlock](#unlock(java.lang.String,java.net.URL))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource)
Unlock a given resource.
  void [unlock](#unlock(java.lang.String,java.net.URL,java.util.List,java.util.List))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> headerKeys, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> headerValues)
Unlock a given resource.
  void [updateLock](#updateLock(java.lang.String,java.net.URL,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource, int lockTimeoutSeconds)
Lock a given resource.
  void [updateLock](#updateLock(java.lang.String,java.net.URL,int,java.util.List,java.util.List))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource, int lockTimeoutSeconds, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> headerKeys, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> headerValues)
Lock a given resource.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WebdavLockHelper

public WebdavLockHelper()

Constructor.

## Method Details

### updateLock

public void updateLock([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource, int lockTimeoutSeconds)throws [LockException](../../../exml/plugin/lock/LockException.md)

Lock a given resource.
  Parameters: sessionId - The session ID. resource - The resource to lock lockTimeoutSeconds - The timeout in seconds. Throws: [LockException](../../../exml/plugin/lock/LockException.md)
### updateLock

public void updateLock([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource, int lockTimeoutSeconds, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> headerKeys, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> headerValues)throws [LockException](../../../exml/plugin/lock/LockException.md)

Lock a given resource.
  Parameters: sessionId - The session ID. resource - The resource to lock lockTimeoutSeconds - The timeout in seconds. headerKeys - The header keys. headerValues - The header values. Throws: [LockException](../../../exml/plugin/lock/LockException.md)
### setLockOwner

public void setLockOwner([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lockOwnerName)

Sets the lock owner for the specified session Id.
  Parameters: sessionId - The session Id. lockOwnerName - The lock owner.
### unlock

public void unlock([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource)throws [LockException](../../../exml/plugin/lock/LockException.md)

Unlock a given resource.
  Parameters: sessionId - The session Id. resource - The resource to unlock Throws: [LockException](../../../exml/plugin/lock/LockException.md)
### unlock

public void unlock([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> headerKeys, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> headerValues)throws [LockException](../../../exml/plugin/lock/LockException.md)

Unlock a given resource.
  Parameters: sessionId - The session Id. resource - The resource to unlock headerKeys - the header keys. headerValues - the header values. Throws: [LockException](../../../exml/plugin/lock/LockException.md)
### isLockEnabled

public boolean isLockEnabled()

Checks if locking is enabled.
  Returns: true if locking is enabled
### getServerPreferredTimeout

public long getServerPreferredTimeout()
  Returns: The server preferred timeout.
### isSaveAllowed

public boolean isSaveAllowed([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, int timeoutSeconds)

Checks if save is allowed for a resource identified by its URL.
  Parameters: sessionId - The session ID. url - The URL for which the check is performed. timeoutSeconds - The timeout in seconds to set for the lock . Returns: true if saving is allowed.
### addLockHeader

public void addLockHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [HttpURLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/HttpURLConnection.html) conn)

Adds the lock header so that we can perform write operations on a resource that we locked ourselves.
  Parameters: sessionId - The session ID. conn - The connection to enrich with the lock header.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
