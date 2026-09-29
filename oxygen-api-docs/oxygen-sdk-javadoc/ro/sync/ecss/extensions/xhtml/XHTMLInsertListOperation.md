Package [ro.sync.ecss.extensions.xhtml](package-summary.md)

# Class XHTMLInsertListOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.operations.InsertListOperation](../commons/operations/InsertListOperation.md)
        * ro.sync.ecss.extensions.xhtml.XHTMLInsertListOperation
   All Implemented Interfaces: [AuthorOperation](../api/AuthorOperation.md), [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class XHTMLInsertListOperation extends [InsertListOperation](../commons/operations/InsertListOperation.md)
Operation used to convert selected paragraphs to ordered/unordered list.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.operations.[InsertListOperation](../commons/operations/InsertListOperation.md)
 [authorAccess](../commons/operations/InsertListOperation.md#authorAccess), [CONVERT_ELEMENT_AT_CARET_ARGUMENT](../commons/operations/InsertListOperation.md#CONVERT_ELEMENT_AT_CARET_ARGUMENT), [CONVERT_ELEMENT_AT_CARET_ARGUMENT_DESCRIPTOR](../commons/operations/InsertListOperation.md#CONVERT_ELEMENT_AT_CARET_ARGUMENT_DESCRIPTOR), [LIST_TYPE_ARGUMENT](../commons/operations/InsertListOperation.md#LIST_TYPE_ARGUMENT), [listType](../commons/operations/InsertListOperation.md#listType), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../commons/operations/InsertListOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT)
## Constructor Summary
 Constructors
Constructor

Description
 [XHTMLInsertListOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [ArgumentDescriptor](../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 protected [CommonsOperationsUtil.ConversionElementHelper](../commons/operations/CommonsOperationsUtil.ConversionElementHelper.md) [getConversionElementsChecker](#getConversionElementsChecker())()
Get the conversion element checker.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getListTypeDescription](#getListTypeDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType)
Obtain the name of every list type.
  protected [StringBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/StringBuilder.html) [getListXMLFragment](#getListXMLFragment(java.lang.String,java.util.Map,int,ro.sync.ecss.extensions.api.AuthorAccess))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> attributes, int numberOfListItems, [AuthorAccess](../api/AuthorAccess.md) authorAccess)
Get list XML fragment.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNamespace](#getNamespace())()
Get namespace.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getParentListType](#getParentListType(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Get the type of the list in which the new list will be inserted.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXMLFragment](#getXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String))([AuthorAccess](../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentListType)
Get XML fragment to be inserted when nothing is selected.
  protected void [insertContent](#insertContent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,java.util.List))([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorNode](../api/node/AuthorNode.md) listNode, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CommonsOperationsUtil.SelectedFragmentInfo](../commons/operations/CommonsOperationsUtil.SelectedFragmentInfo.md)> selectedFragmentsInfos)
Insert content.
  protected boolean [isList](#isList(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Checks if the given node is a list.
  protected boolean [isListElement](#isListElement(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Checks if the given node is a list element or list item.

### Methods inherited from class ro.sync.ecss.extensions.commons.operations.[InsertListOperation](../commons/operations/InsertListOperation.md)
 [doOperation](../commons/operations/InsertListOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getElementAtCaretToConvert](../commons/operations/InsertListOperation.md#getElementAtCaretToConvert(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.commons.operations.CommonsOperationsUtil.ConversionElementHelper))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XHTMLInsertListOperation

public XHTMLInsertListOperation()

## Method Details

### getArguments

public [ArgumentDescriptor](../api/ArgumentDescriptor.md)[] getArguments()
  Returns: An array of [ArgumentDescriptor](../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../api/AuthorOperation.md#getArguments())

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../api/Extension.md#getDescription())

### insertContent

protected void insertContent([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorNode](../api/node/AuthorNode.md) listNode, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CommonsOperationsUtil.SelectedFragmentInfo](../commons/operations/CommonsOperationsUtil.SelectedFragmentInfo.md)> selectedFragmentsInfos)
 Description copied from class: [InsertListOperation](../commons/operations/InsertListOperation.md#insertContent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,java.util.List))
Insert content.
  Specified by: [insertContent](../commons/operations/InsertListOperation.md#insertContent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,java.util.List)) in class [InsertListOperation](../commons/operations/InsertListOperation.md) Parameters: authorAccess - The author access. listNode - The list node. selectedFragmentsInfos - The fragments to be inserted. See Also:
        * [InsertListOperation.insertContent(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorNode, java.util.List)](../commons/operations/InsertListOperation.md#insertContent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,java.util.List))

### getNamespace

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNamespace()
 Description copied from class: [InsertListOperation](../commons/operations/InsertListOperation.md#getNamespace())
Get namespace.
  Specified by: [getNamespace](../commons/operations/InsertListOperation.md#getNamespace()) in class [InsertListOperation](../commons/operations/InsertListOperation.md) Returns: The namespace to be used at insertion. See Also:
        * [InsertListOperation.getNamespace()](../commons/operations/InsertListOperation.md#getNamespace())

### getXMLFragment

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXMLFragment([AuthorAccess](../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentListType)
 Description copied from class: [InsertListOperation](../commons/operations/InsertListOperation.md#getXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String))
Get XML fragment to be inserted when nothing is selected.
  Specified by: [getXMLFragment](../commons/operations/InsertListOperation.md#getXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String)) in class [InsertListOperation](../commons/operations/InsertListOperation.md) Parameters: authorAccess - The author access. listType - The type of the list to be inserted. parentListType - The type of the parent list, can be null Returns: the fragment to be inserted. See Also:
        * [InsertListOperation.getXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess, java.lang.String, java.lang.String)](../commons/operations/InsertListOperation.md#getXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String))

### getListXMLFragment

protected [StringBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/StringBuilder.html) getListXMLFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> attributes, int numberOfListItems, [AuthorAccess](../api/AuthorAccess.md) authorAccess)
 Description copied from class: [InsertListOperation](../commons/operations/InsertListOperation.md#getListXMLFragment(java.lang.String,java.util.Map,int,ro.sync.ecss.extensions.api.AuthorAccess))
Get list XML fragment.
  Specified by: [getListXMLFragment](../commons/operations/InsertListOperation.md#getListXMLFragment(java.lang.String,java.util.Map,int,ro.sync.ecss.extensions.api.AuthorAccess)) in class [InsertListOperation](../commons/operations/InsertListOperation.md) Parameters: listType - The list type. attributes - The attributes to add to list items. numberOfListItems - The number of list items. authorAccess - The author access. Returns: The list XML fragment. See Also:
        * [InsertListOperation.getListXMLFragment(java.lang.String, java.util.Map, int, ro.sync.ecss.extensions.api.AuthorAccess)](../commons/operations/InsertListOperation.md#getListXMLFragment(java.lang.String,java.util.Map,int,ro.sync.ecss.extensions.api.AuthorAccess))

### getConversionElementsChecker

protected [CommonsOperationsUtil.ConversionElementHelper](../commons/operations/CommonsOperationsUtil.ConversionElementHelper.md) getConversionElementsChecker()
 Description copied from class: [InsertListOperation](../commons/operations/InsertListOperation.md#getConversionElementsChecker())
Get the conversion element checker.
  Specified by: [getConversionElementsChecker](../commons/operations/InsertListOperation.md#getConversionElementsChecker()) in class [InsertListOperation](../commons/operations/InsertListOperation.md) Returns: The conversion element checker. See Also:
        * [InsertListOperation.getConversionElementsChecker()](../commons/operations/InsertListOperation.md#getConversionElementsChecker())

### getParentListType

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getParentListType([AuthorNode](../api/node/AuthorNode.md) node)
 Description copied from class: [InsertListOperation](../commons/operations/InsertListOperation.md#getParentListType(ro.sync.ecss.extensions.api.node.AuthorNode))
Get the type of the list in which the new list will be inserted. Can be null.
  Specified by: [getParentListType](../commons/operations/InsertListOperation.md#getParentListType(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [InsertListOperation](../commons/operations/InsertListOperation.md) Parameters: node - The node at offset. Returns: the type of the list in which the new list will be inserted. Can be null. See Also:
        * [InsertListOperation.getParentListType(ro.sync.ecss.extensions.api.node.AuthorNode)](../commons/operations/InsertListOperation.md#getParentListType(ro.sync.ecss.extensions.api.node.AuthorNode))

### isListElement

protected boolean isListElement([AuthorNode](../api/node/AuthorNode.md) node)
 Description copied from class: [InsertListOperation](../commons/operations/InsertListOperation.md#isListElement(ro.sync.ecss.extensions.api.node.AuthorNode))
Checks if the given node is a list element or list item.
  Overrides: [isListElement](../commons/operations/InsertListOperation.md#isListElement(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [InsertListOperation](../commons/operations/InsertListOperation.md) Parameters: node - The element to check. Returns: true if the node is a list element. See Also:
        * [InsertListOperation.isListElement(ro.sync.ecss.extensions.api.node.AuthorNode)](../commons/operations/InsertListOperation.md#isListElement(ro.sync.ecss.extensions.api.node.AuthorNode))

### isList

protected boolean isList([AuthorNode](../api/node/AuthorNode.md) node)
 Description copied from class: [InsertListOperation](../commons/operations/InsertListOperation.md#isList(ro.sync.ecss.extensions.api.node.AuthorNode))
Checks if the given node is a list.
  Specified by: [isList](../commons/operations/InsertListOperation.md#isList(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [InsertListOperation](../commons/operations/InsertListOperation.md) Parameters: node - The element to check. Returns: true if the node is a list. See Also:
        * [InsertListOperation.isList(ro.sync.ecss.extensions.api.node.AuthorNode)](../commons/operations/InsertListOperation.md#isList(ro.sync.ecss.extensions.api.node.AuthorNode))

### getListTypeDescription

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getListTypeDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listType)
 Description copied from class: [InsertListOperation](../commons/operations/InsertListOperation.md#getListTypeDescription(java.lang.String))
Obtain the name of every list type.
  Specified by: [getListTypeDescription](../commons/operations/InsertListOperation.md#getListTypeDescription(java.lang.String)) in class [InsertListOperation](../commons/operations/InsertListOperation.md) Parameters: listType - The list type. Returns: A string representing the name of the given list type. See Also:
        * [InsertListOperation.getListTypeDescription(java.lang.String)](../commons/operations/InsertListOperation.md#getListTypeDescription(java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
