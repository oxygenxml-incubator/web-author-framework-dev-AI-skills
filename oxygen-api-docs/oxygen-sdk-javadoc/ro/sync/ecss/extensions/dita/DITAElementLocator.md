Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DITAElementLocator

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.link.ElementLocator](../api/link/ElementLocator.md)
        * ro.sync.ecss.extensions.dita.DITAElementLocator
   @API(type=INTERNAL, src=PUBLIC) public class DITAElementLocator extends [ElementLocator](../api/link/ElementLocator.md)
An implementation for a DITA element when the referred element is not a topic. So the link has the following pattern: topicID/elementID

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.api.link.[ElementLocator](../api/link/ElementLocator.md)
 [link](../api/link/ElementLocator.md#link)
## Constructor Summary
 Constructors
Constructor

Description
 [DITAElementLocator](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)
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

### DITAElementLocator

public DITAElementLocator([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)

Constructor.
  Parameters: link - The link used to identify the element.
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
