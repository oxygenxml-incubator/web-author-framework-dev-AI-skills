Package [ro.sync.ecss.extensions](package-summary.md)

# Interface ExecuteMultipleActionsWithExtraAskValuesOperation
    All Superinterfaces: [AuthorOperation](api/AuthorOperation.md), [Extension](api/Extension.md)   All Known Implementing Classes: [ExecuteMultipleWebappCompatibleActionsOperation](commons/operations/ExecuteMultipleWebappCompatibleActionsOperation.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface ExecuteMultipleActionsWithExtraAskValuesOperationextends [AuthorOperation](api/AuthorOperation.md)
Interface defining an author extension operation taht executes multiple actions and receive a list with expanded ask variables values, when invoked

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap,java.util.List))([AuthorAccess](api/AuthorAccess.md) authorAccess, [ArgumentsMap](api/ArgumentsMap.md) args, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> asksValues)
Do the operation taking into account the provided asks variables values.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> [getActions](#getActions(ro.sync.ecss.extensions.api.AuthorAccess,java.util.Map))([AuthorAccess](api/AuthorAccess.md) authorAccess, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html) arguments)
Get all the actions from this operation.

### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](api/AuthorOperation.md)
 [doOperation](api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](api/AuthorOperation.md#getArguments())
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](api/Extension.md)
 [getDescription](api/Extension.md#getDescription())
## Method Details

### doOperation

void doOperation([AuthorAccess](api/AuthorAccess.md) authorAccess, [ArgumentsMap](api/ArgumentsMap.md) args, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> asksValues)throws [AuthorOperationException](api/AuthorOperationException.md)

Do the operation taking into account the provided asks variables values.
  Parameters: authorAccess - The Author access. args - The arguments. asksValues - The list of expanded asks variables for all inner actions. Throws: [AuthorOperationException](api/AuthorOperationException.md)
### getActions

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> getActions([AuthorAccess](api/AuthorAccess.md) authorAccess, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html) arguments)throws [AuthorOperationException](api/AuthorOperationException.md)

Get all the actions from this operation.
  Parameters: authorAccess - Author access. arguments - The arguments. Returns: The list with all actions. Throws: [AuthorOperationException](api/AuthorOperationException.md)
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
