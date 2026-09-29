Package [ro.sync.contentcompletion.xml](package-summary.md)

# Class CIElementAdapter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.contentcompletion.xml.CIElementAdapter
   All Implemented Interfaces: [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CIElement](CIElement.md)>, [CIElement](CIElement.md), [NodeDescription](NodeDescription.md)   @API(type=EXTENDABLE, src=PRIVATE) public class CIElementAdapter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [CIElement](CIElement.md)
A CIElement adapter. Simplifies the implementation.

## Field Summary

### Fields inherited from interface ro.sync.contentcompletion.xml.[CIElement](CIElement.md)
 [CONTENT_TYPE_ELEMENT_ONLY](CIElement.md#CONTENT_TYPE_ELEMENT_ONLY), [CONTENT_TYPE_EMPTY](CIElement.md#CONTENT_TYPE_EMPTY), [CONTENT_TYPE_MIXED](CIElement.md#CONTENT_TYPE_MIXED), [CONTENT_TYPE_NOT_DETERMINED](CIElement.md#CONTENT_TYPE_NOT_DETERMINED)
## Constructor Summary
 Constructors
Constructor

Description
 [CIElementAdapter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addGuessElement](#addGuessElement(ro.sync.contentcompletion.xml.CIElement))([CIElement](CIElement.md) childElement)
Add a child element to the list of element's children.
  int [compareTo](#compareTo(ro.sync.contentcompletion.xml.CIElement))([CIElement](CIElement.md) o)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAnnotation](#getAnnotation())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAssertions](#getAssertions())()
Returns the string representation for all assertions.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> [getAttributes](#getAttributes())()
Returns the list with the element attributes.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> [getAttributesWithDefaultValues](#getAttributesWithDefaultValues())()
Returns the list with the element attributes which have default values.
  int [getContentType](#getContentType())()
Get the content type of the element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetFractionDigitsValue](#getFacetFractionDigitsValue())()
Get the value of the FRACTION_DIGITS facet, can be null if it is not defined.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetLengthValue](#getFacetLengthValue())()
Get the value of the LENGTH facet, can be null if it is not defined.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetMaxExclusiveValue](#getFacetMaxExclusiveValue())()
Get the value of the MAX_EXCLUSIVE facet, can be null if it is not defined.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetMaxInclusiveValue](#getFacetMaxInclusiveValue())()
Get the value of the MAX_INCLUSIVE facet, can be null if it is not defined.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetMaxLengthValue](#getFacetMaxLengthValue())()
Get the value of the MAX LENGTH facet, can be null if it is not defined.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetMinExclusiveValue](#getFacetMinExclusiveValue())()
Get the value of the MIN_EXCLUSIVE facet, can be null if it is not defined.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetMinInclusiveValue](#getFacetMinInclusiveValue())()
Get the value of the MIN_INCLUSIVE facet, can be null if it is not defined.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetMinLengthValue](#getFacetMinLengthValue())()
Get the value of the MIN LENGTH facet, can be null if it is not defined.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetPattern](#getFacetPattern())()
Get the value of the PATTERN facets as [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html), can be null if is not defined.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetTotalDigitsValue](#getFacetTotalDigitsValue())()
Get the value of the TOTAL_DIGITS facet, can be null if it is not defined.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetWhitespaceValue](#getFacetWhitespaceValue())()
Get the value of the WHITESPACE facet, can be null if it is not defined.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](CIElement.md)> [getGuessElements](#getGuessElements())()
Get the list with the children elements of the current element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getModelDescription](#getModelDescription())()
Get the model description.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Get the node(attribute or element) name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNamespace](#getNamespace())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOpenContentMode](#getOpenContentMode())()
Returns the mode of the open content.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOpenContentWildcardDescription](#getOpenContentWildcardDescription())()
Returns the description for the open content wildcard.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getPossibleValues](#getPossibleValues())()
Get the possible values as a list of [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) values.
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
  void [setAssertions](#setAssertions(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) assertions)
Sets the string representation for the node type assertions.
  void [setAttributes](#setAttributes(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> attributes)
Sets the list with the element attributes.
  void [setContentType](#setContentType(int))(int contentType)
Sets the content type of the element.
  void [setDeclareXmlns](#setDeclareXmlns(boolean))(boolean declareXmlns)
Sets the value of the flag indicating if the xmlns declaration must be added for the element.
  void [setFacetFractionDigitsValue](#setFacetFractionDigitsValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fractionDigitsFacetValue)
Set the value of the FRACTION_DIGITS facet.
  void [setFacetLengthValue](#setFacetLengthValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lengthFacetValue)
Set the value of the LENGTH facet.
  void [setFacetMaxExclusiveValue](#setFacetMaxExclusiveValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxExclusiveFacetValue)
Set the value of the MAX_EXCLUSIVE facet.
  void [setFacetMaxInclusiveValue](#setFacetMaxInclusiveValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxInclusiveFacetValue)
Set the value of the MAX_INCLUSIVE facet.
  void [setFacetMaxLengthValue](#setFacetMaxLengthValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxLengthFacetValue)
Set the value of the MAX_LENGTH facet.
  void [setFacetMinExclusiveValue](#setFacetMinExclusiveValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minExclusiveFacetValue)
Set the value of the MIN_EXCLUSIVE facet.
  void [setFacetMinInclusiveValue](#setFacetMinInclusiveValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minInclusiveFacetValue)
Set the value of the MIN_INCLUSIVE facet.
  void [setFacetMinLengthValue](#setFacetMinLengthValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minLengthFacetValue)
Set the value of the MIN_LENGTH facet.
  void [setFacetPattern](#setFacetPattern(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) patternFacets)
Set the value of the PATTERN facets.
  void [setFacetTotalDigitsValue](#setFacetTotalDigitsValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) totalDigitsFacetValue)
Set the value of the TOTAL_DIGITS facet.
  void [setFacetWhitespaceValue](#setFacetWhitespaceValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) whitespaceFacetValue)
Set the value of the WHITESPACE facet.
  void [setHasFixedValueType](#setHasFixedValueType(boolean))(boolean hasFixedValue)
Set if the element has a fixed value.
  void [setModelDescription](#setModelDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) modelDescription)
Set the model description for the node.
  void [setName](#setName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Set the name of the element.
  void [setNamespace](#setNamespace(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Set the namespace URI for the element.
  void [setNillable](#setNillable(boolean))(boolean nillable)
Sets the flag representing the value of the nillable attribute of element.
  void [setOpenContentMode](#setOpenContentMode(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mode)
Sets the mode of the open content.
  void [setOpenContentWildcardDescription](#setOpenContentWildcardDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) wildcardDescription)
Sets the description for the open content wildcard.
  void [setPossiblesValues](#setPossiblesValues(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> possiblesValues)
Set the list of possible values for the node.
  void [setPrefix](#setPrefix(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix)
Set the prefix associated with the element namespace.
  void [setTypeDescription](#setTypeDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeDescription)
Sets the type description for the current element

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CIElementAdapter

public CIElementAdapter()

## Method Details

### addGuessElement

public void addGuessElement([CIElement](CIElement.md) childElement)
 Description copied from interface: [CIElement](CIElement.md#addGuessElement(ro.sync.contentcompletion.xml.CIElement))
Add a child element to the list of element's children. When the current CIElement is chosen from the list of proposed elements (e.g. the list of proposals from the Content Completion window), the children elements are also inserted. For example if person is the current CIElement, and the list of children contains the elements nameand address, the result of choosing the **person** entry from the Content Completion window will be the insertion of the following sequence:
```

 <person>
     <name>...</name>
     <address>...</address>
 </person>

```
This method can be used in the [SchemaManagerFilter.filterElements(List, WhatElementsCanGoHereContext)](SchemaManagerFilter.md#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))method to add new children to the CIElements proposed by the original SchemaManager.
  Specified by: [addGuessElement](CIElement.md#addGuessElement(ro.sync.contentcompletion.xml.CIElement)) in interface [CIElement](CIElement.md) Parameters: childElement - The [CIElement](CIElement.md) element to be added as child. See Also:
        * [CIElement.addGuessElement(ro.sync.contentcompletion.xml.CIElement)](CIElement.md#addGuessElement(ro.sync.contentcompletion.xml.CIElement))

### getAttributes

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> getAttributes()
 Description copied from interface: [CIElement](CIElement.md#getAttributes())
Returns the list with the element attributes.
  Specified by: [getAttributes](CIElement.md#getAttributes()) in interface [CIElement](CIElement.md) Returns: The list with [CIAttribute](CIAttribute.md) or null if the element has no attributes. See Also:
        * [CIElement.getAttributes()](CIElement.md#getAttributes())

### getAttributesWithDefaultValues

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> getAttributesWithDefaultValues()
 Description copied from interface: [CIElement](CIElement.md#getAttributesWithDefaultValues())
Returns the list with the element attributes which have default values.
  Specified by: [getAttributesWithDefaultValues](CIElement.md#getAttributesWithDefaultValues()) in interface [CIElement](CIElement.md) Returns: The list with [CIAttribute](CIAttribute.md) which have default values or null if the element has no attributes. See Also:
        * [CIElement.getAttributesWithDefaultValues()](CIElement.md#getAttributesWithDefaultValues())

### getContentType

public int getContentType()
 Description copied from interface: [CIElement](CIElement.md#getContentType())
Get the content type of the element.
  Specified by: [getContentType](CIElement.md#getContentType()) in interface [CIElement](CIElement.md) Returns: The content type of the element. Can be one of the constants: [CIElement.CONTENT_TYPE_ELEMENT_ONLY](CIElement.md#CONTENT_TYPE_ELEMENT_ONLY), [CIElement.CONTENT_TYPE_EMPTY](CIElement.md#CONTENT_TYPE_EMPTY), [CIElement.CONTENT_TYPE_MIXED](CIElement.md#CONTENT_TYPE_MIXED), [CIElement.CONTENT_TYPE_NOT_DETERMINED](CIElement.md#CONTENT_TYPE_NOT_DETERMINED). See Also:
        * [CIElement.getContentType()](CIElement.md#getContentType())

### getGuessElements

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](CIElement.md)> getGuessElements()
 Description copied from interface: [CIElement](CIElement.md#getGuessElements())
Get the list with the children elements of the current element. When the current CIElement is chosen from the list of proposed elements (e.g. the list of proposals from the Content Completion window), the children elements are also inserted in the document. For example if person is the current CIElement, and the list of children contains the elements nameand address, the result of choosing the **person** entry from the Content Completion window will be the insertion of the following sequence:
```

 <person>
     <name>...</name>
     <address>...</address>
 </person>

```
This method can be implemented by the CIElements returned by the [SchemaManagerFilter.filterElements(List, WhatElementsCanGoHereContext)](SchemaManagerFilter.md#filterElements(java.util.List,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext)) method in order to return a customized list of children, thus modifying the original list proposed by the SchemaManager.
  Specified by: [getGuessElements](CIElement.md#getGuessElements()) in interface [CIElement](CIElement.md) Returns: A list of [CIElement](CIElement.md) objects, or null if the element accepts no children. See Also:
        * [CIElement.getGuessElements()](CIElement.md#getGuessElements())

### getNamespace

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNamespace()
  Specified by: [getNamespace](CIElement.md#getNamespace()) in interface [CIElement](CIElement.md) Returns: The namespace URI of the element string or null if the element has no namespace. See Also:
        * [CIElement.getNamespace()](CIElement.md#getNamespace())

### getPrefix

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPrefix()
  Specified by: [getPrefix](CIElement.md#getPrefix()) in interface [CIElement](CIElement.md) Returns: The namespace prefix or null if the element has no prefix set. See Also:
        * [CIElement.getPrefix()](CIElement.md#getPrefix())

### getQName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getQName()
 Description copied from interface: [CIElement](CIElement.md#getQName())
Returns the qualified name of the element. It is obtained from the namespace prefix and the local name.
  Specified by: [getQName](CIElement.md#getQName()) in interface [CIElement](CIElement.md) Returns: The qualified name of the element or null if the local name and prefix are null. See Also:
        * [CIElement.getQName()](CIElement.md#getQName())

### getTypeDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTypeDescription()
 Description copied from interface: [CIElement](CIElement.md#getTypeDescription())
Gets the type description for the element.
  Specified by: [getTypeDescription](CIElement.md#getTypeDescription()) in interface [CIElement](CIElement.md) Returns: A [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description of the element type. See Also:
        * [CIElement.getTypeDescription()](CIElement.md#getTypeDescription())

### hasPrefix

public boolean hasPrefix()
  Specified by: [hasPrefix](CIElement.md#hasPrefix()) in interface [CIElement](CIElement.md) Returns: true if a namespace prefix was previously set. See Also:
        * [CIElement.hasPrefix()](CIElement.md#hasPrefix())

### isDeclareXmlns

public boolean isDeclareXmlns()
  Specified by: [isDeclareXmlns](CIElement.md#isDeclareXmlns()) in interface [CIElement](CIElement.md) Returns: true if the element has an xmlns declaration. See Also:
        * [CIElement.isDeclareXmlns()](CIElement.md#isDeclareXmlns())

### isEmpty

public boolean isEmpty()
 Description copied from interface: [CIElement](CIElement.md#isEmpty())
true if the element is empty because it has empty content type or the element type is nillable.
  Specified by: [isEmpty](CIElement.md#isEmpty()) in interface [CIElement](CIElement.md) Returns: true if empty content type or nillable content. See Also:
        * [CIElement.isEmpty()](CIElement.md#isEmpty())

### isNillable

public boolean isNillable()
  Specified by: [isNillable](CIElement.md#isNillable()) in interface [CIElement](CIElement.md) Returns: true if the content of the element is nillable. Used only for XML Schema elements. See Also:
        * [CIElement.isNillable()](CIElement.md#isNillable())

### setAnnotation

public void setAnnotation([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation)
 Description copied from interface: [CIElement](CIElement.md#setAnnotation(java.lang.String))
Sets the annotation for the element.
  Specified by: [setAnnotation](CIElement.md#setAnnotation(java.lang.String)) in interface [CIElement](CIElement.md) Parameters: annotation - A text annotation for the element, or null. See Also:
        * [CIElement.setAnnotation(java.lang.String)](CIElement.md#setAnnotation(java.lang.String))

### setAttributes

public void setAttributes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](CIAttribute.md)> attributes)
 Description copied from interface: [CIElement](CIElement.md#setAttributes(java.util.List))
Sets the list with the element attributes.
  Specified by: [setAttributes](CIElement.md#setAttributes(java.util.List)) in interface [CIElement](CIElement.md) Parameters: attributes - The list of [CIAttribute](CIAttribute.md) to be set. See Also:
        * [CIElement.setAttributes(java.util.List)](CIElement.md#setAttributes(java.util.List))

### setContentType

public void setContentType(int contentType)
 Description copied from interface: [CIElement](CIElement.md#setContentType(int))
Sets the content type of the element.
  Specified by: [setContentType](CIElement.md#setContentType(int)) in interface [CIElement](CIElement.md) Parameters: contentType - The content type of the element. It can be one of the constants: [CIElement.CONTENT_TYPE_ELEMENT_ONLY](CIElement.md#CONTENT_TYPE_ELEMENT_ONLY), [CIElement.CONTENT_TYPE_EMPTY](CIElement.md#CONTENT_TYPE_EMPTY), [CIElement.CONTENT_TYPE_MIXED](CIElement.md#CONTENT_TYPE_MIXED), [CIElement.CONTENT_TYPE_NOT_DETERMINED](CIElement.md#CONTENT_TYPE_NOT_DETERMINED). See Also:
        * [CIElement.setContentType(int)](CIElement.md#setContentType(int))

### setDeclareXmlns

public void setDeclareXmlns(boolean declareXmlns)
 Description copied from interface: [CIElement](CIElement.md#setDeclareXmlns(boolean))
Sets the value of the flag indicating if the xmlns declaration must be added for the element.
  Specified by: [setDeclareXmlns](CIElement.md#setDeclareXmlns(boolean)) in interface [CIElement](CIElement.md) Parameters: declareXmlns - true if the namespace must be declared. See Also:
        * [CIElement.setDeclareXmlns(boolean)](CIElement.md#setDeclareXmlns(boolean))

### setName

public void setName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
 Description copied from interface: [CIElement](CIElement.md#setName(java.lang.String))
Set the name of the element.
  Specified by: [setName](CIElement.md#setName(java.lang.String)) in interface [CIElement](CIElement.md) Parameters: name - the name of the element. See Also:
        * [CIElement.setName(java.lang.String)](CIElement.md#setName(java.lang.String))

### setNamespace

public void setNamespace([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
 Description copied from interface: [CIElement](CIElement.md#setNamespace(java.lang.String))
Set the namespace URI for the element.
  Specified by: [setNamespace](CIElement.md#setNamespace(java.lang.String)) in interface [CIElement](CIElement.md) Parameters: namespace - The namespace URI to be set. See Also:
        * [CIElement.setNamespace(java.lang.String)](CIElement.md#setNamespace(java.lang.String))

### setNillable

public void setNillable(boolean nillable)
 Description copied from interface: [CIElement](CIElement.md#setNillable(boolean))
Sets the flag representing the value of the nillable attribute of element. Used only for elements defined in an XML Schema.
  Specified by: [setNillable](CIElement.md#setNillable(boolean)) in interface [CIElement](CIElement.md) Parameters: nillable - true if the content of the element defined in the XML Schema is nillable. See Also:
        * [CIElement.setNillable(boolean)](CIElement.md#setNillable(boolean))

### setPrefix

public void setPrefix([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix)
 Description copied from interface: [CIElement](CIElement.md#setPrefix(java.lang.String))
Set the prefix associated with the element namespace.
  Specified by: [setPrefix](CIElement.md#setPrefix(java.lang.String)) in interface [CIElement](CIElement.md) Parameters: prefix - The namespace prefix to be set. See Also:
        * [CIElement.setPrefix(java.lang.String)](CIElement.md#setPrefix(java.lang.String))

### setTypeDescription

public void setTypeDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) typeDescription)
 Description copied from interface: [CIElement](CIElement.md#setTypeDescription(java.lang.String))
Sets the type description for the current element
  Specified by: [setTypeDescription](CIElement.md#setTypeDescription(java.lang.String)) in interface [CIElement](CIElement.md) Parameters: typeDescription - The String representing the type description. See Also:
        * [CIElement.setTypeDescription(java.lang.String)](CIElement.md#setTypeDescription(java.lang.String))

### compareTo

public int compareTo([CIElement](CIElement.md) o)
  Specified by: [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html#compareTo(T)) in interface [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CIElement](CIElement.md)> See Also:
        * [Comparable.compareTo(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html#compareTo(T))

### getAnnotation

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAnnotation()
  Specified by: [getAnnotation](NodeDescription.md#getAnnotation()) in interface [NodeDescription](NodeDescription.md) Returns: The node annotation, can be null. See Also:
        * [NodeDescription.getAnnotation()](NodeDescription.md#getAnnotation())

### getFacetFractionDigitsValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetFractionDigitsValue()
 Description copied from interface: [NodeDescription](NodeDescription.md#getFacetFractionDigitsValue())
Get the value of the FRACTION_DIGITS facet, can be null if it is not defined.
  Specified by: [getFacetFractionDigitsValue](NodeDescription.md#getFacetFractionDigitsValue()) in interface [NodeDescription](NodeDescription.md) Returns: The value of the FRACTION_DIGITS facet. See Also:
        * [NodeDescription.getFacetFractionDigitsValue()](NodeDescription.md#getFacetFractionDigitsValue())

### getFacetLengthValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetLengthValue()
 Description copied from interface: [NodeDescription](NodeDescription.md#getFacetLengthValue())
Get the value of the LENGTH facet, can be null if it is not defined.
  Specified by: [getFacetLengthValue](NodeDescription.md#getFacetLengthValue()) in interface [NodeDescription](NodeDescription.md) Returns: The value of the LENGTH facet. See Also:
        * [NodeDescription.getFacetLengthValue()](NodeDescription.md#getFacetLengthValue())

### getFacetMaxExclusiveValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMaxExclusiveValue()
 Description copied from interface: [NodeDescription](NodeDescription.md#getFacetMaxExclusiveValue())
Get the value of the MAX_EXCLUSIVE facet, can be null if it is not defined.
  Specified by: [getFacetMaxExclusiveValue](NodeDescription.md#getFacetMaxExclusiveValue()) in interface [NodeDescription](NodeDescription.md) Returns: The value of the MAX_EXCLUSIVE facet. See Also:
        * [NodeDescription.getFacetMaxExclusiveValue()](NodeDescription.md#getFacetMaxExclusiveValue())

### getFacetMaxInclusiveValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMaxInclusiveValue()
 Description copied from interface: [NodeDescription](NodeDescription.md#getFacetMaxInclusiveValue())
Get the value of the MAX_INCLUSIVE facet, can be null if it is not defined.
  Specified by: [getFacetMaxInclusiveValue](NodeDescription.md#getFacetMaxInclusiveValue()) in interface [NodeDescription](NodeDescription.md) Returns: The value of the MAX_INCLUSIVE facet. See Also:
        * [NodeDescription.getFacetMaxInclusiveValue()](NodeDescription.md#getFacetMaxInclusiveValue())

### getFacetMaxLengthValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMaxLengthValue()
 Description copied from interface: [NodeDescription](NodeDescription.md#getFacetMaxLengthValue())
Get the value of the MAX LENGTH facet, can be null if it is not defined.
  Specified by: [getFacetMaxLengthValue](NodeDescription.md#getFacetMaxLengthValue()) in interface [NodeDescription](NodeDescription.md) Returns: The value of the MAX LENGTH facet. See Also:
        * [NodeDescription.getFacetMaxLengthValue()](NodeDescription.md#getFacetMaxLengthValue())

### getFacetMinExclusiveValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMinExclusiveValue()
 Description copied from interface: [NodeDescription](NodeDescription.md#getFacetMinExclusiveValue())
Get the value of the MIN_EXCLUSIVE facet, can be null if it is not defined.
  Specified by: [getFacetMinExclusiveValue](NodeDescription.md#getFacetMinExclusiveValue()) in interface [NodeDescription](NodeDescription.md) Returns: The value of the MIN_EXCLUSIVE facet. See Also:
        * [NodeDescription.getFacetMinExclusiveValue()](NodeDescription.md#getFacetMinExclusiveValue())

### getFacetMinInclusiveValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMinInclusiveValue()
 Description copied from interface: [NodeDescription](NodeDescription.md#getFacetMinInclusiveValue())
Get the value of the MIN_INCLUSIVE facet, can be null if it is not defined.
  Specified by: [getFacetMinInclusiveValue](NodeDescription.md#getFacetMinInclusiveValue()) in interface [NodeDescription](NodeDescription.md) Returns: The value of the MIN_INCLUSIVE facet. See Also:
        * [NodeDescription.getFacetMinInclusiveValue()](NodeDescription.md#getFacetMinInclusiveValue())

### getFacetMinLengthValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMinLengthValue()
 Description copied from interface: [NodeDescription](NodeDescription.md#getFacetMinLengthValue())
Get the value of the MIN LENGTH facet, can be null if it is not defined.
  Specified by: [getFacetMinLengthValue](NodeDescription.md#getFacetMinLengthValue()) in interface [NodeDescription](NodeDescription.md) Returns: The value of the MIN LENGTH facet. See Also:
        * [NodeDescription.getFacetMinLengthValue()](NodeDescription.md#getFacetMinLengthValue())

### getFacetPattern

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetPattern()
 Description copied from interface: [NodeDescription](NodeDescription.md#getFacetPattern())
Get the value of the PATTERN facets as [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html), can be null if is not defined.
  Specified by: [getFacetPattern](NodeDescription.md#getFacetPattern()) in interface [NodeDescription](NodeDescription.md) Returns: The PATTERN facets as a [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html). See Also:
        * [NodeDescription.getFacetPattern()](NodeDescription.md#getFacetPattern())

### getFacetTotalDigitsValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetTotalDigitsValue()
 Description copied from interface: [NodeDescription](NodeDescription.md#getFacetTotalDigitsValue())
Get the value of the TOTAL_DIGITS facet, can be null if it is not defined.
  Specified by: [getFacetTotalDigitsValue](NodeDescription.md#getFacetTotalDigitsValue()) in interface [NodeDescription](NodeDescription.md) Returns: The value of the TOTAL_DIGITS facet. See Also:
        * [NodeDescription.getFacetTotalDigitsValue()](NodeDescription.md#getFacetTotalDigitsValue())

### getFacetWhitespaceValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetWhitespaceValue()
 Description copied from interface: [NodeDescription](NodeDescription.md#getFacetWhitespaceValue())
Get the value of the WHITESPACE facet, can be null if it is not defined.
  Specified by: [getFacetWhitespaceValue](NodeDescription.md#getFacetWhitespaceValue()) in interface [NodeDescription](NodeDescription.md) Returns: The value of the WHITESPACE facet. See Also:
        * [NodeDescription.getFacetWhitespaceValue()](NodeDescription.md#getFacetWhitespaceValue())

### getModelDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getModelDescription()
 Description copied from interface: [NodeDescription](NodeDescription.md#getModelDescription())
Get the model description.
  Specified by: [getModelDescription](NodeDescription.md#getModelDescription()) in interface [NodeDescription](NodeDescription.md) Returns: The model description. See Also:
        * [NodeDescription.getModelDescription()](NodeDescription.md#getModelDescription())

### getName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()
 Description copied from interface: [NodeDescription](NodeDescription.md#getName())
Get the node(attribute or element) name.
  Specified by: [getName](NodeDescription.md#getName()) in interface [NodeDescription](NodeDescription.md) Returns: The node(attribute or element) name. See Also:
        * [NodeDescription.getName()](NodeDescription.md#getName())

### getPossibleValues

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getPossibleValues()
 Description copied from interface: [NodeDescription](NodeDescription.md#getPossibleValues())
Get the possible values as a list of [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) values.
  Specified by: [getPossibleValues](NodeDescription.md#getPossibleValues()) in interface [NodeDescription](NodeDescription.md) Returns: The list of possible values. See Also:
        * [NodeDescription.getPossibleValues()](NodeDescription.md#getPossibleValues())

### setFacetFractionDigitsValue

public void setFacetFractionDigitsValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fractionDigitsFacetValue)
 Description copied from interface: [NodeDescription](NodeDescription.md#setFacetFractionDigitsValue(java.lang.String))
Set the value of the FRACTION_DIGITS facet.
  Specified by: [setFacetFractionDigitsValue](NodeDescription.md#setFacetFractionDigitsValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: fractionDigitsFacetValue - The value of the FRACTION_DIGITS facet to set. See Also:
        * [NodeDescription.setFacetFractionDigitsValue(java.lang.String)](NodeDescription.md#setFacetFractionDigitsValue(java.lang.String))

### setFacetLengthValue

public void setFacetLengthValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lengthFacetValue)
 Description copied from interface: [NodeDescription](NodeDescription.md#setFacetLengthValue(java.lang.String))
Set the value of the LENGTH facet.
  Specified by: [setFacetLengthValue](NodeDescription.md#setFacetLengthValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: lengthFacetValue - The value of the LENGTH facet to set. See Also:
        * [NodeDescription.setFacetLengthValue(java.lang.String)](NodeDescription.md#setFacetLengthValue(java.lang.String))

### setFacetMaxExclusiveValue

public void setFacetMaxExclusiveValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxExclusiveFacetValue)
 Description copied from interface: [NodeDescription](NodeDescription.md#setFacetMaxExclusiveValue(java.lang.String))
Set the value of the MAX_EXCLUSIVE facet.
  Specified by: [setFacetMaxExclusiveValue](NodeDescription.md#setFacetMaxExclusiveValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: maxExclusiveFacetValue - The value of the MAX_EXCLUSIVE facet to set. See Also:
        * [NodeDescription.setFacetMaxExclusiveValue(java.lang.String)](NodeDescription.md#setFacetMaxExclusiveValue(java.lang.String))

### setFacetMaxInclusiveValue

public void setFacetMaxInclusiveValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxInclusiveFacetValue)
 Description copied from interface: [NodeDescription](NodeDescription.md#setFacetMaxInclusiveValue(java.lang.String))
Set the value of the MAX_INCLUSIVE facet.
  Specified by: [setFacetMaxInclusiveValue](NodeDescription.md#setFacetMaxInclusiveValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: maxInclusiveFacetValue - The value of the MAX_INCLUSIVE facet to set. See Also:
        * [NodeDescription.setFacetMaxInclusiveValue(java.lang.String)](NodeDescription.md#setFacetMaxInclusiveValue(java.lang.String))

### setFacetMaxLengthValue

public void setFacetMaxLengthValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxLengthFacetValue)
 Description copied from interface: [NodeDescription](NodeDescription.md#setFacetMaxLengthValue(java.lang.String))
Set the value of the MAX_LENGTH facet.
  Specified by: [setFacetMaxLengthValue](NodeDescription.md#setFacetMaxLengthValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: maxLengthFacetValue - The value of the MAX_LENGTH facet to set. See Also:
        * [NodeDescription.setFacetMaxLengthValue(java.lang.String)](NodeDescription.md#setFacetMaxLengthValue(java.lang.String))

### setFacetMinExclusiveValue

public void setFacetMinExclusiveValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minExclusiveFacetValue)
 Description copied from interface: [NodeDescription](NodeDescription.md#setFacetMinExclusiveValue(java.lang.String))
Set the value of the MIN_EXCLUSIVE facet.
  Specified by: [setFacetMinExclusiveValue](NodeDescription.md#setFacetMinExclusiveValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: minExclusiveFacetValue - The value of the MIN_EXCLUSIVE facet to set. See Also:
        * [NodeDescription.setFacetMinExclusiveValue(java.lang.String)](NodeDescription.md#setFacetMinExclusiveValue(java.lang.String))

### setFacetMinInclusiveValue

public void setFacetMinInclusiveValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minInclusiveFacetValue)
 Description copied from interface: [NodeDescription](NodeDescription.md#setFacetMinInclusiveValue(java.lang.String))
Set the value of the MIN_INCLUSIVE facet.
  Specified by: [setFacetMinInclusiveValue](NodeDescription.md#setFacetMinInclusiveValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: minInclusiveFacetValue - The value of the MIN_INCLUSIVE facet to set. See Also:
        * [NodeDescription.setFacetMinInclusiveValue(java.lang.String)](NodeDescription.md#setFacetMinInclusiveValue(java.lang.String))

### setFacetMinLengthValue

public void setFacetMinLengthValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minLengthFacetValue)
 Description copied from interface: [NodeDescription](NodeDescription.md#setFacetMinLengthValue(java.lang.String))
Set the value of the MIN_LENGTH facet.
  Specified by: [setFacetMinLengthValue](NodeDescription.md#setFacetMinLengthValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: minLengthFacetValue - The value of the MIN_LENGTH facet to set. See Also:
        * [NodeDescription.setFacetMinLengthValue(java.lang.String)](NodeDescription.md#setFacetMinLengthValue(java.lang.String))

### setFacetPattern

public void setFacetPattern([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) patternFacets)
 Description copied from interface: [NodeDescription](NodeDescription.md#setFacetPattern(java.lang.String))
Set the value of the PATTERN facets.
  Specified by: [setFacetPattern](NodeDescription.md#setFacetPattern(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: patternFacets - The value of the PATTERN facets to set. See Also:
        * [NodeDescription.setFacetPattern(java.lang.String)](NodeDescription.md#setFacetPattern(java.lang.String))

### setFacetTotalDigitsValue

public void setFacetTotalDigitsValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) totalDigitsFacetValue)
 Description copied from interface: [NodeDescription](NodeDescription.md#setFacetTotalDigitsValue(java.lang.String))
Set the value of the TOTAL_DIGITS facet.
  Specified by: [setFacetTotalDigitsValue](NodeDescription.md#setFacetTotalDigitsValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: totalDigitsFacetValue - The value of the TOTAL_DIGITS facet to set. See Also:
        * [NodeDescription.setFacetTotalDigitsValue(java.lang.String)](NodeDescription.md#setFacetTotalDigitsValue(java.lang.String))

### setFacetWhitespaceValue

public void setFacetWhitespaceValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) whitespaceFacetValue)
 Description copied from interface: [NodeDescription](NodeDescription.md#setFacetWhitespaceValue(java.lang.String))
Set the value of the WHITESPACE facet.
  Specified by: [setFacetWhitespaceValue](NodeDescription.md#setFacetWhitespaceValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: whitespaceFacetValue - The value of the WHITESPACE facet to set. See Also:
        * [NodeDescription.setFacetWhitespaceValue(java.lang.String)](NodeDescription.md#setFacetWhitespaceValue(java.lang.String))

### setModelDescription

public void setModelDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) modelDescription)
 Description copied from interface: [NodeDescription](NodeDescription.md#setModelDescription(java.lang.String))
Set the model description for the node.
  Specified by: [setModelDescription](NodeDescription.md#setModelDescription(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: modelDescription - The modelDescription to set. See Also:
        * [NodeDescription.setModelDescription(java.lang.String)](NodeDescription.md#setModelDescription(java.lang.String))

### setPossiblesValues

public void setPossiblesValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> possiblesValues)
 Description copied from interface: [NodeDescription](NodeDescription.md#setPossiblesValues(java.util.List))
Set the list of possible values for the node.
  Specified by: [setPossiblesValues](NodeDescription.md#setPossiblesValues(java.util.List)) in interface [NodeDescription](NodeDescription.md) Parameters: possiblesValues - The list with possible ([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)) values. See Also:
        * [NodeDescription.setPossiblesValues(java.util.List)](NodeDescription.md#setPossiblesValues(java.util.List))

### setAssertions

public void setAssertions([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) assertions)
 Description copied from interface: [NodeDescription](NodeDescription.md#setAssertions(java.lang.String))
Sets the string representation for the node type assertions.
  Specified by: [setAssertions](NodeDescription.md#setAssertions(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: assertions - The string representing all assertions. See Also:
        * [NodeDescription.setAssertions(String)](NodeDescription.md#setAssertions(java.lang.String))

### getAssertions

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAssertions()
 Description copied from interface: [NodeDescription](NodeDescription.md#getAssertions())
Returns the string representation for all assertions. The assertions are collected from node type, by example for simple types they are collected using assertion facets. The representation is (assertion1) && (assertion2) && etc.
  Specified by: [getAssertions](NodeDescription.md#getAssertions()) in interface [NodeDescription](NodeDescription.md) Returns: The string containing all assertions. Is null if node type does not have any assertion. See Also:
        * [NodeDescription.getAssertions()](NodeDescription.md#getAssertions())

### setOpenContentMode

public void setOpenContentMode([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mode)
 Description copied from interface: [NodeDescription](NodeDescription.md#setOpenContentMode(java.lang.String))
Sets the mode of the open content. Can be one of 'interleave', 'suffix' or 'none'.
  Specified by: [setOpenContentMode](NodeDescription.md#setOpenContentMode(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: mode - The mode of the open content. See Also:
        * [NodeDescription.setOpenContentMode(java.lang.String)](NodeDescription.md#setOpenContentMode(java.lang.String))

### getOpenContentMode

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOpenContentMode()
 Description copied from interface: [NodeDescription](NodeDescription.md#getOpenContentMode())
Returns the mode of the open content. Null if element type does not contains an open content.
  Specified by: [getOpenContentMode](NodeDescription.md#getOpenContentMode()) in interface [NodeDescription](NodeDescription.md) Returns: The mode of the open content. See Also:
        * [NodeDescription.getOpenContentMode()](NodeDescription.md#getOpenContentMode())

### setOpenContentWildcardDescription

public void setOpenContentWildcardDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) wildcardDescription)
 Description copied from interface: [NodeDescription](NodeDescription.md#setOpenContentWildcardDescription(java.lang.String))
Sets the description for the open content wildcard.
  Specified by: [setOpenContentWildcardDescription](NodeDescription.md#setOpenContentWildcardDescription(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: wildcardDescription - The wildcard description. See Also:
        * [NodeDescription.setOpenContentWildcardDescription(java.lang.String)](NodeDescription.md#setOpenContentWildcardDescription(java.lang.String))

### getOpenContentWildcardDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOpenContentWildcardDescription()
 Description copied from interface: [NodeDescription](NodeDescription.md#getOpenContentWildcardDescription())
Returns the description for the open content wildcard.
  Specified by: [getOpenContentWildcardDescription](NodeDescription.md#getOpenContentWildcardDescription()) in interface [NodeDescription](NodeDescription.md) Returns: The description for the open content wildcard. Null if wildcard is missing. See Also:
        * [NodeDescription.getOpenContentWildcardDescription()](NodeDescription.md#getOpenContentWildcardDescription())

### hasFixedValue

public boolean hasFixedValue()
 Description copied from interface: [CIElement](CIElement.md#hasFixedValue())
true if the element has a fixed value.
  Specified by: [hasFixedValue](CIElement.md#hasFixedValue()) in interface [CIElement](CIElement.md) Returns: true if the element has a fixed value. See Also:
        * [CIElement.hasFixedValue()](CIElement.md#hasFixedValue())

### setHasFixedValueType

public void setHasFixedValueType(boolean hasFixedValue)
 Description copied from interface: [CIElement](CIElement.md#setHasFixedValueType(boolean))
Set if the element has a fixed value.
  Specified by: [setHasFixedValueType](CIElement.md#setHasFixedValueType(boolean)) in interface [CIElement](CIElement.md) Parameters: hasFixedValue - true if the element has a fixed value. See Also:
        * [CIElement.setHasFixedValueType(boolean)](CIElement.md#setHasFixedValueType(boolean))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
