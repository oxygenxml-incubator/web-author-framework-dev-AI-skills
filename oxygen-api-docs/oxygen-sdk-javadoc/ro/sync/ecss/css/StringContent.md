Package [ro.sync.ecss.css](package-summary.md)

# Class StringContent

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.css.StringContent
   All Implemented Interfaces: [StaticContent](StaticContent.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class StringContent extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [StaticContent](StaticContent.md)
String content

## Field Summary

### Fields inherited from interface ro.sync.ecss.css.[StaticContent](StaticContent.md)
 [CONTENT_CONTENT](StaticContent.md#CONTENT_CONTENT), [COUNTER_CONTENT](StaticContent.md#COUNTER_CONTENT), [COUNTERS_CONTENT](StaticContent.md#COUNTERS_CONTENT), [EDITOR_CONTENT](StaticContent.md#EDITOR_CONTENT), [LABEL_CONTENT](StaticContent.md#LABEL_CONTENT), [LEADER_CONTENT](StaticContent.md#LEADER_CONTENT), [STRING_FUNCTION_CONTENT](StaticContent.md#STRING_FUNCTION_CONTENT), [TARGET_COUNTER_CONTENT](StaticContent.md#TARGET_COUNTER_CONTENT), [TARGET_COUNTERS_CONTENT](StaticContent.md#TARGET_COUNTERS_CONTENT), [TEXT_CONTENT](StaticContent.md#TEXT_CONTENT), [URI_CONTENT](StaticContent.md#URI_CONTENT)
## Constructor Summary
 Constructors
Constructor

Description
 [StringContent](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Constructor

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 int [getType](#getType())()
Gets the content type.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getValue](#getValue())()

 int [hashCode](#hashCode())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### StringContent

public StringContent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Constructor
  Parameters: value - Value
## Method Details

### getType

public int getType()
 Description copied from interface: [StaticContent](StaticContent.md#getType())
Gets the content type.
  Specified by: [getType](StaticContent.md#getType()) in interface [StaticContent](StaticContent.md) Returns: The content type. See Also:
        * [StaticContent.getType()](StaticContent.md#getType())

### getValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getValue()
  Returns: The text value
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
