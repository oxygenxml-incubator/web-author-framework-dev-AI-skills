Package [ro.sync.ecss.extensions.commons.operations](package-summary.md)

# Class InsertListOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.operations.InsertListOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   Direct Known Subclasses: [DITAInsertListOperation](../../dita/DITAInsertListOperation.md), [DocbookInsertListOperation](../../docbook/DocbookInsertListOperation.md), [TEIInsertListOperation](../../tei/TEIInsertListOperation.md), [XHTMLInsertListOperation](../../xhtml/XHTMLInsertListOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class InsertListOperation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorOperation](../../api/AuthorOperation.md)
Operation used to convert a selection to an ordered/unordered list.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [AuthorAccess](../../api/AuthorAccess.md) [authorAccess](#authorAccess)
The author access.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CONVERT_ELEMENT_AT_CARET_ARGUMENT](#CONVERT_ELEMENT_AT_CARET_ARGUMENT)
Argument that controls whether the action inserts a new list or converts the element at caret if no selection is made.
  protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) [CONVERT_ELEMENT_AT_CARET_ARGUMENT_DESCRIPTOR](#CONVERT_ELEMENT_AT_CARET_ARGUMENT_DESCRIPTOR)
Schema aware argument.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LIST_TYPE_ARGUMENT](#LIST_TYPE_ARGUMENT)
Argument that controls the type of the list that will be inserted.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [listType](#listType)
The new list type.
  protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
Schema aware argument.

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT)
## Constructor Summary
 Constructors
Constructor

Description
 [InsertListOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)
Perform the actual operation.
  protected abstract [CommonsOperationsUtil.ConversionElementHelper](CommonsOperationsUtil.ConversionElementHelper.md) [getConversionElementsChecker](#getConversionElementsChecker())()
Get the conversion element checker.
  [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[AuthorNode](../../api/node/AuthorNode.md)> [getElementAtCaretToConvert](#getElementAtCaretToConvert(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.commons.operations.CommonsOperationsUtil.ConversionElementHelper))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [CommonsOperationsUtil.ConversionElementHelper](CommonsOperationsUtil.ConversionElementHelper.md) helper)
Returns the element at caret that is suitable to be converted.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getListTypeDescription](#getListTypeDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType)
Obtain the name of every list type.
  protected abstract [StringBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/StringBuilder.html) [getListXMLFragment](#getListXMLFragment(java.lang.String,java.util.Map,int,ro.sync.ecss.extensions.api.AuthorAccess))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> listAttributes, int numberOfListItems, [AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Get list XML fragment.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNamespace](#getNamespace())()
Get namespace.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getParentListType](#getParentListType(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
Get the type of the list in which the new list will be inserted.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXMLFragment](#getXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentListType)
Get XML fragment to be inserted when nothing is selected.
  protected abstract void [insertContent](#insertContent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,java.util.List))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorNode](../../api/node/AuthorNode.md) listNode, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CommonsOperationsUtil.SelectedFragmentInfo](CommonsOperationsUtil.SelectedFragmentInfo.md)> selectedFragmentsInfos)
Insert content.
  protected abstract boolean [isList](#isList(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
Checks if the given node is a list.
  protected boolean [isListElement](#isListElement(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
Checks if the given node is a list element or list item.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [getArguments](../../api/AuthorOperation.md#getArguments())
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../api/Extension.md)
 [getDescription](../../api/Extension.md#getDescription())
## Field Details

### SCHEMA_AWARE_ARGUMENT_DESCRIPTOR

protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) SCHEMA_AWARE_ARGUMENT_DESCRIPTOR

Schema aware argument.

### CONVERT_ELEMENT_AT_CARET_ARGUMENT

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CONVERT_ELEMENT_AT_CARET_ARGUMENT

Argument that controls whether the action inserts a new list or converts the element at caret if no selection is made.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.InsertListOperation.CONVERT_ELEMENT_AT_CARET_ARGUMENT)

### CONVERT_ELEMENT_AT_CARET_ARGUMENT_DESCRIPTOR

protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) CONVERT_ELEMENT_AT_CARET_ARGUMENT_DESCRIPTOR

Schema aware argument.

### LIST_TYPE_ARGUMENT

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LIST_TYPE_ARGUMENT

Argument that controls the type of the list that will be inserted.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.InsertListOperation.LIST_TYPE_ARGUMENT)

### authorAccess

protected [AuthorAccess](../../api/AuthorAccess.md) authorAccess

The author access.

### listType

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType

The new list type.

## Constructor Details

### InsertListOperation

public InsertListOperation()

## Method Details

### doOperation

public void doOperation([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation. You can check if the operation was invoked from the oXygen standalone application or from the oXygen plugin for Eclipse by using the method: [ApplicationInformationAccess.getPlatform()](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()). To get to the [Workspace](../../../../exml/workspace/api/Workspace.md) you may use: [AuthorAccess.getWorkspaceAccess()](../../api/AuthorAccess.md#getWorkspaceAccess()).
  Specified by: [doOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in interface [AuthorOperation](../../api/AuthorOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AuthorOperation.doOperation(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### getElementAtCaretToConvert

public [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[AuthorNode](../../api/node/AuthorNode.md)> getElementAtCaretToConvert([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [CommonsOperationsUtil.ConversionElementHelper](CommonsOperationsUtil.ConversionElementHelper.md) helper)

Returns the element at caret that is suitable to be converted.
  Parameters: authorAccess - The author access. helper - Used to check if the elements from selection can be converted in other elements (table cells or list entries) Returns: The element to convert.
### isListElement

protected boolean isListElement([AuthorNode](../../api/node/AuthorNode.md) node)

Checks if the given node is a list element or list item.
  Parameters: node - The element to check. Returns: true if the node is a list element.
### isList

protected abstract boolean isList([AuthorNode](../../api/node/AuthorNode.md) node)

Checks if the given node is a list.
  Parameters: node - The element to check. Returns: true if the node is a list.
### getParentListType

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getParentListType([AuthorNode](../../api/node/AuthorNode.md) node)

Get the type of the list in which the new list will be inserted. Can be null.
  Parameters: node - The node at offset. Returns: the type of the list in which the new list will be inserted. Can be null.
### getConversionElementsChecker

protected abstract [CommonsOperationsUtil.ConversionElementHelper](CommonsOperationsUtil.ConversionElementHelper.md) getConversionElementsChecker()

Get the conversion element checker.
  Returns: The conversion element checker.
### insertContent

protected abstract void insertContent([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorNode](../../api/node/AuthorNode.md) listNode, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CommonsOperationsUtil.SelectedFragmentInfo](CommonsOperationsUtil.SelectedFragmentInfo.md)> selectedFragmentsInfos)

Insert content.
  Parameters: authorAccess - The author access. listNode - The list node. selectedFragmentsInfos - The fragments to be inserted.
### getNamespace

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNamespace()

Get namespace.
  Returns: The namespace to be used at insertion.
### getXMLFragment

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXMLFragment([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentListType)

Get XML fragment to be inserted when nothing is selected.
  Parameters: authorAccess - The author access. listType - The type of the list to be inserted. parentListType - The type of the parent list, can be null Returns: the fragment to be inserted.
### getListXMLFragment

protected abstract [StringBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/StringBuilder.html) getListXMLFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> listAttributes, int numberOfListItems, [AuthorAccess](../../api/AuthorAccess.md) authorAccess)

Get list XML fragment.
  Parameters: listType - The list type. listAttributes - The attributes to add to list items. numberOfListItems - The number of list items. authorAccess - The author access. Returns: The list XML fragment.
### getListTypeDescription

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getListTypeDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType)

Obtain the name of every list type.
  Parameters: listType - The list type. Returns: A string representing the name of the given list type.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
