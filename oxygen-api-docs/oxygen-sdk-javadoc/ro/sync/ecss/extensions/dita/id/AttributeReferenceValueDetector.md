Package [ro.sync.ecss.extensions.dita.id](package-summary.md)

# Class AttributeReferenceValueDetector

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.id.AttributeReferenceValueDetector
   @API(type=INTERNAL, src=PUBLIC) public class AttributeReferenceValueDetector extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Detects the [AttrValue](../../api/node/AttrValue.md) of a node and the name of the attribute.

## Constructor Summary
 Constructors
Constructor

Description
 [AttributeReferenceValueDetector](#%3Cinit%3E(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) element)
Creates the detector.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AttrValue](../../api/node/AttrValue.md) [detectRefAttrValue](#detectRefAttrValue())()
Detects the reference attribute value of local elements.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDetectedRefAttrName](#getDetectedRefAttrName())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AttributeReferenceValueDetector

public AttributeReferenceValueDetector([AuthorElement](../../api/node/AuthorElement.md) element)

Creates the detector.
  Parameters: element - The element to check for reference attributes.
## Method Details

### detectRefAttrValue

public [AttrValue](../../api/node/AttrValue.md) detectRefAttrValue()

Detects the reference attribute value of local elements.
  Returns: The [AttrValue](../../api/node/AttrValue.md) provided by the href, conref or others reference attributes. null if nothing is detected or element has a non-local scope.
### getDetectedRefAttrName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDetectedRefAttrName()
  Returns: The name of the attribute that contains the reference. Can be href, conref and others. null if the element does not have a reference.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
