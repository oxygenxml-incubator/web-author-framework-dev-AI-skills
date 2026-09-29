Package [ro.sync.ecss.dom.wrappers.mutable](package-summary.md)

# Class AuthorSource

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [javax.xml.transform.dom.DOMSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html)
        * ro.sync.ecss.dom.wrappers.mutable.AuthorSource
   All Implemented Interfaces: [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html)   @API(type=INTERNAL, src=PUBLIC) public class AuthorSource extends [DOMSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html)
A DOM-like source over a author document model. [DOMSource.getNode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html#getNode()) will return a DOM implementation over the Author nodes model.

## Field Summary

### Fields inherited from class javax.xml.transform.dom.[DOMSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html)
 [FEATURE](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html#FEATURE)
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorSource](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../extensions/api/AuthorAccess.md) authorAccess)
Constructor.
  [AuthorSource](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,boolean))([AuthorAccess](../../../extensions/api/AuthorAccess.md) authorAccess, boolean transparentXqueryUpdateReferences)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorAccess](../../../extensions/api/AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()

 [AuthorDocumentController](../../../extensions/api/AuthorDocumentController.md) [getController](#getController())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSystemId](#getSystemId())()

 void [setSystemId](#setSystemId(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId)

### Methods inherited from class javax.xml.transform.dom.[DOMSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html)
 [getNode](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html#getNode()), [isEmpty](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html#isEmpty()), [setNode](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html#setNode(org.w3c.dom.Node))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorSource

public AuthorSource([AuthorAccess](../../../extensions/api/AuthorAccess.md) authorAccess)

Constructor. The XInclude references over XQuery are not transparent, by default.
  Parameters: authorAccess - The author access of the author document.
### AuthorSource

public AuthorSource([AuthorAccess](../../../extensions/api/AuthorAccess.md) authorAccess, boolean transparentXqueryUpdateReferences)

Constructor.
  Parameters: authorAccess - The author access of the author document. transparentXqueryUpdateReferences - true to make xinclude nodes transparent in the document model.
## Method Details

### setSystemId

public void setSystemId([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId)
  Specified by: [setSystemId](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html#setSystemId(java.lang.String)) in interface [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) Overrides: [setSystemId](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html#setSystemId(java.lang.String)) in class [DOMSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html) See Also:
        * [Source.setSystemId(java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html#setSystemId(java.lang.String))

### getSystemId

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSystemId()
  Specified by: [getSystemId](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html#getSystemId()) in interface [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) Overrides: [getSystemId](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html#getSystemId()) in class [DOMSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/dom/DOMSource.html) See Also:
        * [Source.getSystemId()](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html#getSystemId())

### getController

public [AuthorDocumentController](../../../extensions/api/AuthorDocumentController.md) getController()
  Returns: Returns the controller.
### getAuthorAccess

public [AuthorAccess](../../../extensions/api/AuthorAccess.md) getAuthorAccess()
  Returns: Returns the author access for the current wrapped document.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
