Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DITASchemaManagerFilter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.contentcompletion.xml.SchemaManagerFilterBase](../../../contentcompletion/xml/SchemaManagerFilterBase.md)
        * ro.sync.ecss.extensions.dita.DITASchemaManagerFilter
   All Implemented Interfaces: [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md), [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DITASchemaManagerFilter extends [SchemaManagerFilterBase](../../../contentcompletion/xml/SchemaManagerFilterBase.md)
Schema manager filter which provides the available keyref + condition values.

## Constructor Summary
 Constructors
Constructor

Description
 [DITASchemaManagerFilter](#%3Cinit%3E(java.lang.String,ro.sync.ecss.dita.ContextKeyManagerProvider,java.util.function.Supplier))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypeName, [ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) contextKeyManagerProvider, [Supplier](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Supplier.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> userNameProvider)
Constructor

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../contentcompletion/xml/CIAttribute.md)> [filterAttributes](#filterAttributes(java.util.List,ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../contentcompletion/xml/CIAttribute.md)> attributes, [WhatAttributesCanGoHereContext](../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) context)
Filter attributes.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> [filterAttributeValues](#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context)
Filter attribute values.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> [filterElements](#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> elements, [WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context)
Filter elements.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> [filterElementValues](#filterElementValues(java.util.List,ro.sync.contentcompletion.xml.Context))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> elementValues, [Context](../../../contentcompletion/xml/Context.md) context)
Filter element values.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

### Methods inherited from class ro.sync.contentcompletion.xml.[SchemaManagerFilterBase](../../../contentcompletion/xml/SchemaManagerFilterBase.md)
 [getAttributeDescription](../../../contentcompletion/xml/SchemaManagerFilterBase.md#getAttributeDescription(ro.sync.contentcompletion.xml.CIAttribute,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext)), [getElementDescription](../../../contentcompletion/xml/SchemaManagerFilterBase.md#getElementDescription(ro.sync.contentcompletion.xml.CIElement,ro.sync.contentcompletion.xml.Context)), [invalidate](../../../contentcompletion/xml/SchemaManagerFilterBase.md#invalidate())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITASchemaManagerFilter

public DITASchemaManagerFilter([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypeName, [ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md) contextKeyManagerProvider, [Supplier](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Supplier.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> userNameProvider)

Constructor
  Parameters: documentTypeName - The document type name contextKeyManagerProvider - A provider of a context key manager used to propose attributes values for attributes like keyref. userNameProvider - User name provider - it may return null in which case a fallback is used.
## Method Details

### filterAttributeValues

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> filterAttributeValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context)

Filter attribute values.
  Parameters: attributeValues - The list of attribute values ([CIValue](../../../contentcompletion/xml/CIValue.md)) to be filtered. context - The [WhatPossibleValuesHasAttributeContext](../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) where the list of attribute values is requested. Returns: The filtered list of [CIValue](../../../contentcompletion/xml/CIValue.md) representing possible values of the attribute or null if all values are rejected by the filter. See Also:
        * [SchemaManagerFilter.filterAttributeValues(java.util.List, ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext)](../../../contentcompletion/xml/SchemaManagerFilter.md#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))

### filterAttributes

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../contentcompletion/xml/CIAttribute.md)> filterAttributes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../contentcompletion/xml/CIAttribute.md)> attributes, [WhatAttributesCanGoHereContext](../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) context)

Filter attributes.
  Parameters: attributes - The list of attributes ([CIAttribute](../../../contentcompletion/xml/CIAttribute.md)) to be filtered. Can be NULL context - The [WhatAttributesCanGoHereContext](../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) where the list of attributes is requested. Returns: The filtered list of [CIAttribute](../../../contentcompletion/xml/CIAttribute.md) or null if all attributes are rejected by the filter. See Also:
        * [SchemaManagerFilter.filterAttributes(java.util.List, ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext)](../../../contentcompletion/xml/SchemaManagerFilter.md#filterAttributes(java.util.List,ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))

### filterElementValues

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> filterElementValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> elementValues, [Context](../../../contentcompletion/xml/Context.md) context)

Filter element values.
  Parameters: elementValues - The list of element values ([CIValue](../../../contentcompletion/xml/CIValue.md)) to be filtered. context - The [Context](../../../contentcompletion/xml/Context.md) where the list of element values is requested. Returns: The filtered list of [CIValue](../../../contentcompletion/xml/CIValue.md) representing the possible values of the element or null if all values are rejected by the filter. See Also:
        * [SchemaManagerFilter.filterElementValues(java.util.List, ro.sync.contentcompletion.xml.Context)](../../../contentcompletion/xml/SchemaManagerFilter.md#filterElementValues(java.util.List,ro.sync.contentcompletion.xml.Context))

### filterElements

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> filterElements([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> elements, [WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context)

Filter elements.
  Parameters: elements - The list of elements ([CIElement](../../../contentcompletion/xml/CIElement.md)) to be filtered. context - The [WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) where the list of elements is requested. If null then the given list of content completion elements contains global elements. Returns: The filtered list of [CIElement](../../../contentcompletion/xml/CIElement.md) or null if all elements are rejected by the filter. See Also:
        * [SchemaManagerFilter.filterElements(java.util.List, ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext)](../../../contentcompletion/xml/SchemaManagerFilter.md#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
