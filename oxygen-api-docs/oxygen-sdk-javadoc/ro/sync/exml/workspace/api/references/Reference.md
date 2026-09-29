Package [ro.sync.exml.workspace.api.references](package-summary.md)

# Class Reference

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.references.Reference
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class Reference extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Simple bean class used to contain references. References have a type and an URL
  Since: 21.1
## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static enum  [Reference.Type](Reference.Type.md)
Constants enumerating the resource types.

## Constructor Summary
 Constructors
Constructor

Description
 [Reference](#%3Cinit%3E(ro.sync.exml.workspace.api.references.Reference.Type,java.lang.String))([Reference.Type](Reference.Type.md) type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri)
Constructs a new Reference with a type and an URI.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [Reference.Type](Reference.Type.md) [getType](#getType())()
Getter for the type of the reference (static content, link, CSS, etc.)
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getURL](#getURL())()
Getter for the string representing the URL of the external resource
  int [hashCode](#hashCode())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### Reference

public Reference([Reference.Type](Reference.Type.md) type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri)

Constructs a new Reference with a type and an URI.
  Parameters: type - the type of the reference uri - the URI
## Method Details

### getURL

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getURL()

Getter for the string representing the URL of the external resource
  Returns: the URL of the reference as string
### getType

public [Reference.Type](Reference.Type.md) getType()

Getter for the type of the reference (static content, link, CSS, etc.)
  Returns: the type of the reference
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
