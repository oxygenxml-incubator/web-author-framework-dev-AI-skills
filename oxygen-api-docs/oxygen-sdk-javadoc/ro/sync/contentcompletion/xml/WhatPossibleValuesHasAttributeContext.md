Package [ro.sync.contentcompletion.xml](package-summary.md)

# Class WhatPossibleValuesHasAttributeContext

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.contentcompletion.xml.Context](Context.md)
        * ro.sync.contentcompletion.xml.WhatContextInParent
            * ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext
   All Implemented Interfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)   @API(type=EXTENDABLE, src=PRIVATE) public class WhatPossibleValuesHasAttributeContext extends ro.sync.contentcompletion.xml.WhatContextInParent
It is used to determine the possible values of the current attribute.

## Field Summary

### Fields inherited from class ro.sync.contentcompletion.xml.WhatContextInParent
 parentElement
### Fields inherited from class ro.sync.contentcompletion.xml.[Context](Context.md)
 [elementStack](Context.md#elementStack), [idValuesList](Context.md#idValuesList), [infoProvider](Context.md#infoProvider), [nextSiblingElements](Context.md#nextSiblingElements), [prefixNamespaceMapping](Context.md#prefixNamespaceMapping), [previousSiblingElements](Context.md#previousSiblingElements), [xmlReader](Context.md#xmlReader)
## Constructor Summary
 Constructors
Constructor

Description
 [WhatPossibleValuesHasAttributeContext](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getAncestorValues](#getAncestorValues(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attribute)
Get the values of the specified (by name) attribute from the ancestors with the given name and namespace.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeName](#getAttributeName())()
Gets the name of the attribute, including the namespace prefix, if any.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeValue](#getAttributeValue())()
Gets the Value of the attribute, if any.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCurrentValueBeforeActivationChar](#getCurrentValueBeforeActivationChar())()
Get the existing attribute value before the activation char.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCurrentValuePrefix](#getCurrentValuePrefix())()
Get the already inserted value prefix.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultAttributeValue](#getDefaultAttributeValue())()

 [Attribute](../../outline/xml/Attribute.md)[] [getGrandparentAttributes](#getGrandparentAttributes())()
Get the grandparent's attributes.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getGrandparentElement](#getGrandparentElement())()
Get the qualified name of the grand parent element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getGrandparentNamespace](#getGrandparentNamespace())()
Get the namespace of the grand parent element.
  void [setAttributeName](#setAttributeName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
Sets the attribute name, including the namespace prefix, if any.
  void [setAttributeValue](#setAttributeValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)
Sets the existing attribute value, if any.
  void [setCurrentValueBeforeActivationChar](#setCurrentValueBeforeActivationChar(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValueBeforeActivationChar)
Set the current attribute value before the activation character
  void [setCurrentValuePrefix](#setCurrentValuePrefix(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValuePrefix)
Set the the already inserted value prefix.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()
Get a description of the current context.

### Methods inherited from class ro.sync.contentcompletion.xml.WhatContextInParent
 getParentElement, getPreviousAttributeNames, getPreviousAttributes, getPreviousAttributesList, getRootAttributes, pushContextElement, setParentElement
### Methods inherited from class ro.sync.contentcompletion.xml.[Context](Context.md)
 [computeContextXPathExpression](Context.md#computeContextXPathExpression()), [equals](Context.md#equals(java.lang.Object)), [executeXPath](Context.md#executeXPath(java.lang.String,java.lang.String%5B%5D)), [executeXPath](Context.md#executeXPath(java.lang.String,java.lang.String%5B%5D,boolean)), [getDefaultAttributeValue](Context.md#getDefaultAttributeValue(ro.sync.contentcompletion.xml.ContextElement,java.lang.String)), [getElementStack](Context.md#getElementStack()), [getIdValuesList](Context.md#getIdValuesList()), [getNextSiblingElements](Context.md#getNextSiblingElements()), [getPrefixNamespaceMapping](Context.md#getPrefixNamespaceMapping()), [getPreviousSiblingElements](Context.md#getPreviousSiblingElements()), [getProxyNamespaceMapping](Context.md#getProxyNamespaceMapping(ro.sync.contentcompletion.xml.Context)), [getSystemID](Context.md#getSystemID()), [setAdditionalContextInformationProvider](Context.md#setAdditionalContextInformationProvider(ro.sync.contentcompletion.xml.AdditionalContextInformationProvider)), [setElementStack](Context.md#setElementStack(java.util.Stack)), [setIdValuesList](Context.md#setIdValuesList(java.util.List)), [setNextSiblingElements](Context.md#setNextSiblingElements(java.util.List)), [setPrefixNamespaceMapping](Context.md#setPrefixNamespaceMapping(ro.sync.xml.ProxyNamespaceMapping)), [setPreviousSiblingElements](Context.md#setPreviousSiblingElements(java.util.List)), [setXMLReader](Context.md#setXMLReader(org.xml.sax.XMLReader))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WhatPossibleValuesHasAttributeContext

public WhatPossibleValuesHasAttributeContext()

## Method Details

### getAttributeName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeName()

Gets the name of the attribute, including the namespace prefix, if any.
  Returns: The attribute name.
### setAttributeName

public void setAttributeName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)

Sets the attribute name, including the namespace prefix, if any.
  Parameters: attributeName - The attribute name.
### getAttributeValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeValue()

Gets the Value of the attribute, if any.
  Returns: The attribute value.
### setAttributeValue

public void setAttributeValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)

Sets the existing attribute value, if any.
  Parameters: attributeValue - The attribute value.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()

Get a description of the current context.
  Overrides: toString in class ro.sync.contentcompletion.xml.WhatContextInParent Returns: A string containing information about the current context: attribute name, parent element qualified name, parent element type, element stack. See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### getGrandparentAttributes

public [Attribute](../../outline/xml/Attribute.md)[] getGrandparentAttributes()

Get the grandparent's attributes.
  Returns: The grandparent attributes.
### getGrandparentElement

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getGrandparentElement()

Get the qualified name of the grand parent element.
  Returns: The name of the attribute grandparent element. Throws: [EmptyStackException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/EmptyStackException.html) - In case the stack is empty.
### getGrandparentNamespace

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getGrandparentNamespace()

Get the namespace of the grand parent element.
  Returns: The element namespace for the element that is the grandparent of the current attribute. Throws: [EmptyStackException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/EmptyStackException.html) - In case the stack is empty.
### getAncestorValues

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getAncestorValues([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attribute)

Get the values of the specified (by name) attribute from the ancestors with the given name and namespace.
  Parameters: name - The name of the element where the attribute must be searched. namespace - The namespace of the element where the attribute must be searched. attribute - The attribute local name. Returns: A list of attribute values, never null.
### getCurrentValuePrefix

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCurrentValuePrefix()

Get the already inserted value prefix.
  Returns: The text from the start position of the attribute value and the caret position. Can be null if no prefix was found.
### setCurrentValuePrefix

public void setCurrentValuePrefix([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValuePrefix)

Set the the already inserted value prefix. For instance, if having starting the CC at the position "|"
```

 test="element/na|"

```
Then the value returned is "element/na".
  Parameters: currentValuePrefix - The text from the start position of the attribute value and the caret position.
### getCurrentValueBeforeActivationChar

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCurrentValueBeforeActivationChar()

Get the existing attribute value before the activation char. For instance, if having starting the CC at the position "|"
```

 <xsl:if test="element/na|" />

```
Then the value returned is "element".
  Returns: Returns the current attribute value before the activation char.
### setCurrentValueBeforeActivationChar

public void setCurrentValueBeforeActivationChar([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValueBeforeActivationChar)

Set the current attribute value before the activation character
  Parameters: currentValueBeforeActivationChar -
### clone

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone()
  Overrides: clone in class ro.sync.contentcompletion.xml.WhatContextInParent See Also:
        * WhatContextInParent.clone()

### getDefaultAttributeValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultAttributeValue()
  Returns: The default value of the attribute in the associated schema.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
