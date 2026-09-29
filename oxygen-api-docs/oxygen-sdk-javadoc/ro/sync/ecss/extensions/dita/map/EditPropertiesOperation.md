Package [ro.sync.ecss.extensions.dita.map](package-summary.md)

# Class EditPropertiesOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.map.EditPropertiesOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class EditPropertiesOperation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorOperation](../../api/AuthorOperation.md)
Operation used to edit the properties of a topic reference.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [EditPropertiesOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)
Perform the actual operation.
  [ArgumentDescriptor](../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### EditPropertiesOperation

public EditPropertiesOperation()

## Method Details

### doOperation

public void doOperation([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation. You can check if the operation was invoked from the oXygen standalone application or from the oXygen plugin for Eclipse by using the method: [ApplicationInformationAccess.getPlatform()](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()). To get to the [Workspace](../../../../exml/workspace/api/Workspace.md) you may use: [AuthorAccess.getWorkspaceAccess()](../../api/AuthorAccess.md#getWorkspaceAccess()).
  Specified by: [doOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in interface [AuthorOperation](../../api/AuthorOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AuthorOperation.doOperation(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### getArguments

public [ArgumentDescriptor](../../api/ArgumentDescriptor.md)[] getArguments()
  Specified by: [getArguments](../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../api/AuthorOperation.md) Returns: An array of [ArgumentDescriptor](../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../api/AuthorOperation.md#getArguments())

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../api/Extension.md#getDescription()) in interface [Extension](../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
