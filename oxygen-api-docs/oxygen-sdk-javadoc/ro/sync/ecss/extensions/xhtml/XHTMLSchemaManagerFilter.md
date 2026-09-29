Package [ro.sync.ecss.extensions.xhtml](package-summary.md)

# Class XHTMLSchemaManagerFilter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.xhtml.XHTMLSchemaManagerFilter
   All Implemented Interfaces: [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md), [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class XHTMLSchemaManagerFilter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md)
XHTML implementation for schema manager filter for adding type attribute values for script and style elements in content completion proposals list.

## Constructor Summary
 Constructors
Constructor

Description
 [XHTMLSchemaManagerFilter](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../contentcompletion/xml/CIAttribute.md)> [filterAttributes](#filterAttributes(java.util.List,ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../contentcompletion/xml/CIAttribute.md)> attributes, [WhatAttributesCanGoHereContext](../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) context)
Filters the attributes proposed by the editor content completion schema manager.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> [filterAttributeValues](#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context)
Filters the attribute values proposed by the editor content completion schema manager.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> [filterElements](#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> elements, [WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context)
Filters the elements proposed by the editor content completion schema manager.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> [filterElementValues](#filterElementValues(java.util.List,ro.sync.contentcompletion.xml.Context))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> elementValues, [Context](../../../contentcompletion/xml/Context.md) context)
Filters the element values proposed by the editor content completion schema manager.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLocalName](#getLocalName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName)
Get the local name from an qualified element or attribute name.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XHTMLSchemaManagerFilter

public XHTMLSchemaManagerFilter()

## Method Details

### filterElements

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> filterElements([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> elements, [WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context)
 Description copied from interface: [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))
Filters the elements proposed by the editor content completion schema manager. The original list of elements is obtained by examining the current document schema and determining what possible elements can be inserted in the current context. For example if person is the current CIElement, and the list of children contains the elements nameand address, the result of choosing the **person** entry from the content completion window will be the insertion of the following sequence:
```


 <person>
     <name>...</name>
     <address>...</address>
 </person>


```
Given this example, the original name CIElement can be replaced by a new one which returns a list with two new CIElements, firstName and lastName, on the [CIElement.getGuessElements()](../../../contentcompletion/xml/CIElement.md#getGuessElements()) method call. The new generated sequence would be:
```


 <person>
     <name>
         <firstName>...</firstName>
         <lastName>...</lastName>
     </name>
     <address>...</address>
 </person>


```

  Specified by: [filterElements](../../../contentcompletion/xml/SchemaManagerFilter.md#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext)) in interface [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) Parameters: elements - The list of elements ([CIElement](../../../contentcompletion/xml/CIElement.md)) to be filtered. context - The [WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) where the list of elements is requested. If null then the given list of content completion elements contains global elements. Returns: The filtered list of [CIElement](../../../contentcompletion/xml/CIElement.md) or null if all elements are rejected by the filter. See Also:
        * [SchemaManagerFilter.filterElements(java.util.List, ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext)](../../../contentcompletion/xml/SchemaManagerFilter.md#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))

### filterAttributes

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../contentcompletion/xml/CIAttribute.md)> filterAttributes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../contentcompletion/xml/CIAttribute.md)> attributes, [WhatAttributesCanGoHereContext](../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) context)
 Description copied from interface: [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md#filterAttributes(java.util.List,ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))
Filters the attributes proposed by the editor content completion schema manager. The original list of attributes is obtained by examining the current document schema and determining what attributes can be inserted in the current element and taking into account the list of existing attributes.
  Specified by: [filterAttributes](../../../contentcompletion/xml/SchemaManagerFilter.md#filterAttributes(java.util.List,ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext)) in interface [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) Parameters: attributes - The list of attributes ([CIAttribute](../../../contentcompletion/xml/CIAttribute.md)) to be filtered. Can be NULL context - The [WhatAttributesCanGoHereContext](../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) where the list of attributes is requested. Returns: The filtered list of [CIAttribute](../../../contentcompletion/xml/CIAttribute.md) or null if all attributes are rejected by the filter. See Also:
        * [SchemaManagerFilter.filterAttributes(java.util.List, ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext)](../../../contentcompletion/xml/SchemaManagerFilter.md#filterAttributes(java.util.List,ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))

### filterAttributeValues

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> filterAttributeValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context)
 Description copied from interface: [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))
Filters the attribute values proposed by the editor content completion schema manager. The original list of attribute values is obtained by examining the current document schema and determining what values are permitted for the current attribute. If the attribute type was an enumeration, then a list with the tokens of the enumeration will be returned for that attribute.
  Specified by: [filterAttributeValues](../../../contentcompletion/xml/SchemaManagerFilter.md#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext)) in interface [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) Parameters: attributeValues - The list of attribute values ([CIValue](../../../contentcompletion/xml/CIValue.md)) to be filtered. context - The [WhatPossibleValuesHasAttributeContext](../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) where the list of attribute values is requested. Returns: The filtered list of [CIValue](../../../contentcompletion/xml/CIValue.md) representing possible values of the attribute or null if all values are rejected by the filter. See Also:
        * [SchemaManagerFilter.filterAttributeValues(java.util.List, ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext)](../../../contentcompletion/xml/SchemaManagerFilter.md#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))

### getLocalName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLocalName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName)

Get the local name from an qualified element or attribute name.
  Parameters: qName - Qualified name. Returns: the local name, or null if the argument is null.
### filterElementValues

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> filterElementValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> elementValues, [Context](../../../contentcompletion/xml/Context.md) context)
 Description copied from interface: [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md#filterElementValues(java.util.List,ro.sync.contentcompletion.xml.Context))
Filters the element values proposed by the editor content completion schema manager. The original list of element values is obtained by examining the current document schema and determining what values are permitted for the current element. If the element type was an enumeration, then a list with the values of the enumeration will be returned for that element.
  Specified by: [filterElementValues](../../../contentcompletion/xml/SchemaManagerFilter.md#filterElementValues(java.util.List,ro.sync.contentcompletion.xml.Context)) in interface [SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md) Parameters: elementValues - The list of element values ([CIValue](../../../contentcompletion/xml/CIValue.md)) to be filtered. context - The [Context](../../../contentcompletion/xml/Context.md) where the list of element values is requested. Returns: The filtered list of [CIValue](../../../contentcompletion/xml/CIValue.md) representing the possible values of the element or null if all values are rejected by the filter. See Also:
        * [SchemaManagerFilter.filterElementValues(java.util.List, ro.sync.contentcompletion.xml.Context)](../../../contentcompletion/xml/SchemaManagerFilter.md#filterElementValues(java.util.List,ro.sync.contentcompletion.xml.Context))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../api/Extension.md#getDescription()) in interface [Extension](../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
