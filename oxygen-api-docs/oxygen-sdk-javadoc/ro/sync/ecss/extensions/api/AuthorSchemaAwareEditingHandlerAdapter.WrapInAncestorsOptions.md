Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions
   Enclosing class: [AuthorSchemaAwareEditingHandlerAdapter](AuthorSchemaAwareEditingHandlerAdapter.md)   public static class AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
One of the default smart paste strategies involves detecting an path o ancestors from the context element to the inserted one. These are the preferences that control how these ancestors are chosen.

## Constructor Summary
 Constructors
Constructor

Description
 [WrapInAncestorsOptions](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html)> [getForbiddenParents](#getForbiddenParents(javax.xml.namespace.QName,java.util.Collection))([QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html) elementName, [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html)> possibleParents)
Gets a list with the parents that should be used in a solution.
  [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html)> [getPreferredParents](#getPreferredParents(javax.xml.namespace.QName,java.util.Collection))([QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html) elementName, [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html)> possibleParents)
Gets a list of preferred parents for the given element.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WrapInAncestorsOptions

public WrapInAncestorsOptions()

## Method Details

### getPreferredParents

public [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html)> getPreferredParents([QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html) elementName, [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html)> possibleParents)

Gets a list of preferred parents for the given element.
  Parameters: elementName - Element name. possibleParents - The detected possible parents. Returns: The list with preferred parents or null to go with the defaults.
### getForbiddenParents

public [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html)> getForbiddenParents([QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html) elementName, [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html)> possibleParents)

Gets a list with the parents that should be used in a solution.
  Parameters: elementName - Element name. possibleParents - The detected possible parents. Returns: The list with forbidden parents or null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
