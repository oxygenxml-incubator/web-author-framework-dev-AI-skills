Package [ro.sync.exml.workspace.api.editor.page.ditamap.keys](package-summary.md)

# Class KeyDefinitionInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionInfo
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class KeyDefinitionInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Information about a key definition. This is filled on the API side.
  Since: 14
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DEFINITION_LOCATION](#DEFINITION_LOCATION)
The location of the DITA Map where the key definition was defined.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DESCRIPTION](#DESCRIPTION)
This could be the navigation title on the topic ref which defines the key.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [HREF](#HREF)
The relative href value of the topic ref which defines the key.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [IS_SUBJECT_DEF](#IS_SUBJECT_DEF)
A boolean flag which defines whether or not this key definition corresponds to a <subjectdef> element
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [META_CONTENT_PROVIDER](#META_CONTENT_PROVIDER)
May return a [MetaContentProvider](MetaContentProvider.md) implementation which returns the text which should appear on an element which has the keyref if the element has no content.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [NAME](#NAME)
The key name.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SUBJECT_DEF_CHILDREN](#SUBJECT_DEF_CHILDREN)
A list of child <subjectdef> KeyDefinitionInfo children.

## Constructor Summary
 Constructors
Constructor

Description
 [KeyDefinitionInfo](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getAttributes](#getAttributes())()
Get the set of attributes which are defined or cascade to on the key definition.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getProperty](#getProperty(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName)
Get the value of a recognized property.
  void [setAttribute](#setAttribute(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)
Set the value of an XML attribute which is defined on the key or cascades to it.
  void [setProperty](#setProperty(java.lang.String,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) propertyValue)
Get the value of a recognized property.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### NAME

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) NAME

The key name.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionInfo.NAME)

### HREF

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) HREF

The relative href value of the topic ref which defines the key. Can be null. If the defined key points indirectly (using a keyref) to other definitions, it is the responsibility of the developer to set here the final href value. The absolute reference will be resolved based on the "DEFINITION_LOCATION" property which needs to be set in the KeyDefinitionInfo.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionInfo.HREF)

### DESCRIPTION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DESCRIPTION

This could be the navigation title on the topic ref which defines the key. It is used for display purposes when a key reference is inserted. Can be null.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionInfo.DESCRIPTION)

### DEFINITION_LOCATION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DEFINITION_LOCATION

The location of the DITA Map where the key definition was defined. This must be given as an URL in the Oxygen standalone version. In the Oxygen plugin for Eclipse this can be also given as a native resource like IResource. The location is useful in order for Oxygen to determine the absolute location where the keyref is pointing. When the user clicks a keyref or a conkeyref in the Author page Oxygen has to open the target location corresponding to it.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionInfo.DEFINITION_LOCATION)

### META_CONTENT_PROVIDER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) META_CONTENT_PROVIDER

May return a [MetaContentProvider](MetaContentProvider.md) implementation which returns the text which should appear on an element which has the keyref if the element has no content. The provider is useful in order for Oxygen to show the static text in place in the Author page.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionInfo.META_CONTENT_PROVIDER)

### IS_SUBJECT_DEF

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) IS_SUBJECT_DEF

A boolean flag which defines whether or not this key definition corresponds to a <subjectdef> element
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionInfo.IS_SUBJECT_DEF)

### SUBJECT_DEF_CHILDREN

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SUBJECT_DEF_CHILDREN

A list of child <subjectdef> KeyDefinitionInfo children.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.ditamap.keys.KeyDefinitionInfo.SUBJECT_DEF_CHILDREN)

## Constructor Details

### KeyDefinitionInfo

public KeyDefinitionInfo()

## Method Details

### getProperty

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName)

Get the value of a recognized property.
  Parameters: propertyName - The property name. One of the following constants:
        * [DESCRIPTION](#DESCRIPTION)
        * [NAME](#NAME)
        * [HREF](#HREF)
        * [DEFINITION_LOCATION](#DEFINITION_LOCATION)
        * [IS_SUBJECT_DEF](#IS_SUBJECT_DEF)
        * [SUBJECT_DEF_CHILDREN](#SUBJECT_DEF_CHILDREN)
 Returns: The property value or null if not available.
### setProperty

public void setProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) propertyValue)

Get the value of a recognized property.
  Parameters: propertyName - The property name. One of the following constants:
        * [DESCRIPTION](#DESCRIPTION)
        * [NAME](#NAME)
        * [HREF](#HREF)
        * [DEFINITION_LOCATION](#DEFINITION_LOCATION)
        * [IS_SUBJECT_DEF](#IS_SUBJECT_DEF)
        * [SUBJECT_DEF_CHILDREN](#SUBJECT_DEF_CHILDREN)
 propertyValue - The value of the property. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - If the property name is not one of the constants in this class.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### setAttribute

public void setAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)

Set the value of an XML attribute which is defined on the key or cascades to it. For example the application may use the "format" attribute to hide when inserting key references, key definitions which point to DITA resources.
  Parameters: attributeName - The attribute name. attributeValue - The value of the attribute. Since: 18.1
### getAttributes

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getAttributes()

Get the set of attributes which are defined or cascade to on the key definition. Can be null
  Returns: Returns the set of attributes which are defined or cascade to on the key definition. Since: 18.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
