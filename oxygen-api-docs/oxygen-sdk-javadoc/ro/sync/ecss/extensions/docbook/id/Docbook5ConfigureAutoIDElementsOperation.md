Package [ro.sync.ecss.extensions.docbook.id](package-summary.md)

# Class Docbook5ConfigureAutoIDElementsOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.id.ConfigureAutoIDElementsOperation](../../commons/id/ConfigureAutoIDElementsOperation.md)
        * [ro.sync.ecss.extensions.docbook.id.DocbookConfigureAutoIDElementsOperation](DocbookConfigureAutoIDElementsOperation.md)
            * ro.sync.ecss.extensions.docbook.id.Docbook5ConfigureAutoIDElementsOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class Docbook5ConfigureAutoIDElementsOperation extends [DocbookConfigureAutoIDElementsOperation](DocbookConfigureAutoIDElementsOperation.md)
Operation specific for Docbook 5

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [Docbook5ConfigureAutoIDElementsOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultOptionsXMLResourceName](#getDefaultOptionsXMLResourceName())()
Get the name of the XML resource from which to load the default options.

### Methods inherited from class ro.sync.ecss.extensions.docbook.id.[DocbookConfigureAutoIDElementsOperation](DocbookConfigureAutoIDElementsOperation.md)
 [getDescription](DocbookConfigureAutoIDElementsOperation.md#getDescription()), [getListMessage](DocbookConfigureAutoIDElementsOperation.md#getListMessage()), [isDocBook](DocbookConfigureAutoIDElementsOperation.md#isDocBook())
### Methods inherited from class ro.sync.ecss.extensions.commons.id.[ConfigureAutoIDElementsOperation](../../commons/id/ConfigureAutoIDElementsOperation.md)
 [doOperation](../../commons/id/ConfigureAutoIDElementsOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../commons/id/ConfigureAutoIDElementsOperation.md#getArguments()), [getDefaultOptions](../../commons/id/ConfigureAutoIDElementsOperation.md#getDefaultOptions(ro.sync.ecss.extensions.api.AuthorAccess)), [getHelpPageID](../../commons/id/ConfigureAutoIDElementsOperation.md#getHelpPageID())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### Docbook5ConfigureAutoIDElementsOperation

public Docbook5ConfigureAutoIDElementsOperation()

## Method Details

### getDefaultOptionsXMLResourceName

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultOptionsXMLResourceName()
 Description copied from class: [ConfigureAutoIDElementsOperation](../../commons/id/ConfigureAutoIDElementsOperation.md#getDefaultOptionsXMLResourceName())
Get the name of the XML resource from which to load the default options.
  Overrides: [getDefaultOptionsXMLResourceName](../../commons/id/ConfigureAutoIDElementsOperation.md#getDefaultOptionsXMLResourceName()) in class [ConfigureAutoIDElementsOperation](../../commons/id/ConfigureAutoIDElementsOperation.md) Returns: the name of the XML resource from which to load the default options. See Also:
        * [ConfigureAutoIDElementsOperation.getDefaultOptionsXMLResourceName()](../../commons/id/ConfigureAutoIDElementsOperation.md#getDefaultOptionsXMLResourceName())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
