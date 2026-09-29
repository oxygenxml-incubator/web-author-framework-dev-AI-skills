Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class DefaultAuthorActionEventHandler.CiElementAndOffset

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.DefaultAuthorActionEventHandler.CiElementAndOffset
   Enclosing class: [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md)   protected static class DefaultAuthorActionEventHandler.CiElementAndOffset extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
A simple structure to return from the method getInsertableFormForElement both the CIElement that can be inserted for a given element and the offset that should be applied to the insertion position in order to insert it.

## Constructor Summary
 Constructors
Constructor

Description
 [CiElementAndOffset](#%3Cinit%3E(ro.sync.contentcompletion.xml.CIElement,int))([CIElement](../../../contentcompletion/xml/CIElement.md) ciElement, int offset)
Constructor.

## Method Summary

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CiElementAndOffset

public CiElementAndOffset([CIElement](../../../contentcompletion/xml/CIElement.md) ciElement, int offset)

Constructor.
  Parameters: ciElement - The CIElement that can be inserted for a given element. offset - The offset that should be applied to the insertion position in order to insert the CIElement.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
