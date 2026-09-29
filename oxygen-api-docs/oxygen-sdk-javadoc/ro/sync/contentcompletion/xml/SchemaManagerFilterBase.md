Package [ro.sync.contentcompletion.xml](package-summary.md)

# Class SchemaManagerFilterBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.contentcompletion.xml.SchemaManagerFilterBase
   All Implemented Interfaces: [SchemaManagerFilter](SchemaManagerFilter.md), [Extension](../../ecss/extensions/api/Extension.md)   Direct Known Subclasses: [DITASchemaManagerFilter](../../ecss/extensions/dita/DITASchemaManagerFilter.md), [DITAValSchemaManagerFilter](../../ecss/extensions/dita/DITAValSchemaManagerFilter.md), [DocbookSchemaManagerFilter](../../ecss/extensions/docbook/DocbookSchemaManagerFilter.md), [StyleGuideSchemaManagerFilterBase](StyleGuideSchemaManagerFilterBase.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class SchemaManagerFilterBase extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [SchemaManagerFilter](SchemaManagerFilter.md)
Base class for objects used to filter the editor content completion schema manager proposals. This should be implemented if the list of content completion proposals must be filtered based on some criteria or some new entries need to be added.
  Since: 15
## Constructor Summary
 Constructors
Constructor

Description
 [SchemaManagerFilterBase](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [CIAttribute](CIAttribute.md) [getAttributeDescription](#getAttributeDescription(ro.sync.contentcompletion.xml.CIAttribute,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))([CIAttribute](CIAttribute.md) attribute, [WhatPossibleValuesHasAttributeContext](WhatPossibleValuesHasAttributeContext.md) ctxt)
Get an element's description in a certain context.
  [CIElement](CIElement.md) [getElementDescription](#getElementDescription(ro.sync.contentcompletion.xml.CIElement,ro.sync.contentcompletion.xml.Context))([CIElement](CIElement.md) element, [Context](Context.md) ctxt)
Get an element's description in a certain context.
  void [invalidate](#invalidate())()
Invalidates any cached data.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../ecss/extensions/api/Extension.md)
 [getDescription](../../ecss/extensions/api/Extension.md#getDescription())
### Methods inherited from interface ro.sync.contentcompletion.xml.[SchemaManagerFilter](SchemaManagerFilter.md)
 [filterAttributes](SchemaManagerFilter.md#filterAttributes(java.util.List,ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext)), [filterAttributeValues](SchemaManagerFilter.md#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext)), [filterElements](SchemaManagerFilter.md#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext)), [filterElementValues](SchemaManagerFilter.md#filterElementValues(java.util.List,ro.sync.contentcompletion.xml.Context))
## Constructor Details

### SchemaManagerFilterBase

public SchemaManagerFilterBase()

## Method Details

### getElementDescription

public [CIElement](CIElement.md) getElementDescription([CIElement](CIElement.md) element, [Context](Context.md) ctxt)

Get an element's description in a certain context.
  Parameters: element - The element description which has been computed in the context by the default schema manager implementation. ctxt - The context. Returns: The element description which could be changed by this implementation or the same description.
### getAttributeDescription

public [CIAttribute](CIAttribute.md) getAttributeDescription([CIAttribute](CIAttribute.md) attribute, [WhatPossibleValuesHasAttributeContext](WhatPossibleValuesHasAttributeContext.md) ctxt)

Get an element's description in a certain context.
  Parameters: attribute - The attribute description which has been computed in the context by the default schema manager implementation. ctxt - The context. Returns: The attribute description which could be changed by this implementation or the same description.
### invalidate

public void invalidate()

Invalidates any cached data.
  Since: 16
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
