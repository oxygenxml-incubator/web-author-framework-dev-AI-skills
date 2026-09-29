Package [ro.sync.ecss.extensions.commons.operations](package-summary.md)

# Class ExecuteMultipleWebappCompatibleActionsOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.operations.ExecuteMultipleActionsOperation](ExecuteMultipleActionsOperation.md)
        * ro.sync.ecss.extensions.commons.operations.ExecuteMultipleWebappCompatibleActionsOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md), [ExecuteMultipleActionsWithExtraAskValuesOperation](../../ExecuteMultipleActionsWithExtraAskValuesOperation.md)   @API(type=INTERNAL, src=PUBLIC) public class ExecuteMultipleWebappCompatibleActionsOperation extends [ExecuteMultipleActionsOperation](ExecuteMultipleActionsOperation.md)implements [ExecuteMultipleActionsWithExtraAskValuesOperation](../../ExecuteMultipleActionsWithExtraAskValuesOperation.md)
An implementation of an operation which runs a sequence of webapp-compatible ([WebappCompatible](../../api/WebappCompatible.md)) actions, defined as a list of IDs. This class is also marked as webapp-compatible. The actions must be defined by the corresponding framework, or one of the common actions for all frameworks supplied by Oxygen.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.operations.[ExecuteMultipleActionsOperation](ExecuteMultipleActionsOperation.md)
 [ACTION_IDS](ExecuteMultipleActionsOperation.md#ACTION_IDS)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [ExecuteMultipleWebappCompatibleActionsOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap,java.util.List))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> asksValues)
Do the operation taking into account the provided asks variables values.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> [getActions](#getActions(ro.sync.ecss.extensions.api.AuthorAccess,java.util.Map))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html) args)
Get all the actions from this operation.

### Methods inherited from class ro.sync.ecss.extensions.commons.operations.[ExecuteMultipleActionsOperation](ExecuteMultipleActionsOperation.md)
 [doOperation](ExecuteMultipleActionsOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getActions](ExecuteMultipleActionsOperation.md#getActions(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.Object)), [getArguments](ExecuteMultipleActionsOperation.md#getArguments()), [getDescription](ExecuteMultipleActionsOperation.md#getDescription())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [doOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../api/AuthorOperation.md#getArguments())
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../api/Extension.md)
 [getDescription](../../api/Extension.md#getDescription())
## Constructor Details

### ExecuteMultipleWebappCompatibleActionsOperation

public ExecuteMultipleWebappCompatibleActionsOperation()

## Method Details

### doOperation

public void doOperation([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> asksValues)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Do the operation taking into account the provided asks variables values.
  Specified by: [doOperation](../../ExecuteMultipleActionsWithExtraAskValuesOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap,java.util.List)) in interface [ExecuteMultipleActionsWithExtraAskValuesOperation](../../ExecuteMultipleActionsWithExtraAskValuesOperation.md) Parameters: authorAccess - The Author access. args - The arguments. asksValues - The list of expanded asks variables for all inner actions. Throws: [AuthorOperationException](../../api/AuthorOperationException.md)
### getActions

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> getActions([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html) args)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from interface: [ExecuteMultipleActionsWithExtraAskValuesOperation](../../ExecuteMultipleActionsWithExtraAskValuesOperation.md#getActions(ro.sync.ecss.extensions.api.AuthorAccess,java.util.Map))
Get all the actions from this operation.
  Specified by: [getActions](../../ExecuteMultipleActionsWithExtraAskValuesOperation.md#getActions(ro.sync.ecss.extensions.api.AuthorAccess,java.util.Map)) in interface [ExecuteMultipleActionsWithExtraAskValuesOperation](../../ExecuteMultipleActionsWithExtraAskValuesOperation.md) Parameters: authorAccess - Author access. args - The arguments. Returns: The list with all actions. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) See Also:
        * [ExecuteMultipleActionsWithExtraAskValuesOperation.getActions(ro.sync.ecss.extensions.api.AuthorAccess, java.util.Map)](../../ExecuteMultipleActionsWithExtraAskValuesOperation.md#getActions(ro.sync.ecss.extensions.api.AuthorAccess,java.util.Map))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
