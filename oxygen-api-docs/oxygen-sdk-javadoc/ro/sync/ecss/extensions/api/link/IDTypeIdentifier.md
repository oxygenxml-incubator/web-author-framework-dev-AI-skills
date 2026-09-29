Package [ro.sync.ecss.extensions.api.link](package-summary.md)

# Class IDTypeIdentifier

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.link.IDTypeIdentifier
   Direct Known Subclasses: [DefaultIDTypeIdentifier](DefaultIDTypeIdentifier.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class IDTypeIdentifier extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Identifier for an ID declaration or reference.

## Constructor Summary
 Constructors
Constructor

Description
 [IDTypeIdentifier](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getIdentifierType](#getIdentifierType())()
Gets a short description of the identifier type.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getValue](#getValue())()

 abstract boolean [isDeclaration](#isDeclaration())()
Checks if identifier corresponds to a declaration.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### IDTypeIdentifier

public IDTypeIdentifier()

## Method Details

### isDeclaration

public abstract boolean isDeclaration()

Checks if identifier corresponds to a declaration.
  Returns: true if identifier corresponds to a declaration.
### getValue

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getValue()
  Returns: The ID value.
### getIdentifierType

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getIdentifierType()

Gets a short description of the identifier type. By example for the default ID type recognition returns XML ID.
  Returns: A short description of the identifier type.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
