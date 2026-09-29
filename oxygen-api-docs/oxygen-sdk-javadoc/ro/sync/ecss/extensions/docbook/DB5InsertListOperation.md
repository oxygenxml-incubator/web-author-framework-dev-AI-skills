Package [ro.sync.ecss.extensions.docbook](package-summary.md)

# Class DB5InsertListOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.operations.InsertListOperation](../commons/operations/InsertListOperation.md)
        * [ro.sync.ecss.extensions.docbook.DocbookInsertListOperation](DocbookInsertListOperation.md)
            * ro.sync.ecss.extensions.docbook.DB5InsertListOperation
   All Implemented Interfaces: [AuthorOperation](../api/AuthorOperation.md), [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DB5InsertListOperation extends [DocbookInsertListOperation](DocbookInsertListOperation.md)
Insert List operation for Docbook 5.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.docbook.[DocbookInsertListOperation](DocbookInsertListOperation.md)
 [ITEMIZED_LIST](DocbookInsertListOperation.md#ITEMIZED_LIST), [LIST_TYPE_ARGUMENT](DocbookInsertListOperation.md#LIST_TYPE_ARGUMENT), [ORDERED_LIST](DocbookInsertListOperation.md#ORDERED_LIST), [PROCEDURE](DocbookInsertListOperation.md#PROCEDURE), [VARIABLE_LIST](DocbookInsertListOperation.md#VARIABLE_LIST)
### Fields inherited from class ro.sync.ecss.extensions.commons.operations.[InsertListOperation](../commons/operations/InsertListOperation.md)
 [authorAccess](../commons/operations/InsertListOperation.md#authorAccess), [CONVERT_ELEMENT_AT_CARET_ARGUMENT](../commons/operations/InsertListOperation.md#CONVERT_ELEMENT_AT_CARET_ARGUMENT), [CONVERT_ELEMENT_AT_CARET_ARGUMENT_DESCRIPTOR](../commons/operations/InsertListOperation.md#CONVERT_ELEMENT_AT_CARET_ARGUMENT_DESCRIPTOR), [listType](../commons/operations/InsertListOperation.md#listType), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../commons/operations/InsertListOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT)
## Constructor Summary
 Constructors
Constructor

Description
 [DB5InsertListOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNamespace](#getNamespace())()
Get namespace.

### Methods inherited from class ro.sync.ecss.extensions.docbook.[DocbookInsertListOperation](DocbookInsertListOperation.md)
 [getArguments](DocbookInsertListOperation.md#getArguments()), [getConversionElementsChecker](DocbookInsertListOperation.md#getConversionElementsChecker()), [getDescription](DocbookInsertListOperation.md#getDescription()), [getListTypeDescription](DocbookInsertListOperation.md#getListTypeDescription(java.lang.String)), [getListXMLFragment](DocbookInsertListOperation.md#getListXMLFragment(java.lang.String,java.util.Map,int,ro.sync.ecss.extensions.api.AuthorAccess)), [getParentListType](DocbookInsertListOperation.md#getParentListType(ro.sync.ecss.extensions.api.node.AuthorNode)), [getXMLFragment](DocbookInsertListOperation.md#getXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String)), [insertContent](DocbookInsertListOperation.md#insertContent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,java.util.List)), [isList](DocbookInsertListOperation.md#isList(ro.sync.ecss.extensions.api.node.AuthorNode)), [isListElement](DocbookInsertListOperation.md#isListElement(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class ro.sync.ecss.extensions.commons.operations.[InsertListOperation](../commons/operations/InsertListOperation.md)
 [doOperation](../commons/operations/InsertListOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getElementAtCaretToConvert](../commons/operations/InsertListOperation.md#getElementAtCaretToConvert(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.commons.operations.CommonsOperationsUtil.ConversionElementHelper))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DB5InsertListOperation

public DB5InsertListOperation()

## Method Details

### getNamespace

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNamespace()
 Description copied from class: [InsertListOperation](../commons/operations/InsertListOperation.md#getNamespace())
Get namespace.
  Specified by: [getNamespace](../commons/operations/InsertListOperation.md#getNamespace()) in class [InsertListOperation](../commons/operations/InsertListOperation.md) Returns: The namespace to be used at insertion. See Also:
        * [InsertListOperation.getNamespace()](../commons/operations/InsertListOperation.md#getNamespace())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
