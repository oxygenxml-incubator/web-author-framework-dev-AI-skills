Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Class TableProperty

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.properties.TableProperty
   @API(type=INTERNAL, src=PUBLIC) public class TableProperty extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Class representing a table property. It contains the name of the property, possible values, icons for the values, current set value of the property, the group that contains it, the type of GUI elements that will be used to present the property in the "Table properties" dialog.

## Constructor Summary
 Constructors
Constructor

Description
 [TableProperty](#%3Cinit%3E(java.lang.String,java.lang.String,java.util.List,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyRenderString, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> propertyValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValue)
Constructor.
  [TableProperty](#%3Cinit%3E(java.lang.String,java.lang.String,java.util.List,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyRenderString, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> propertyValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValue, boolean isAttribute)
Constructor.
  [TableProperty](#%3Cinit%3E(java.lang.String,java.lang.String,java.util.List,java.lang.String,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyRenderString, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> propertyValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValue, boolean isAttribute, boolean isActive)
Constructor.
  [TableProperty](#%3Cinit%3E(java.lang.String,java.lang.String,java.util.List,java.lang.String,java.lang.String,ro.sync.ecss.extensions.commons.table.properties.GuiElements,java.util.Map,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyRenderString, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> propertyValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentGroup, [GuiElements](GuiElements.md) guiType, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> icons, boolean isAttribute, boolean isActive)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeName](#getAttributeName())()
Obtain the property name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeRenderString](#getAttributeRenderString())()
Obtain the render string fort the property.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCurrentValue](#getCurrentValue())()
Obtain the current value for the attributes.
  [GuiElements](GuiElements.md) [getGuiType](#getGuiType())()
Obtain the type of GUI elements which will be used to present the values for the property.
  [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getIcons](#getIcons())()
Obtain the icons for the property values.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOldValue](#getOldValue())()
Obtain the old set value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getParentGroup](#getParentGroup())()
Obtain the group that includes the current property.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getValues](#getValues())()
Obtain the property possible values.
  int [hashCode](#hashCode())()

 boolean [isActive](#isActive())()
Check if the property can be edited through the properties dialog.
  boolean [isAttribute](#isAttribute())()
true if the current property represents an attribute.
  void [setCurrentValue](#setCurrentValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValue)
Set a new current value for the property.
  void [setGuiType](#setGuiType(ro.sync.ecss.extensions.commons.table.properties.GuiElements))([GuiElements](GuiElements.md) guiType)
Set the type of GUI elements which will be used to present the values for the property.
  void [setIcons](#setIcons(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> icons)
Set the icons for the property possible values.
  void [setOldValue](#setOldValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) oldValue)
Set the old value for the property.
  void [setParentGroup](#setParentGroup(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentGroup)
Sets the group that includes the current property.
  void [setValues](#setValues(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values)
Sets the values for the current property.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TableProperty

public TableProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyRenderString, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> propertyValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValue)

Constructor.
  Parameters: propertyName - The qName of the current attribute. propertyRenderString - The string that will be presented in the [SATablePropertiesCustomizerDialog](SATablePropertiesCustomizerDialog.md). It can be different from the attribute name or it can be even the same. propertyValues - The list with the attribute's possible values. currentValue - The current of the attribute.
### TableProperty

public TableProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyRenderString, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> propertyValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValue, boolean isAttribute)

Constructor.
  Parameters: propertyName - The qName of the current attribute. propertyRenderString - The string that will be presented in the [SATablePropertiesCustomizerDialog](SATablePropertiesCustomizerDialog.md). It can be different from the attribute name or it can be even the same. propertyValues - The list with the attribute's possible values. currentValue - The current of the attribute. isAttribute - true if the current property represents an attribute.
### TableProperty

public TableProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyRenderString, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> propertyValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValue, boolean isAttribute, boolean isActive)

Constructor.
  Parameters: propertyName - The qName of the current attribute. propertyRenderString - The string that will be presented in the [SATablePropertiesCustomizerDialog](SATablePropertiesCustomizerDialog.md). It can be different from the attribute name or it can be even the same. propertyValues - The list with the attribute's possible values. currentValue - The current of the attribute. isAttribute - true if the current property represents an attribute. isActive - true if the combobox corresponding to the current property is enabled, false otherwise.
### TableProperty

public TableProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyRenderString, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> propertyValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentGroup, [GuiElements](GuiElements.md) guiType, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> icons, boolean isAttribute, boolean isActive)

Constructor.
  Parameters: propertyName - The qName of the current attribute. propertyRenderString - The string that will be presented in the [SATablePropertiesCustomizerDialog](SATablePropertiesCustomizerDialog.md). It can be different from the attribute name or it can be even the same. propertyValues - The list with the attribute's possible values. currentValue - The current of the attribute. parentGroup - The group name that will include the current property. guiType - The type of GUI element that will be used to represent the values for the current property. If is one of [GuiElements.COMBOBOX](GuiElements.md#COMBOBOX), [GuiElements.RADIO_BUTTONS](GuiElements.md#RADIO_BUTTONS). The default is [GuiElements.COMBOBOX](GuiElements.md#COMBOBOX). If this parameter is set to null, the element that will be used is [GuiElements.COMBOBOX](GuiElements.md#COMBOBOX). icons - The list of icons. An icon for every value. If empty icon corresponds to a value, the icon will be null isAttribute - true if the current property represents an attribute. isActive - true if the combobox corresponding to the current property is enabled, false otherwise.
## Method Details

### getAttributeName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeName()

Obtain the property name.
  Returns: Returns the property name.
### getAttributeRenderString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeRenderString()

Obtain the render string fort the property.
  Returns: the render string fort the property
### getValues

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getValues()

Obtain the property possible values.
  Returns: Returns the values.
### getCurrentValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCurrentValue()

Obtain the current value for the attributes.
  Returns: Returns the current value of the attribute.
### setCurrentValue

public void setCurrentValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValue)

Set a new current value for the property.
  Parameters: currentValue - The new value to set.
### getParentGroup

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getParentGroup()

Obtain the group that includes the current property.
  Returns: Returns the group name or null if no group contains this property.
### setParentGroup

public void setParentGroup([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentGroup)

Sets the group that includes the current property.
  Parameters: parentGroup - The group that includes the current property.
### isAttribute

public boolean isAttribute()

true if the current property represents an attribute.
  Returns: Returns true if the property is an attribute.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### getOldValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOldValue()

Obtain the old set value.
  Returns: Returns the old value.
### setOldValue

public void setOldValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) oldValue)

Set the old value for the property. It should be correlated with setting a new value.
  Parameters: oldValue - The old value to set.
### isActive

public boolean isActive()

Check if the property can be edited through the properties dialog.
  Returns: true if the combobox corresponding to the current property is enabled, false otherwise.
### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### setValues

public void setValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> values)

Sets the values for the current property.
  Parameters: values - Values for the current property.
### setGuiType

public void setGuiType([GuiElements](GuiElements.md) guiType)

Set the type of GUI elements which will be used to present the values for the property.
  Parameters: guiType - The new type GUI elements which will be used to present the values for the property.
### getGuiType

public [GuiElements](GuiElements.md) getGuiType()

Obtain the type of GUI elements which will be used to present the values for the property.
  Returns: Returns the type of GUI elements which will be used to present the values for the property.
### getIcons

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getIcons()

Obtain the icons for the property values. If the list contains null objects, then an empty icon should be used.
  Returns: Returns the icons for all the possible values. Every values is mapped to an icon path.
### setIcons

public void setIcons([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> icons)

Set the icons for the property possible values.
  Parameters: icons - The icons to set.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
