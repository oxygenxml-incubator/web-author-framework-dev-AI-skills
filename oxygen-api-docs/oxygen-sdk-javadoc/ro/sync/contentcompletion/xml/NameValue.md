Package [ro.sync.contentcompletion.xml](package-summary.md)

# Class NameValue

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.contentcompletion.xml.NameValue
   Direct Known Subclasses: [ExternalEntityNameValue](ExternalEntityNameValue.md)   @API(type=EXTENDABLE, src=PRIVATE) public class NameValue extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
A pair class with name and value.

## Constructor Summary
 Constructors
Constructor

Description
 [NameValue](#%3Cinit%3E(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Constructor.
  [NameValue](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentation)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) other)
Verifies if two objects are equals
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentation](#getDocumentation())()
Gets the documentation.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Gets the name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getValue](#getValue())()
Gets the value.
  int [hashCode](#hashCode())()

 void [setDocumentation](#setDocumentation(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentation)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()
Returns the name and value formated as  **n: name v: value**

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### NameValue

public NameValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Constructor.
  Parameters: name - The name. value - The value.
### NameValue

public NameValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentation)

Constructor.
  Parameters: name - The name. value - The value. documentation - The documentation.
## Method Details

### getName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

Gets the name.
  Returns: The name.
### getValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getValue()

Gets the value.
  Returns: The value.
### getDocumentation

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentation()

Gets the documentation.
  Returns: The documentation.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()

Returns the name and value formated as  **n: name v: value**
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Returns: the name and value of the NameValue object.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) other)

Verifies if two objects are equals
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Parameters: other - The object to compare to. Returns: True if the two object have the same name and value. False otherwise.
### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### setDocumentation

public void setDocumentation([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentation)
  Parameters: documentation - The documentation to set.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
