Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class WidthRepresentation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.WidthRepresentation
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)   @API(type=EXTENDABLE, src=PUBLIC) public class WidthRepresentation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)
Specifies the fixed and relative width determined from the value of width/colwidth attribute of the col.
  See Also:
* [Serialized Form](../../../../../serialized-form.md#ro.sync.ecss.extensions.api.WidthRepresentation)

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static enum  [WidthRepresentation.Unit](WidthRepresentation.Unit.md)
The fixed width unit.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [WidthRepresentation](WidthRepresentation.md) [DEFAULT_WIDTH_REPRESENTATION](#DEFAULT_WIDTH_REPRESENTATION)
The default width representation.

## Constructor Summary
 Constructors
Constructor

Description
 [WidthRepresentation](#%3Cinit%3E(float,ro.sync.ecss.extensions.api.WidthRepresentation.Unit,float,boolean))(float fixedWidthValue, [WidthRepresentation.Unit](WidthRepresentation.Unit.md) fixedWidthUnit, float relativeWidth, boolean isRelativeToParent)
Constructor.
  [WidthRepresentation](#%3Cinit%3E(java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) widthString, boolean acceptPercents)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAlign](#getAlign())()
Get the text align specified on the colspec.
  float [getFixedWidth](#getFixedWidth())()

 [WidthRepresentation.Unit](WidthRepresentation.Unit.md) [getFixedWidthUnit](#getFixedWidthUnit())()

 float [getRelativeWidth](#getRelativeWidth())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getWidthRepresentation](#getWidthRepresentation())()

 boolean [isApplicable](#isApplicable())()

 boolean [isRelativeToParent](#isRelativeToParent())()

 boolean [isSpecified](#isSpecified())()
Check if this width is specified.
  void [setAlign](#setAlign(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) align)
Set the text align specified on the colspec.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### DEFAULT_WIDTH_REPRESENTATION

public static final [WidthRepresentation](WidthRepresentation.md) DEFAULT_WIDTH_REPRESENTATION

The default width representation. EXM-32772 KEEP THIS HERE, IMPORTANT FOR BACKWARD COMPATIBILITY.

## Constructor Details

### WidthRepresentation

public WidthRepresentation(float fixedWidthValue, [WidthRepresentation.Unit](WidthRepresentation.Unit.md) fixedWidthUnit, float relativeWidth, boolean isRelativeToParent)

Constructor.
  Parameters: fixedWidthValue - The fixed width value. Ex: 2.5 fixedWidthUnit - The unit of fixed width. Defaults to PIXEL. relativeWidth - The relative width part. Ex: 0.33 isRelativeToParent - If true then the relative width represents a percentage of the parent table width, otherwise the relative value represent a proportional width which is evaluated taking into account the proportional values of the other columns. For example, if there are two columns with 70% and 30% relative widths then the table total width will be divided according with this values. If the relative widths for the two columns are specified in proportional units and, for example, have the values 1 for the first column and 2 for the second column then the second column will be twice as large as the first one.
### WidthRepresentation

public WidthRepresentation([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) widthString, boolean acceptPercents)

Constructor. Create a ColWidth corresponding to the given width representation.
  Parameters: widthString - The string representation of the Width. The representation format must be a sum of terms with the following format: n(\*|%|units). If there are more that one terms with the same form (fixed or relative) then corresponding width (fixed or relative) will be reseted. acceptPercents - If true then percentage values are accepted
## Method Details

### getFixedWidth

public float getFixedWidth()
  Returns: Returns the fixed width part of the width representation. Ex: 2.5
### getFixedWidthUnit

public [WidthRepresentation.Unit](WidthRepresentation.Unit.md) getFixedWidthUnit()
  Returns: Returns the fixed width unit. Ex: Unit.CENTIMETER
### getRelativeWidth

public float getRelativeWidth()
  Returns: Returns the relative width part of the width representation.
### isRelativeToParent

public boolean isRelativeToParent()
  Returns: Returns true if the relative part of the width is expressed relative to the parent width, false if is expressed relative to other siblings.
### isApplicable

public boolean isApplicable()
  Returns: true if the current width representation should be taken into account when building the layout.
### isSpecified

public boolean isSpecified()

Check if this width is specified.
  Returns: true if the width representation is resulted from a width specified in the document or false if this a default width representation.
### getAlign

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAlign()

Get the text align specified on the colspec.
  Returns: Returns the text align.
### setAlign

public void setAlign([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) align)

Set the text align specified on the colspec.
  Parameters: align - The align value.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### getWidthRepresentation

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getWidthRepresentation()
  Returns: The string representation of the width. The format of the width is  [fixed_width][fixed_width_unit] + [relative_width %|\*]
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
