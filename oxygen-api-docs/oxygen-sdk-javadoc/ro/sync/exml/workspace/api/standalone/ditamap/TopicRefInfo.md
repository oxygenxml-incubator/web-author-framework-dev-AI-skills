Package [ro.sync.exml.workspace.api.standalone.ditamap](package-summary.md)

# Class TopicRefInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.standalone.ditamap.TopicRefInfo
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class TopicRefInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
A map holding information about the topic reference in the DITA Map. This is filled on the Oxygen side.
  Since: 12.2
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ABSOLUTE_BASE_URL](#ABSOLUTE_BASE_URL)
The absolute URL of the map in which the topicref is located.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ABSOLUTE_URL](#ABSOLUTE_URL)
The absolute URL of the topic reference computed by Oxygen from the "href" value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [HREF_VALUE](#HREF_VALUE)
The value of the "href" attribute of the <topicref> element.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ID_PATH](#ID_PATH)
The ID location (if any) inside the targeted URL.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [KEY_SCOPES](#KEY_SCOPES)
The key scopes context in which the topicref is placed.

## Constructor Summary
 Constructors
Constructor

Description
 [TopicRefInfo](#%3Cinit%3E())()

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

### ABSOLUTE_URL

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ABSOLUTE_URL

The absolute URL of the topic reference computed by Oxygen from the "href" value. It does not include the id location.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.ditamap.TopicRefInfo.ABSOLUTE_URL)

### ID_PATH

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ID_PATH

The ID location (if any) inside the targeted URL.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.ditamap.TopicRefInfo.ID_PATH)

### HREF_VALUE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) HREF_VALUE

The value of the "href" attribute of the <topicref> element.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.ditamap.TopicRefInfo.HREF_VALUE)

### KEY_SCOPES

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) KEY_SCOPES

The key scopes context in which the topicref is placed. Either empty string or something like "ks1.ks2".
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.ditamap.TopicRefInfo.KEY_SCOPES)

### ABSOLUTE_BASE_URL

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ABSOLUTE_BASE_URL

The absolute URL of the map in which the topicref is located.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.ditamap.TopicRefInfo.ABSOLUTE_BASE_URL)

## Constructor Details

### TopicRefInfo

public TopicRefInfo()

## Method Details

### getProperty

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName)

Get the value of a recognized property.
  Parameters: propertyName - The property name. One of the following constants:
        * [ABSOLUTE_URL](#ABSOLUTE_URL)
        * [ID_PATH](#ID_PATH)
        * [HREF_VALUE](#HREF_VALUE)
For example if a DITA Map with the URL "cms://test/file.ditamap" references a topic using the [HREF_VALUE](#HREF_VALUE)  **task.dita#task**then the [ABSOLUTE_URL](#ABSOLUTE_URL) of the topic reference will be **cms://test/task.dita** and the [ID_PATH](#ID_PATH) will be **task** Returns: The property value or null if not available.
### setProperty

public void setProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) propertyValue)

Get the value of a recognized property.
  Parameters: propertyName - The property name. One of the following constants:
        * [ABSOLUTE_URL](#ABSOLUTE_URL)
        * [ID_PATH](#ID_PATH)
        * [HREF_VALUE](#HREF_VALUE)
 propertyValue - The value of the property. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - If the property name is not one of the constants in this class.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
