Package [ro.sync.contentcompletion.xml](package-summary.md)

# Class StyleGuideSchemaManagerFilterBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.contentcompletion.xml.SchemaManagerFilterBase](SchemaManagerFilterBase.md)
        * ro.sync.contentcompletion.xml.StyleGuideSchemaManagerFilterBase
   All Implemented Interfaces: [SchemaManagerFilter](SchemaManagerFilter.md), [Extension](../../ecss/extensions/api/Extension.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class StyleGuideSchemaManagerFilterBase extends [SchemaManagerFilterBase](SchemaManagerFilterBase.md)
Style guide schema manager filter base. The default implementation adds annotations to elements and attributes by looking into a mapping file URI which is passed through the XML Catalog system...
  Since: 15
## Field Summary
 Fields
Modifier and Type

Field

Description
 protected static final ro.sync.i18n.MessageBundle [messages](#messages)
The messages resource bundle.

## Constructor Summary
 Constructors
Constructor

Description
 [StyleGuideSchemaManagerFilterBase](#%3Cinit%3E())()
Constructor.
  [StyleGuideSchemaManagerFilterBase](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) locationOfMappingFile)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> [filterAttributes](#filterAttributes(java.util.List,ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> attributes, [WhatAttributesCanGoHereContext](WhatAttributesCanGoHereContext.md) context)
Filters the attributes proposed by the editor content completion schema manager.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](CIElement.md)> [filterElements](#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](CIElement.md)> elements, [WhatElementsCanGoHereContext](WhatElementsCanGoHereContext.md) context)
Filters the elements proposed by the editor content completion schema manager.
  [CIAttribute](CIAttribute.md) [getAttributeDescription](#getAttributeDescription(ro.sync.contentcompletion.xml.CIAttribute,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))([CIAttribute](CIAttribute.md) attribute, [WhatPossibleValuesHasAttributeContext](WhatPossibleValuesHasAttributeContext.md) ctxt)
Get an element's description in a certain context.
  [CIElement](CIElement.md) [getElementDescription](#getElementDescription(ro.sync.contentcompletion.xml.CIElement,ro.sync.contentcompletion.xml.Context))([CIElement](CIElement.md) element, [Context](Context.md) ctxt)
Get element description, contributes HTML annotation to it..
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMappingFileLocation](#getMappingFileLocation(ro.sync.contentcompletion.xml.Context))([Context](Context.md) context)
Get the location for the mapping between elements name and their documentation.
  void [invalidate](#invalidate())()
Invalidates any cached data.
  protected boolean [shouldRedirectThroughOxygenWebSite](#shouldRedirectThroughOxygenWebSite())()
If true will redirect all links through the Oxygen web site.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../ecss/extensions/api/Extension.md)
 [getDescription](../../ecss/extensions/api/Extension.md#getDescription())
### Methods inherited from interface ro.sync.contentcompletion.xml.[SchemaManagerFilter](SchemaManagerFilter.md)
 [filterAttributeValues](SchemaManagerFilter.md#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext)), [filterElementValues](SchemaManagerFilter.md#filterElementValues(java.util.List,ro.sync.contentcompletion.xml.Context))
## Field Details

### messages

protected static final ro.sync.i18n.MessageBundle messages

The messages resource bundle.

## Constructor Details

### StyleGuideSchemaManagerFilterBase

public StyleGuideSchemaManagerFilterBase()

Constructor.

### StyleGuideSchemaManagerFilterBase

public StyleGuideSchemaManagerFilterBase([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) locationOfMappingFile)

Constructor.
  Parameters: locationOfMappingFile - Location of the mapping file.
## Method Details

### filterElements

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](CIElement.md)> filterElements([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](CIElement.md)> elements, [WhatElementsCanGoHereContext](WhatElementsCanGoHereContext.md) context)
 Description copied from interface: [SchemaManagerFilter](SchemaManagerFilter.md#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))
Filters the elements proposed by the editor content completion schema manager. The original list of elements is obtained by examining the current document schema and determining what possible elements can be inserted in the current context. For example if person is the current CIElement, and the list of children contains the elements nameand address, the result of choosing the **person** entry from the content completion window will be the insertion of the following sequence:
```


 <person>
     <name>...</name>
     <address>...</address>
 </person>


```
Given this example, the original name CIElement can be replaced by a new one which returns a list with two new CIElements, firstName and lastName, on the [CIElement.getGuessElements()](CIElement.md#getGuessElements()) method call. The new generated sequence would be:
```


 <person>
     <name>
         <firstName>...</firstName>
         <lastName>...</lastName>
     </name>
     <address>...</address>
 </person>


```

  Parameters: elements - The list of elements ([CIElement](CIElement.md)) to be filtered. context - The [WhatElementsCanGoHereContext](WhatElementsCanGoHereContext.md) where the list of elements is requested. If null then the given list of content completion elements contains global elements. Returns: The filtered list of [CIElement](CIElement.md) or null if all elements are rejected by the filter. See Also:
        * [SchemaManagerFilter.filterElements(java.util.List, ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext)](SchemaManagerFilter.md#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))

### getMappingFileLocation

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMappingFileLocation([Context](Context.md) context)

Get the location for the mapping between elements name and their documentation.
  Parameters: context - The current elements context. Returns: The styles guide mapping location.
### filterAttributes

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> filterAttributes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> attributes, [WhatAttributesCanGoHereContext](WhatAttributesCanGoHereContext.md) context)
 Description copied from interface: [SchemaManagerFilter](SchemaManagerFilter.md#filterAttributes(java.util.List,ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))
Filters the attributes proposed by the editor content completion schema manager. The original list of attributes is obtained by examining the current document schema and determining what attributes can be inserted in the current element and taking into account the list of existing attributes.
  Parameters: attributes - The list of attributes ([CIAttribute](CIAttribute.md)) to be filtered. Can be NULL context - The [WhatAttributesCanGoHereContext](WhatAttributesCanGoHereContext.md) where the list of attributes is requested. Returns: The filtered list of [CIAttribute](CIAttribute.md) or null if all attributes are rejected by the filter. See Also:
        * [SchemaManagerFilter.filterAttributes(java.util.List, ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext)](SchemaManagerFilter.md#filterAttributes(java.util.List,ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))

### getElementDescription

public [CIElement](CIElement.md) getElementDescription([CIElement](CIElement.md) element, [Context](Context.md) ctxt)

Get element description, contributes HTML annotation to it..
  Overrides: [getElementDescription](SchemaManagerFilterBase.md#getElementDescription(ro.sync.contentcompletion.xml.CIElement,ro.sync.contentcompletion.xml.Context)) in class [SchemaManagerFilterBase](SchemaManagerFilterBase.md) Parameters: element - The CIElement ctxt - The context. Returns: The modified CIElement with HTML annotation.
### getAttributeDescription

public [CIAttribute](CIAttribute.md) getAttributeDescription([CIAttribute](CIAttribute.md) attribute, [WhatPossibleValuesHasAttributeContext](WhatPossibleValuesHasAttributeContext.md) ctxt)
 Description copied from class: [SchemaManagerFilterBase](SchemaManagerFilterBase.md#getAttributeDescription(ro.sync.contentcompletion.xml.CIAttribute,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))
Get an element's description in a certain context.
  Overrides: [getAttributeDescription](SchemaManagerFilterBase.md#getAttributeDescription(ro.sync.contentcompletion.xml.CIAttribute,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext)) in class [SchemaManagerFilterBase](SchemaManagerFilterBase.md) Parameters: attribute - The attribute description which has been computed in the context by the default schema manager implementation. ctxt - The context. Returns: The attribute description which could be changed by this implementation or the same description. See Also:
        * [SchemaManagerFilterBase.getAttributeDescription(ro.sync.contentcompletion.xml.CIAttribute, ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext)](SchemaManagerFilterBase.md#getAttributeDescription(ro.sync.contentcompletion.xml.CIAttribute,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))

### invalidate

public void invalidate()
 Description copied from class: [SchemaManagerFilterBase](SchemaManagerFilterBase.md#invalidate())
Invalidates any cached data.
  Overrides: [invalidate](SchemaManagerFilterBase.md#invalidate()) in class [SchemaManagerFilterBase](SchemaManagerFilterBase.md) See Also:
        * [SchemaManagerFilterBase.invalidate()](SchemaManagerFilterBase.md#invalidate())

### shouldRedirectThroughOxygenWebSite

protected boolean shouldRedirectThroughOxygenWebSite()

If true will redirect all links through the Oxygen web site.
  Returns: true if the filter will redirect all links through the Oxygen web site.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
