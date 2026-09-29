Package [ro.sync.contentcompletion.xml](package-summary.md)

# Class CIAttribute

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.contentcompletion.xml.CIAttribute
   All Implemented Interfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CIAttribute](CIAttribute.md)>, [NodeDescription](NodeDescription.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class CIAttribute extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CIAttribute](CIAttribute.md)>, [NodeDescription](NodeDescription.md), [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)
Interface for objects holding information about attributes used in the content completion process.

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static interface  [CIAttribute.DefaultValueProvider](CIAttribute.DefaultValueProvider.md)
Default value provider for an attribute.
  static enum  [CIAttribute.EditableState](CIAttribute.EditableState.md)
The editable state of the attribute.

## Constructor Summary
 Constructors
Constructor

Description
 [CIAttribute](#%3Cinit%3E())()
Default Constructor.
  [CIAttribute](#%3Cinit%3E(java.lang.String,boolean,boolean,java.lang.String,java.util.List))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, boolean required, boolean fixed, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> possibleValues)
Constructor.
  [CIAttribute](#%3Cinit%3E(java.lang.String,java.lang.String,boolean,boolean,java.lang.String,java.util.List))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, boolean required, boolean fixed, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> possibleValues)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()
Allows cloning.
  int [compareTo](#compareTo(ro.sync.contentcompletion.xml.CIAttribute))([CIAttribute](CIAttribute.md) otherAttribute)
Compare two attributes based on the string obtained by concatenating the name and the namespace of each attribute.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAnnotation](#getAnnotation())()
Get the annotation for the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAssertions](#getAssertions())()
Returns the string representation for all assertions.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultValue](#getDefaultValue())()
Gets the default value attribute of the attribute.
  [CIAttribute.EditableState](CIAttribute.EditableState.md) [getEditableState](#getEditableState())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetFractionDigitsValue](#getFacetFractionDigitsValue())()
Gets the value of the FRACTION_DIGITS facet corresponding to the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetLengthValue](#getFacetLengthValue())()
Gets the value of the LENGTH facet corresponding to the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetMaxExclusiveValue](#getFacetMaxExclusiveValue())()
Gets the value of the MAX_EXCLUSIVE facet corresponding to the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetMaxInclusiveValue](#getFacetMaxInclusiveValue())()
Gets the value of the MAX_INCLUSIVE facet corresponding to the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetMaxLengthValue](#getFacetMaxLengthValue())()
Gets the value of the MAX_LENGTH facet corresponding to the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetMinExclusiveValue](#getFacetMinExclusiveValue())()
Gets the value of the MIN_EXCLUSIVE facet corresponding to the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetMinInclusiveValue](#getFacetMinInclusiveValue())()
Gets the value of the MIN_INCLUSIVE facet corresponding to the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetMinLengthValue](#getFacetMinLengthValue())()
Gets the value of the MIN_LENGTH facet corresponding to the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetPattern](#getFacetPattern())()
Gets the value of the PATTERN facet corresponding to the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetTotalDigitsValue](#getFacetTotalDigitsValue())()
Gets the value of the TOTAL_DIGITS facet corresponding to the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFacetWhitespaceValue](#getFacetWhitespaceValue())()
Gets the value of the WHITESPACE facet corresponding to the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getModelDescription](#getModelDescription())()
Gets the model description.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Gets the QName of the attribute in almost all cases.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNamespace](#getNamespace())()
Gets the namespace attribute of the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOpenContentMode](#getOpenContentMode())()
Returns the mode of the open content.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOpenContentWildcardDescription](#getOpenContentWildcardDescription())()
Returns the description for the open content wildcard.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getPossibleValues](#getPossibleValues())()
Gets the possible values this attribute can have.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPrefix](#getPrefix())()
Get the attribute prefix.
  boolean [hasDefaultValue](#hasDefaultValue())()
Check if has default value attribute of the attribute.
  int [hashCode](#hashCode())()

 boolean [isAttributeNameQualified](#isAttributeNameQualified())()
Returns true if the name of the attribute is a QName.
  boolean [isDeclareXmlns](#isDeclareXmlns())()
Check if attribute should add an xmlns declaration.
  boolean [isFixed](#isFixed())()
Find if the attribute is fixed.
  boolean [isRequired](#isRequired())()
Gets the required attribute of the attribute.
  void [setAnnotation](#setAnnotation(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation)
Set the annotation for the attribute.
  void [setAssertions](#setAssertions(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) assertionsDescription)
Sets the string representation for the node type assertions.
  void [setDeclareXmlns](#setDeclareXmlns(boolean))(boolean declareXmlns)
Set if the attribute should add an xmlns declaration.
  void [setDefaultValue](#setDefaultValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)
Sets the default value attribute of the attribute.
  void [setEditableState](#setEditableState(ro.sync.contentcompletion.xml.CIAttribute.EditableState))([CIAttribute.EditableState](CIAttribute.EditableState.md) editableState)

 void [setFacetFractionDigitsValue](#setFacetFractionDigitsValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fractionDigitsFacetValue)
Sets the value of the FRACTION_DIGITS facet corresponding to the attribute.
  void [setFacetLengthValue](#setFacetLengthValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lengthFacetValue)
Sets the value of the LENGTH facet corresponding to the attribute.
  void [setFacetMaxExclusiveValue](#setFacetMaxExclusiveValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxExclusiveFacetValue)
Sets the value of the MAX_EXCLUSIVE facet corresponding to the attribute.
  void [setFacetMaxInclusiveValue](#setFacetMaxInclusiveValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxInclusiveFacetValue)
Sets the value of the MAX_INCLUSIVE facet corresponding to the attribute.
  void [setFacetMaxLengthValue](#setFacetMaxLengthValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxLengthFacetValue)
Sets the value of the MAX_LENGTH facet corresponding to the attribute.
  void [setFacetMinExclusiveValue](#setFacetMinExclusiveValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minExclusiveFacetValue)
Sets the value of the MIN_EXCLUSIVE facet corresponding to the attribute.
  void [setFacetMinInclusiveValue](#setFacetMinInclusiveValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minInclusiveFacetValue)
Sets the value of the MIN_INCLUSIVE facet corresponding to the attribute.
  void [setFacetMinLengthValue](#setFacetMinLengthValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minLengthFacetValue)
Sets the value of the MIN_LENGTH facet corresponding to the attribute.
  void [setFacetPattern](#setFacetPattern(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) patternFacets)
Sets the value of the PATTERN facet corresponding to the attribute.
  void [setFacetTotalDigitsValue](#setFacetTotalDigitsValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) totalDigitsFacetValue)
Sets the value of the TOTAL_DIGITS facet corresponding to the attribute.
  void [setFacetWhitespaceValue](#setFacetWhitespaceValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) whitespaceFacetValue)
Sets the value of the WHITESPACE facet corresponding to the attribute.
  void [setFixed](#setFixed(boolean))(boolean fixed)
Sets the fixed mode of the attribute.
  void [setModelDescription](#setModelDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) modelDescription)
Sets the model description.
  void [setName](#setName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Sets the local name of the attribute.
  void [setNamespace](#setNamespace(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Sets the namespace value for the attribute.
  void [setOpenContentMode](#setOpenContentMode(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mode)
Sets the mode of the open content.
  void [setOpenContentWildcardDescription](#setOpenContentWildcardDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) wildcardDescription)
Sets the description for the open content wildcard.
  void [setOverridingDefaultValueProvider](#setOverridingDefaultValueProvider(ro.sync.contentcompletion.xml.CIAttribute.DefaultValueProvider))([CIAttribute.DefaultValueProvider](CIAttribute.DefaultValueProvider.md) defaultValueProvider)
Sets the default value provider that overrides the default value.
  void [setPossiblesValues](#setPossiblesValues(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> possiblesValues)
Sets the possible values this attribute can have.
  void [setPrefix](#setPrefix(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix)
Set the attribute prefix.
  void [setRequired](#setRequired(boolean))(boolean required)
Sets the required value for the attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CIAttribute

public CIAttribute()

Default Constructor.

### CIAttribute

public CIAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, boolean required, boolean fixed, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> possibleValues)

Constructor.
  Parameters: name - The attribute name. required - True if the attribute is required. fixed - True if the attribute is fixed. defaultValue - The default value of the attribute. possibleValues - The list of possible values for the attribute.
### CIAttribute

public CIAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, boolean required, boolean fixed, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> possibleValues)

Constructor.
  Parameters: namespace - The attribute namespace. name - The attribute name. required - True if the attribute is required. fixed - True if the attribute is fixed. defaultValue - The default value of the attribute. possibleValues - The list of possible values for the attribute.
## Method Details

### getEditableState

public [CIAttribute.EditableState](CIAttribute.EditableState.md) getEditableState()
  Returns: Returns the editable state.
### setEditableState

public void setEditableState([CIAttribute.EditableState](CIAttribute.EditableState.md) editableState)
  Parameters: editableState - The editable state to set.
### isFixed

public boolean isFixed()

Find if the attribute is fixed.
  Returns: true if the attribute is fixed.
### getName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

Gets the QName of the attribute in almost all cases. In the case when the namespace of the attribute is not declared, then this method returns the local name. To verify this situation you can use the method [isDeclareXmlns()](#isDeclareXmlns()).
  Specified by: [getName](NodeDescription.md#getName()) in interface [NodeDescription](NodeDescription.md) Returns: The attribute qualified name (QName). The local name is returned when the namespace declaration is missing.
### setName

public void setName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Sets the local name of the attribute.
  Parameters: name - The local name of the attribute to be set.
### getNamespace

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNamespace()

Gets the namespace attribute of the attribute.
  Returns: The namespace of the attribute.
### isRequired

public boolean isRequired()

Gets the required attribute of the attribute.
  Returns: The required value of the attribute.
### getDefaultValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultValue()

Gets the default value attribute of the attribute.
  Returns: The default value or null if a default value was not previously set, nor the default value provider was set.
### hasDefaultValue

public boolean hasDefaultValue()

Check if has default value attribute of the attribute.
  Returns: true if has default value for attribute.
### getPossibleValues

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getPossibleValues()

Gets the possible values this attribute can have.
  Specified by: [getPossibleValues](NodeDescription.md#getPossibleValues()) in interface [NodeDescription](NodeDescription.md) Returns: The list of possible values, or null if a possible values list cannot be determined.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### compareTo

public int compareTo([CIAttribute](CIAttribute.md) otherAttribute)

Compare two attributes based on the string obtained by concatenating the name and the namespace of each attribute.
  Specified by: [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html#compareTo(T)) in interface [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CIAttribute](CIAttribute.md)> Parameters: otherAttribute - The CIAttribute to compare with. Returns: a negative integer, zero, or a positive integer as this attribute is less than, equal to, or greater than the specified attribute.
### getFacetFractionDigitsValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetFractionDigitsValue()

Gets the value of the FRACTION_DIGITS facet corresponding to the attribute.
  Specified by: [getFacetFractionDigitsValue](NodeDescription.md#getFacetFractionDigitsValue()) in interface [NodeDescription](NodeDescription.md) Returns: Returns the value of the FRACTION_DIGITS facet. Can be null.
### setFacetFractionDigitsValue

public void setFacetFractionDigitsValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fractionDigitsFacetValue)

Sets the value of the FRACTION_DIGITS facet corresponding to the attribute.
  Specified by: [setFacetFractionDigitsValue](NodeDescription.md#setFacetFractionDigitsValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: fractionDigitsFacetValue - The value of the FRACTION_DIGITSfacet to be set.
### getFacetLengthValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetLengthValue()

Gets the value of the LENGTH facet corresponding to the attribute.
  Specified by: [getFacetLengthValue](NodeDescription.md#getFacetLengthValue()) in interface [NodeDescription](NodeDescription.md) Returns: Returns the value of the LENGTH facet. Can be null.
### setFacetLengthValue

public void setFacetLengthValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lengthFacetValue)

Sets the value of the LENGTH facet corresponding to the attribute.
  Specified by: [setFacetLengthValue](NodeDescription.md#setFacetLengthValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: lengthFacetValue - The value of the LENGTHfacet to be set.
### getFacetMaxExclusiveValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMaxExclusiveValue()

Gets the value of the MAX_EXCLUSIVE facet corresponding to the attribute.
  Specified by: [getFacetMaxExclusiveValue](NodeDescription.md#getFacetMaxExclusiveValue()) in interface [NodeDescription](NodeDescription.md) Returns: Returns the value of the MAX_EXCLUSIVE facet. Can be null.
### setFacetMaxExclusiveValue

public void setFacetMaxExclusiveValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxExclusiveFacetValue)

Sets the value of the MAX_EXCLUSIVE facet corresponding to the attribute.
  Specified by: [setFacetMaxExclusiveValue](NodeDescription.md#setFacetMaxExclusiveValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: maxExclusiveFacetValue - The value of the MAX_EXCLUSIVEfacet to be set.
### getFacetMaxInclusiveValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMaxInclusiveValue()

Gets the value of the MAX_INCLUSIVE facet corresponding to the attribute.
  Specified by: [getFacetMaxInclusiveValue](NodeDescription.md#getFacetMaxInclusiveValue()) in interface [NodeDescription](NodeDescription.md) Returns: Returns the value of the MAX_INCLUSIVE facet. Can be null.
### setFacetMaxInclusiveValue

public void setFacetMaxInclusiveValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxInclusiveFacetValue)

Sets the value of the MAX_INCLUSIVE facet corresponding to the attribute.
  Specified by: [setFacetMaxInclusiveValue](NodeDescription.md#setFacetMaxInclusiveValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: maxInclusiveFacetValue - The value of the MAX_INCLUSIVEfacet to be set.
### getFacetMaxLengthValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMaxLengthValue()

Gets the value of the MAX_LENGTH facet corresponding to the attribute.
  Specified by: [getFacetMaxLengthValue](NodeDescription.md#getFacetMaxLengthValue()) in interface [NodeDescription](NodeDescription.md) Returns: Returns the value of the MAX_LENGTH facet. Can be null.
### setFacetMaxLengthValue

public void setFacetMaxLengthValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) maxLengthFacetValue)

Sets the value of the MAX_LENGTH facet corresponding to the attribute.
  Specified by: [setFacetMaxLengthValue](NodeDescription.md#setFacetMaxLengthValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: maxLengthFacetValue - The value of the MAX_LENGTHfacet to be set.
### getFacetMinExclusiveValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMinExclusiveValue()

Gets the value of the MIN_EXCLUSIVE facet corresponding to the attribute.
  Specified by: [getFacetMinExclusiveValue](NodeDescription.md#getFacetMinExclusiveValue()) in interface [NodeDescription](NodeDescription.md) Returns: Returns the value of the MIN_EXCLUSIVE facet. Can be null.
### setFacetMinExclusiveValue

public void setFacetMinExclusiveValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minExclusiveFacetValue)

Sets the value of the MIN_EXCLUSIVE facet corresponding to the attribute.
  Specified by: [setFacetMinExclusiveValue](NodeDescription.md#setFacetMinExclusiveValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: minExclusiveFacetValue - The value of the MIN_EXCLUSIVEfacet to be set.
### getFacetMinInclusiveValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMinInclusiveValue()

Gets the value of the MIN_INCLUSIVE facet corresponding to the attribute.
  Specified by: [getFacetMinInclusiveValue](NodeDescription.md#getFacetMinInclusiveValue()) in interface [NodeDescription](NodeDescription.md) Returns: Returns the value of the MIN_INCLUSIVE facet. Can be null.
### setFacetMinInclusiveValue

public void setFacetMinInclusiveValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minInclusiveFacetValue)

Sets the value of the MIN_INCLUSIVE facet corresponding to the attribute.
  Specified by: [setFacetMinInclusiveValue](NodeDescription.md#setFacetMinInclusiveValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: minInclusiveFacetValue - The value of the MIN_INCLUSIVEfacet to be set.
### getFacetMinLengthValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetMinLengthValue()

Gets the value of the MIN_LENGTH facet corresponding to the attribute.
  Specified by: [getFacetMinLengthValue](NodeDescription.md#getFacetMinLengthValue()) in interface [NodeDescription](NodeDescription.md) Returns: Returns the value of the MIN_LENGTH facet. Can be null.
### setFacetMinLengthValue

public void setFacetMinLengthValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) minLengthFacetValue)

Sets the value of the MIN_LENGTH facet corresponding to the attribute.
  Specified by: [setFacetMinLengthValue](NodeDescription.md#setFacetMinLengthValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: minLengthFacetValue - The value of the MIN_LENGTHfacet to be set.
### getFacetTotalDigitsValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetTotalDigitsValue()

Gets the value of the TOTAL_DIGITS facet corresponding to the attribute.
  Specified by: [getFacetTotalDigitsValue](NodeDescription.md#getFacetTotalDigitsValue()) in interface [NodeDescription](NodeDescription.md) Returns: Returns the value of the TOTAL_DIGITS facet. Can be null.
### setFacetTotalDigitsValue

public void setFacetTotalDigitsValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) totalDigitsFacetValue)

Sets the value of the TOTAL_DIGITS facet corresponding to the attribute.
  Specified by: [setFacetTotalDigitsValue](NodeDescription.md#setFacetTotalDigitsValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: totalDigitsFacetValue - The value of the TOTAL_DIGITSfacet to be set.
### getFacetWhitespaceValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetWhitespaceValue()

Gets the value of the WHITESPACE facet corresponding to the attribute.
  Specified by: [getFacetWhitespaceValue](NodeDescription.md#getFacetWhitespaceValue()) in interface [NodeDescription](NodeDescription.md) Returns: Returns the value of the WHITESPACE facet. Can be null.
### setFacetWhitespaceValue

public void setFacetWhitespaceValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) whitespaceFacetValue)

Sets the value of the WHITESPACE facet corresponding to the attribute.
  Specified by: [setFacetWhitespaceValue](NodeDescription.md#setFacetWhitespaceValue(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: whitespaceFacetValue - The value of the WHITESPACEfacet to be set.
### getFacetPattern

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFacetPattern()

Gets the value of the PATTERN facet corresponding to the attribute.
  Specified by: [getFacetPattern](NodeDescription.md#getFacetPattern()) in interface [NodeDescription](NodeDescription.md) Returns: Returns the value of the PATTERN facet. Can be null.
### setFacetPattern

public void setFacetPattern([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) patternFacets)

Sets the value of the PATTERN facet corresponding to the attribute.
  Specified by: [setFacetPattern](NodeDescription.md#setFacetPattern(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: patternFacets - The value of the PATTERNfacet to be set.
### getModelDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getModelDescription()

Gets the model description.
  Specified by: [getModelDescription](NodeDescription.md#getModelDescription()) in interface [NodeDescription](NodeDescription.md) Returns: Returns the attribute model description. Can be null.
### setModelDescription

public void setModelDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) modelDescription)

Sets the model description.
  Specified by: [setModelDescription](NodeDescription.md#setModelDescription(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: modelDescription - The model description of the attribute to be set.
### setDefaultValue

public void setDefaultValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)

Sets the default value attribute of the attribute.
  Parameters: defaultValue - The default value of the attribute.
### setOverridingDefaultValueProvider

public void setOverridingDefaultValueProvider([CIAttribute.DefaultValueProvider](CIAttribute.DefaultValueProvider.md) defaultValueProvider)

Sets the default value provider that overrides the default value.
  Parameters: defaultValueProvider - The default value provider.
### setPossiblesValues

public void setPossiblesValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> possiblesValues)

Sets the possible values this attribute can have.
  Specified by: [setPossiblesValues](NodeDescription.md#setPossiblesValues(java.util.List)) in interface [NodeDescription](NodeDescription.md) Parameters: possiblesValues - The list of possible values to set. See Also:
        * [NodeDescription.setPossiblesValues(java.util.List)](NodeDescription.md#setPossiblesValues(java.util.List))

### setRequired

public void setRequired(boolean required)

Sets the required value for the attribute.
  Parameters: required - If true the attribute is required.
### setNamespace

public void setNamespace([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)

Sets the namespace value for the attribute.
  Parameters: namespace - The namespace to be set.
### setFixed

public void setFixed(boolean fixed)

Sets the fixed mode of the attribute.
  Parameters: fixed - True if the attribute has a fixed value.
### getAnnotation

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAnnotation()

Get the annotation for the attribute.
  Specified by: [getAnnotation](NodeDescription.md#getAnnotation()) in interface [NodeDescription](NodeDescription.md) Returns: A text that explains how to use the attribute, or null.
### setAnnotation

public void setAnnotation([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation)

Set the annotation for the attribute.
  Parameters: annotation - The annotation of the attribute, or null.
### isDeclareXmlns

public boolean isDeclareXmlns()

Check if attribute should add an xmlns declaration.
  Returns: Returns true if attribute should add an xmlns declaration.
### setDeclareXmlns

public void setDeclareXmlns(boolean declareXmlns)

Set if the attribute should add an xmlns declaration.
  Parameters: declareXmlns - true if the attribute should add an xmlns declaration.
### getPrefix

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPrefix()

Get the attribute prefix.
  Returns: Returns the prefix.
### setPrefix

public void setPrefix([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix)

Set the attribute prefix.
  Parameters: prefix - The prefix to set.
### setAssertions

public void setAssertions([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) assertionsDescription)
 Description copied from interface: [NodeDescription](NodeDescription.md#setAssertions(java.lang.String))
Sets the string representation for the node type assertions.
  Specified by: [setAssertions](NodeDescription.md#setAssertions(java.lang.String)) in interface [NodeDescription](NodeDescription.md) Parameters: assertionsDescription - The string representing all assertions. See Also:
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

### isAttributeNameQualified

public boolean isAttributeNameQualified()

Returns true if the name of the attribute is a QName. This means that it already contains the prefix before the local name.
  Returns: true if the attribute name is actually a QName.
### clone

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone() throws [CloneNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CloneNotSupportedException.html)

Allows cloning.
  Overrides: [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Throws: [CloneNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CloneNotSupportedException.html) See Also:
        * [Object.clone()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
