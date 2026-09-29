Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorSchemaManager
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorSchemaManager
Author schema manager. Provides support for obtaining information about what elements, attributes can be inserted in a given context.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final short [VALIDATION_MODE_LAX](#VALIDATION_MODE_LAX)
Defines LAX validation of the elements from a fragment in a given context (they are found in the list of possible children of the context element).
  static final short [VALIDATION_MODE_STRICT_FIRST_CHILD_LAX_OTHERS](#VALIDATION_MODE_STRICT_FIRST_CHILD_LAX_OTHERS)
Defines STRICT validation for the first element from the fragment in a given context (it is accepted by the parent in the exact position he is about to be inserted) and LAX validation for all other siblings (they are found in the list of possible children of the context element).

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [canInsertDocumentFragment](#canInsertDocumentFragment(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment,int,short))([AuthorDocumentFragment](node/AuthorDocumentFragment.md) fragment, int offset, short validationMode)
Check if the given fragment can be inserted at the given offset with respect to the given validation mode.
  boolean [canInsertDocumentFragments](#canInsertDocumentFragments(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,int,short))([AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragments, int offset, short validationMode)
Check if the given fragments can be inserted at the given offset with respect to the given validation mode.
  boolean [canInsertDocumentFragments](#canInsertDocumentFragments(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext,short))([AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragments, [WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) insertionContext, short validationMode)
Check if the given fragments can be inserted in the given context with respect to the given validation mode.
  boolean [canInsertText](#canInsertText(int))(int offset)
Check if the element at the given offset accepts text (in other words element content type is not ELEMENT ONLY or EMPTY).
  [AuthorDocumentFragment](node/AuthorDocumentFragment.md) [createAuthorDocumentFragment](#createAuthorDocumentFragment(ro.sync.contentcompletion.xml.CIElement))([CIElement](../../../contentcompletion/xml/CIElement.md) element)
Create an author document fragment from a CIElement
  [WhatAttributesCanGoHereContext](../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) [createWhatAttributesCanGoHereContext](#createWhatAttributesCanGoHereContext(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) element)
Create a context for the given element that can be used to obtain the list with attributes that element accepts.
  [WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) [createWhatElementsCanGoHereContext](#createWhatElementsCanGoHereContext(int))(int offset)
Create an element context for the given offset.
  [WhatPossibleValuesHasAttributeContext](../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) [createWhatPossibleValuesHasAttributeContext](#createWhatPossibleValuesHasAttributeContext(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String))([AuthorElement](node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
Create an attribute values context for the given element and attribute name.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> [getAllPossibleElements](#getAllPossibleElements())()
Get all the elements, including eventual local ones.
  [CIAttribute](../../../contentcompletion/xml/CIAttribute.md) [getAttributeDescription](#getAttributeDescription(ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))([WhatPossibleValuesHasAttributeContext](../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) ctxt)
Get the description of an attribute.
  ro.sync.ecss.component.AuthorSchemaAwareOptions [getAuthorSchemaAwareOptions](#getAuthorSchemaAwareOptions())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> [getChildrenElements](#getChildrenElements(ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))([WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context)
Get the elements that can be children of the element for which the context was built.
  [CIElement](../../../contentcompletion/xml/CIElement.md) [getElementDescription](#getElementDescription(ro.sync.contentcompletion.xml.Context))([Context](../../../contentcompletion/xml/Context.md) ctxt)
Get the description of an element.
  [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html),[Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html)>> [getElementToParentsMap](#getElementToParentsMap(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) nodeContext)
Returns a graph with the links from a node to its potential parents.
  [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html),[Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html)>> [getElementToParentsMap](#getElementToParentsMap(ro.sync.ecss.extensions.api.node.NamespaceContext))([NamespaceContext](node/NamespaceContext.md) namespaceContext)
Returns a graph with the links from a node to its potential parents.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[NameValue](../../../contentcompletion/xml/NameValue.md)> [getEntities](#getEntities())()
Gets the context-independent list of entities declared in the document's DOCTYPE declaration.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> [getGlobalElements](#getGlobalElements())()
Get all the names of global elements defined in the associated grammar.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> [getGlobalElements](#getGlobalElements(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) nodeContext)
Get all the names of global elements defined in the associated grammar.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] [getGrammarURLs](#getGrammarURLs())()
Get the array of URLs of the loaded DTD or XML Schema.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSchemaRepresentationAsJson](#getSchemaRepresentationAsJson())()
Returns the schema representation as JSON.
  boolean [hasLoadingErrors](#hasLoadingErrors())()

 boolean [isElementDescriptionSupported](#isElementDescriptionSupported())()
If true the element description(model) support is available, otherwise not.
  boolean [isLearnSchema](#isLearnSchema())()
Returns true if schema was learned by Oxygen only from the structure of the XML document.
  boolean [isRequiredElement](#isRequiredElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) element)
Check if the given element is required, based on the schema rules.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../contentcompletion/xml/CIAttribute.md)> [whatAttributesCanGoHere](#whatAttributesCanGoHere(ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))([WhatAttributesCanGoHereContext](../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) whatAttributesCanGoHereContext)
Examines the grammar and decides what attributes can be inserted in the parent element.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> [whatElementsCanGoHere](#whatElementsCanGoHere(ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))([WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) whatElementsCanGoHereContext)
Examines the grammar and decides what elements can be inserted in the parent element, after the list of child names.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> [whatPossibleValuesHasAttribute](#whatPossibleValuesHasAttribute(ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext))([WhatPossibleValuesHasAttributeContext](../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) ctxt)
Queries the possible values of an element attribute.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> [whatPossibleValuesHasElement](#whatPossibleValuesHasElement(ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext))([WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) ctxt)
Queries the possible values of an element.

## Field Details

### VALIDATION_MODE_LAX

static final short VALIDATION_MODE_LAX

Defines LAX validation of the elements from a fragment in a given context (they are found in the list of possible children of the context element).
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaManager.VALIDATION_MODE_LAX)

### VALIDATION_MODE_STRICT_FIRST_CHILD_LAX_OTHERS

static final short VALIDATION_MODE_STRICT_FIRST_CHILD_LAX_OTHERS

Defines STRICT validation for the first element from the fragment in a given context (it is accepted by the parent in the exact position he is about to be inserted) and LAX validation for all other siblings (they are found in the list of possible children of the context element).
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorSchemaManager.VALIDATION_MODE_STRICT_FIRST_CHILD_LAX_OTHERS)

## Method Details

### canInsertDocumentFragment

boolean canInsertDocumentFragment([AuthorDocumentFragment](node/AuthorDocumentFragment.md) fragment, int offset, short validationMode)

Check if the given fragment can be inserted at the given offset with respect to the given validation mode.
  Parameters: fragment - Author fragment. offset - The offset where to check if the fragment can be inserted. validationMode - VALIDATION_MODE_LAX or VALIDATION_MODE_STRICT_FIRST_CHILD_LAX_OTHERS. Returns: true if the fragment can be inserted with respect to the given validation mode.
### canInsertDocumentFragments

boolean canInsertDocumentFragments([AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragments, int offset, short validationMode)

Check if the given fragments can be inserted at the given offset with respect to the given validation mode.
  Parameters: fragments - Author fragment. offset - The offset where to check if the fragments can be inserted. validationMode - VALIDATION_MODE_LAX or VALIDATION_MODE_STRICT_FIRST_CHILD_LAX_OTHERS. Returns: true if the fragments can be inserted with respect to the given validation mode.
### canInsertText

boolean canInsertText(int offset)

Check if the element at the given offset accepts text (in other words element content type is not ELEMENT ONLY or EMPTY).
  Parameters: offset - The offset where to check if text can be inserted. Returns: true if text can be inserted at the given offset.
### canInsertDocumentFragments

boolean canInsertDocumentFragments([AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragments, [WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) insertionContext, short validationMode)

Check if the given fragments can be inserted in the given context with respect to the given validation mode. The insertion context will also be used for resolving namespaces for the nodes inside the fragment.
  Parameters: fragments - Author fragments. insertionContext - Insertion context. validationMode - VALIDATION_MODE_LAX or VALIDATION_MODE_STRICT_FIRST_CHILD_LAX_OTHERS. Returns: true if the fragment can be inserted with respect to the given validation mode.
### createWhatElementsCanGoHereContext

[WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) createWhatElementsCanGoHereContext(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create an element context for the given offset.
  Parameters: offset - Offset in document for which to create an element context. Returns: The element context. null will be returned if node at given offset is not an element. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offset is below zero or greater than the content.
### createWhatAttributesCanGoHereContext

[WhatAttributesCanGoHereContext](../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) createWhatAttributesCanGoHereContext([AuthorElement](node/AuthorElement.md) element)

Create a context for the given element that can be used to obtain the list with attributes that element accepts.
  Parameters: element - The element to to create [WhatAttributesCanGoHereContext](../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) Returns: An attribute context. See Also:
        * [whatAttributesCanGoHere(WhatAttributesCanGoHereContext)](#whatAttributesCanGoHere(ro.sync.contentcompletion.xml.WhatAttributesCanGoHereContext))

### createWhatPossibleValuesHasAttributeContext

[WhatPossibleValuesHasAttributeContext](../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) createWhatPossibleValuesHasAttributeContext([AuthorElement](node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)

Create an attribute values context for the given element and attribute name.
  Parameters: element - The element whose attribute values interest us. attributeName - The name of attribute to create context. Returns: An attribute values context.
### getAuthorSchemaAwareOptions

ro.sync.ecss.component.AuthorSchemaAwareOptions getAuthorSchemaAwareOptions()
  Returns: Schema aware options values.
### whatAttributesCanGoHere

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../contentcompletion/xml/CIAttribute.md)> whatAttributesCanGoHere([WhatAttributesCanGoHereContext](../../../contentcompletion/xml/WhatAttributesCanGoHereContext.md) whatAttributesCanGoHereContext)

Examines the grammar and decides what attributes can be inserted in the parent element. The returned list of attributes does not include attribute names which are already set on the element.
  Parameters: whatAttributesCanGoHereContext - the context for the call. It must have:
        * elementName the name of the element in which will be done the insertion.
        * proxyNamespaceMapping the proxy - uri mappings defined before the insertion point.
        * previousAttributesNames the names of the existing attributes in the element, attributes that are before the insertion point.
 Returns: a list of attributes or null if there is none. Null value is also returned when schema is not specified. See Also:
        * [createWhatAttributesCanGoHereContext(AuthorElement)](#createWhatAttributesCanGoHereContext(ro.sync.ecss.extensions.api.node.AuthorElement))

### whatElementsCanGoHere

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> whatElementsCanGoHere([WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) whatElementsCanGoHereContext)

Examines the grammar and decides what elements can be inserted in the parent element, after the list of child names.
  Parameters: whatElementsCanGoHereContext - the context for the call. It must have:
        * parentElementName the qName of the parent element
        * previousElementNames the list of qNames of the previous elements
        * previousElementNamespaces the list of qNames of the previous elements
        * proxyNamespaceMapping the proxy - uri mappings defined before the insertion point.
 Returns: a list of CIElement representing the elements, or null if there is none. Null value is also returned when schema is not specified.
### whatPossibleValuesHasAttribute

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> whatPossibleValuesHasAttribute([WhatPossibleValuesHasAttributeContext](../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) ctxt)

Queries the possible values of an element attribute. If the attribute type was an enumeration, then a list with the tokens of the enumeration will be returned.
  Parameters: ctxt - The context WhatPossiBleValuesHasAttributeContext. Returns: the list of CIValue representing possible values of the attribute or null if they are not known. Null value is also returned when schema is not specified.
### whatPossibleValuesHasElement

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../contentcompletion/xml/CIValue.md)> whatPossibleValuesHasElement([WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) ctxt)

Queries the possible values of an element. If the element type was an enumeration, then a list with the tokens of the enumeration will be returned.
  Parameters: ctxt - The context. Returns: a list of attribute values as CIValue or null if there is none or no schema is specified. The list of values can contain duplicates.
### getGrammarURLs

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] getGrammarURLs()

Get the array of URLs of the loaded DTD or XML Schema. These URLs were set using one of the update methods, and includes the URLs that were collected from the calls of the update(InputSource[]) methods.
  Returns: The URLs of the schemas loaded, or null if there was nothing loaded.
### getAttributeDescription

[CIAttribute](../../../contentcompletion/xml/CIAttribute.md) getAttributeDescription([WhatPossibleValuesHasAttributeContext](../../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) ctxt)

Get the description of an attribute. This model must be human readable.
  Parameters: ctxt - the context describing the target attribute. Returns: a hash describing the model of the element.
### getEntities

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[NameValue](../../../contentcompletion/xml/NameValue.md)> getEntities()

Gets the context-independent list of entities declared in the document's DOCTYPE declaration.
 If the DOCTYPE declaration is not changed, the document should not be processed each time this method is called.

  Returns: a list of name value representing the entities, or null if there is none. The reference of the list is changed on update.
### getElementDescription

[CIElement](../../../contentcompletion/xml/CIElement.md) getElementDescription([Context](../../../contentcompletion/xml/Context.md) ctxt)

Get the description of an element. This model must be human readable.
  Parameters: ctxt - the context describing the target element. It contains:
        * The element names stack, having at top the current element name.
        * The element namespaces stack, having at top the current element namespace.
 Returns: a description the model of the element, or null.
### isElementDescriptionSupported

boolean isElementDescriptionSupported()

If true the element description(model) support is available, otherwise not.
  Returns: True if element description is supported by the SM.
### getChildrenElements

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> getChildrenElements([WhatElementsCanGoHereContext](../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context)

Get the elements that can be children of the element for which the context was built.
  Parameters: context - The element context. Returns: A list with CIElements that are allowed as children.
### isLearnSchema

boolean isLearnSchema()

Returns true if schema was learned by Oxygen only from the structure of the XML document. This only happens when Oxygen does not detect an associated schema for the XML document and learns the structure of the XML file directly.
  Returns: Return true if schema was learned by Oxygen only from the structure of the XML document.
### hasLoadingErrors

boolean hasLoadingErrors()
  Returns: Return true if there were errors when loading schema document(missing, not wellformed, not valid schema).
### createAuthorDocumentFragment

[AuthorDocumentFragment](node/AuthorDocumentFragment.md) createAuthorDocumentFragment([CIElement](../../../contentcompletion/xml/CIElement.md) element)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create an author document fragment from a CIElement
  Parameters: element - The CI Element from which to create a full fragment which can be inserted Returns: The created document fragment. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) Since: 11.2
### getGlobalElements

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> getGlobalElements()

Get all the names of global elements defined in the associated grammar.
  Returns: A list of CIElements. Since: 11.2
### getAllPossibleElements

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> getAllPossibleElements()

Get all the elements, including eventual local ones. We need this for instance if providing content completion proposals as a result schema manager for XSLT.
  Returns: A list of CIElement. Since: 12.1
### getElementToParentsMap

[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html),[Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html)>> getElementToParentsMap([NamespaceContext](node/NamespaceContext.md) namespaceContext)

Returns a graph with the links from a node to its potential parents.
  Parameters: namespaceContext - The namespace declarations active in the document context where this information is requested. Can be null. Returns: Returns a graph with the links from a node to its potential parents or null if this information is unavailable for this type of schema. Since: 18
### getElementToParentsMap

[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html),[Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html)>> getElementToParentsMap([AuthorNode](node/AuthorNode.md) nodeContext)

Returns a graph with the links from a node to its potential parents.
  Parameters: nodeContext - The node context where this information is requested. Can be null. Returns: Returns a graph with the links from a node to its potential parents or null if this information is unavailable for this type of schema. Since: 23
### getGlobalElements

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIElement](../../../contentcompletion/xml/CIElement.md)> getGlobalElements([AuthorNode](node/AuthorNode.md) nodeContext)

Get all the names of global elements defined in the associated grammar.
  Parameters: nodeContext - The context node Returns: A list of CIElements. Since: 23
### isRequiredElement

boolean isRequiredElement([AuthorElement](node/AuthorElement.md) element)

Check if the given element is required, based on the schema rules.
  Parameters: element - the element for which the check is performed. Returns: true if the element is defined as required in the schema, false otherwise. Since: 19
### getSchemaRepresentationAsJson

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSchemaRepresentationAsJson()

Returns the schema representation as JSON.
  Returns: A JSON representation of the schema, may be an empty JSON if the schema type is not supported. Since: 21
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
