Package [ro.sync.contentcompletion.xml](package-summary.md)

# Interface NodeDescription
    All Known Subinterfaces: [CIElement](CIElement.md)   All Known Implementing Classes: [CIAttribute](CIAttribute.md), [CIElementAdapter](CIElementAdapter.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public interface NodeDescription
Node description is in fact a collection of properties for a node. The node can be either an attribute or an element.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAnnotation](#getAnnotation())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAssertions](#getAssertions())()
Returns the string representation for all assertions.
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
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getModelDescription](#getModelDescription())()
Get the model description.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Get the node(attribute or element) name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOpenContentMode](#getOpenContentMode())()
Returns the mode of the open content.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOpenContentWildcardDescription](#getOpenContentWildcardDescription())()
Returns the description for the open content wildcard.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getPossibleValues](#getPossibleValues())()
Get the possible values as a list of [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) values.
  void [setAssertions](#setAssertions(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) assertionsDescription)
Sets the string representation for the node type assertions.
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
  void [setModelDescription](#setModelDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) modelDescription)
Set the model description for the node.
  void [setOpenContentMode](#setOpenContentMode(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mode)
Sets the mode of the open content.
  void [setOpenContentWildcardDescription](#setOpenContentWildcardDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) wildcardDescription)
Sets the description for the open content wildcard.
  void [setPossiblesValues](#setPossiblesValues(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> possiblesValues)
Set the list of possible values for the node.

## Method Details

### getName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

Get the node(attribute or element) name.
  Returns: The node(attribute or element) name.
### getPossibleValues

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getPossibleValues()

Get the possible values as a list of [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) values.
  Returns: The list of possible values.
### getModelDescription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getModelDescription()

Get the model description.
  Returns: The model description.
### getFacetLengthValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetLengthValue()

Get the value of the LENGTH facet, can be null if it is not defined.
  Returns: The value of the LENGTH facet.
### getFacetMinLengthValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMinLengthValue()

Get the value of the MIN LENGTH facet, can be null if it is not defined.
  Returns: The value of the MIN LENGTH facet.
### getFacetMaxLengthValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMaxLengthValue()

Get the value of the MAX LENGTH facet, can be null if it is not defined.
  Returns: The value of the MAX LENGTH facet.
### getFacetWhitespaceValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetWhitespaceValue()

Get the value of the WHITESPACE facet, can be null if it is not defined.
  Returns: The value of the WHITESPACE facet.
### getFacetMinInclusiveValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMinInclusiveValue()

Get the value of the MIN_INCLUSIVE facet, can be null if it is not defined.
  Returns: The value of the MIN_INCLUSIVE facet.
### getFacetMinExclusiveValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMinExclusiveValue()

Get the value of the MIN_EXCLUSIVE facet, can be null if it is not defined.
  Returns: The value of the MIN_EXCLUSIVE facet.
### getFacetMaxInclusiveValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMaxInclusiveValue()

Get the value of the MAX_INCLUSIVE facet, can be null if it is not defined.
  Returns: The value of the MAX_INCLUSIVE facet.
### getFacetMaxExclusiveValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMaxExclusiveValue()

Get the value of the MAX_EXCLUSIVE facet, can be null if it is not defined.
  Returns: The value of the MAX_EXCLUSIVE facet.
### getFacetTotalDigitsValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetTotalDigitsValue()

Get the value of the TOTAL_DIGITS facet, can be null if it is not defined.
  Returns: The value of the TOTAL_DIGITS facet.
### getFacetFractionDigitsValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetFractionDigitsValue()

Get the value of the FRACTION_DIGITS facet, can be null if it is not defined.
  Returns: The value of the FRACTION_DIGITS facet.
### setFacetFractionDigitsValue

void setFacetFractionDigitsValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fractionDigitsFacetValue)

Set the value of the FRACTION_DIGITS facet.
  Parameters: fractionDigitsFacetValue - The value of the FRACTION_DIGITS facet to set.
### setFacetMaxExclusiveValue

void setFacetMaxExclusiveValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxExclusiveFacetValue)

Set the value of the MAX_EXCLUSIVE facet.
  Parameters: maxExclusiveFacetValue - The value of the MAX_EXCLUSIVE facet to set.
### setFacetMaxInclusiveValue

void setFacetMaxInclusiveValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxInclusiveFacetValue)

Set the value of the MAX_INCLUSIVE facet.
  Parameters: maxInclusiveFacetValue - The value of the MAX_INCLUSIVE facet to set.
### setFacetMaxLengthValue

void setFacetMaxLengthValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxLengthFacetValue)

Set the value of the MAX_LENGTH facet.
  Parameters: maxLengthFacetValue - The value of the MAX_LENGTH facet to set.
### setFacetMinInclusiveValue

void setFacetMinInclusiveValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minInclusiveFacetValue)

Set the value of the MIN_INCLUSIVE facet.
  Parameters: minInclusiveFacetValue - The value of the MIN_INCLUSIVE facet to set.
### setPossiblesValues

void setPossiblesValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> possiblesValues)

Set the list of possible values for the node.
  Parameters: possiblesValues - The list with possible ([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)) values.
### setFacetTotalDigitsValue

void setFacetTotalDigitsValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) totalDigitsFacetValue)

Set the value of the TOTAL_DIGITS facet.
  Parameters: totalDigitsFacetValue - The value of the TOTAL_DIGITS facet to set.
### setFacetWhitespaceValue

void setFacetWhitespaceValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) whitespaceFacetValue)

Set the value of the WHITESPACE facet.
  Parameters: whitespaceFacetValue - The value of the WHITESPACE facet to set.
### setModelDescription

void setModelDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) modelDescription)

Set the model description for the node.
  Parameters: modelDescription - The modelDescription to set.
### setFacetLengthValue

void setFacetLengthValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lengthFacetValue)

Set the value of the LENGTH facet.
  Parameters: lengthFacetValue - The value of the LENGTH facet to set.
### setFacetMinLengthValue

void setFacetMinLengthValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minLengthFacetValue)

Set the value of the MIN_LENGTH facet.
  Parameters: minLengthFacetValue - The value of the MIN_LENGTH facet to set.
### setFacetMinExclusiveValue

void setFacetMinExclusiveValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minExclusiveFacetValue)

Set the value of the MIN_EXCLUSIVE facet.
  Parameters: minExclusiveFacetValue - The value of the MIN_EXCLUSIVE facet to set.
### getFacetPattern

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetPattern()

Get the value of the PATTERN facets as [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html), can be null if is not defined.
  Returns: The PATTERN facets as a [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html).
### setFacetPattern

void setFacetPattern([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) patternFacets)

Set the value of the PATTERN facets.
  Parameters: patternFacets - The value of the PATTERN facets to set.
### getAnnotation

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAnnotation()
  Returns: The node annotation, can be null.
### setAssertions

void setAssertions([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) assertionsDescription)

Sets the string representation for the node type assertions.
  Parameters: assertionsDescription - The string representing all assertions.
### getAssertions

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAssertions()

Returns the string representation for all assertions. The assertions are collected from node type, by example for simple types they are collected using assertion facets. The representation is (assertion1) && (assertion2) && etc.
  Returns: The string containing all assertions. Is null if node type does not have any assertion.
### setOpenContentMode

void setOpenContentMode([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mode)

Sets the mode of the open content. Can be one of 'interleave', 'suffix' or 'none'.
  Parameters: mode - The mode of the open content.
### getOpenContentMode

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOpenContentMode()

Returns the mode of the open content. Null if element type does not contains an open content.
  Returns: The mode of the open content.
### setOpenContentWildcardDescription

void setOpenContentWildcardDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) wildcardDescription)

Sets the description for the open content wildcard.
  Parameters: wildcardDescription - The wildcard description.
### getOpenContentWildcardDescription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOpenContentWildcardDescription()

Returns the description for the open content wildcard.
  Returns: The description for the open content wildcard. Null if wildcard is missing.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
