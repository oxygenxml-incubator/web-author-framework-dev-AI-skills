Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DITAIDElementLocator

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.link.ElementLocator](../api/link/ElementLocator.md)
        * [ro.sync.ecss.extensions.commons.IDElementLocator](../commons/IDElementLocator.md)
            * ro.sync.ecss.extensions.dita.DITAIDElementLocator
   @API(type=INTERNAL, src=PUBLIC) public class DITAIDElementLocator extends [IDElementLocator](../commons/IDElementLocator.md)
Implementation of an ElementLocator that locates elements based on a given link and checks if the attribute with the type ID matches the provided link and the class attribute contains 'topic/topic'.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.[IDElementLocator](../commons/IDElementLocator.md)
 [idVerifier](../commons/IDElementLocator.md#idVerifier)
### Fields inherited from class ro.sync.ecss.extensions.api.link.[ElementLocator](../api/link/ElementLocator.md)
 [link](../api/link/ElementLocator.md#link)
## Constructor Summary
 Constructors
Constructor

Description
 [DITAIDElementLocator](#%3Cinit%3E(ro.sync.ecss.extensions.api.link.IDTypeVerifier,java.lang.String,boolean))([IDTypeVerifier](../api/link/IDTypeVerifier.md) idVerifier, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link, boolean locateOnlyByElementID)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [startElement](#startElement(java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.Attr%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [Attr](../api/link/Attr.md)[] atts)
Notification received when the beginning of an element has been encountered.

### Methods inherited from class ro.sync.ecss.extensions.commons.[IDElementLocator](../commons/IDElementLocator.md)
 [endElement](../commons/IDElementLocator.md#endElement(java.lang.String,java.lang.String,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAIDElementLocator

public DITAIDElementLocator([IDTypeVerifier](../api/link/IDTypeVerifier.md) idVerifier, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) link, boolean locateOnlyByElementID)

Constructor.
  Parameters: idVerifier - Id type verifier link - The reference link locateOnlyByElementID - true to only locate based on the element ID.
## Method Details

### startElement

public boolean startElement([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) localName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [Attr](../api/link/Attr.md)[] atts)
 Description copied from class: [ElementLocator](../api/link/ElementLocator.md#startElement(java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.Attr%5B%5D))
Notification received when the beginning of an element has been encountered. This method is invoked at the beginning of every element in the XML document; an event will be fired for every startElement (even when the element is empty).
  Overrides: [startElement](../commons/IDElementLocator.md#startElement(java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.Attr%5B%5D)) in class [IDElementLocator](../commons/IDElementLocator.md) Parameters: uri - the namespace URI, or the empty string if the element has no namespace URI or if namespace processing is not being performed localName - the local name of the element name - the qualified name of the element atts - an array with the attributes attached to the element. If there are no attributes, it shall be empty. The attributes are represented as [Attr](../api/link/Attr.md) objects. Returns: true if the current element is indicated by the link. See Also:
        * [IDElementLocator.startElement(java.lang.String, java.lang.String, java.lang.String, ro.sync.ecss.extensions.api.link.Attr[])](../commons/IDElementLocator.md#startElement(java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.Attr%5B%5D))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
