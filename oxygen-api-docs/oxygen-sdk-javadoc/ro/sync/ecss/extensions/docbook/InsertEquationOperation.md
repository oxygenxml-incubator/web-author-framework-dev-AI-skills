Package [ro.sync.ecss.extensions.docbook](package-summary.md)

# Class InsertEquationOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.operations.InsertEquationOperation](../commons/operations/InsertEquationOperation.md)
        * ro.sync.ecss.extensions.docbook.InsertEquationOperation
   All Implemented Interfaces: [AuthorOperation](../api/AuthorOperation.md), [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertEquationOperation extends [InsertEquationOperation](../commons/operations/InsertEquationOperation.md)
Operation used to insert an equation in Docbook documents.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.operations.[InsertEquationOperation](../commons/operations/InsertEquationOperation.md)
 [MATH_ML](../commons/operations/InsertEquationOperation.md#MATH_ML), [MATH_ML_FOR_HTML_DOC_TYPE](../commons/operations/InsertEquationOperation.md#MATH_ML_FOR_HTML_DOC_TYPE), [MATH_ML_NAMESPACE](../commons/operations/InsertEquationOperation.md#MATH_ML_NAMESPACE), [WEBAPP_MATH_ML](../commons/operations/InsertEquationOperation.md#WEBAPP_MATH_ML)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [InsertEquationOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [createDefaultFragmentToEdit](#createDefaultFragmentToEdit(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorSchemaManager))([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorSchemaManager](../api/AuthorSchemaManager.md) asm)
Return default fragment.

### Methods inherited from class ro.sync.ecss.extensions.commons.operations.[InsertEquationOperation](../commons/operations/InsertEquationOperation.md)
 [doOperation](../commons/operations/InsertEquationOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../commons/operations/InsertEquationOperation.md#getArguments()), [getDescription](../commons/operations/InsertEquationOperation.md#getDescription())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### InsertEquationOperation

public InsertEquationOperation()

## Method Details

### createDefaultFragmentToEdit

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) createDefaultFragmentToEdit([AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorSchemaManager](../api/AuthorSchemaManager.md) asm)
 Description copied from class: [InsertEquationOperation](../commons/operations/InsertEquationOperation.md#createDefaultFragmentToEdit(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorSchemaManager))
Return default fragment.
  Overrides: [createDefaultFragmentToEdit](../commons/operations/InsertEquationOperation.md#createDefaultFragmentToEdit(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorSchemaManager)) in class [InsertEquationOperation](../commons/operations/InsertEquationOperation.md) Parameters: authorAccess - Author access. asm - The author schema manager. Returns: The default fragment. See Also:
        * [InsertEquationOperation.createDefaultFragmentToEdit(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorSchemaManager)](../commons/operations/InsertEquationOperation.md#createDefaultFragmentToEdit(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorSchemaManager))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
