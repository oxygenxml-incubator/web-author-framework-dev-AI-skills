Package [ro.sync.ecss.extensions.api.node](package-summary.md)

# Class AttrValue

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.node.AttrValue
   @API(type=EXTENDABLE, src=PUBLIC) public class AttrValue extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Contains informations about an attribute value. WARNING: This class should be immutable. Objects of this class are sometimes cached in the AuthorDocumentHandler

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [AttrValue](AttrValue.md) [EMPTY_VALUE](#EMPTY_VALUE)
Empty attribute value constant.

## Constructor Summary
 Constructors
Constructor

Description
 [AttrValue](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) specifiedValue)
Constructor for the attribute value.
  [AttrValue](#%3Cinit%3E(java.lang.String,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) normalizedValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rawValue, boolean isSpecified)
Constructor for the attribute value.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRawValue](#getRawValue())()
Get the attribute's raw value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getValue](#getValue())()
Get the attribute normalized value.
  int [hashCode](#hashCode())()

 boolean [isSpecified](#isSpecified())()
Checks if the attribute was specified in the XML document or comes as a default value from the schema, DTD, etc..
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### EMPTY_VALUE

public static final [AttrValue](AttrValue.md) EMPTY_VALUE

Empty attribute value constant.

## Constructor Details

### AttrValue

public AttrValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) specifiedValue)

Constructor for the attribute value.
  Parameters: specifiedValue - The simple attribute value which will be used both as raw value and normalized value.
### AttrValue

public AttrValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) normalizedValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rawValue, boolean isSpecified)

Constructor for the attribute value.
  Parameters: normalizedValue - Attribute normalized value (with entities expanded and WS's collapsed). rawValue - Attribute raw value (as it is specified in text with no white space collapsed and **entities** not expanded). isSpecified - true if specified in XML, false if this is a default value.
## Method Details

### getValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getValue()

Get the attribute normalized value.
  Returns: The attribute normalized value (with entities expanded and white spaces collapsed).
### getRawValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRawValue()

Get the attribute's raw value.
  Returns: Attribute raw value (as it is specified in text with no white space collapsed and **entities** not expanded).
### isSpecified

public boolean isSpecified()

Checks if the attribute was specified in the XML document or comes as a default value from the schema, DTD, etc..
  Returns: true if the element is specified in XML, false if this is a default value.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
