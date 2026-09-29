Package [ro.sync.ecss.dita](package-summary.md)

# Class CILevelValue

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.contentcompletion.xml.CIValue](../../contentcompletion/xml/CIValue.md)
        * ro.sync.ecss.dita.CILevelValue
   All Implemented Interfaces: [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CIValue](../../contentcompletion/xml/CIValue.md)>   @API(type=EXTENDABLE, src=PRIVATE) public class CILevelValue extends [CIValue](../../contentcompletion/xml/CIValue.md)
CI Value which also has a level.

## Field Summary

### Fields inherited from class ro.sync.contentcompletion.xml.[CIValue](../../contentcompletion/xml/CIValue.md)
 [afterInsertCaretPosition](../../contentcompletion/xml/CIValue.md#afterInsertCaretPosition), [TYPE_AI_POSITRON_FUNCTION](../../contentcompletion/xml/CIValue.md#TYPE_AI_POSITRON_FUNCTION), [TYPE_ANT_EXTENSION_POINT](../../contentcompletion/xml/CIValue.md#TYPE_ANT_EXTENSION_POINT), [TYPE_ANT_PROPERTY](../../contentcompletion/xml/CIValue.md#TYPE_ANT_PROPERTY), [TYPE_ANT_REFERENCE](../../contentcompletion/xml/CIValue.md#TYPE_ANT_REFERENCE), [TYPE_ANT_TARGET](../../contentcompletion/xml/CIValue.md#TYPE_ANT_TARGET), [TYPE_FILE_NAME](../../contentcompletion/xml/CIValue.md#TYPE_FILE_NAME), [TYPE_FOLDER](../../contentcompletion/xml/CIValue.md#TYPE_FOLDER), [TYPE_OXYGEN_XPATH_FUNCTION](../../contentcompletion/xml/CIValue.md#TYPE_OXYGEN_XPATH_FUNCTION), [TYPE_PLAIN](../../contentcompletion/xml/CIValue.md#TYPE_PLAIN), [TYPE_SCH_DIAGNOSTIC](../../contentcompletion/xml/CIValue.md#TYPE_SCH_DIAGNOSTIC), [TYPE_SCH_PATTERN](../../contentcompletion/xml/CIValue.md#TYPE_SCH_PATTERN), [TYPE_SCH_PHASE](../../contentcompletion/xml/CIValue.md#TYPE_SCH_PHASE), [TYPE_SCH_PROPERTY](../../contentcompletion/xml/CIValue.md#TYPE_SCH_PROPERTY), [TYPE_SCH_RULE](../../contentcompletion/xml/CIValue.md#TYPE_SCH_RULE), [TYPE_SCH_VARIABLE](../../contentcompletion/xml/CIValue.md#TYPE_SCH_VARIABLE), [TYPE_UNKNOWN](../../contentcompletion/xml/CIValue.md#TYPE_UNKNOWN), [TYPE_WSDL_BINDING](../../contentcompletion/xml/CIValue.md#TYPE_WSDL_BINDING), [TYPE_WSDL_MESSAGE](../../contentcompletion/xml/CIValue.md#TYPE_WSDL_MESSAGE), [TYPE_WSDL_MESSAGE_PART](../../contentcompletion/xml/CIValue.md#TYPE_WSDL_MESSAGE_PART), [TYPE_WSDL_OPERATION_FAULT](../../contentcompletion/xml/CIValue.md#TYPE_WSDL_OPERATION_FAULT), [TYPE_WSDL_OPERATION_INPUT](../../contentcompletion/xml/CIValue.md#TYPE_WSDL_OPERATION_INPUT), [TYPE_WSDL_OPERATION_OUTPUT](../../contentcompletion/xml/CIValue.md#TYPE_WSDL_OPERATION_OUTPUT), [TYPE_WSDL_PORT_TYPE](../../contentcompletion/xml/CIValue.md#TYPE_WSDL_PORT_TYPE), [TYPE_WSDL_PORT_TYPE_OPERATION](../../contentcompletion/xml/CIValue.md#TYPE_WSDL_PORT_TYPE_OPERATION), [TYPE_XSD_ATTRIBUTE](../../contentcompletion/xml/CIValue.md#TYPE_XSD_ATTRIBUTE), [TYPE_XSD_ATTRIBUTE_GROUP](../../contentcompletion/xml/CIValue.md#TYPE_XSD_ATTRIBUTE_GROUP), [TYPE_XSD_COMPLEX_TYPE](../../contentcompletion/xml/CIValue.md#TYPE_XSD_COMPLEX_TYPE), [TYPE_XSD_CONSTRAINT](../../contentcompletion/xml/CIValue.md#TYPE_XSD_CONSTRAINT), [TYPE_XSD_ELEMENT](../../contentcompletion/xml/CIValue.md#TYPE_XSD_ELEMENT), [TYPE_XSD_GROUP](../../contentcompletion/xml/CIValue.md#TYPE_XSD_GROUP), [TYPE_XSD_NOTATION](../../contentcompletion/xml/CIValue.md#TYPE_XSD_NOTATION), [TYPE_XSD_SIMPLE_OR_COMPLEX_TYPE](../../contentcompletion/xml/CIValue.md#TYPE_XSD_SIMPLE_OR_COMPLEX_TYPE), [TYPE_XSD_SIMPLE_TYPE](../../contentcompletion/xml/CIValue.md#TYPE_XSD_SIMPLE_TYPE), [TYPE_XSLT_ACCUMULATOR](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_ACCUMULATOR), [TYPE_XSLT_ATTRIBUTE](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_ATTRIBUTE), [TYPE_XSLT_ATTRIBUTE_SET](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_ATTRIBUTE_SET), [TYPE_XSLT_AXIS](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_AXIS), [TYPE_XSLT_CHARACTER_MAP](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_CHARACTER_MAP), [TYPE_XSLT_ELEMENT](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_ELEMENT), [TYPE_XSLT_FUNCTION](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_FUNCTION), [TYPE_XSLT_KEY](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_KEY), [TYPE_XSLT_LOCAL_PARAM](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_LOCAL_PARAM), [TYPE_XSLT_LOCAL_VARIABLE](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_LOCAL_VARIABLE), [TYPE_XSLT_MODE](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_MODE), [TYPE_XSLT_OUTPUT](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_OUTPUT), [TYPE_XSLT_PARAM](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_PARAM), [TYPE_XSLT_TEMPLATE](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_TEMPLATE), [TYPE_XSLT_VARIABLE](../../contentcompletion/xml/CIValue.md#TYPE_XSLT_VARIABLE)
## Constructor Summary
 Constructors
Constructor

Description
 [CILevelValue](#%3Cinit%3E(java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int level)
Constructor.
  [CILevelValue](#%3Cinit%3E(java.lang.String,int,java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int level, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] parentPath)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
Test if a CIValue is equal with this one.
  int [getLevel](#getLevel())()
Get the level in the Subject Scheme hierarchy.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getParentPath](#getParentPath())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPresentationName](#getPresentationName())()
Returns a human friendly name used to present the value in a dialog.
  int [hashCode](#hashCode())()

 void [setPresentationName](#setPresentationName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) presentationName)
Set a human friendly name used to present the value in a dialog.

### Methods inherited from class ro.sync.contentcompletion.xml.[CIValue](../../contentcompletion/xml/CIValue.md)
 [compareTo](../../contentcompletion/xml/CIValue.md#compareTo(ro.sync.contentcompletion.xml.CIValue)), [getAfterInsertCaretPosition](../../contentcompletion/xml/CIValue.md#getAfterInsertCaretPosition()), [getAnnotation](../../contentcompletion/xml/CIValue.md#getAnnotation()), [getAnnotationAsPlainText](../../contentcompletion/xml/CIValue.md#getAnnotationAsPlainText()), [getCIFromIDValues](../../contentcompletion/xml/CIValue.md#getCIFromIDValues(java.util.Collection,boolean)), [getCIValues](../../contentcompletion/xml/CIValue.md#getCIValues(java.util.Collection)), [getCIValues](../../contentcompletion/xml/CIValue.md#getCIValues(java.util.Collection,int)), [getCIValues](../../contentcompletion/xml/CIValue.md#getCIValues(java.util.Collection,int,boolean)), [getCIValues](../../contentcompletion/xml/CIValue.md#getCIValues(java.util.Collection,int,boolean,boolean)), [getCIValuesAsList](../../contentcompletion/xml/CIValue.md#getCIValuesAsList(java.util.Collection)), [getCIValuesAsList](../../contentcompletion/xml/CIValue.md#getCIValuesAsList(java.util.Collection,java.lang.String)), [getCIValuesAsList](../../contentcompletion/xml/CIValue.md#getCIValuesAsList(java.util.Collection,java.lang.String,int)), [getInsertString](../../contentcompletion/xml/CIValue.md#getInsertString()), [getType](../../contentcompletion/xml/CIValue.md#getType()), [getValue](../../contentcompletion/xml/CIValue.md#getValue()), [isDefaultValue](../../contentcompletion/xml/CIValue.md#isDefaultValue()), [isListValue](../../contentcompletion/xml/CIValue.md#isListValue()), [isUsedInURLAnchors](../../contentcompletion/xml/CIValue.md#isUsedInURLAnchors()), [setAfterInsertCaretPosition](../../contentcompletion/xml/CIValue.md#setAfterInsertCaretPosition(int)), [setAnnotation](../../contentcompletion/xml/CIValue.md#setAnnotation(java.lang.String)), [setDefaultValue](../../contentcompletion/xml/CIValue.md#setDefaultValue()), [setInsertString](../../contentcompletion/xml/CIValue.md#setInsertString(java.lang.String)), [setListValue](../../contentcompletion/xml/CIValue.md#setListValue()), [setType](../../contentcompletion/xml/CIValue.md#setType(int)), [setValue](../../contentcompletion/xml/CIValue.md#setValue(java.lang.String)), [toString](../../contentcompletion/xml/CIValue.md#toString()), [valueOf](../../contentcompletion/xml/CIValue.md#valueOf(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CILevelValue

public CILevelValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int level)

Constructor.
  Parameters: name - The actual value. level - The level in the Subject Scheme hierarchy.
### CILevelValue

public CILevelValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int level, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] parentPath)

Constructor.
  Parameters: name - The actual value. level - The level in the Subject Scheme hierarchy. parentPath - The path of ancestors values.
## Method Details

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
 Description copied from class: [CIValue](../../contentcompletion/xml/CIValue.md#equals(java.lang.Object))
Test if a CIValue is equal with this one.
  Overrides: [equals](../../contentcompletion/xml/CIValue.md#equals(java.lang.Object)) in class [CIValue](../../contentcompletion/xml/CIValue.md) See Also:
        * [CIValue.equals(java.lang.Object)](../../contentcompletion/xml/CIValue.md#equals(java.lang.Object))

### hashCode

public int hashCode()
  Overrides: [hashCode](../../contentcompletion/xml/CIValue.md#hashCode()) in class [CIValue](../../contentcompletion/xml/CIValue.md) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### getLevel

public int getLevel()

Get the level in the Subject Scheme hierarchy.
  Returns: Returns the level in the Subject Scheme hierarchy.
### getPresentationName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPresentationName()

Returns a human friendly name used to present the value in a dialog.
  Returns: a human friendly name used to present the value in a dialog.
### setPresentationName

public void setPresentationName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) presentationName)

Set a human friendly name used to present the value in a dialog.
  Parameters: presentationName - The presentation.
### getParentPath

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getParentPath()
  Returns: Returns the parents path.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
