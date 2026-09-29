Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Class AuthorOperationWithResult

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.AuthorOperationWithResult
   All Implemented Interfaces: [Extension](../Extension.md)   Direct Known Subclasses: [TableMoveOrCopyColumnOperation](../../../webapp/actions/TableMoveOrCopyColumnOperation.md), [TableMoveOrCopyRowsOperation](../../../webapp/actions/TableMoveOrCopyRowsOperation.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorOperationWithResult extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Extension](../Extension.md)
Operation that returns a result when invoked from the Web Author JS API.
  Since: 18.1
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorOperationWithResult](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [doOperation](#doOperation(ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorDocumentModel](AuthorDocumentModel.md) model, [ArgumentsMap](../ArgumentsMap.md) args)
Performs the actual operation and return a result to be sent to the client-side code.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorOperationWithResult

public AuthorOperationWithResult()

## Method Details

### doOperation

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doOperation([AuthorDocumentModel](AuthorDocumentModel.md) model, [ArgumentsMap](../ArgumentsMap.md) args)throws [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html), [AuthorOperationException](../AuthorOperationException.md)

Performs the actual operation and return a result to be sent to the client-side code.
  Parameters: model - The web author document model. args - The map of arguments. The argument names are the names passed by the calling JS code. Returns: The result of the operation that will be passed to the client-side code. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - Thrown when one or more arguments are illegal. [AuthorOperationException](../AuthorOperationException.md) - Thrown when the operation fails.
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../Extension.md#getDescription()) in interface [Extension](../Extension.md) Returns: the description of this operation.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
