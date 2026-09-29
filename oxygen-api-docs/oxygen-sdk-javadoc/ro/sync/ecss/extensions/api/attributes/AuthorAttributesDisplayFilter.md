Package [ro.sync.ecss.extensions.api.attributes](package-summary.md)

# Class AuthorAttributesDisplayFilter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorAttributesDisplayFilter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Filter certain attributes from being displayed in certain parts of the Author editor (the Attributes view, the Attributes editor, the Outline).
  Since: 13
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [SOURCE_ATTRIBUTES_VIEW](#SOURCE_ATTRIBUTES_VIEW)
Source from where the callback is received.
  static final int [SOURCE_CSS_CONTENT](#SOURCE_CSS_CONTENT)
Source from where the callback is received.
  static final int [SOURCE_EDIT_PROPERTIES](#SOURCE_EDIT_PROPERTIES)
Source from where the callback is received.
  static final int [SOURCE_FULL_TAGS_WITH_ATTRS](#SOURCE_FULL_TAGS_WITH_ATTRS)
Source from where the callback is received.
  static final int [SOURCE_INSERT_REFERENCE](#SOURCE_INSERT_REFERENCE)
Source from where the callback is received.
  static final int [SOURCE_OUTLINE_VIEW](#SOURCE_OUTLINE_VIEW)
Source from where the callback is received.

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorAttributesDisplayFilter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [shouldFilterAttribute](#shouldFilterAttribute(ro.sync.contentcompletion.xml.CIElement,java.lang.String,int))([CIElement](../../../../contentcompletion/xml/CIElement.md) parentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeQName, int source)
Check if a certain attribute should be filtered from display.
  boolean [shouldFilterAttribute](#shouldFilterAttribute(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,int))([AuthorElement](../node/AuthorElement.md) parentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeQName, int source)
Check if a certain attribute should be filtered from display.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### SOURCE_ATTRIBUTES_VIEW

public static final int SOURCE_ATTRIBUTES_VIEW

Source from where the callback is received. This type of source means that the callback is received either from the Attributes view associated to an Author page or from the in-place Attributes editor from either the Author or the DITA Maps Manager editing page.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter.SOURCE_ATTRIBUTES_VIEW)

### SOURCE_OUTLINE_VIEW

public static final int SOURCE_OUTLINE_VIEW

Source from where the callback is received. This type of source means that the callback is received either from the Outline view associated to an Author page.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter.SOURCE_OUTLINE_VIEW)

### SOURCE_FULL_TAGS_WITH_ATTRS

public static final int SOURCE_FULL_TAGS_WITH_ATTRS

Source from where the callback is received. This type of source means that the callback is received when displaying the node in the Full Tags with Attributes in the Author page.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter.SOURCE_FULL_TAGS_WITH_ATTRS)

### SOURCE_CSS_CONTENT

public static final int SOURCE_CSS_CONTENT

Source from where the callback is received. This type of source means that the callback is received when having CSS extension functions like attributes().
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter.SOURCE_CSS_CONTENT)

### SOURCE_EDIT_PROPERTIES

public static final int SOURCE_EDIT_PROPERTIES

Source from where the callback is received. This type of source means that the callback is received from "Edit Properties" (available for DITA documents).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter.SOURCE_EDIT_PROPERTIES)

### SOURCE_INSERT_REFERENCE

public static final int SOURCE_INSERT_REFERENCE

Source from where the callback is received. This type of source means that the callback is received from "Insert reference" dialogs (available for DITA documents).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter.SOURCE_INSERT_REFERENCE)

## Constructor Details

### AuthorAttributesDisplayFilter

public AuthorAttributesDisplayFilter()

## Method Details

### shouldFilterAttribute

public boolean shouldFilterAttribute([AuthorElement](../node/AuthorElement.md) parentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeQName, int source)

Check if a certain attribute should be filtered from display. This method should be implemented in subclasses.
  Parameters: parentElement - The parent element. attributeQName - The name of the attribute. source - The place from which the attribute should be filtered. One of the constants [SOURCE_ATTRIBUTES_VIEW](#SOURCE_ATTRIBUTES_VIEW) or [SOURCE_OUTLINE_VIEW](#SOURCE_OUTLINE_VIEW) Returns: true to avoid displaying the attribute.
### shouldFilterAttribute

public boolean shouldFilterAttribute([CIElement](../../../../contentcompletion/xml/CIElement.md) parentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeQName, int source)

Check if a certain attribute should be filtered from display. This method should be implemented in subclasses.
  Parameters: parentElement - The parent CI element. attributeQName - The name of the attribute. source - The place from which the attribute should be filtered. A possible value can be [SOURCE_INSERT_REFERENCE](#SOURCE_INSERT_REFERENCE) Returns: true to avoid displaying the attribute. Since: 18.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
