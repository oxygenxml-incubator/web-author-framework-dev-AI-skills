Package [ro.sync.ecss.extensions.tei.id](package-summary.md)

# Class GenerateIDsTEIP5Operation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.id.GenerateIDsOperation](../../commons/id/GenerateIDsOperation.md)
        * ro.sync.ecss.extensions.tei.id.GenerateIDsTEIP5Operation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class GenerateIDsTEIP5Operation extends [GenerateIDsOperation](../../commons/id/GenerateIDsOperation.md)
Operation to auto generate IDs on the selected content.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [GenerateIDsTEIP5Operation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [UniqueAttributesRecognizer](../../api/UniqueAttributesRecognizer.md) [getUniqueAttributesRecognizer](#getUniqueAttributesRecognizer())()

### Methods inherited from class ro.sync.ecss.extensions.commons.id.[GenerateIDsOperation](../../commons/id/GenerateIDsOperation.md)
 [doOperation](../../commons/id/GenerateIDsOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../commons/id/GenerateIDsOperation.md#getArguments()), [getDescription](../../commons/id/GenerateIDsOperation.md#getDescription())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### GenerateIDsTEIP5Operation

public GenerateIDsTEIP5Operation()

## Method Details

### getUniqueAttributesRecognizer

protected [UniqueAttributesRecognizer](../../api/UniqueAttributesRecognizer.md) getUniqueAttributesRecognizer()
  Specified by: [getUniqueAttributesRecognizer](../../commons/id/GenerateIDsOperation.md#getUniqueAttributesRecognizer()) in class [GenerateIDsOperation](../../commons/id/GenerateIDsOperation.md) Returns: The unique attributes handler See Also:
        * [GenerateIDsOperation.getUniqueAttributesRecognizer()](../../commons/id/GenerateIDsOperation.md#getUniqueAttributesRecognizer())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
