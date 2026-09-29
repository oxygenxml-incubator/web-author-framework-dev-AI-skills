Package [ro.sync.outline.xml](package-summary.md)

# Class Attribute

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.outline.xml.Attribute
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class Attribute extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
An attribute representation used mainly in the content completion process.

## Constructor Summary
 Constructors
Constructor

Description
 [Attribute](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix)
Creates an attribute with a specified qualified name, value, namespace and prefix.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLocalName](#getLocalName())()
Gets the attribute local name.
  int [getNameEndOffset](#getNameEndOffset())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNamespace](#getNamespace())()
Gets the attribute namespace.
  int [getNameStartOffset](#getNameStartOffset())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPrefix](#getPrefix())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getQName](#getQName())()
Gets the attribute fully qualified name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getValue](#getValue())()
Gets for the attribute value.
  int [getValueEndOffset](#getValueEndOffset())()

 int [getValueStartOffset](#getValueStartOffset())()

 boolean [hasValue](#hasValue())()
Check if the attribute has a value, or is empty attribute.
  boolean [isDefaultNamespaceDeclaration](#isDefaultNamespaceDeclaration())()

 boolean [isNamespaceDeclaration](#isNamespaceDeclaration())()

 void [setNameEndOffset](#setNameEndOffset(int))(int nameEndOffset)

 void [setNamespace](#setNamespace(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)

 void [setNameStartOffset](#setNameStartOffset(int))(int nameStartOffset)

 void [setValueEndOffset](#setValueEndOffset(int))(int valueEndOffset)

 void [setValueStartOffset](#setValueStartOffset(int))(int valueStartOffset)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()
Return the string representation of the attribute.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### Attribute

public Attribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prefix)

Creates an attribute with a specified qualified name, value, namespace and prefix.
  Parameters: qName - The attribute fully qualified name. value - The attribute value. namespace - The attribute namespace. prefix - The attribute prefix.
## Method Details

### getQName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getQName()

Gets the attribute fully qualified name.
  Returns: The attribute qualified name of the attribute.
### getValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getValue()

Gets for the attribute value.
  Returns: The value. Not null.
### getNamespace

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNamespace()

Gets the attribute namespace.
  Returns: The attribute namespace.
### getLocalName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLocalName()

Gets the attribute local name.
  Returns: The attribute local name.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()

Return the string representation of the attribute. It contains the attribute qualified name, the namespace and the attribute value.
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
### getNameEndOffset

public int getNameEndOffset()
  Returns: The end offset of the name.
### getNameStartOffset

public int getNameStartOffset()
  Returns: The start offset of the name.
### getValueEndOffset

public int getValueEndOffset()
  Returns: The end offset of the value.
### getValueStartOffset

public int getValueStartOffset()
  Returns: The start offset of the value.
### isNamespaceDeclaration

public boolean isNamespaceDeclaration()
  Returns: If true the attribute is namespace declaration.
### getPrefix

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPrefix()
  Returns: Returns the attribute prefix.
### setNamespace

public void setNamespace([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
  Parameters: namespace - The attribute namespace to set.
### setNameStartOffset

public void setNameStartOffset(int nameStartOffset)
  Parameters: nameStartOffset - The attribute name start offset to set.
### setNameEndOffset

public void setNameEndOffset(int nameEndOffset)
  Parameters: nameEndOffset - The attribute name end offset to set.
### setValueStartOffset

public void setValueStartOffset(int valueStartOffset)
  Parameters: valueStartOffset - The value start offset to set.
### setValueEndOffset

public void setValueEndOffset(int valueEndOffset)
  Parameters: valueEndOffset - The value end offset to set.
### isDefaultNamespaceDeclaration

public boolean isDefaultNamespaceDeclaration()
  Returns: Returns the default namespace declaration.
### hasValue

public boolean hasValue()

Check if the attribute has a value, or is empty attribute.
  Returns: true if it has a value, false for empty attributes.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
