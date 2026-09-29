Package [ro.sync.ecss.conditions](package-summary.md)

# Class ProfilingAttributeStylePO

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.conditions.ProfilingAttributeStylePO
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), [PersistentObject](../../options/PersistentObject.md)   @API(type=EXTENDABLE, src=PRIVATE) public class ProfilingAttributeStylePO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [PersistentObject](../../options/PersistentObject.md)
Contains information about a profiling attribute value and associated profiling styles.
  See Also:
* [Serialized Form](../../../../serialized-form.md#ro.sync.ecss.conditions.ProfilingAttributeStylePO)

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ANY_VALUE](#ANY_VALUE)
Wildcard constant for the attribute value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DOUBLE_UNDERLINE](#DOUBLE_UNDERLINE)
Text decoration double underline
  static final int [NO_COLOR](#NO_COLOR)
No color.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OVERLINE](#OVERLINE)
Text decoration overline
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UNDERLINE](#UNDERLINE)
Text decoration underline

## Constructor Summary
 Constructors
Constructor

Description
 [ProfilingAttributeStylePO](#%3Cinit%3E())()
Constructor.
  [ProfilingAttributeStylePO](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String,int,int,java.lang.String,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) framework, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue, int foreground, int background, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textDecoration, boolean bold, boolean italic)
Constructor.
  [ProfilingAttributeStylePO](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String,java.lang.String,int,int,java.lang.String,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) framework, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributGroupName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue, int foreground, int background, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textDecoration, boolean bold, boolean italic)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [checkValid](#checkValid())()
Check if object is valid to be used.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()
Forces all the persistent objects to be cloneable.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeGroupName](#getAttributeGroupName())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeName](#getAttributeName())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeValue](#getAttributeValue())()

 int [getBackgroundColor](#getBackgroundColor())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplayedValue](#getDisplayedValue())()
Get the display value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentTypePattern](#getDocumentTypePattern())()

 int [getForegroundColor](#getForegroundColor())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getNotPersistentFieldNames](#getNotPersistentFieldNames())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTextDecoration](#getTextDecoration())()
Get the text decoration to be applied on the content profiled by using this condition value.
  int [hashCode](#hashCode())()

 boolean [isBold](#isBold())()

 boolean [isEmpty](#isEmpty())()

 boolean [isItalic](#isItalic())()

 void [setAttributeGroupName](#setAttributeGroupName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeGroupName)
Set the attribute group name.
  void [setAttributeName](#setAttributeName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
Set the profiling attribute name.
  void [setAttributeValue](#setAttributeValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)
Set the profiling attribute value.
  void [setBackgroundColor](#setBackgroundColor(int))(int backgroundColor)
Set the background color to be applied on the content profiled by using this condition value.
  void [setBold](#setBold(boolean))(boolean bold)

 void [setDocTypePattern](#setDocTypePattern(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) docTypePattern)
Set the document type pattern.
  void [setForegroundColor](#setForegroundColor(int))(int foregroundColor)
Set the foreground color to be applied on the content profiled by using this condition value.
  void [setItalic](#setItalic(boolean))(boolean italic)

 void [setTextDecoration](#setTextDecoration(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textDecoration)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### UNDERLINE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UNDERLINE

Text decoration underline
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.conditions.ProfilingAttributeStylePO.UNDERLINE)

### DOUBLE_UNDERLINE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DOUBLE_UNDERLINE

Text decoration double underline
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.conditions.ProfilingAttributeStylePO.DOUBLE_UNDERLINE)

### OVERLINE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OVERLINE

Text decoration overline
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.conditions.ProfilingAttributeStylePO.OVERLINE)

### ANY_VALUE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ANY_VALUE

Wildcard constant for the attribute value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.conditions.ProfilingAttributeStylePO.ANY_VALUE)

### NO_COLOR

public static final int NO_COLOR

No color.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.conditions.ProfilingAttributeStylePO.NO_COLOR)

## Constructor Details

### ProfilingAttributeStylePO

public ProfilingAttributeStylePO()

Constructor.

### ProfilingAttributeStylePO

public ProfilingAttributeStylePO([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) framework, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue, int foreground, int background, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textDecoration, boolean bold, boolean italic)

Constructor.
  Parameters: framework - The name of the document type. attributeName - The attribute name. attributeValue - The attribute value. foreground - Foreground color to be applied on the content profiled by using this condition value. background - Background color to be applied on the content profiled by using this condition value. textDecoration - Text decoration to be applied on the content profiled by using this condition value. bold - true if the bold style should be applied on the content profiled by using this condition value. italic - true if the italic style should be applied on the content profiled by using this condition value.
### ProfilingAttributeStylePO

public ProfilingAttributeStylePO([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) framework, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributGroupName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue, int foreground, int background, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textDecoration, boolean bold, boolean italic)

Constructor.
  Parameters: framework - The name of the document type. attributeName - The attribute name. attributGroupName - The attribute group name. attributeValue - The attribute value. foreground - Foreground color to be applied on the content profiled by using this condition value. background - Background color to be applied on the content profiled by using this condition value. textDecoration - Text decoration to be applied on the content profiled by using this condition value. bold - true if the bold style should be applied on the content profiled by using this condition value. italic - true if the italic style should be applied on the content profiled by using this condition value.
## Method Details

### setDocTypePattern

public void setDocTypePattern([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) docTypePattern)

Set the document type pattern.
  Parameters: docTypePattern - The document type pattern.
### setAttributeName

public void setAttributeName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)

Set the profiling attribute name.
  Parameters: attributeName - The profiling attribute name.
### setAttributeGroupName

public void setAttributeGroupName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeGroupName)

Set the attribute group name.
  Parameters: attributeGroupName - The attributeGroupName to set.
### setAttributeValue

public void setAttributeValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)

Set the profiling attribute value.
  Parameters: attributeValue - The profiling attribute value.
### setForegroundColor

public void setForegroundColor(int foregroundColor)

Set the foreground color to be applied on the content profiled by using this condition value.
  Parameters: foregroundColor - The foreground color.
### getForegroundColor

public int getForegroundColor()
  Returns: Returns the foreground color to be applied on the content profiled by using this condition value.
### setBackgroundColor

public void setBackgroundColor(int backgroundColor)

Set the background color to be applied on the content profiled by using this condition value.
  Parameters: backgroundColor - The background color.
### getBackgroundColor

public int getBackgroundColor()
  Returns: Returns the background color to be applied on the content profiled by using this condition value.
### checkValid

public void checkValid() throws [InvalidPersistentObjException](../../options/InvalidPersistentObjException.md)
 Description copied from interface: [PersistentObject](../../options/PersistentObject.md#checkValid())
Check if object is valid to be used. Method is called after it is deserialized from options. If not then throw an InvalidPersistentObjException exception.
  Specified by: [checkValid](../../options/PersistentObject.md#checkValid()) in interface [PersistentObject](../../options/PersistentObject.md) Throws: [InvalidPersistentObjException](../../options/InvalidPersistentObjException.md) - Thrown when instance is not valid. See Also:
        * [PersistentObject.checkValid()](../../options/PersistentObject.md#checkValid())

### getNotPersistentFieldNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getNotPersistentFieldNames()
  Specified by: [getNotPersistentFieldNames](../../options/PersistentObject.md#getNotPersistentFieldNames()) in interface [PersistentObject](../../options/PersistentObject.md) Returns: The names of the field from this object which should not be serialized. See Also:
        * [PersistentObject.getNotPersistentFieldNames()](../../options/PersistentObject.md#getNotPersistentFieldNames())

### clone

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone()
 Description copied from interface: [PersistentObject](../../options/PersistentObject.md#clone())
Forces all the persistent objects to be cloneable.
  Specified by: [clone](../../options/PersistentObject.md#clone()) in interface [PersistentObject](../../options/PersistentObject.md) Overrides: [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Returns: A clone of this object. The clone and the original are disjunct. They share only immutable objects, like Strings, Integers, etc. See Also:
        * [Object.clone()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone())

### getDocumentTypePattern

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentTypePattern()
  Returns: The document type pattern
### getAttributeName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeName()
  Returns: The attribute name.
### getAttributeGroupName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeGroupName()
  Returns: The attribute group name.
### getAttributeValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeValue()
  Returns: The attribute value
### setTextDecoration

public void setTextDecoration([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textDecoration)
  Parameters: textDecoration - Text decoration to be applied on the content profiled by using this condition value.
### getTextDecoration

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTextDecoration()

Get the text decoration to be applied on the content profiled by using this condition value. Example values: "underline", "overline", "double_underline".
  Returns: Returns the text decoration.
### setBold

public void setBold(boolean bold)
  Parameters: bold - true if the bold style should be applied on the content profiled by using this condition value.
### isBold

public boolean isBold()
  Returns: Returns true if the bold style should be applied on the content profiled by using this condition value.
### setItalic

public void setItalic(boolean italic)
  Parameters: italic - true if the italic style should be applied on the content profiled by using this condition value.
### isItalic

public boolean isItalic()
  Returns: Returns true if the italic style should be applied on the content profiled by using this condition value.
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

### isEmpty

public boolean isEmpty()
  Returns: true if the profiling style is empty, meaning no text style, decoration and colors have been set.
### getDisplayedValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplayedValue()

Get the display value. If the attribute group is defined, will be contains by the displayed value.
  Returns: The displayed value.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
