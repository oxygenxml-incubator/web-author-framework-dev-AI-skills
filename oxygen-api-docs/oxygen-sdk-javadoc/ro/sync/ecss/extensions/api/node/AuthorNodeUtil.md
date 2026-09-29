Package [ro.sync.ecss.extensions.api.node](package-summary.md)

# Class AuthorNodeUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.node.AuthorNodeUtil
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorNodeUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Utility functions for working with AuthorNodes.
  Since: 15.2
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_VALUE_MARKER](#ATTRIBUTE_VALUE_MARKER)
Marker used to find a certain element

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorNodeUtil](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static int [getChildIndex](#getChildIndex(int,java.util.List))(int offset, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> children)
Looks for the child that contains the given offset.
  static [AuthorElement](AuthorElement.md) [getFirstChildElement](#getFirstChildElement(ro.sync.ecss.extensions.api.node.AuthorParentNode))([AuthorParentNode](AuthorParentNode.md) parentNode)
Return the first child element.
  static [AuthorNode](AuthorNode.md) [getFirstLeaf](#getFirstLeaf(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment))([AuthorDocumentFragment](AuthorDocumentFragment.md) fragment)
Finds the first leaf node in the document fragment.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> [minimizeAuthorCollection](#minimizeAuthorCollection(java.util.Collection))([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<? extends [AuthorNode](AuthorNode.md)> collection)
Remove from the collection of nodes any descendants so the only nodes that are kept are disjunct.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### ATTRIBUTE_VALUE_MARKER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_VALUE_MARKER

Marker used to find a certain element
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNodeUtil.ATTRIBUTE_VALUE_MARKER)

## Constructor Details

### AuthorNodeUtil

public AuthorNodeUtil()

## Method Details

### minimizeAuthorCollection

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> minimizeAuthorCollection([Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<? extends [AuthorNode](AuthorNode.md)> collection)

Remove from the collection of nodes any descendants so the only nodes that are kept are disjunct.
  Parameters: collection - A collection of nodes. Returns: A list of disjunct nodes.
### getFirstLeaf

public static [AuthorNode](AuthorNode.md) getFirstLeaf([AuthorDocumentFragment](AuthorDocumentFragment.md) fragment)

Finds the first leaf node in the document fragment.
  Parameters: fragment - The document fragment. Returns: The first leaf.
### getFirstChildElement

public static [AuthorElement](AuthorElement.md) getFirstChildElement([AuthorParentNode](AuthorParentNode.md) parentNode)

Return the first child element.
  Parameters: parentNode - The parent element. Returns: the first child element.
### getChildIndex

public static int getChildIndex(int offset, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> children)

Looks for the child that contains the given offset.
  Parameters: offset - Searched offset. children - The list of children. Returns: The index of the child in the list of children or -1 if not found.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
