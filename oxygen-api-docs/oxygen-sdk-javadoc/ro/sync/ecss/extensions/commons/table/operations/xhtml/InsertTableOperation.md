Package [ro.sync.ecss.extensions.commons.table.operations.xhtml](package-summary.md)

# Class InsertTableOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.operations.xhtml.InsertTableOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [InsertTableOperationBase](../InsertTableOperationBase.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertTableOperation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorOperation](../../../../api/AuthorOperation.md), [InsertTableOperationBase](../InsertTableOperationBase.md)
Operation used to insert a XHTML table.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [InsertTableOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../../api/ArgumentsMap.md) args)
Perform the actual operation.
  [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()
No arguments.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 void [insertTable](#insertTable(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,boolean,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper,ro.sync.ecss.extensions.commons.table.operations.TableInfo))([AuthorDocumentFragment](../../../../api/node/AuthorDocumentFragment.md)[] fragments, boolean cellsFragments, [AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorTableHelper](../AuthorTableHelper.md) tableHelper, [TableInfo](../TableInfo.md) tableInfo)
If the fragments array is not null, this method converts the given fragments array into a table.
  void [insertTable](#insertTable(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,java.util.List,boolean,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper,ro.sync.ecss.extensions.commons.table.operations.TableInfo))([AuthorDocumentFragment](../../../../api/node/AuthorDocumentFragment.md)[] fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> rowAttributes, boolean cellsFragments, [AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorTableHelper](../AuthorTableHelper.md) tableHelper, [TableInfo](../TableInfo.md) tableInfo)
If the fragments array is not null, this method converts the given fragments array into a table.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### InsertTableOperation

public InsertTableOperation()

## Method Details

### doOperation

public void doOperation([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorOperation](../../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation. You can check if the operation was invoked from the oXygen standalone application or from the oXygen plugin for Eclipse by using the method: [ApplicationInformationAccess.getPlatform()](../../../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()). To get to the [Workspace](../../../../../../exml/workspace/api/Workspace.md) you may use: [AuthorAccess.getWorkspaceAccess()](../../../../api/AuthorAccess.md#getWorkspaceAccess()).
  Specified by: [doOperation](../../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in interface [AuthorOperation](../../../../api/AuthorOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AuthorOperation.doOperation(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### insertTable

public void insertTable([AuthorDocumentFragment](../../../../api/node/AuthorDocumentFragment.md)[] fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> rowAttributes, boolean cellsFragments, [AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorTableHelper](../AuthorTableHelper.md) tableHelper, [TableInfo](../TableInfo.md) tableInfo)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)

If the fragments array is not null, this method converts the given fragments array into a table. Each fragments will correspond to a cell. The resulting table will have one column and as many rows as fragments length. If no fragment is provided an empty table is inserted (a dialog is shown to choose all the table properties)
  Parameters: fragments - An array of AuthorDocumentFragments that are used as content of the inserted cells. rowAttributes - For each fragment this list can contain a list of corresponding attributes that can be set on the row element. cellsFragments - If the value is true then the fragments where originally cells. authorAccess - The author access. namespace - The namespace. tableHelper - The table helper. tableInfo - The details about table creation. If null, a dialog is presented to let the user choose the details. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md)
### insertTable

public void insertTable([AuthorDocumentFragment](../../../../api/node/AuthorDocumentFragment.md)[] fragments, boolean cellsFragments, [AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorTableHelper](../AuthorTableHelper.md) tableHelper, [TableInfo](../TableInfo.md) tableInfo)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from interface: [InsertTableOperationBase](../InsertTableOperationBase.md#insertTable(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,boolean,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper,ro.sync.ecss.extensions.commons.table.operations.TableInfo))
If the fragments array is not null, this method converts the given fragments array into a table. Each fragments will correspond to a cell. The resulting table will have one column and as many rows as fragments length. If no fragment is provided an empty table is inserted (a dialog is shown to choose all the table properties)
  Specified by: [insertTable](../InsertTableOperationBase.md#insertTable(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,boolean,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper,ro.sync.ecss.extensions.commons.table.operations.TableInfo)) in interface [InsertTableOperationBase](../InsertTableOperationBase.md) Parameters: fragments - An array of AuthorDocumentFragments that are used as content of the inserted cells. cellsFragments - If the value is true then the fragments where originally cells. authorAccess - The author access. namespace - The namespace. tableHelper - The table helper. tableInfo - The details about table creation. If null, a dialog is presented to let the user choose the details. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) See Also:
        * [InsertTableOperationBase.insertTable(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment[], boolean, ro.sync.ecss.extensions.api.AuthorAccess, java.lang.String, ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper, ro.sync.ecss.extensions.commons.table.operations.TableInfo)](../InsertTableOperationBase.md#insertTable(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,boolean,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper,ro.sync.ecss.extensions.commons.table.operations.TableInfo))

### getArguments

public [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md)[] getArguments()

No arguments. The operation will display a dialog for choosing the table attributes.
  Specified by: [getArguments](../../../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../../../api/AuthorOperation.md) Returns: An array of [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../../../api/AuthorOperation.md#getArguments())

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../../../api/Extension.md#getDescription()) in interface [Extension](../../../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
