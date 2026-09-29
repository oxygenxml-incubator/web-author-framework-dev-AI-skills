Package [ro.sync.contentcompletion.xml](package-summary.md)

# Interface SchemaManagerFilter
    All Superinterfaces: [Extension](../../ecss/extensions/api/Extension.md)   All Known Implementing Classes: [DITASchemaManagerFilter](../../ecss/extensions/dita/DITASchemaManagerFilter.md), [DITAValSchemaManagerFilter](../../ecss/extensions/dita/DITAValSchemaManagerFilter.md), [DocbookSchemaManagerFilter](../../ecss/extensions/docbook/DocbookSchemaManagerFilter.md), [SchemaManagerFilterBase](SchemaManagerFilterBase.md), [StyleGuideSchemaManagerFilterBase](StyleGuideSchemaManagerFilterBase.md), [XHTMLSchemaManagerFilter](../../ecss/extensions/xhtml/XHTMLSchemaManagerFilter.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface SchemaManagerFilterextends [Extension](../../ecss/extensions/api/Extension.md)
Interface for objects used to filter the editor content completion schema manager proposals. This should be implemented if the list of content completion proposals must be filtered based on some criteria or some new entries need to be added.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> [filterAttributes](#filterAttributes(java.util.List,ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> attributes, [WhatAttributesCanGoHereContext](WhatAttributesCanGoHereContext.md) context)
Filters the attributes proposed by the editor content completion schema manager.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> [filterAttributeValues](#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](WhatPossibleValuesHasAttributeContext.md) context)
Filters the attribute values proposed by the editor content completion schema manager.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](CIElement.md)> [filterElements](#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](CIElement.md)> elements, [WhatElementsCanGoHereContext](WhatElementsCanGoHereContext.md) context)
Filters the elements proposed by the editor content completion schema manager.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> [filterElementValues](#filterElementValues(java.util.List,ro.sync.contentcompletion.xml.Context))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> elementValues, [Context](Context.md) context)
Filters the element values proposed by the editor content completion schema manager.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../ecss/extensions/api/Extension.md)
 [getDescription](../../ecss/extensions/api/Extension.md#getDescription())
## Method Details

### filterElements

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](CIElement.md)> filterElements([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](CIElement.md)> elements, [WhatElementsCanGoHereContext](WhatElementsCanGoHereContext.md) context)

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

  Parameters: elements - The list of elements ([CIElement](CIElement.md)) to be filtered. context - The [WhatElementsCanGoHereContext](WhatElementsCanGoHereContext.md) where the list of elements is requested. If null then the given list of content completion elements contains global elements. Returns: The filtered list of [CIElement](CIElement.md) or null if all elements are rejected by the filter.
### filterAttributes

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> filterAttributes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> attributes, [WhatAttributesCanGoHereContext](WhatAttributesCanGoHereContext.md) context)

Filters the attributes proposed by the editor content completion schema manager. The original list of attributes is obtained by examining the current document schema and determining what attributes can be inserted in the current element and taking into account the list of existing attributes.
  Parameters: attributes - The list of attributes ([CIAttribute](CIAttribute.md)) to be filtered. Can be NULL context - The [WhatAttributesCanGoHereContext](WhatAttributesCanGoHereContext.md) where the list of attributes is requested. Returns: The filtered list of [CIAttribute](CIAttribute.md) or null if all attributes are rejected by the filter.
### filterAttributeValues

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> filterAttributeValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](WhatPossibleValuesHasAttributeContext.md) context)

Filters the attribute values proposed by the editor content completion schema manager. The original list of attribute values is obtained by examining the current document schema and determining what values are permitted for the current attribute. If the attribute type was an enumeration, then a list with the tokens of the enumeration will be returned for that attribute.
  Parameters: attributeValues - The list of attribute values ([CIValue](CIValue.md)) to be filtered. context - The [WhatPossibleValuesHasAttributeContext](WhatPossibleValuesHasAttributeContext.md) where the list of attribute values is requested. Returns: The filtered list of [CIValue](CIValue.md) representing possible values of the attribute or null if all values are rejected by the filter.
### filterElementValues

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> filterElementValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> elementValues, [Context](Context.md) context)

Filters the element values proposed by the editor content completion schema manager. The original list of element values is obtained by examining the current document schema and determining what values are permitted for the current element. If the element type was an enumeration, then a list with the values of the enumeration will be returned for that element.
  Parameters: elementValues - The list of element values ([CIValue](CIValue.md)) to be filtered. context - The [Context](Context.md) where the list of element values is requested. Returns: The filtered list of [CIValue](CIValue.md) representing the possible values of the element or null if all values are rejected by the filter.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
