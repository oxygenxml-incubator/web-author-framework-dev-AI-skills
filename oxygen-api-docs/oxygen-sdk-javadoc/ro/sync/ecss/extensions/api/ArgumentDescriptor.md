Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class ArgumentDescriptor

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.ArgumentDescriptor
   @API(type=EXTENDABLE, src=PUBLIC) public class ArgumentDescriptor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Descriptor class for an author operation argument.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [allowedValues](#allowedValues)
The array containing the allowed values for the arguments with type TYPE_CONSTANTS_LIST.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [defaultValue](#defaultValue)
The default value of the argument.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [description](#description)
The string argument description.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [name](#name)
The argument name.
  protected int [type](#type)
The argument type, can be one of: [TYPE_STRING](#TYPE_STRING), [TYPE_FRAGMENT](#TYPE_FRAGMENT), [TYPE_SCRIPT](#TYPE_SCRIPT), [TYPE_XPATH_EXPRESSION](#TYPE_XPATH_EXPRESSION), [TYPE_CONSTANT_LIST](#TYPE_CONSTANT_LIST),
  static final int [TYPE_CONSTANT_LIST](#TYPE_CONSTANT_LIST)
List of constant strings argument type.
  static final int [TYPE_FRAGMENT](#TYPE_FRAGMENT)
XML fragment argument type.
  static final int [TYPE_JAVA_OBJECT](#TYPE_JAVA_OBJECT)
An argument of this type is a Java object represented as a Map.
  static final int [TYPE_SCRIPT](#TYPE_SCRIPT)
Script type (XSLT or XQuery).
  static final int [TYPE_STRING](#TYPE_STRING)
String argument type.
  static final int [TYPE_XPATH_EXPRESSION](#TYPE_XPATH_EXPRESSION)
Xpath expression argument type.

## Constructor Summary
 Constructors
Constructor

Description
 [ArgumentDescriptor](#%3Cinit%3E(java.lang.String,int,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description)
Constructor of the argument descriptor class.
  [ArgumentDescriptor](#%3Cinit%3E(java.lang.String,int,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)
Constructor of the argument descriptor class.
  [ArgumentDescriptor](#%3Cinit%3E(java.lang.String,int,java.lang.String,java.lang.String%5B%5D,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)
Constructor of the argument descriptor class.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [decodeType](#decodeType(int))(int type)
Returns a [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description of the given argument type.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getAllowedValues](#getAllowedValues())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultValue](#getDefaultValue())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()

 int [getType](#getType())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### TYPE_STRING

public static final int TYPE_STRING

String argument type. The value is 0.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.ArgumentDescriptor.TYPE_STRING)

### TYPE_FRAGMENT

public static final int TYPE_FRAGMENT

XML fragment argument type. It is represented as a [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)The value is 1.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.ArgumentDescriptor.TYPE_FRAGMENT)

### TYPE_XPATH_EXPRESSION

public static final int TYPE_XPATH_EXPRESSION

Xpath expression argument type. It is represented as a [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)The value is 2.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.ArgumentDescriptor.TYPE_XPATH_EXPRESSION)

### TYPE_CONSTANT_LIST

public static final int TYPE_CONSTANT_LIST

List of constant strings argument type. The value is 3.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.ArgumentDescriptor.TYPE_CONSTANT_LIST)

### TYPE_SCRIPT

public static final int TYPE_SCRIPT

Script type (XSLT or XQuery). It is represented as a [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)The value is 4.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.ArgumentDescriptor.TYPE_SCRIPT)

### TYPE_JAVA_OBJECT

public static final int TYPE_JAVA_OBJECT

An argument of this type is a Java object represented as a Map. This Map is interpreted by the operation that receives it.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.ArgumentDescriptor.TYPE_JAVA_OBJECT)

### name

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name

The argument name.

### type

protected int type

The argument type, can be one of: [TYPE_STRING](#TYPE_STRING), [TYPE_FRAGMENT](#TYPE_FRAGMENT), [TYPE_SCRIPT](#TYPE_SCRIPT), [TYPE_XPATH_EXPRESSION](#TYPE_XPATH_EXPRESSION), [TYPE_CONSTANT_LIST](#TYPE_CONSTANT_LIST),

### description

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description

The string argument description.

### allowedValues

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedValues

The array containing the allowed values for the arguments with type TYPE_CONSTANTS_LIST.

### defaultValue

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue

The default value of the argument.

## Constructor Details

### ArgumentDescriptor

public ArgumentDescriptor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description)

Constructor of the argument descriptor class.
  Parameters: name - The name of the argument. type - The type of the argument, one of: [TYPE_STRING](#TYPE_STRING), [TYPE_FRAGMENT](#TYPE_FRAGMENT), [TYPE_SCRIPT](#TYPE_SCRIPT), [TYPE_XPATH_EXPRESSION](#TYPE_XPATH_EXPRESSION), [TYPE_CONSTANT_LIST](#TYPE_CONSTANT_LIST), description - The description of the argument.
### ArgumentDescriptor

public ArgumentDescriptor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)

Constructor of the argument descriptor class.
  Parameters: name - The name of the argument. type - The type of the argument, one of: [TYPE_STRING](#TYPE_STRING), [TYPE_FRAGMENT](#TYPE_FRAGMENT), [TYPE_SCRIPT](#TYPE_SCRIPT), [TYPE_XPATH_EXPRESSION](#TYPE_XPATH_EXPRESSION), [TYPE_CONSTANT_LIST](#TYPE_CONSTANT_LIST), description - The description of the argument. defaultValue - The default value of the argument.
### ArgumentDescriptor

public ArgumentDescriptor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] allowedValues, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)

Constructor of the argument descriptor class.
  Parameters: name - The name of the argument. type - The type of the argument, one of: [TYPE_STRING](#TYPE_STRING), [TYPE_FRAGMENT](#TYPE_FRAGMENT), [TYPE_SCRIPT](#TYPE_SCRIPT), [TYPE_XPATH_EXPRESSION](#TYPE_XPATH_EXPRESSION), [TYPE_CONSTANT_LIST](#TYPE_CONSTANT_LIST), description - The description of the argument. allowedValues - The allowed values for the defined argument. defaultValue - The default value of the argument.
## Method Details

### getName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()
  Returns: The name of the argument.
### getType

public int getType()
  Returns: The type of the argument, one of: [TYPE_STRING](#TYPE_STRING), [TYPE_FRAGMENT](#TYPE_FRAGMENT), [TYPE_SCRIPT](#TYPE_SCRIPT), [TYPE_XPATH_EXPRESSION](#TYPE_XPATH_EXPRESSION), [TYPE_CONSTANT_LIST](#TYPE_CONSTANT_LIST),
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the argument.
### decodeType

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) decodeType(int type)

Returns a [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description of the given argument type.
  Parameters: type - The argument type, one of: [TYPE_STRING](#TYPE_STRING), [TYPE_FRAGMENT](#TYPE_FRAGMENT), [TYPE_SCRIPT](#TYPE_SCRIPT), [TYPE_XPATH_EXPRESSION](#TYPE_XPATH_EXPRESSION), [TYPE_CONSTANT_LIST](#TYPE_CONSTANT_LIST), Returns: The type description, or null if the type is not valid.
### getAllowedValues

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getAllowedValues()
  Returns: The array with allowed values. Is used for TYPE_CONSTANTS_LIST arguments.
### getDefaultValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultValue()
  Returns: The default value of the argument.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
