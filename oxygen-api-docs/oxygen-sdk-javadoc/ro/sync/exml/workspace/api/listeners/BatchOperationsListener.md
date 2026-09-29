Package [ro.sync.exml.workspace.api.listeners](package-summary.md)

# Class BatchOperationsListener

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.listeners.BatchOperationsListener
   @API(type=EXTENDABLE, src=PUBLIC) public class BatchOperationsListener extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Listener which can be notified before and after a batch operation which will modify lots of resources (Replace All in Files, Rename in Files) is started. For example a CMS may automatically check out resources if Oxygen wants to modify them during such operations.
  Since: 18.1
## Constructor Summary
 Constructors
Constructor

Description
 [BatchOperationsListener](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [aboutToModifyResource](#aboutToModifyResource(ro.sync.exml.workspace.api.listeners.BatchOperationInfo,java.net.URL))([BatchOperationInfo](BatchOperationInfo.md) batchOperationInfo, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
A resource is about to be modified.
  void [operationAboutToStart](#operationAboutToStart(ro.sync.exml.workspace.api.listeners.BatchOperationInfo))([BatchOperationInfo](BatchOperationInfo.md) batchOperationInfo)
About to start a batch operation.
  void [operationFinished](#operationFinished(ro.sync.exml.workspace.api.listeners.BatchOperationInfo))([BatchOperationInfo](BatchOperationInfo.md) batchOperationInfo)
The batch operation finished.
  void [resourceModified](#resourceModified(ro.sync.exml.workspace.api.listeners.BatchOperationInfo,java.net.URL))([BatchOperationInfo](BatchOperationInfo.md) batchOperationInfo, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
A resource was modified.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### BatchOperationsListener

public BatchOperationsListener()

## Method Details

### operationAboutToStart

public void operationAboutToStart([BatchOperationInfo](BatchOperationInfo.md) batchOperationInfo)

About to start a batch operation.
  Parameters: batchOperationInfo - Information about the operation that will start.
### operationFinished

public void operationFinished([BatchOperationInfo](BatchOperationInfo.md) batchOperationInfo)

The batch operation finished.
  Parameters: batchOperationInfo - Information about the operation that was finished.
### aboutToModifyResource

public void aboutToModifyResource([BatchOperationInfo](BatchOperationInfo.md) batchOperationInfo, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

A resource is about to be modified. This is called after the content from the URL has been read and before it is saved back.
  Parameters: batchOperationInfo - Information about the current operation. url - The URL of the resource which will be modified.
### resourceModified

public void resourceModified([BatchOperationInfo](BatchOperationInfo.md) batchOperationInfo, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

A resource was modified.
  Parameters: batchOperationInfo - Information about the current operation. url - The URL of the resource which was modified.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
