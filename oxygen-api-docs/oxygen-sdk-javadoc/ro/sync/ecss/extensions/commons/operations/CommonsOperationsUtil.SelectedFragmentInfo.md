Package [ro.sync.ecss.extensions.commons.operations](package-summary.md)

# Class CommonsOperationsUtil.SelectedFragmentInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.operations.CommonsOperationsUtil.SelectedFragmentInfo
   Enclosing class: [CommonsOperationsUtil](CommonsOperationsUtil.md)   public static class CommonsOperationsUtil.SelectedFragmentInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Class containing the new fragment and info about it.

## Constructor Summary
 Constructors
Constructor

Description
 [SelectedFragmentInfo](#%3Cinit%3E(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment,java.util.Map))([AuthorDocumentFragment](../../api/node/AuthorDocumentFragment.md) selectedFragment, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> attributes)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getAttributes](#getAttributes())()

 [AuthorDocumentFragment](../../api/node/AuthorDocumentFragment.md) [getSelectedFragment](#getSelectedFragment())()

 void [setAttributes](#setAttributes(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> attributes)

 void [setSelectedFragment](#setSelectedFragment(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment))([AuthorDocumentFragment](../../api/node/AuthorDocumentFragment.md) selectedFragment)

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SelectedFragmentInfo

public SelectedFragmentInfo([AuthorDocumentFragment](../../api/node/AuthorDocumentFragment.md) selectedFragment, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> attributes)

Constructor.
  Parameters: selectedFragment - The current fragment. attributes - Attributes associated with the current fragment.
## Method Details

### getSelectedFragment

public [AuthorDocumentFragment](../../api/node/AuthorDocumentFragment.md) getSelectedFragment()
  Returns: Returns the selected fragment.
### setSelectedFragment

public void setSelectedFragment([AuthorDocumentFragment](../../api/node/AuthorDocumentFragment.md) selectedFragment)
  Parameters: selectedFragment - The selected fragment to set.
### getAttributes

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getAttributes()
  Returns: Returns the attributes.
### setAttributes

public void setAttributes([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> attributes)
  Parameters: attributes - The attributes to set.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
