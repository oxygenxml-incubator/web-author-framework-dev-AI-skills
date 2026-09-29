Package [ro.sync.ecss.extensions.commons](package-summary.md)

# Class XPointerElementLocator

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.link.ElementLocator](../api/link/ElementLocator.md)
        * ro.sync.ecss.extensions.commons.XPointerElementLocator
   @API(type=INTERNAL, src=PUBLIC) public class XPointerElementLocator extends [ElementLocator](../api/link/ElementLocator.md)
Element locator for links that have the one of the following patterns:
* element(elementID) - locate the element with the same id
* element(/1/2/5) - A child sequence appearing alone identifies an element by means of stepwise navigation, which is directed by a sequence of integers separated by slashes (/); each integer n locates the nth child element of the previously located element.
* element(elementID/3/4) - A child sequence appearing after an NCName identifies an element by means of stepwise navigation, starting from the element located by the given name.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.api.link.[ElementLocator](../api/link/ElementLocator.md)
 [link](../api/link/ElementLocator.md#link)
## Constructor Summary
 Constructors
Constructor

Description
 [XPointerElementLocator](#%3Cinit%3E(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String))([IDTypeVerifier](../api/link/IDTypeVerifier.md) idVerifier, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [endElement](#endElement(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Notification received when the end of an element has been encountered.
  boolean [startElement](#startElement(java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.Attr%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [Attr](../api/link/Attr.md)[] atts)
Notification received when the beginning of an element has been encountered.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XPointerElementLocator

public XPointerElementLocator([IDTypeVerifier](../api/link/IDTypeVerifier.md) idVerifier, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)throws [ElementLocatorException](../api/link/ElementLocatorException.md)

Constructor.
  Parameters: idVerifier - Verifies if an given attribute has the type ID. link - The link that gives the element position. Throws: [ElementLocatorException](../api/link/ElementLocatorException.md) - When the link format is not supported.
## Method Details

### endElement

public void endElement([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
 Description copied from class: [ElementLocator](../api/link/ElementLocator.md#endElement(java.lang.String,java.lang.String,java.lang.String))
Notification received when the end of an element has been encountered. This method is invoked at the end of every element in the XML document; an event will be fired for every endElement (even when the element is empty).
  Specified by: [endElement](../api/link/ElementLocator.md#endElement(java.lang.String,java.lang.String,java.lang.String)) in class [ElementLocator](../api/link/ElementLocator.md) Parameters: uri - the namespace URI, or the empty string if the element has no namespace URI or if namespace processing is not being performed localName - the local name of the element name - the qualified XML name of the element See Also:
        * [ElementLocator.endElement(java.lang.String, java.lang.String, java.lang.String)](../api/link/ElementLocator.md#endElement(java.lang.String,java.lang.String,java.lang.String))

### startElement

public boolean startElement([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [Attr](../api/link/Attr.md)[] atts)
 Description copied from class: [ElementLocator](../api/link/ElementLocator.md#startElement(java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.Attr%5B%5D))
Notification received when the beginning of an element has been encountered. This method is invoked at the beginning of every element in the XML document; an event will be fired for every startElement (even when the element is empty).
  Specified by: [startElement](../api/link/ElementLocator.md#startElement(java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.Attr%5B%5D)) in class [ElementLocator](../api/link/ElementLocator.md) Parameters: uri - the namespace URI, or the empty string if the element has no namespace URI or if namespace processing is not being performed localName - the local name of the element name - the qualified name of the element atts - an array with the attributes attached to the element. If there are no attributes, it shall be empty. The attributes are represented as [Attr](../api/link/Attr.md) objects. Returns: true if the current element is indicated by the link. See Also:
        * [ElementLocator.startElement(java.lang.String, java.lang.String, java.lang.String, ro.sync.ecss.extensions.api.link.Attr[])](../api/link/ElementLocator.md#startElement(java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.Attr%5B%5D))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
