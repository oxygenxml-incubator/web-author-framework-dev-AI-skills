Package [ro.sync.contentcompletion.xml](package-summary.md)

# Class ContextElement

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.contentcompletion.xml.ContextElement
   All Implemented Interfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)   @API(type=EXTENDABLE, src=PRIVATE) public class ContextElement extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)
Store information about an element inside a context, involved in the content completion process.

## Constructor Summary
 Constructors
Constructor

Description
 [ContextElement](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [clear](#clear())()
Clear the context element properties.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()

 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [Attribute](../../outline/xml/Attribute.md)[] [getAttributes](#getAttributes())()
Returns the element attributes.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNamespace](#getNamespace())()
Gets the element namespace.
  [ProxyNamespaceMapping](../../xml/ProxyNamespaceMapping.md) [getPrefixNamespaceMapping](#getPrefixNamespaceMapping())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getQName](#getQName())()
Gets the element qualified name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getType](#getType())()
Gets the context element type.
  void [setAttributes](#setAttributes(ro.sync.outline.xml.Attribute%5B%5D))([Attribute](../../outline/xml/Attribute.md)[] attributes)
Sets the element attributes.
  void [setNamespace](#setNamespace(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Sets the element namespace.
  void [setPnm](#setPnm(ro.sync.xml.ProxyNamespaceMapping))([ProxyNamespaceMapping](../../xml/ProxyNamespaceMapping.md) prefixNamespaceMapping)

 void [setQName](#setQName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Sets the element qualified name.
  void [setType](#setType(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) type)
Sets the context element type.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()
Gets description of the context element containing the following element properties: namespace, qualified name, type, attributes and the prefix-namespace mapping.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ContextElement

public ContextElement()

## Method Details

### getAttributes

public [Attribute](../../outline/xml/Attribute.md)[] getAttributes()

Returns the element attributes.
  Returns: An array of [Attribute](../../outline/xml/Attribute.md) objects corresponding to the context element. May be null
### setAttributes

public void setAttributes([Attribute](../../outline/xml/Attribute.md)[] attributes)

Sets the element attributes.
  Parameters: attributes - The array of [Attribute](../../outline/xml/Attribute.md) to set.
### getNamespace

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNamespace()

Gets the element namespace.
  Returns: Returns the element namespace or null if the element has no namespace.
### setNamespace

public void setNamespace([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)

Sets the element namespace.
  Parameters: namespace - The namespace to set.
### getPrefixNamespaceMapping

public [ProxyNamespaceMapping](../../xml/ProxyNamespaceMapping.md) getPrefixNamespaceMapping()
  Returns: Returns the prefix-namespace mapping.
### setPnm

public void setPnm([ProxyNamespaceMapping](../../xml/ProxyNamespaceMapping.md) prefixNamespaceMapping)
  Parameters: prefixNamespaceMapping - The prefix-namespace mapping to set.
### getQName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getQName()

Gets the element qualified name.
  Returns: Returns the element qName.
### setQName

public void setQName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Sets the element qualified name.
  Parameters: name - The qName to set.
### getType

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getType()

Gets the context element type.
  Returns: Returns the element type.
### setType

public void setType([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) type)

Sets the context element type. [See xsi:type specifications](http://www.w3.org/TR/xmlschema-1/#xsi_type)
  Parameters: type - The type to set.
### clear

public void clear()

Clear the context element properties.

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()

Gets description of the context element containing the following element properties: namespace, qualified name, type, attributes and the prefix-namespace mapping.
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
### clone

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone()
  Overrides: [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.clone()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone())

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
