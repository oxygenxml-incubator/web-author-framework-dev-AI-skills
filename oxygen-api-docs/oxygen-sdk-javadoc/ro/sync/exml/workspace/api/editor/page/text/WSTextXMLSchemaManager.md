Package [ro.sync.exml.workspace.api.editor.page.text](package-summary.md)

# Class WSTextXMLSchemaManager

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.text.WSTextXMLSchemaManager
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class WSTextXMLSchemaManager extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Text page XML schema manager. Provides support for obtaining information about what elements, attributes can be inserted in a given context.
  Since: 12.1
## Constructor Summary
 Constructors
Constructor

Description
 [WSTextXMLSchemaManager](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract [WhatAttributesCanGoHereContext](../../../../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) [createWhatAttributesCanGoHereContext](#createWhatAttributesCanGoHereContext(int))(int offset)
Create a context for the given element that can be used to obtain the list with attributes that element accepts.
  abstract [WhatElementsCanGoHereContext](../../../../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) [createWhatElementsCanGoHereContext](#createWhatElementsCanGoHereContext(int))(int offset)
Create an element context for the given offset.
  abstract [WhatPossibleValuesHasAttributeContext](../../../../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) [createWhatPossibleValuesHasAttributeContext](#createWhatPossibleValuesHasAttributeContext(int))(int offset)
Create an attribute values context for the given element and attribute name.
  abstract [CIAttribute](../../../../../../contentcompletion/xml/CIAttribute.md) [getAttributeDescription](#getAttributeDescription(ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))([WhatPossibleValuesHasAttributeContext](../../../../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) ctxt)
Get the description of an attribute.
  abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../../../../contentcompletion/xml/CIElement.md)> [getChildrenElements](#getChildrenElements(ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))([WhatElementsCanGoHereContext](../../../../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context)
Get the elements that can be children of the element for which the context was built.
  abstract [CIElement](../../../../../../contentcompletion/xml/CIElement.md) [getElementDescription](#getElementDescription(ro.sync.contentcompletion.xml.Context))([Context](../../../../../../contentcompletion/xml/Context.md) ctxt)
Get the description of an element.
  abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[NameValue](../../../../../../contentcompletion/xml/NameValue.md)> [getEntities](#getEntities())()
Gets the context-independent list of entities declared in the document's DOCTYPE declaration.
  abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../../../../contentcompletion/xml/CIElement.md)> [getGlobalElements](#getGlobalElements())()
Get all the names of global elements defined in the associated grammar.
  abstract [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] [getGrammarURLs](#getGrammarURLs())()
Get the array of URLs of the loaded DTD or XML Schema.
  abstract boolean [hasLoadingErrors](#hasLoadingErrors())()

 abstract boolean [isElementDescriptionSupported](#isElementDescriptionSupported())()
If true the element description(model) support is available, otherwise not.
  abstract boolean [isLearnSchema](#isLearnSchema())()

 abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../../../../contentcompletion/xml/CIAttribute.md)> [whatAttributesCanGoHere](#whatAttributesCanGoHere(ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))([WhatAttributesCanGoHereContext](../../../../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) whatAttributesCanGoHereContext)
Examines the grammar and decides what attributes can be inserted in the parent element, after the list of attributes names.
  abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../../../../contentcompletion/xml/CIElement.md)> [whatElementsCanGoHere](#whatElementsCanGoHere(ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))([WhatElementsCanGoHereContext](../../../../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) whatElementsCanGoHereContext)
Examines the grammar and decides what elements can be inserted in the parent element, after the list of child names.
  abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../../../../contentcompletion/xml/CIValue.md)> [whatPossibleValuesHasAttribute](#whatPossibleValuesHasAttribute(ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))([WhatPossibleValuesHasAttributeContext](../../../../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) ctxt)
Queries the possible values of an element attribute.
  abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../../../../contentcompletion/xml/CIValue.md)> [whatPossibleValuesHasElement](#whatPossibleValuesHasElement(ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))([WhatElementsCanGoHereContext](../../../../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) ctxt)
Queries the possible values of an element.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WSTextXMLSchemaManager

public WSTextXMLSchemaManager()

## Method Details

### createWhatElementsCanGoHereContext

public abstract [WhatElementsCanGoHereContext](../../../../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) createWhatElementsCanGoHereContext(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create an element context for the given offset.
  Parameters: offset - Offset in document for which to create an element context. Returns: The element context. Null value will be returned if node at given offset is not an element. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offset is below zero or greater than the content.
### createWhatAttributesCanGoHereContext

public abstract [WhatAttributesCanGoHereContext](../../../../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) createWhatAttributesCanGoHereContext(int offset)

Create a context for the given element that can be used to obtain the list with attributes that element accepts.
  Parameters: offset - The current offset Returns: An attribute context. See Also:
        * [whatAttributesCanGoHere(WhatAttributesCanGoHereContext)](#whatAttributesCanGoHere(ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))

### createWhatPossibleValuesHasAttributeContext

public abstract [WhatPossibleValuesHasAttributeContext](../../../../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) createWhatPossibleValuesHasAttributeContext(int offset)

Create an attribute values context for the given element and attribute name.
  Parameters: offset - The offset of the attribute name on the element whose attribute values interest us. Returns: An attribute values context.
### whatAttributesCanGoHere

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../../../../contentcompletion/xml/CIAttribute.md)> whatAttributesCanGoHere([WhatAttributesCanGoHereContext](../../../../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) whatAttributesCanGoHereContext)

Examines the grammar and decides what attributes can be inserted in the parent element, after the list of attributes names.
  Parameters: whatAttributesCanGoHereContext - the context for the call. It must have:
        * elementName the name of the element in which will be done the insertion.
        * proxyNamespaceMapping the proxy - uri mappings defined before the insertion point.
        * previousAttributesNames the names of the existing attributes in the element, attributes that are before the insertion point.
 Returns: a list of attributes or null if there is none. Null value is also returned when schema is not specified.
### whatElementsCanGoHere

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../../../../contentcompletion/xml/CIElement.md)> whatElementsCanGoHere([WhatElementsCanGoHereContext](../../../../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) whatElementsCanGoHereContext)

Examines the grammar and decides what elements can be inserted in the parent element, after the list of child names.
  Parameters: whatElementsCanGoHereContext - the context for the call. It must have:
        * parentElementName the qName of the parent element
        * previousElementNames the list of qNames of the previous elements
        * previousElementNamespaces the list of qNames of the previous elements
        * proxyNamespaceMapping the proxy - uri mappings defined before the insertion point.
 Returns: a list of CIElement representing the elements, or null if there is none. Null value is also returned when schema is not specified.
### whatPossibleValuesHasAttribute

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../../../../contentcompletion/xml/CIValue.md)> whatPossibleValuesHasAttribute([WhatPossibleValuesHasAttributeContext](../../../../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) ctxt)

Queries the possible values of an element attribute. If the attribute type was an enumeration, then a list with the tokens of the enumeration will be returned.
  Parameters: ctxt - The context WhatPossiBleValuesHasAttributeContext. Returns: the list of CIValue representing possible values of the attribute or null if they are not known. Null value is also returned when schema is not specified.
### whatPossibleValuesHasElement

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../../../../contentcompletion/xml/CIValue.md)> whatPossibleValuesHasElement([WhatElementsCanGoHereContext](../../../../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) ctxt)

Queries the possible values of an element. If the element type was an enumeration, then a list with the tokens of the enumeration will be returned.
  Parameters: ctxt - The context. Returns: a list of attribute values as CIValue or null if there is none or no schema is specified. The list of values can contain duplicates.
### getGrammarURLs

public abstract [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] getGrammarURLs()

Get the array of URLs of the loaded DTD or XML Schema. These URLs were set using one of the update methods, and includes the URLs that were collected from the calls of the update(InputSource[]) methods.
  Returns: The URLs of the schemas loaded, or null if there was nothing loaded.
### getAttributeDescription

public abstract [CIAttribute](../../../../../../contentcompletion/xml/CIAttribute.md) getAttributeDescription([WhatPossibleValuesHasAttributeContext](../../../../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) ctxt)

Get the description of an attribute. This model must be human readable.
  Parameters: ctxt - the context describing the target attribute. Returns: a hash describing the model of the element.
### getEntities

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[NameValue](../../../../../../contentcompletion/xml/NameValue.md)> getEntities()

Gets the context-independent list of entities declared in the document's DOCTYPE declaration.
 If the DOCTYPE declaration is not changed, the document should not be processed each time this method is called.

  Returns: a list of name value representing the entities, or null if there is none. The reference of the list is changed on update.
### getElementDescription

public abstract [CIElement](../../../../../../contentcompletion/xml/CIElement.md) getElementDescription([Context](../../../../../../contentcompletion/xml/Context.md) ctxt)

Get the description of an element. This model must be human readable.
  Parameters: ctxt - the context describing the target element. It contains:
        * The element names stack, having at top the current element name.
        * The element namespaces stack, having at top the current element namespace.
 Returns: a description the model of the element, or null.
### isElementDescriptionSupported

public abstract boolean isElementDescriptionSupported()

If true the element description(model) support is available, otherwise not.
  Returns: True if element description is supported by the SM.
### getChildrenElements

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../../../../contentcompletion/xml/CIElement.md)> getChildrenElements([WhatElementsCanGoHereContext](../../../../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context)

Get the elements that can be children of the element for which the context was built.
  Parameters: context - The element context. Returns: A list with CIElements that are allowed as children.
### isLearnSchema

public abstract boolean isLearnSchema()
  Returns: Return true if schema was learned by Oxygen from the structure of the document.
### hasLoadingErrors

public abstract boolean hasLoadingErrors()
  Returns: Return true if there were errors when loading schema document(missing, not wellformed, not valid schema).
### getGlobalElements

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../../../../contentcompletion/xml/CIElement.md)> getGlobalElements()

Get all the names of global elements defined in the associated grammar.
  Returns: A list of CIElements. Since: 11.2
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
