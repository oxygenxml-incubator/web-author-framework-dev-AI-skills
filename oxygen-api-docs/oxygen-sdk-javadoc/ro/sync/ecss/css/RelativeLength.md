Package [ro.sync.ecss.css](package-summary.md)

# Class RelativeLength

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.css.RelativeLength
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class RelativeLength extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
A length that may be expressed as an absolute or relative value, or as an "auto" value, that is to be computed at later time, by the layout engine.

## Constructor Summary
 Constructors
Modifier

Constructor

Description
 protected  [RelativeLength](#%3Cinit%3E(float,byte))(float value, byte type)
Constructor

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static [RelativeLength](RelativeLength.md) [createAbsolute](#createAbsolute(int))(int value)
Create an absolute value length.
  static [RelativeLength](RelativeLength.md) [createAbsolute](#createAbsolute(org.w3c.css.sac.LexicalUnit,float,ro.sync.ecss.css.LexicalUnitEvaluator))(org.w3c.css.sac.LexicalUnit lu, float fontSize, ro.sync.ecss.css.LexicalUnitEvaluator evaluator)
Create an absolute value length.
  static [RelativeLength](RelativeLength.md) [createAuto](#createAuto())()
Create an automatic relative length.
  static [RelativeLength](RelativeLength.md) [createRelative](#createRelative(float))(float percentage)
Create a relative length representing a relative value.
  static [RelativeLength](RelativeLength.md) [createRelativeOrCalc](#createRelativeOrCalc(org.w3c.css.sac.LexicalUnit,float,ro.sync.ecss.css.LexicalUnitEvaluator))(org.w3c.css.sac.LexicalUnit lu, float fontSize, ro.sync.ecss.css.LexicalUnitEvaluator evaluator)
Create a relative length representing a relative value, like a percent, or a calc expression.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 int [get](#get(int))(int referenceLength)
Return the evaluated value of the RelativeLength given a reference value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLengthRepr](#getLengthRepr())()

 float [getValue](#getValue())()

 int [hashCode](#hashCode())()

 boolean [isAbsolute](#isAbsolute())()

 boolean [isAuto](#isAuto())()

 boolean [isCalc](#isCalc())()

 boolean [isRelative](#isRelative())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### RelativeLength

protected RelativeLength(float value, byte type)

Constructor
  Parameters: value - The absolute or percentage value. type - Indicates if the value is absolute, relative or "auto".
## Method Details

### createAbsolute

public static [RelativeLength](RelativeLength.md) createAbsolute(int value)

Create an absolute value length.
  Parameters: value - The value of the absolute length. Returns: The new absolute value RelativeLength.
### createRelative

public static [RelativeLength](RelativeLength.md) createRelative(float percentage)

Create a relative length representing a relative value.
  Parameters: percentage - The percentage from the value this length will refer to. (e.g: 50%) Returns: The new relative value RelativeLength.
### createAuto

public static [RelativeLength](RelativeLength.md) createAuto()

Create an automatic relative length. This is just an immutable constant marker.
  Returns: The "auto" relative length. Always the same object.
### get

public int get(int referenceLength)

Return the evaluated value of the RelativeLength given a reference value. If this object represents an absolute value, that value is simply returned. Otherwise, returns the given reference length multiplied by the given percentage divided to 100 and rounded to the nearest integer, or maybe a calculated expression.
  Parameters: referenceLength - Reference length for percentage lengths. Returns: The actual value.
### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### getLengthRepr

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLengthRepr()
  Returns: a string representing the equivalent CSS expression.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### isAuto

public boolean isAuto()
  Returns: True if the relative length is automatic.
### isRelative

public boolean isRelative()
  Returns: True if the length is relative.
### isAbsolute

public boolean isAbsolute()
  Returns: True if the length is absolute.
### getValue

public float getValue()
  Returns: The value of the absolute length or the percentage of a relative length.
### isCalc

public boolean isCalc()
  Returns: True if the length is a calculated value.
### createAbsolute

public static [RelativeLength](RelativeLength.md) createAbsolute(org.w3c.css.sac.LexicalUnit lu, float fontSize, ro.sync.ecss.css.LexicalUnitEvaluator evaluator)

Create an absolute value length.
  Parameters: lu - The value of the absolute length. fontSize - the size of the font, used to solve ems. evaluator - The evaluator, used to solve rems, pc, pt, in, cm. Returns: The new absolute value RelativeLength.
### createRelativeOrCalc

public static [RelativeLength](RelativeLength.md) createRelativeOrCalc(org.w3c.css.sac.LexicalUnit lu, float fontSize, ro.sync.ecss.css.LexicalUnitEvaluator evaluator)

Create a relative length representing a relative value, like a percent, or a calc expression.
  Parameters: lu - The percentage from the value this length will refer to. (e.g: 50%) or a calc expression (e.g 50% - 3pt). fontSize - The element font size. This is used to solve em's. evaluator - The lexical unit evaluator. This is used to solve rem's, pt's, and othersizes. Returns: The new relative value RelativeLength.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
