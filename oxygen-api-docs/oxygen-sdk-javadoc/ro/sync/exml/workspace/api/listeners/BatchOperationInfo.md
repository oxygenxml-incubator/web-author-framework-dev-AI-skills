Package [ro.sync.exml.workspace.api.listeners](package-summary.md)

# Class BatchOperationInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.listeners.BatchOperationInfo
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class BatchOperationInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The type of batch operation.
  Since: 18.1
## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static enum  [BatchOperationInfo.Type](BatchOperationInfo.Type.md)
The type of the batch operation.

## Constructor Summary
 Constructors
Constructor

Description
 [BatchOperationInfo](#%3Cinit%3E(ro.sync.exml.workspace.api.listeners.BatchOperationInfo.Type))([BatchOperationInfo.Type](BatchOperationInfo.Type.md) type)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [BatchOperationInfo.Type](BatchOperationInfo.Type.md) [getType](#getType())()
Get the batch operation type.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### BatchOperationInfo

public BatchOperationInfo([BatchOperationInfo.Type](BatchOperationInfo.Type.md) type)

Constructor.
  Parameters: type - The operation type.
## Method Details

### getType

public [BatchOperationInfo.Type](BatchOperationInfo.Type.md) getType()

Get the batch operation type.
  Returns: Returns the batch operation type.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
