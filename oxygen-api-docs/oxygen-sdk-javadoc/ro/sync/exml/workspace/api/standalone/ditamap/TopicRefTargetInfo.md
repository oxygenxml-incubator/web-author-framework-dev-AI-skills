Package [ro.sync.exml.workspace.api.standalone.ditamap](package-summary.md)

# Class TopicRefTargetInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.standalone.ditamap.TopicRefTargetInfo
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class TopicRefTargetInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
A map holding information about the target of a topic reference. This is filled on the API side.
  Since: 12.2
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CLASS_VALUE](#CLASS_VALUE)
The class value of the target.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME](#ELEMENT_NAME)
The element name.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PARSE_ERROR](#PARSE_ERROR)
An error message if error (file not found or parse) occured reading the topic
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [RESOLVED](#RESOLVED)
If set to the string "true" then the Plugin API handled the reference, if not the default approach should be performed (Oxygen requests the entire content of the reference and parses the title and other properties).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TITLE](#TITLE)
The title of the target

## Constructor Summary
 Constructors
Constructor

Description
 [TopicRefTargetInfo](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getProperty](#getProperty(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName)
Get the value of a recognized property.
  void [setProperty](#setProperty(java.lang.String,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) propertyValue)
Get the value of a recognized property.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### TITLE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TITLE

The title of the target
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.ditamap.TopicRefTargetInfo.TITLE)

### CLASS_VALUE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CLASS_VALUE

The class value of the target.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.ditamap.TopicRefTargetInfo.CLASS_VALUE)

### ELEMENT_NAME

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME

The element name.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.ditamap.TopicRefTargetInfo.ELEMENT_NAME)

### PARSE_ERROR

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PARSE_ERROR

An error message if error (file not found or parse) occured reading the topic
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.ditamap.TopicRefTargetInfo.PARSE_ERROR)

### RESOLVED

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) RESOLVED

If set to the string "true" then the Plugin API handled the reference, if not the default approach should be performed (Oxygen requests the entire content of the reference and parses the title and other properties).
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.ditamap.TopicRefTargetInfo.RESOLVED)

## Constructor Details

### TopicRefTargetInfo

public TopicRefTargetInfo()

## Method Details

### getProperty

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName)

Get the value of a recognized property.
  Parameters: propertyName - The property name. One of the following constants:
        * [RESOLVED](#RESOLVED)
        * [TITLE](#TITLE)
        * [CLASS_VALUE](#CLASS_VALUE)
        * [ELEMENT_NAME](#ELEMENT_NAME)
        * [PARSE_ERROR](#PARSE_ERROR)
 Returns: The property value or null if not available.
### setProperty

public void setProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) propertyValue)

Get the value of a recognized property.
  Parameters: propertyName - The property name. One of the following constants:
        * [RESOLVED](#RESOLVED)
        * [TITLE](#TITLE)
        * [CLASS_VALUE](#CLASS_VALUE)
        * [ELEMENT_NAME](#ELEMENT_NAME)
        * [PARSE_ERROR](#PARSE_ERROR)
 propertyValue - The value of the property. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - If the property name is not one of the constants in this class.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
