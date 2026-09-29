Package [ro.sync.contentcompletion.xml](package-summary.md)

# Class CIValue

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.contentcompletion.xml.CIValue
   All Implemented Interfaces: [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CIValue](CIValue.md)>   Direct Known Subclasses: [CILevelValue](../../ecss/dita/CILevelValue.md)   @API(type=EXTENDABLE, src=PRIVATE) public class CIValue extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CIValue](CIValue.md)>
Interface for objects holding information about element or attribute values used in the content completion process.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected int [afterInsertCaretPosition](#afterInsertCaretPosition)
The position in text where to place the caret position after insert value.
  static final int [TYPE_AI_POSITRON_FUNCTION](#TYPE_AI_POSITRON_FUNCTION)
AI Positron Functions.
  static final int [TYPE_ANT_EXTENSION_POINT](#TYPE_ANT_EXTENSION_POINT)
Marks that the value represents an Ant extension-point.
  static final int [TYPE_ANT_PROPERTY](#TYPE_ANT_PROPERTY)
Marks that the value represents an Ant property.
  static final int [TYPE_ANT_REFERENCE](#TYPE_ANT_REFERENCE)
Marks that the value represents an Ant reference.
  static final int [TYPE_ANT_TARGET](#TYPE_ANT_TARGET)
Marks that the value represents an Ant target.
  static final int [TYPE_FILE_NAME](#TYPE_FILE_NAME)
Marks that the value represents a name of a file.
  static final int [TYPE_FOLDER](#TYPE_FOLDER)
Marks that the value represents a name of a folder.
  static final int [TYPE_OXYGEN_XPATH_FUNCTION](#TYPE_OXYGEN_XPATH_FUNCTION)
Oxygen's custom XPath functions.
  static final int [TYPE_PLAIN](#TYPE_PLAIN)
Marks that the value is a plain text value with no additional meaning.
  static final int [TYPE_SCH_DIAGNOSTIC](#TYPE_SCH_DIAGNOSTIC)
Marks that the value represents a schematron diagnostic type.
  static final int [TYPE_SCH_PATTERN](#TYPE_SCH_PATTERN)
Marks that the value represents a schematron pattern type.
  static final int [TYPE_SCH_PHASE](#TYPE_SCH_PHASE)
Marks that the value represents a schematron phase type.
  static final int [TYPE_SCH_PROPERTY](#TYPE_SCH_PROPERTY)
Marks that the value represents a schematron property type.
  static final int [TYPE_SCH_RULE](#TYPE_SCH_RULE)
Marks that the value represents a schematron rule type.
  static final int [TYPE_SCH_VARIABLE](#TYPE_SCH_VARIABLE)
Marks that the value represents a schematron variable type.
  static final int [TYPE_UNKNOWN](#TYPE_UNKNOWN)
Marks that value represents either a name of a file or a name of a folder, but it cannot be easily established because of a very time-consuming operation involved.
  static final int [TYPE_WSDL_BINDING](#TYPE_WSDL_BINDING)
Marks that the value represents a WSDL binding type.
  static final int [TYPE_WSDL_MESSAGE](#TYPE_WSDL_MESSAGE)
Marks that the value represents a WSDL message type.
  static final int [TYPE_WSDL_MESSAGE_PART](#TYPE_WSDL_MESSAGE_PART)
Marks that the value represents a WSDL message part type.
  static final int [TYPE_WSDL_OPERATION_FAULT](#TYPE_WSDL_OPERATION_FAULT)
Marks that the value represents a WSDL operation fault type.
  static final int [TYPE_WSDL_OPERATION_INPUT](#TYPE_WSDL_OPERATION_INPUT)
Marks that the value represents a WSDL operation input type.
  static final int [TYPE_WSDL_OPERATION_OUTPUT](#TYPE_WSDL_OPERATION_OUTPUT)
Marks that the value represents a WSDL operation output type.
  static final int [TYPE_WSDL_PORT_TYPE](#TYPE_WSDL_PORT_TYPE)
Marks that the value represents a WSDL port type type.
  static final int [TYPE_WSDL_PORT_TYPE_OPERATION](#TYPE_WSDL_PORT_TYPE_OPERATION)
Marks that the value represents a WSDL port type operation type.
  static final int [TYPE_XSD_ATTRIBUTE](#TYPE_XSD_ATTRIBUTE)
Marks that the value represents a XSD attribute.
  static final int [TYPE_XSD_ATTRIBUTE_GROUP](#TYPE_XSD_ATTRIBUTE_GROUP)
Marks that the value represents a XSD attribute group.
  static final int [TYPE_XSD_COMPLEX_TYPE](#TYPE_XSD_COMPLEX_TYPE)
Marks that the value represents a XSD complex type.
  static final int [TYPE_XSD_CONSTRAINT](#TYPE_XSD_CONSTRAINT)
Marks that the value represents a XSD key or unique element.
  static final int [TYPE_XSD_ELEMENT](#TYPE_XSD_ELEMENT)
Marks that the value represents a XSD element.
  static final int [TYPE_XSD_GROUP](#TYPE_XSD_GROUP)
Marks that the value represents a XSD group.
  static final int [TYPE_XSD_NOTATION](#TYPE_XSD_NOTATION)
Marks that the value represents a XSD notation.
  static final int [TYPE_XSD_SIMPLE_OR_COMPLEX_TYPE](#TYPE_XSD_SIMPLE_OR_COMPLEX_TYPE)
Marks that the value represents a XSD simple or complex type.
  static final int [TYPE_XSD_SIMPLE_TYPE](#TYPE_XSD_SIMPLE_TYPE)
Marks that the value represents a XSD simple type.
  static final int [TYPE_XSLT_ACCUMULATOR](#TYPE_XSLT_ACCUMULATOR)
XSLT 3.0 Accumulator.
  static final int [TYPE_XSLT_ATTRIBUTE](#TYPE_XSLT_ATTRIBUTE)
Marks that the value represents a name of an attribute from the document.
  static final int [TYPE_XSLT_ATTRIBUTE_SET](#TYPE_XSLT_ATTRIBUTE_SET)
Marks that the value represents a XSLT attribute set.
  static final int [TYPE_XSLT_AXIS](#TYPE_XSLT_AXIS)
Marks that the value represents an axis in XSLT.
  static final int [TYPE_XSLT_CHARACTER_MAP](#TYPE_XSLT_CHARACTER_MAP)
Marks that the value represents a XSLT character map.
  static final int [TYPE_XSLT_ELEMENT](#TYPE_XSLT_ELEMENT)
Marks that the value represents a name of an element from the document.
  static final int [TYPE_XSLT_FUNCTION](#TYPE_XSLT_FUNCTION)
Marks that the value represents an XSLT function.
  static final int [TYPE_XSLT_KEY](#TYPE_XSLT_KEY)
Marks that the value represents a XSLT key.
  static final int [TYPE_XSLT_LOCAL_PARAM](#TYPE_XSLT_LOCAL_PARAM)
Marks that the value represents an XSLT local parameter.
  static final int [TYPE_XSLT_LOCAL_VARIABLE](#TYPE_XSLT_LOCAL_VARIABLE)
Marks that the value represents an XSLT local variable.
  static final int [TYPE_XSLT_MODE](#TYPE_XSLT_MODE)
Marks that the value represents a XSLT mode.
  static final int [TYPE_XSLT_OUTPUT](#TYPE_XSLT_OUTPUT)
Marks that the value represents a XSLT output.
  static final int [TYPE_XSLT_PARAM](#TYPE_XSLT_PARAM)
Marks that the value represents a XSLT param.
  static final int [TYPE_XSLT_TEMPLATE](#TYPE_XSLT_TEMPLATE)
Marks that the value represents a XSLT template.
  static final int [TYPE_XSLT_VARIABLE](#TYPE_XSLT_VARIABLE)
Marks that the value represents a XSLT variable.

## Constructor Summary
 Constructors
Constructor

Description
 [CIValue](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Creates a CIValue.
  [CIValue](#%3Cinit%3E(java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean listValue)
Creates a CIValue.
  [CIValue](#%3Cinit%3E(java.lang.String,boolean,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean listValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation)
Creates a CIValue.
  [CIValue](#%3Cinit%3E(java.lang.String,boolean,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean listValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation, boolean defaultValue)
Creates a CIValue.
  [CIValue](#%3Cinit%3E(java.lang.String,boolean,java.lang.String,java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean listValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertString, int type)
Creates a CIValue.
  [CIValue](#%3Cinit%3E(java.lang.String,boolean,java.lang.String,java.lang.String,int,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean listValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertString, int type, boolean defaultValue)
Creates a CIValue.
  [CIValue](#%3Cinit%3E(java.lang.String,boolean,java.lang.String,java.lang.String,int,boolean,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean listValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertString, int type, boolean defaultValue, int afterInsertCaretPosition)
Creates a CIValue.
  [CIValue](#%3Cinit%3E(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation)
Creates a CIValue.
  [CIValue](#%3Cinit%3E(java.lang.String,java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation, int type)
Creates a CIValue.
  [CIValue](#%3Cinit%3E(java.lang.String,ro.sync.contentcompletion.xml.CIValue))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fullPrefix, [CIValue](CIValue.md) ciValue)
Create a CIValue from another one by adding a prefix to the original value.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [compareTo](#compareTo(ro.sync.contentcompletion.xml.CIValue))([CIValue](CIValue.md) other)
Compares the String values.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
Test if a CIValue is equal with this one.
  int [getAfterInsertCaretPosition](#getAfterInsertCaretPosition())()
Get the relative position where to place the caret after the value is inserted.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAnnotation](#getAnnotation())()
Get the annotation associated with this value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAnnotationAsPlainText](#getAnnotationAsPlainText())()
Get the annotation associated with this value.
  static [CIValue](CIValue.md)[] [getCIFromIDValues](#getCIFromIDValues(java.util.Collection,boolean))([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<ro.sync.xml.parser.IDValue> values, boolean multipleValue)
Utility method to get an array of CIValue from a list of strings.
  static [CIValue](CIValue.md)[] [getCIValues](#getCIValues(java.util.Collection))([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values)
Utility method to get an array of CIValue from a list of strings.
  static [CIValue](CIValue.md)[] [getCIValues](#getCIValues(java.util.Collection,int))([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values, int type)
Utility method to get an array of CIValue from a list of strings.
  static [CIValue](CIValue.md)[] [getCIValues](#getCIValues(java.util.Collection,int,boolean))([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values, int type, boolean listValue)
Utility method to get an array of CIValue from a list of strings.
  static [CIValue](CIValue.md)[] [getCIValues](#getCIValues(java.util.Collection,int,boolean,boolean))([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values, int type, boolean listValue, boolean addDollar)
Utility method to get an array of CIValue from a list of strings.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> [getCIValuesAsList](#getCIValuesAsList(java.util.Collection))([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values)
Get a list of CIValue from a list of strings.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> [getCIValuesAsList](#getCIValuesAsList(java.util.Collection,java.lang.String))([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)
Get a list of CIValue from a list of strings.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> [getCIValuesAsList](#getCIValuesAsList(java.util.Collection,java.lang.String,int))([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue, int type)
Get a list of CIValue from a list of strings.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getInsertString](#getInsertString())()
Get the insert string.
  int [getType](#getType())()
Get the type of the value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getValue](#getValue())()
Get the actual value as detected in the associated schema.
  int [hashCode](#hashCode())()

 boolean [isDefaultValue](#isDefaultValue())()
Get the default value flag.
  boolean [isListValue](#isListValue())()
Check if the value is an entry in a list value.
  protected boolean [isUsedInURLAnchors](#isUsedInURLAnchors())()

 void [setAfterInsertCaretPosition](#setAfterInsertCaretPosition(int))(int afterInsertCaretPosition)
Set the relative position where to place the caret after the value is inserted.
  void [setAnnotation](#setAnnotation(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation)
Set the annotation associated with this value.
  void [setDefaultValue](#setDefaultValue())()
Mark the value as default value.
  void [setInsertString](#setInsertString(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertString)
Sets the insert string.
  void [setListValue](#setListValue())()
Mark the value as belonging to a list value.
  void [setType](#setType(int))(int type)
Set the value type.
  void [setValue](#setValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Sets the value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()
Get a String representation of this CIValue.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [valueOf](#valueOf(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) str)
IMPORTANT DO NOT DELETE! This is needed by a combo box editor to see if it is the same value as the old one.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### afterInsertCaretPosition

protected int afterInsertCaretPosition

The position in text where to place the caret position after insert value. If value is -1, then the caret position is not and must be computed.

### TYPE_PLAIN

public static final int TYPE_PLAIN

Marks that the value is a plain text value with no additional meaning. The value is 0
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_PLAIN)

### TYPE_XSLT_AXIS

public static final int TYPE_XSLT_AXIS

Marks that the value represents an axis in XSLT. The value is 1
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_AXIS)

### TYPE_XSLT_FUNCTION

public static final int TYPE_XSLT_FUNCTION

Marks that the value represents an XSLT function. The value is 2
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_FUNCTION)

### TYPE_XSLT_ELEMENT

public static final int TYPE_XSLT_ELEMENT

Marks that the value represents a name of an element from the document. The value is 3
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_ELEMENT)

### TYPE_XSLT_ATTRIBUTE

public static final int TYPE_XSLT_ATTRIBUTE

Marks that the value represents a name of an attribute from the document. The value is 4
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_ATTRIBUTE)

### TYPE_FOLDER

public static final int TYPE_FOLDER

Marks that the value represents a name of a folder. The value is 5
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_FOLDER)

### TYPE_FILE_NAME

public static final int TYPE_FILE_NAME

Marks that the value represents a name of a file. The value is 6
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_FILE_NAME)

### TYPE_UNKNOWN

public static final int TYPE_UNKNOWN

Marks that value represents either a name of a file or a name of a folder, but it cannot be easily established because of a very time-consuming operation involved. The value is 7
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_UNKNOWN)

### TYPE_ANT_PROPERTY

public static final int TYPE_ANT_PROPERTY

Marks that the value represents an Ant property. The value is 8
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_ANT_PROPERTY)

### TYPE_ANT_TARGET

public static final int TYPE_ANT_TARGET

Marks that the value represents an Ant target. The value is 9
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_ANT_TARGET)

### TYPE_ANT_EXTENSION_POINT

public static final int TYPE_ANT_EXTENSION_POINT

Marks that the value represents an Ant extension-point. The value is 10
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_ANT_EXTENSION_POINT)

### TYPE_ANT_REFERENCE

public static final int TYPE_ANT_REFERENCE

Marks that the value represents an Ant reference. The value is 11
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_ANT_REFERENCE)

### TYPE_XSLT_PARAM

public static final int TYPE_XSLT_PARAM

Marks that the value represents a XSLT param. The value is 12
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_PARAM)

### TYPE_XSLT_MODE

public static final int TYPE_XSLT_MODE

Marks that the value represents a XSLT mode. The value is 13
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_MODE)

### TYPE_XSLT_TEMPLATE

public static final int TYPE_XSLT_TEMPLATE

Marks that the value represents a XSLT template. The value is 14
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_TEMPLATE)

### TYPE_XSLT_KEY

public static final int TYPE_XSLT_KEY

Marks that the value represents a XSLT key. The value is 15
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_KEY)

### TYPE_XSLT_OUTPUT

public static final int TYPE_XSLT_OUTPUT

Marks that the value represents a XSLT output. The value is 16
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_OUTPUT)

### TYPE_XSLT_ATTRIBUTE_SET

public static final int TYPE_XSLT_ATTRIBUTE_SET

Marks that the value represents a XSLT attribute set. The value is 17
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_ATTRIBUTE_SET)

### TYPE_XSLT_CHARACTER_MAP

public static final int TYPE_XSLT_CHARACTER_MAP

Marks that the value represents a XSLT character map. The value is 18
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_CHARACTER_MAP)

### TYPE_XSLT_VARIABLE

public static final int TYPE_XSLT_VARIABLE

Marks that the value represents a XSLT variable. The value is 19
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_VARIABLE)

### TYPE_XSD_COMPLEX_TYPE

public static final int TYPE_XSD_COMPLEX_TYPE

Marks that the value represents a XSD complex type. The value is 20
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSD_COMPLEX_TYPE)

### TYPE_XSD_SIMPLE_TYPE

public static final int TYPE_XSD_SIMPLE_TYPE

Marks that the value represents a XSD simple type. The value is 21
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSD_SIMPLE_TYPE)

### TYPE_XSD_ATTRIBUTE

public static final int TYPE_XSD_ATTRIBUTE

Marks that the value represents a XSD attribute. The value is 22
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSD_ATTRIBUTE)

### TYPE_XSD_ATTRIBUTE_GROUP

public static final int TYPE_XSD_ATTRIBUTE_GROUP

Marks that the value represents a XSD attribute group. The value is 23
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSD_ATTRIBUTE_GROUP)

### TYPE_XSD_ELEMENT

public static final int TYPE_XSD_ELEMENT

Marks that the value represents a XSD element. The value is 24
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSD_ELEMENT)

### TYPE_XSD_NOTATION

public static final int TYPE_XSD_NOTATION

Marks that the value represents a XSD notation. The value is 25
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSD_NOTATION)

### TYPE_XSD_GROUP

public static final int TYPE_XSD_GROUP

Marks that the value represents a XSD group. The value is 26
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSD_GROUP)

### TYPE_XSD_SIMPLE_OR_COMPLEX_TYPE

public static final int TYPE_XSD_SIMPLE_OR_COMPLEX_TYPE

Marks that the value represents a XSD simple or complex type. The value is 27
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSD_SIMPLE_OR_COMPLEX_TYPE)

### TYPE_WSDL_PORT_TYPE_OPERATION

public static final int TYPE_WSDL_PORT_TYPE_OPERATION

Marks that the value represents a WSDL port type operation type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_WSDL_PORT_TYPE_OPERATION)

### TYPE_WSDL_PORT_TYPE

public static final int TYPE_WSDL_PORT_TYPE

Marks that the value represents a WSDL port type type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_WSDL_PORT_TYPE)

### TYPE_WSDL_MESSAGE

public static final int TYPE_WSDL_MESSAGE

Marks that the value represents a WSDL message type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_WSDL_MESSAGE)

### TYPE_WSDL_OPERATION_INPUT

public static final int TYPE_WSDL_OPERATION_INPUT

Marks that the value represents a WSDL operation input type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_WSDL_OPERATION_INPUT)

### TYPE_WSDL_OPERATION_OUTPUT

public static final int TYPE_WSDL_OPERATION_OUTPUT

Marks that the value represents a WSDL operation output type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_WSDL_OPERATION_OUTPUT)

### TYPE_WSDL_OPERATION_FAULT

public static final int TYPE_WSDL_OPERATION_FAULT

Marks that the value represents a WSDL operation fault type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_WSDL_OPERATION_FAULT)

### TYPE_WSDL_BINDING

public static final int TYPE_WSDL_BINDING

Marks that the value represents a WSDL binding type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_WSDL_BINDING)

### TYPE_WSDL_MESSAGE_PART

public static final int TYPE_WSDL_MESSAGE_PART

Marks that the value represents a WSDL message part type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_WSDL_MESSAGE_PART)

### TYPE_XSD_CONSTRAINT

public static final int TYPE_XSD_CONSTRAINT

Marks that the value represents a XSD key or unique element.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSD_CONSTRAINT)

### TYPE_SCH_VARIABLE

public static final int TYPE_SCH_VARIABLE

Marks that the value represents a schematron variable type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_SCH_VARIABLE)

### TYPE_SCH_DIAGNOSTIC

public static final int TYPE_SCH_DIAGNOSTIC

Marks that the value represents a schematron diagnostic type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_SCH_DIAGNOSTIC)

### TYPE_SCH_PATTERN

public static final int TYPE_SCH_PATTERN

Marks that the value represents a schematron pattern type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_SCH_PATTERN)

### TYPE_SCH_PHASE

public static final int TYPE_SCH_PHASE

Marks that the value represents a schematron phase type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_SCH_PHASE)

### TYPE_SCH_RULE

public static final int TYPE_SCH_RULE

Marks that the value represents a schematron rule type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_SCH_RULE)

### TYPE_XSLT_LOCAL_PARAM

public static final int TYPE_XSLT_LOCAL_PARAM

Marks that the value represents an XSLT local parameter.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_LOCAL_PARAM)

### TYPE_XSLT_LOCAL_VARIABLE

public static final int TYPE_XSLT_LOCAL_VARIABLE

Marks that the value represents an XSLT local variable.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_LOCAL_VARIABLE)

### TYPE_SCH_PROPERTY

public static final int TYPE_SCH_PROPERTY

Marks that the value represents a schematron property type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_SCH_PROPERTY)

### TYPE_OXYGEN_XPATH_FUNCTION

public static final int TYPE_OXYGEN_XPATH_FUNCTION

Oxygen's custom XPath functions.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_OXYGEN_XPATH_FUNCTION)

### TYPE_XSLT_ACCUMULATOR

public static final int TYPE_XSLT_ACCUMULATOR

XSLT 3.0 Accumulator.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_XSLT_ACCUMULATOR)

### TYPE_AI_POSITRON_FUNCTION

public static final int TYPE_AI_POSITRON_FUNCTION

AI Positron Functions.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.xml.CIValue.TYPE_AI_POSITRON_FUNCTION)

## Constructor Details

### CIValue

public CIValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Creates a CIValue.
  Parameters: value - The actual value.
### CIValue

public CIValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean listValue)

Creates a CIValue.
  Parameters: value - The actual value. listValue - Flag indicating if the value is an entry from a list value.
### CIValue

public CIValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation)

Creates a CIValue.
  Parameters: value - The actual value. annotation - The annotation associated with this value.
### CIValue

public CIValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation, int type)

Creates a CIValue.
  Parameters: value - The actual value. annotation - The annotation associated with this value. type - The value type.
### CIValue

public CIValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean listValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation)

Creates a CIValue.
  Parameters: value - The actual value. listValue - Flag indicating if the value is an entry from a list value. annotation - The annotation associated with this value.
### CIValue

public CIValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean listValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation, boolean defaultValue)

Creates a CIValue.
  Parameters: value - The actual value. listValue - Flag indicating if the value is an entry from a list value. annotation - The annotation associated with this value. defaultValue - true if it is the default value.
### CIValue

public CIValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean listValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertString, int type)

Creates a CIValue.
  Parameters: value - The actual value. listValue - Flag indicating if the value is an entry from a list value. annotation - The annotation associated with this value. insertString - The string to be inserted in the document when the CIValue is chosen from the content completion list of proposals. If null, the value will be used. type - The type of the value. Use by the renderer. Can be one of the constants: [TYPE_PLAIN](#TYPE_PLAIN), [TYPE_XSLT_AXIS](#TYPE_XSLT_AXIS), [TYPE_XSLT_FUNCTION](#TYPE_XSLT_FUNCTION), [TYPE_XSLT_ELEMENT](#TYPE_XSLT_ELEMENT), [TYPE_XSLT_ATTRIBUTE](#TYPE_XSLT_ATTRIBUTE), [TYPE_ANT_EXTENSION_POINT](#TYPE_ANT_EXTENSION_POINT), [TYPE_ANT_PROPERTY](#TYPE_ANT_PROPERTY), [TYPE_ANT_REFERENCE](#TYPE_ANT_REFERENCE), [TYPE_ANT_TARGET](#TYPE_ANT_TARGET).
### CIValue

public CIValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean listValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertString, int type, boolean defaultValue)

Creates a CIValue.
  Parameters: value - The actual value. listValue - Flag indicating if the value is an entry from a list value. annotation - The annotation associated with this value. insertString - The string to be inserted in the document when the CIValue is chosen from the content completion list of proposals. If null, the value will be used. type - The type of the value. Use by the renderer. Can be one of the constants: [TYPE_PLAIN](#TYPE_PLAIN), [TYPE_XSLT_AXIS](#TYPE_XSLT_AXIS), [TYPE_XSLT_FUNCTION](#TYPE_XSLT_FUNCTION), [TYPE_XSLT_ELEMENT](#TYPE_XSLT_ELEMENT), [TYPE_XSLT_ATTRIBUTE](#TYPE_XSLT_ATTRIBUTE) defaultValue - true if it is the default value.
### CIValue

public CIValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean listValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertString, int type, boolean defaultValue, int afterInsertCaretPosition)

Creates a CIValue.
  Parameters: value - The actual value. listValue - Flag indicating if the value is an entry from a list value. annotation - The annotation associated with this value. insertString - The string to be inserted in the document when the CIValue is chosen from the content completion list of proposals. If null, the value will be used. type - The type of the value. Use by the renderer. Can be one of the constants: [TYPE_PLAIN](#TYPE_PLAIN), [TYPE_XSLT_AXIS](#TYPE_XSLT_AXIS), [TYPE_XSLT_FUNCTION](#TYPE_XSLT_FUNCTION), [TYPE_XSLT_ELEMENT](#TYPE_XSLT_ELEMENT), [TYPE_XSLT_ATTRIBUTE](#TYPE_XSLT_ATTRIBUTE) defaultValue - true if it is the default value. afterInsertCaretPosition - The position in text where to place the caret position after insert value. If value is -1, then the caret position is not and must be computed.
### CIValue

public CIValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fullPrefix, [CIValue](CIValue.md) ciValue)

Create a CIValue from another one by adding a prefix to the original value.
  Parameters: fullPrefix - The full prefix of the value field. ciValue - The CIValue to use when creating a new one.
## Method Details

### getValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getValue()

Get the actual value as detected in the associated schema.
  Returns: The value of the CIValue.
### isListValue

public boolean isListValue()

Check if the value is an entry in a list value.
  Returns: true if the value is part of a list.
### setListValue

public void setListValue()

Mark the value as belonging to a list value.

### getAnnotation

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAnnotation()

Get the annotation associated with this value. The annotation is an additional text description (for example documentation) of the value which is usually displayed when the user browses possible values.
  Returns: The value annotation.
### getAnnotationAsPlainText

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAnnotationAsPlainText()

Get the annotation associated with this value. The annotation is an additional text description (for example documentation) of the value which is usually displayed when the user browses possible values. If the annotation contains HTML elements, it will be converted to plain text.
  Returns: The value annotation in plain text, with possible HTML tags removed.
### setAnnotation

public void setAnnotation([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) annotation)

Set the annotation associated with this value. The annotation is an additional text description (for example documentation) of the value which is usually displayed when the user browses possible values.
  Parameters: annotation - The value annotation.
### getCIValues

public static [CIValue](CIValue.md)[] getCIValues([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values)

Utility method to get an array of CIValue from a list of strings. Assumes no annotations and no list types are present.
  Parameters: values - A collection of String values. Returns: An array of CIValues.
### getCIValues

public static [CIValue](CIValue.md)[] getCIValues([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values, int type)

Utility method to get an array of CIValue from a list of strings. Assumes no annotations and no list types are present.
  Parameters: values - A collection of String values. type - The type of value. Returns: An array of CIValues.
### getCIValues

public static [CIValue](CIValue.md)[] getCIValues([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values, int type, boolean listValue)

Utility method to get an array of CIValue from a list of strings. Assumes no annotations and no list types are present.
  Parameters: values - A collection of String values. type - The type of value. listValue - true if the values must be marked as belonging to a list. Returns: An array of CIValues.
### getCIValues

public static [CIValue](CIValue.md)[] getCIValues([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values, int type, boolean listValue, boolean addDollar)

Utility method to get an array of CIValue from a list of strings. Assumes no annotations and no list types are present.
  Parameters: values - A collection of String values. type - The type of value. listValue - true if the values must be marked as belonging to a list. addDollar - If true the $ sign must be added. Returns: An array of CIValues.
### getCIFromIDValues

public static [CIValue](CIValue.md)[] getCIFromIDValues([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<ro.sync.xml.parser.IDValue> values, boolean multipleValue)

Utility method to get an array of CIValue from a list of strings. Assumes no annotations and no list types are present.
  Parameters: values - A collection of String values. multipleValue - true if the value allows multiple values. Returns: An array of CIValues.
### getCIValuesAsList

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> getCIValuesAsList([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values)

Get a list of CIValue from a list of strings. Assumes no annotation and no list types are present.
  Parameters: values - A collection of String values. Returns: An new list of CIValues.
### getCIValuesAsList

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> getCIValuesAsList([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)

Get a list of CIValue from a list of strings. Assumes no annotation and no list types are present.
  Parameters: values - A collection of String values. defaultValue - The default value Returns: An new list of CIValues.
### getCIValuesAsList

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](CIValue.md)> getCIValuesAsList([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue, int type)

Get a list of CIValue from a list of strings. Assumes no annotation and no list types are present.
  Parameters: values - A collection of String values. defaultValue - The default value type - The value type. Returns: An new list of CIValues.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

Test if a CIValue is equal with this one.
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### isDefaultValue

public boolean isDefaultValue()

Get the default value flag.
  Returns: True if the value is marked as default.
### setDefaultValue

public void setDefaultValue()

Mark the value as default value.

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()

Get a String representation of this CIValue.
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### compareTo

public int compareTo([CIValue](CIValue.md) other)

Compares the String values.
  Specified by: [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html#compareTo(T)) in interface [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CIValue](CIValue.md)> See Also:
        * [Comparable.compareTo(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html#compareTo(T))

### isUsedInURLAnchors

protected boolean isUsedInURLAnchors()
  Returns: true if the ID is used in an URL anchor
### getInsertString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getInsertString()

Get the insert string. It represents an escaped version of the value and can be inserted directly in the document.
  Returns: The escaped value to be inserted in the document.
### setInsertString

public void setInsertString([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) insertString)

Sets the insert string. It is taken into consideration only in the Text page.
  Parameters: insertString - The value to be inserted in the document.
### getType

public int getType()

Get the type of the value. It may be plain text value, an axe or a function in xslt or an element from the input document involved in an transformation scenario.
  Returns: The value type. Can be one of: [TYPE_PLAIN](#TYPE_PLAIN), [TYPE_XSLT_AXIS](#TYPE_XSLT_AXIS), [TYPE_XSLT_FUNCTION](#TYPE_XSLT_FUNCTION), [TYPE_XSLT_ELEMENT](#TYPE_XSLT_ELEMENT), [TYPE_XSLT_ATTRIBUTE](#TYPE_XSLT_ATTRIBUTE), [TYPE_FILE_NAME](#TYPE_FILE_NAME), [TYPE_FOLDER](#TYPE_FOLDER) or [TYPE_UNKNOWN](#TYPE_UNKNOWN).
### valueOf

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) valueOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) str)

IMPORTANT DO NOT DELETE! This is needed by a combo box editor to see if it is the same value as the old one.
  Parameters: str - The str. Returns: The same object.
### getAfterInsertCaretPosition

public int getAfterInsertCaretPosition()

Get the relative position where to place the caret after the value is inserted.
  Returns: The position to place the caret after inserting the string. If -1 the caret position was not computed.
### setAfterInsertCaretPosition

public void setAfterInsertCaretPosition(int afterInsertCaretPosition)

Set the relative position where to place the caret after the value is inserted.
  Parameters: afterInsertCaretPosition - The afterInsertCaretPosition to set.
### setValue

public void setValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Sets the value.
  Parameters: value - The new value.
### setType

public void setType(int type)

Set the value type.
  Parameters: type - The value type.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
