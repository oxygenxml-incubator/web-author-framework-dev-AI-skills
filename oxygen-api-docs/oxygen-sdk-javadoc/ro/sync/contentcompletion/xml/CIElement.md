Package [ro.sync.contentcompletion.xml](package-summary.md)

# Interface CIElement
    All Superinterfaces: [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CIElement](CIElement.md)>, [NodeDescription](NodeDescription.md)   All Known Implementing Classes: [CIElementAdapter](CIElementAdapter.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public interface CIElementextends [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CIElement](CIElement.md)>, [NodeDescription](NodeDescription.md)
Interface for objects holding information about element proposals used in the content completion process.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [CONTENT_TYPE_ELEMENT_ONLY](#CONTENT_TYPE_ELEMENT_ONLY)
Elements with complex content, element only content type.
  static final int [CONTENT_TYPE_EMPTY](#CONTENT_TYPE_EMPTY)
Elements with complex content, empty content type.
  static final int [CONTENT_TYPE_MIXED](#CONTENT_TYPE_MIXED)
Elements with complex content, mixed content type.
  static final int [CONTENT_TYPE_NOT_DETERMINED](#CONTENT_TYPE_NOT_DETERMINED)
Type for elements with simple content.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addGuessElement](#addGuessElement(ro.sync.contentcompletion.xml.CIElement))([CIElement](CIElement.md) childElement)
Add a child element to the list of element's children.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> [getAttributes](#getAttributes())()
Returns the list with the element attributes.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> [getAttributesWithDefaultValues](#getAttributesWithDefaultValues())()
Returns the list with the element attributes which have default values.
  int [getContentType](#getContentType())()
Get the content type of the element.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](CIElement.md)> [getGuessElements](#getGuessElements())()
Get the list with the children elements of the current element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNamespace](#getNamespace())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPrefix](#getPrefix())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getQName](#getQName())()
Returns the qualified name of the element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTypeDescription](#getTypeDescription())()
Gets the type description for the element.
  boolean [hasFixedValue](#hasFixedValue())()
true if the element has a fixed value.
  boolean [hasPrefix](#hasPrefix())()

 boolean [isDeclareXmlns](#isDeclareXmlns())()

 boolean [isEmpty](#isEmpty())()
true if the element is empty because it has empty content type or the element type is nillable.
  boolean [isNillable](#isNillable())()

 void [setAnnotation](#setAnnotation(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation)
Sets the annotation for the element.
  void [setAttributes](#setAttributes(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> attributes)
Sets the list with the element attributes.
  void [setContentType](#setContentType(int))(int contentType)
Sets the content type of the element.
  void [setDeclareXmlns](#setDeclareXmlns(boolean))(boolean declareXmlns)
Sets the value of the flag indicating if the xmlns declaration must be added for the element.
  void [setHasFixedValueType](#setHasFixedValueType(boolean))(boolean hasFixedValue)
Set if the element has a fixed value.
  void [setName](#setName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Set the name of the element.
  void [setNamespace](#setNamespace(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Set the namespace URI for the element.
  void [setNillable](#setNillable(boolean))(boolean nillable)
Sets the flag representing the value of the nillable attribute of element.
  void [setPrefix](#setPrefix(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix)
Set the prefix associated with the element namespace.
  void [setTypeDescription](#setTypeDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeDescription)
Sets the type description for the current element

### Methods inherited from interface java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)
 [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html#compareTo(T))
### Methods inherited from interface ro.sync.contentcompletion.xml.[NodeDescription](NodeDescription.md)
 [getAnnotation](NodeDescription.md#getAnnotation()), [getAssertions](NodeDescription.md#getAssertions()), [getFacetFractionDigitsValue](NodeDescription.md#getFacetFractionDigitsValue()), [getFacetLengthValue](NodeDescription.md#getFacetLengthValue()), [getFacetMaxExclusiveValue](NodeDescription.md#getFacetMaxExclusiveValue()), [getFacetMaxInclusiveValue](NodeDescription.md#getFacetMaxInclusiveValue()), [getFacetMaxLengthValue](NodeDescription.md#getFacetMaxLengthValue()), [getFacetMinExclusiveValue](NodeDescription.md#getFacetMinExclusiveValue()), [getFacetMinInclusiveValue](NodeDescription.md#getFacetMinInclusiveValue()), [getFacetMinLengthValue](NodeDescription.md#getFacetMinLengthValue()), [getFacetPattern](NodeDescription.md#getFacetPattern()), [getFacetTotalDigitsValue](NodeDescription.md#getFacetTotalDigitsValue()), [getFacetWhitespaceValue](NodeDescription.md#getFacetWhitespaceValue()), [getModelDescription](NodeDescription.md#getModelDescription()), [getName](NodeDescription.md#getName()), [getOpenContentMode](NodeDescription.md#getOpenContentMode()), [getOpenContentWildcardDescription](NodeDescription.md#getOpenContentWildcardDescription()), [getPossibleValues](NodeDescription.md#getPossibleValues()), [setAssertions](NodeDescription.md#setAssertions(java.lang.String)), [setFacetFractionDigitsValue](NodeDescription.md#setFacetFractionDigitsValue(java.lang.String)), [setFacetLengthValue](NodeDescription.md#setFacetLengthValue(java.lang.String)), [setFacetMaxExclusiveValue](NodeDescription.md#setFacetMaxExclusiveValue(java.lang.String)), [setFacetMaxInclusiveValue](NodeDescription.md#setFacetMaxInclusiveValue(java.lang.String)), [setFacetMaxLengthValue](NodeDescription.md#setFacetMaxLengthValue(java.lang.String)), [setFacetMinExclusiveValue](NodeDescription.md#setFacetMinExclusiveValue(java.lang.String)), [setFacetMinInclusiveValue](NodeDescription.md#setFacetMinInclusiveValue(java.lang.String)), [setFacetMinLengthValue](NodeDescription.md#setFacetMinLengthValue(java.lang.String)), [setFacetPattern](NodeDescription.md#setFacetPattern(java.lang.String)), [setFacetTotalDigitsValue](NodeDescription.md#setFacetTotalDigitsValue(java.lang.String)), [setFacetWhitespaceValue](NodeDescription.md#setFacetWhitespaceValue(java.lang.String)), [setModelDescription](NodeDescription.md#setModelDescription(java.lang.String)), [setOpenContentMode](NodeDescription.md#setOpenContentMode(java.lang.String)), [setOpenContentWildcardDescription](NodeDescription.md#setOpenContentWildcardDescription(java.lang.String)), [setPossiblesValues](NodeDescription.md#setPossiblesValues(java.util.List))
## Field Details

### CONTENT_TYPE_NOT_DETERMINED

static final int CONTENT_TYPE_NOT_DETERMINED

Type for elements with simple content. The value is -1
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIElement.CONTENT_TYPE_NOT_DETERMINED)

### CONTENT_TYPE_EMPTY

static final int CONTENT_TYPE_EMPTY

Elements with complex content, empty content type. The value is 1.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIElement.CONTENT_TYPE_EMPTY)

### CONTENT_TYPE_ELEMENT_ONLY

static final int CONTENT_TYPE_ELEMENT_ONLY

Elements with complex content, element only content type. The value is 2.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIElement.CONTENT_TYPE_ELEMENT_ONLY)

### CONTENT_TYPE_MIXED

static final int CONTENT_TYPE_MIXED

Elements with complex content, mixed content type. The value is 3.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIElement.CONTENT_TYPE_MIXED)

## Method Details

### getGuessElements

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](CIElement.md)> getGuessElements()

Get the list with the children elements of the current element. When the current CIElement is chosen from the list of proposed elements (e.g. the list of proposals from the Content Completion window), the children elements are also inserted in the document. For example if person is the current CIElement, and the list of children contains the elements nameand address, the result of choosing the **person** entry from the Content Completion window will be the insertion of the following sequence:
```

 <person>
     <name>...</name>
     <address>...</address>
 </person>

```
This method can be implemented by the CIElements returned by the [SchemaManagerFilter.filterElements(List, WhatElementsCanGoHereContext)](SchemaManagerFilter.md#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext)) method in order to return a customized list of children, thus modifying the original list proposed by the SchemaManager.
  Returns: A list of [CIElement](CIElement.md) objects, or null if the element accepts no children.
### addGuessElement

void addGuessElement([CIElement](CIElement.md) childElement)

Add a child element to the list of element's children. When the current CIElement is chosen from the list of proposed elements (e.g. the list of proposals from the Content Completion window), the children elements are also inserted. For example if person is the current CIElement, and the list of children contains the elements nameand address, the result of choosing the **person** entry from the Content Completion window will be the insertion of the following sequence:
```

 <person>
     <name>...</name>
     <address>...</address>
 </person>

```
This method can be used in the [SchemaManagerFilter.filterElements(List, WhatElementsCanGoHereContext)](SchemaManagerFilter.md#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))method to add new children to the CIElements proposed by the original SchemaManager.
  Parameters: childElement - The [CIElement](CIElement.md) element to be added as child.
### getNamespace

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNamespace()
  Returns: The namespace URI of the element string or null if the element has no namespace.
### setDeclareXmlns

void setDeclareXmlns(boolean declareXmlns)

Sets the value of the flag indicating if the xmlns declaration must be added for the element.
  Parameters: declareXmlns - true if the namespace must be declared.
### setContentType

void setContentType(int contentType)

Sets the content type of the element.
  Parameters: contentType - The content type of the element. It can be one of the constants: [CONTENT_TYPE_ELEMENT_ONLY](#CONTENT_TYPE_ELEMENT_ONLY), [CONTENT_TYPE_EMPTY](#CONTENT_TYPE_EMPTY), [CONTENT_TYPE_MIXED](#CONTENT_TYPE_MIXED), [CONTENT_TYPE_NOT_DETERMINED](#CONTENT_TYPE_NOT_DETERMINED).
### setHasFixedValueType

void setHasFixedValueType(boolean hasFixedValue)

Set if the element has a fixed value.
  Parameters: hasFixedValue - true if the element has a fixed value.
### isEmpty

boolean isEmpty()

true if the element is empty because it has empty content type or the element type is nillable.
  Returns: true if empty content type or nillable content.
### hasFixedValue

boolean hasFixedValue()

true if the element has a fixed value.
  Returns: true if the element has a fixed value.
### getContentType

int getContentType()

Get the content type of the element.
  Returns: The content type of the element. Can be one of the constants: [CONTENT_TYPE_ELEMENT_ONLY](#CONTENT_TYPE_ELEMENT_ONLY), [CONTENT_TYPE_EMPTY](#CONTENT_TYPE_EMPTY), [CONTENT_TYPE_MIXED](#CONTENT_TYPE_MIXED), [CONTENT_TYPE_NOT_DETERMINED](#CONTENT_TYPE_NOT_DETERMINED).
### isDeclareXmlns

boolean isDeclareXmlns()
  Returns: true if the element has an xmlns declaration.
### setName

void setName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Set the name of the element.
  Parameters: name - the name of the element.
### setPrefix

void setPrefix([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix)

Set the prefix associated with the element namespace.
  Parameters: prefix - The namespace prefix to be set.
### setNamespace

void setNamespace([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)

Set the namespace URI for the element.
  Parameters: namespace - The namespace URI to be set.
### getQName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getQName()

Returns the qualified name of the element. It is obtained from the namespace prefix and the local name.
  Returns: The qualified name of the element or null if the local name and prefix are null.
### getAttributes

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> getAttributes()

Returns the list with the element attributes.
  Returns: The list with [CIAttribute](CIAttribute.md) or null if the element has no attributes.
### getAttributesWithDefaultValues

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> getAttributesWithDefaultValues()

Returns the list with the element attributes which have default values.
  Returns: The list with [CIAttribute](CIAttribute.md) which have default values or null if the element has no attributes.
### setAttributes

void setAttributes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> attributes)

Sets the list with the element attributes.
  Parameters: attributes - The list of [CIAttribute](CIAttribute.md) to be set.
### hasPrefix

boolean hasPrefix()
  Returns: true if a namespace prefix was previously set.
### getPrefix

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPrefix()
  Returns: The namespace prefix or null if the element has no prefix set.
### setAnnotation

void setAnnotation([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation)

Sets the annotation for the element.
  Parameters: annotation - A text annotation for the element, or null.
### getTypeDescription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTypeDescription()

Gets the type description for the element.
  Returns: A [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description of the element type.
### setTypeDescription

void setTypeDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeDescription)

Sets the type description for the current element
  Parameters: typeDescription - The String representing the type description.
### setNillable

void setNillable(boolean nillable)

Sets the flag representing the value of the nillable attribute of element. Used only for elements defined in an XML Schema.
  Parameters: nillable - true if the content of the element defined in the XML Schema is nillable.
### isNillable

boolean isNillable()
  Returns: true if the content of the element is nillable. Used only for XML Schema elements.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
