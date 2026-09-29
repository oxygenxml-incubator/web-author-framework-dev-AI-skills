Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Class WebappLockManager

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.WebappLockManager
   @API(src=PRIVATE, type=NOT_EXTENDABLE) public abstract class WebappLockManager extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The lock manager associated with a document.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LOCKED_BY_SOMEONE_ELSE_REASON_CODE](#LOCKED_BY_SOMEONE_ELSE_REASON_CODE)
Reason code for the editor being read-only because is locked by someone else.

## Constructor Summary
 Constructors
Constructor

Description
 [WebappLockManager](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract boolean [isEnabled](#isEnabled())()

 abstract void [unlock](#unlock())()
Releases lock associated with the corresponding document.
  abstract void [updateLock](#updateLock())()
Updates the lock associated with the corresponding document.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### LOCKED_BY_SOMEONE_ELSE_REASON_CODE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LOCKED_BY_SOMEONE_ELSE_REASON_CODE

Reason code for the editor being read-only because is locked by someone else.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.WebappLockManager.LOCKED_BY_SOMEONE_ELSE_REASON_CODE)

## Constructor Details

### WebappLockManager

public WebappLockManager()

## Method Details

### updateLock

public abstract void updateLock() throws [LockException](../../../../exml/plugin/lock/LockException.md)

Updates the lock associated with the corresponding document.
  Throws: [LockException](../../../../exml/plugin/lock/LockException.md) - An exception thrown if the lock could not be updated.
### unlock

public abstract void unlock()

Releases lock associated with the corresponding document.

### isEnabled

public abstract boolean isEnabled()
  Returns: true if locking is enabled for the current document.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
