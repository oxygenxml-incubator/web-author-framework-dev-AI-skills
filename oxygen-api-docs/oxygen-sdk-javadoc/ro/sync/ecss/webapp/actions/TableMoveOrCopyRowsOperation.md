Package [ro.sync.ecss.webapp.actions](package-summary.md)

# Class TableMoveOrCopyRowsOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.webapp.AuthorOperationWithResult](../../extensions/api/webapp/AuthorOperationWithResult.md)
        * ro.sync.ecss.webapp.actions.TableMoveOrCopyRowsOperation
   All Implemented Interfaces: [Extension](../../extensions/api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class TableMoveOrCopyRowsOperation extends [AuthorOperationWithResult](../../extensions/api/webapp/AuthorOperationWithResult.md)
Operation that can be used to move table rows.

## Constructor Summary
 Constructors
Constructor

Description
 [TableMoveOrCopyRowsOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [doOperation](#doOperation(ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorDocumentModel](../../extensions/api/webapp/AuthorDocumentModel.md) model, [ArgumentsMap](../../extensions/api/ArgumentsMap.md) args)
Performs the actual operation and return a result to be sent to the client-side code.

### Methods inherited from class ro.sync.ecss.extensions.api.webapp.[AuthorOperationWithResult](../../extensions/api/webapp/AuthorOperationWithResult.md)
 [getDescription](../../extensions/api/webapp/AuthorOperationWithResult.md#getDescription())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TableMoveOrCopyRowsOperation

public TableMoveOrCopyRowsOperation()

## Method Details

### doOperation

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doOperation([AuthorDocumentModel](../../extensions/api/webapp/AuthorDocumentModel.md) model, [ArgumentsMap](../../extensions/api/ArgumentsMap.md) args)throws [AuthorOperationException](../../extensions/api/AuthorOperationException.md)
 Description copied from class: [AuthorOperationWithResult](../../extensions/api/webapp/AuthorOperationWithResult.md#doOperation(ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel,ro.sync.ecss.extensions.api.ArgumentsMap))
Performs the actual operation and return a result to be sent to the client-side code.
  Specified by: [doOperation](../../extensions/api/webapp/AuthorOperationWithResult.md#doOperation(ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [AuthorOperationWithResult](../../extensions/api/webapp/AuthorOperationWithResult.md) Parameters: model - The web author document model. args - The map of arguments. The argument names are the names passed by the calling JS code. Returns: The result of the operation that will be passed to the client-side code. Throws: [AuthorOperationException](../../extensions/api/AuthorOperationException.md) - Thrown when the operation fails.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
