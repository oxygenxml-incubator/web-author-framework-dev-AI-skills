Package [ro.sync.ecss.extensions.api.link](package-summary.md)

# Class DefaultIDTypeIdentifier

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.link.IDTypeIdentifier](IDTypeIdentifier.md)
        * ro.sync.ecss.extensions.api.link.DefaultIDTypeIdentifier
   @API(type=EXTENDABLE, src=PUBLIC) public class DefaultIDTypeIdentifier extends [IDTypeIdentifier](IDTypeIdentifier.md)
Default implementation for [IDTypeIdentifier](IDTypeIdentifier.md).

## Constructor Summary
 Constructors
Constructor

Description
 [DefaultIDTypeIdentifier](#%3Cinit%3E(java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean isDeclaration)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getIdentifierType](#getIdentifierType())()
Gets a short description of the identifier type.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getValue](#getValue())()

 boolean [isDeclaration](#isDeclaration())()
Checks if identifier corresponds to a declaration.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DefaultIDTypeIdentifier

public DefaultIDTypeIdentifier([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean isDeclaration)

Constructor.
  Parameters: value - The ID value. isDeclaration - True if identifier corresponds to an ID declaration.
## Method Details

### isDeclaration

public boolean isDeclaration()
 Description copied from class: [IDTypeIdentifier](IDTypeIdentifier.md#isDeclaration())
Checks if identifier corresponds to a declaration.
  Specified by: [isDeclaration](IDTypeIdentifier.md#isDeclaration()) in class [IDTypeIdentifier](IDTypeIdentifier.md) Returns: true if identifier corresponds to a declaration. See Also:
        * [IDTypeIdentifier.isDeclaration()](IDTypeIdentifier.md#isDeclaration())

### getValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getValue()
  Specified by: [getValue](IDTypeIdentifier.md#getValue()) in class [IDTypeIdentifier](IDTypeIdentifier.md) Returns: The ID value. See Also:
        * [IDTypeIdentifier.getValue()](IDTypeIdentifier.md#getValue())

### getIdentifierType

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getIdentifierType()
 Description copied from class: [IDTypeIdentifier](IDTypeIdentifier.md#getIdentifierType())
Gets a short description of the identifier type. By example for the default ID type recognition returns XML ID.
  Specified by: [getIdentifierType](IDTypeIdentifier.md#getIdentifierType()) in class [IDTypeIdentifier](IDTypeIdentifier.md) Returns: A short description of the identifier type. See Also:
        * [IDTypeIdentifier.getIdentifierType()](IDTypeIdentifier.md#getIdentifierType())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
