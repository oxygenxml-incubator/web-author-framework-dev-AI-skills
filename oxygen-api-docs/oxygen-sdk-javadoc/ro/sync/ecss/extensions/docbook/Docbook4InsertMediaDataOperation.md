Package [ro.sync.ecss.extensions.docbook](package-summary.md)

# Class Docbook4InsertMediaDataOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.docbook.InsertMediaDataOperationBase](InsertMediaDataOperationBase.md)
        * ro.sync.ecss.extensions.docbook.Docbook4InsertMediaDataOperation
   All Implemented Interfaces: [AuthorOperation](../api/AuthorOperation.md), [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class Docbook4InsertMediaDataOperation extends [InsertMediaDataOperationBase](InsertMediaDataOperationBase.md)
Operation used to insert an media object in DocBook 4 documents.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.docbook.[InsertMediaDataOperationBase](InsertMediaDataOperationBase.md)
 [ARGUMENT_MEDIA_URL](InsertMediaDataOperationBase.md#ARGUMENT_MEDIA_URL)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [Docbook4InsertMediaDataOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [insertNamespace](#insertNamespace())()
Method to insert name space for docbook 4 and 5.

### Methods inherited from class ro.sync.ecss.extensions.docbook.[InsertMediaDataOperationBase](InsertMediaDataOperationBase.md)
 [doOperation](InsertMediaDataOperationBase.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](InsertMediaDataOperationBase.md#getArguments()), [getDescription](InsertMediaDataOperationBase.md#getDescription()), [insertMediaRef](InsertMediaDataOperationBase.md#insertMediaRef(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### Docbook4InsertMediaDataOperation

public Docbook4InsertMediaDataOperation()

## Method Details

### insertNamespace

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertNamespace()
 Description copied from class: [InsertMediaDataOperationBase](InsertMediaDataOperationBase.md#insertNamespace())
Method to insert name space for docbook 4 and 5.
  Specified by: [insertNamespace](InsertMediaDataOperationBase.md#insertNamespace()) in class [InsertMediaDataOperationBase](InsertMediaDataOperationBase.md) See Also:
        * [InsertMediaDataOperationBase.insertNamespace()](InsertMediaDataOperationBase.md#insertNamespace())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
