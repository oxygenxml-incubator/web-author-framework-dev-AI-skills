Package [ro.sync.exml.workspace.api.editor.page.author](package-summary.md)

# Class PseudoElementDescriptor

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.author.PseudoElementDescriptor
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class PseudoElementDescriptor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Describes a pseudo element.
  Since: 23
## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static enum  [PseudoElementDescriptor.PsuedoElementType](PseudoElementDescriptor.PsuedoElementType.md)
Pseudo-element type.

## Constructor Summary
 Constructors
Constructor

Description
 [PseudoElementDescriptor](#%3Cinit%3E(ro.sync.exml.workspace.api.editor.page.author.PseudoElementDescriptor.PsuedoElementType,int))([PseudoElementDescriptor.PsuedoElementType](PseudoElementDescriptor.PsuedoElementType.md) type, int index)
Created a pseudo-element descriptor object.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 int [getIndex](#getIndex())()

 [PseudoElementDescriptor.PsuedoElementType](PseudoElementDescriptor.PsuedoElementType.md) [getType](#getType())()

 int [hashCode](#hashCode())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### PseudoElementDescriptor

public PseudoElementDescriptor([PseudoElementDescriptor.PsuedoElementType](PseudoElementDescriptor.PsuedoElementType.md) type, int index)

Created a pseudo-element descriptor object.
  Parameters: type - The pseudo element type (before, after, marker, etc). index - The index of the pseudo element (e.g. 1 for element:before(1)).
## Method Details

### getType

public [PseudoElementDescriptor.PsuedoElementType](PseudoElementDescriptor.PsuedoElementType.md) getType()
  Returns: Returns the pseudo-element type (before, after, marker, etc.).
### getIndex

public int getIndex()
  Returns: Returns the index of the pseudo-element (e.g. 1 for element:before(1)).
### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
