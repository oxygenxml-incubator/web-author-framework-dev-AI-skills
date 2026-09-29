Package [ro.sync.ecss.extensions.dita.id](package-summary.md)

# Class DITAConfigureAutoIDElementsOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.id.ConfigureAutoIDElementsOperation](../../commons/id/ConfigureAutoIDElementsOperation.md)
        * ro.sync.ecss.extensions.dita.id.DITAConfigureAutoIDElementsOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DITAConfigureAutoIDElementsOperation extends [ConfigureAutoIDElementsOperation](../../commons/id/ConfigureAutoIDElementsOperation.md)
Operation used to insert a Link in DITA documents.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [DITAConfigureAutoIDElementsOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getListMessage](#getListMessage())()

### Methods inherited from class ro.sync.ecss.extensions.commons.id.[ConfigureAutoIDElementsOperation](../../commons/id/ConfigureAutoIDElementsOperation.md)
 [doOperation](../../commons/id/ConfigureAutoIDElementsOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../commons/id/ConfigureAutoIDElementsOperation.md#getArguments()), [getDefaultOptions](../../commons/id/ConfigureAutoIDElementsOperation.md#getDefaultOptions(ro.sync.ecss.extensions.api.AuthorAccess)), [getDefaultOptionsXMLResourceName](../../commons/id/ConfigureAutoIDElementsOperation.md#getDefaultOptionsXMLResourceName()), [getHelpPageID](../../commons/id/ConfigureAutoIDElementsOperation.md#getHelpPageID()), [isDocBook](../../commons/id/ConfigureAutoIDElementsOperation.md#isDocBook())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAConfigureAutoIDElementsOperation

public DITAConfigureAutoIDElementsOperation()

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

### getListMessage

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getListMessage()
  Specified by: [getListMessage](../../commons/id/ConfigureAutoIDElementsOperation.md#getListMessage()) in class [ConfigureAutoIDElementsOperation](../../commons/id/ConfigureAutoIDElementsOperation.md) Returns: The message used on the list See Also:
        * [ConfigureAutoIDElementsOperation.getListMessage()](../../commons/id/ConfigureAutoIDElementsOperation.md#getListMessage())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
