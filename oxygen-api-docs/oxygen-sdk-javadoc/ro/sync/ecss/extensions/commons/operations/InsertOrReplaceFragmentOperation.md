Package [ro.sync.ecss.extensions.commons.operations](package-summary.md)

# Class InsertOrReplaceFragmentOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.operations.InsertFragmentOperation](InsertFragmentOperation.md)
        * ro.sync.ecss.extensions.commons.operations.InsertOrReplaceFragmentOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertOrReplaceFragmentOperation extends [InsertFragmentOperation](InsertFragmentOperation.md)
Identical with [InsertFragmentOperation](InsertFragmentOperation.md) with the difference that the selection will be removed.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.operations.[InsertFragmentOperation](InsertFragmentOperation.md)
 [ARGUMENT_DESCR_INSERT_FRAG_EVEN_IF_INVALID](InsertFragmentOperation.md#ARGUMENT_DESCR_INSERT_FRAG_EVEN_IF_INVALID), [ARGUMENT_DESCRIPTOR_FRAGMENT](InsertFragmentOperation.md#ARGUMENT_DESCRIPTOR_FRAGMENT), [ARGUMENT_DESCRIPTOR_GO_TO_NEXT_EDITABLE_POSITION](InsertFragmentOperation.md#ARGUMENT_DESCRIPTOR_GO_TO_NEXT_EDITABLE_POSITION), [ARGUMENT_DESCRIPTOR_XPATH_LOCATION](InsertFragmentOperation.md#ARGUMENT_DESCRIPTOR_XPATH_LOCATION), [ARGUMENT_FRAGMENT](InsertFragmentOperation.md#ARGUMENT_FRAGMENT), [ARGUMENT_GO_TO_NEXT_EDITABLE_POSITION](InsertFragmentOperation.md#ARGUMENT_GO_TO_NEXT_EDITABLE_POSITION), [ARGUMENT_INSERT_FRAG_EVEN_IF_INVALID](InsertFragmentOperation.md#ARGUMENT_INSERT_FRAG_EVEN_IF_INVALID), [ARGUMENT_RELATIVE_LOCATION](InsertFragmentOperation.md#ARGUMENT_RELATIVE_LOCATION), [ARGUMENT_XPATH_LOCATION](InsertFragmentOperation.md#ARGUMENT_XPATH_LOCATION)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [InsertOrReplaceFragmentOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)
Perform the actual operation.
  [ArgumentDescriptor](../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

### Methods inherited from class ro.sync.ecss.extensions.commons.operations.[InsertFragmentOperation](InsertFragmentOperation.md)
 [doOperationInternal](InsertFragmentOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.Object,java.lang.Object,java.lang.Object,boolean,java.lang.Object)), [doOperationInternal](InsertFragmentOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.Object,java.lang.Object,java.lang.Object,boolean,java.lang.Object,boolean))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### InsertOrReplaceFragmentOperation

public InsertOrReplaceFragmentOperation()

## Method Details

### doOperation

public void doOperation([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation. You can check if the operation was invoked from the oXygen standalone application or from the oXygen plugin for Eclipse by using the method: [ApplicationInformationAccess.getPlatform()](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()). To get to the [Workspace](../../../../exml/workspace/api/Workspace.md) you may use: [AuthorAccess.getWorkspaceAccess()](../../api/AuthorAccess.md#getWorkspaceAccess()).
  Specified by: [doOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in interface [AuthorOperation](../../api/AuthorOperation.md) Overrides: [doOperation](InsertFragmentOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [InsertFragmentOperation](InsertFragmentOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AuthorOperation.doOperation(AuthorAccess, ArgumentsMap)](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../api/Extension.md#getDescription()) in interface [Extension](../../api/Extension.md) Overrides: [getDescription](InsertFragmentOperation.md#getDescription()) in class [InsertFragmentOperation](InsertFragmentOperation.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

### getArguments

public [ArgumentDescriptor](../../api/ArgumentDescriptor.md)[] getArguments()
  Specified by: [getArguments](../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../api/AuthorOperation.md) Overrides: [getArguments](InsertFragmentOperation.md#getArguments()) in class [InsertFragmentOperation](InsertFragmentOperation.md) Returns: An array of [ArgumentDescriptor](../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [InsertFragmentOperation.getArguments()](InsertFragmentOperation.md#getArguments())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
