Package [ro.sync.contentcompletion.xml](package-summary.md)

# Class WhatElementsCanGoHereContext

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.contentcompletion.xml.Context](Context.md)
        * ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext
   All Implemented Interfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)   @API(type=EXTENDABLE, src=PRIVATE) public class WhatElementsCanGoHereContext extends [Context](Context.md)
It is used to determine the elements that can be inserted in the current context.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected ro.sync.document.SyntaxDocumentBase [doc](#doc)
The syntax document.
  protected int [positionInDoc](#positionInDoc)
Position in document.

### Fields inherited from class ro.sync.contentcompletion.xml.[Context](Context.md)
 [elementStack](Context.md#elementStack), [idValuesList](Context.md#idValuesList), [infoProvider](Context.md#infoProvider), [nextSiblingElements](Context.md#nextSiblingElements), [prefixNamespaceMapping](Context.md#prefixNamespaceMapping), [previousSiblingElements](Context.md#previousSiblingElements), [xmlReader](Context.md#xmlReader)
## Constructor Summary
 Constructors
Constructor

Description
 [WhatElementsCanGoHereContext](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()

 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 ro.sync.document.SyntaxDocumentBase [getDoc](#getDoc())()
Get the current document.
  int [getPositionInDoc](#getPositionInDoc())()
Gets the position in the document.
  void [setDoc](#setDoc(ro.sync.document.SyntaxDocumentBase))(ro.sync.document.SyntaxDocumentBase doc)
Set the current document.
  void [setPositionInDoc](#setPositionInDoc(int))(int positionInDoc)
Sets the position in the document.

### Methods inherited from class ro.sync.contentcompletion.xml.[Context](Context.md)
 [computeContextXPathExpression](Context.md#computeContextXPathExpression()), [executeXPath](Context.md#executeXPath(java.lang.String,java.lang.String%5B%5D)), [executeXPath](Context.md#executeXPath(java.lang.String,java.lang.String%5B%5D,boolean)), [getDefaultAttributeValue](Context.md#getDefaultAttributeValue(ro.sync.contentcompletion.xml.ContextElement,java.lang.String)), [getElementStack](Context.md#getElementStack()), [getIdValuesList](Context.md#getIdValuesList()), [getNextSiblingElements](Context.md#getNextSiblingElements()), [getPrefixNamespaceMapping](Context.md#getPrefixNamespaceMapping()), [getPreviousSiblingElements](Context.md#getPreviousSiblingElements()), [getProxyNamespaceMapping](Context.md#getProxyNamespaceMapping(ro.sync.contentcompletion.xml.Context)), [getRootAttributes](Context.md#getRootAttributes()), [getSystemID](Context.md#getSystemID()), [pushContextElement](Context.md#pushContextElement(ro.sync.contentcompletion.xml.ContextElement,java.util.List)), [setAdditionalContextInformationProvider](Context.md#setAdditionalContextInformationProvider(ro.sync.contentcompletion.xml.AdditionalContextInformationProvider)), [setElementStack](Context.md#setElementStack(java.util.Stack)), [setIdValuesList](Context.md#setIdValuesList(java.util.List)), [setNextSiblingElements](Context.md#setNextSiblingElements(java.util.List)), [setPrefixNamespaceMapping](Context.md#setPrefixNamespaceMapping(ro.sync.xml.ProxyNamespaceMapping)), [setPreviousSiblingElements](Context.md#setPreviousSiblingElements(java.util.List)), [setXMLReader](Context.md#setXMLReader(org.xml.sax.XMLReader)), [toString](Context.md#toString())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### positionInDoc

protected int positionInDoc

Position in document.

### doc

protected ro.sync.document.SyntaxDocumentBase doc

The syntax document.

## Constructor Details

### WhatElementsCanGoHereContext

public WhatElementsCanGoHereContext()

## Method Details

### getPositionInDoc

public int getPositionInDoc()

Gets the position in the document.
  Returns: Returns the positionInDoc.
### setPositionInDoc

public void setPositionInDoc(int positionInDoc)

Sets the position in the document.
  Parameters: positionInDoc - The positionInDoc to set.
### getDoc

public ro.sync.document.SyntaxDocumentBase getDoc()

Get the current document.
  Returns: Returns the current document.
### setDoc

public void setDoc(ro.sync.document.SyntaxDocumentBase doc)

Set the current document.
  Parameters: doc - The document to set.
### clone

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone()
  Overrides: [clone](Context.md#clone()) in class [Context](Context.md) See Also:
        * [Context.clone()](Context.md#clone())

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](Context.md#equals(java.lang.Object)) in class [Context](Context.md) See Also:
        * [Context.equals(java.lang.Object)](Context.md#equals(java.lang.Object))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
