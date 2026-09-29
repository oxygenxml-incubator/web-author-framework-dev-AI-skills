Package [ro.sync.ecss.extensions.api.link](package-summary.md)

# Class ElementLocator

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.link.ElementLocator
   Direct Known Subclasses: [DITAElementLocator](../../dita/DITAElementLocator.md), [DITAMapKeyDefElementLocator](../../dita/DITAMapKeyDefElementLocator.md), [IDElementLocator](../../commons/IDElementLocator.md), [XPointerElementLocator](../../commons/XPointerElementLocator.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ElementLocator extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Base class for custom elements locators used to locate an element based on a link. The source XML is parsed and notifications will be forwarded to ElementLocator objects in order for the references to be resolved.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [link](#link)
The link to be used to identify the element.

## Constructor Summary
 Constructors
Constructor

Description
 [ElementLocator](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract void [endElement](#endElement(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName)
Notification received when the end of an element has been encountered.
  abstract boolean [startElement](#startElement(java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.Attr%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName, [Attr](Attr.md)[] atts)
Notification received when the beginning of an element has been encountered.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### link

protected final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link

The link to be used to identify the element.

## Constructor Details

### ElementLocator

public ElementLocator([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link)

Constructor.
  Parameters: link - The link to be used to identify the element.
## Method Details

### startElement

public abstract boolean startElement([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName, [Attr](Attr.md)[] atts)

Notification received when the beginning of an element has been encountered. This method is invoked at the beginning of every element in the XML document; an event will be fired for every startElement (even when the element is empty).
  Parameters: uri - the namespace URI, or the empty string if the element has no namespace URI or if namespace processing is not being performed localName - the local name of the element qName - the qualified name of the element atts - an array with the attributes attached to the element. If there are no attributes, it shall be empty. The attributes are represented as [Attr](Attr.md) objects. Returns: true if the current element is indicated by the link.
### endElement

public abstract void endElement([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName)

Notification received when the end of an element has been encountered. This method is invoked at the end of every element in the XML document; an event will be fired for every endElement (even when the element is empty).
  Parameters: uri - the namespace URI, or the empty string if the element has no namespace URI or if namespace processing is not being performed localName - the local name of the element qName - the qualified XML name of the element
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
