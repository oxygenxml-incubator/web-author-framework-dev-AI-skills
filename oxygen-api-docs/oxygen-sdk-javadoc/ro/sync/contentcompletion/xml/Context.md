Package [ro.sync.contentcompletion.xml](package-summary.md)

# Class Context

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.contentcompletion.xml.Context
   All Implemented Interfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)   Direct Known Subclasses: ro.sync.contentcompletion.xml.WhatContextInParent, [WhatElementsCanGoHereContext](WhatElementsCanGoHereContext.md)   @API(type=EXTENDABLE, src=PRIVATE) public class Context extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)
The context for a node contains:
* elementStack - the stack with [ContextElement](ContextElement.md) up to the root. These represent the ancestors of the element for which the Context was built.
* previousSiblingElements - the list with the [ContextElement](ContextElement.md) representing the siblings of the element for which the Context was built.
* proxyNamespaceMapping - The mapping between namespace prefixes and URI's to the point where the Context was built.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[ContextElement](ContextElement.md)> [elementStack](#elementStack)
The stack with the [ContextElement](ContextElement.md) objects, ancestors of the element for which the Context was built.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> [idValuesList](#idValuesList)
The ID values list.
  protected ro.sync.contentcompletion.xml.AdditionalContextInformationProvider [infoProvider](#infoProvider)
Creates a full SAX source over the document and other useful methods.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> [nextSiblingElements](#nextSiblingElements)
The list of [ContextElement](ContextElement.md) objects representing the next siblings (in document order) of the element for which the Context was built.
  protected [ProxyNamespaceMapping](../../xml/ProxyNamespaceMapping.md) [prefixNamespaceMapping](#prefixNamespaceMapping)
The mapping between namespace prefixes and URI's determined to the point where the Context was built.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> [previousSiblingElements](#previousSiblingElements)
The list of [ContextElement](ContextElement.md) objects representing the previous siblings (in document order) of the element for which the Context was built.
  protected [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [xmlReader](#xmlReader)
The [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) used to create sources for executing XPath expressions in the Context.

## Constructor Summary
 Constructors
Constructor

Description
 [Context](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeContextXPathExpression](#computeContextXPathExpression())()
Takes the position in the document where the content completion was invoked and converts it to an XPath expression that contains the path of elements.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [executeXPath](#executeXPath(java.lang.String,java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expression, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] prefixNamespaceMappings)
Executes an XPath 2.0 expression over a simplified version of the entire document, containing no text nodes for faster processing.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) [executeXPath](#executeXPath(java.lang.String,java.lang.String%5B%5D,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expression, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] prefixNamespaceMappings, boolean useFullDocumentContent)
Executes an XPath 2.0 expression over the current document.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultAttributeValue](#getDefaultAttributeValue(ro.sync.contentcompletion.xml.ContextElement,java.lang.String))([ContextElement](ContextElement.md) elementContext, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
Returns the default value for the specified attribute and context element.
  [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[ContextElement](ContextElement.md)> [getElementStack](#getElementStack())()
Gets the stack of [ContextElement](ContextElement.md) representing the ancestors of the element for which the Context was built.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> [getIdValuesList](#getIdValuesList())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> [getNextSiblingElements](#getNextSiblingElements())()
Get the list of next sibling elements of the element the Context was built for. **WARNING:** The list must be treated as immutable, do not use the getter to modify it.
  [ProxyNamespaceMapping](../../xml/ProxyNamespaceMapping.md) [getPrefixNamespaceMapping](#getPrefixNamespaceMapping())()
Gets the mapping between namespace prefixes and URI's to the point the Context was built.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> [getPreviousSiblingElements](#getPreviousSiblingElements())()
Get the list of previous sibling elements of the element the Context was built for. **WARNING:** The list must be treated as immutable, do not use the getter to modify it.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getProxyNamespaceMapping](#getProxyNamespaceMapping(ro.sync.contentcompletion.xml.Context))([Context](Context.md) context)
Create the proxy-namespace mapping based on the current context.
  [Attribute](../../outline/xml/Attribute.md)[] [getRootAttributes](#getRootAttributes())()
Get the list with the attributes of the root element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSystemID](#getSystemID())()
Get the system ID of the current document for which the context has been built..
  void [pushContextElement](#pushContextElement(ro.sync.contentcompletion.xml.ContextElement,java.util.List))([ContextElement](ContextElement.md) element, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> previousSiblingElements)
Updates the context by adding the given element in the context.
  void [setAdditionalContextInformationProvider](#setAdditionalContextInformationProvider(ro.sync.contentcompletion.xml.AdditionalContextInformationProvider))(ro.sync.contentcompletion.xml.AdditionalContextInformationProvider infoProvider)
Set the AdditionalContextInformationProvider used for creating a SAX source and other useful stuff.
  void [setElementStack](#setElementStack(java.util.Stack))([Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[ContextElement](ContextElement.md)> elementStack)
Sets the stack consisting of [ContextElement](ContextElement.md) representing the ancestor elements of the element for which the Context was built.
  void [setIdValuesList](#setIdValuesList(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValuesList)

 void [setNextSiblingElements](#setNextSiblingElements(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> nextSiblingElements)
Sets the list of [ContextElement](ContextElement.md) representing the next siblings (in document order) of the element the Context was built for.
  void [setPrefixNamespaceMapping](#setPrefixNamespaceMapping(ro.sync.xml.ProxyNamespaceMapping))([ProxyNamespaceMapping](../../xml/ProxyNamespaceMapping.md) prefixNamespaceMapping)
Sets the mapping between the namespace prefixes and URI's to the point where the Context was built.
  void [setPreviousSiblingElements](#setPreviousSiblingElements(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> previousSiblingElements)
Sets the list of [ContextElement](ContextElement.md) representing the previous siblings (in document order) of the element the Context was built for.
  void [setXMLReader](#setXMLReader(org.xml.sax.XMLReader))([XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) xmlReader)
Set the [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) used for creating a SAX source.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### elementStack

protected [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[ContextElement](ContextElement.md)> elementStack

The stack with the [ContextElement](ContextElement.md) objects, ancestors of the element for which the Context was built.

### prefixNamespaceMapping

protected [ProxyNamespaceMapping](../../xml/ProxyNamespaceMapping.md) prefixNamespaceMapping

The mapping between namespace prefixes and URI's determined to the point where the Context was built.

### previousSiblingElements

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> previousSiblingElements

The list of [ContextElement](ContextElement.md) objects representing the previous siblings (in document order) of the element for which the Context was built.

### nextSiblingElements

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> nextSiblingElements

The list of [ContextElement](ContextElement.md) objects representing the next siblings (in document order) of the element for which the Context was built.

### xmlReader

protected [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) xmlReader

The [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) used to create sources for executing XPath expressions in the Context.

### infoProvider

protected ro.sync.contentcompletion.xml.AdditionalContextInformationProvider infoProvider

Creates a full SAX source over the document and other useful methods.

### idValuesList

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValuesList

The ID values list.

## Constructor Details

### Context

public Context()

## Method Details

### setElementStack

public void setElementStack([Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[ContextElement](ContextElement.md)> elementStack)

Sets the stack consisting of [ContextElement](ContextElement.md) representing the ancestor elements of the element for which the Context was built. The root is always added the first on the stack.
  Parameters: elementStack - The stack of ancestor [ContextElement](ContextElement.md).
### getElementStack

public [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[ContextElement](ContextElement.md)> getElementStack()

Gets the stack of [ContextElement](ContextElement.md) representing the ancestors of the element for which the Context was built. The root is always added the first on the stack.
  Returns: The stack with the ancestor [ContextElement](ContextElement.md).
### setPrefixNamespaceMapping

public void setPrefixNamespaceMapping([ProxyNamespaceMapping](../../xml/ProxyNamespaceMapping.md) prefixNamespaceMapping)

Sets the mapping between the namespace prefixes and URI's to the point where the Context was built.
  Parameters: prefixNamespaceMapping - The new mapping to be set.
### getPrefixNamespaceMapping

public [ProxyNamespaceMapping](../../xml/ProxyNamespaceMapping.md) getPrefixNamespaceMapping()

Gets the mapping between namespace prefixes and URI's to the point the Context was built.
  Returns: The mapping between namespace prefixes and URI's.
### getRootAttributes

public [Attribute](../../outline/xml/Attribute.md)[] getRootAttributes()

Get the list with the attributes of the root element.
  Returns: A list of [Attribute](../../outline/xml/Attribute.md) objects representing the attributes of the root element.
### setPreviousSiblingElements

public void setPreviousSiblingElements([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> previousSiblingElements)

Sets the list of [ContextElement](ContextElement.md) representing the previous siblings (in document order) of the element the Context was built for.
  Parameters: previousSiblingElements - The list of previous sibling ContextElement.
### getPreviousSiblingElements

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> getPreviousSiblingElements()

Get the list of previous sibling elements of the element the Context was built for. **WARNING:** The list must be treated as immutable, do not use the getter to modify it.
  Returns: The list of previous sibling [ContextElement](ContextElement.md), null or empty list if no previous siblings exist for the current element.
### setNextSiblingElements

public void setNextSiblingElements([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> nextSiblingElements)

Sets the list of [ContextElement](ContextElement.md) representing the next siblings (in document order) of the element the Context was built for.
  Parameters: nextSiblingElements - The list of next sibling ContextElement.
### getNextSiblingElements

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> getNextSiblingElements()

Get the list of next sibling elements of the element the Context was built for. **WARNING:** The list must be treated as immutable, do not use the getter to modify it.
  Returns: The list of next sibling [ContextElement](ContextElement.md), null or empty list if no next siblings exist for the current element.
### executeXPath

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> executeXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expression, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] prefixNamespaceMappings)

Executes an XPath 2.0 expression over a simplified version of the entire document, containing no text nodes for faster processing. The XML Reader over which the XPath is run does not contain any text nodes so this method is useful only for gathering attribute values which adhere to certain conditions (like //@id).
  Parameters: expression - The XPath expression to be executed. prefixNamespaceMappings - An array of prefixes followed by namespace URI's representing the namespace mappings to the point of the Context. Example:{"xsl", "http://www.w3.org/1999/XSL/Transform", "xsd", "http://www.w3.org/2001/XMLSchema"} Returns: A list of strings representing the text values of the matched XPath nodes, never null.
### executeXPath

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) executeXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expression, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] prefixNamespaceMappings, boolean useFullDocumentContent)

Executes an XPath 2.0 expression over the current document.
  Parameters: expression - The XPath expression to be executed. prefixNamespaceMappings - An array of prefixes followed by namespace URI's representing the namespace mappings to the point of the Context. Example:{"xsl", "http://www.w3.org/1999/XSL/Transform", "xsd", "http://www.w3.org/2001/XMLSchema"} useFullDocumentContent - If false the XML Reader over which the XPath is run does not contain any text nodes so this method is useful only for gathering attribute values which adhere to certain conditions (like //@id). if true the reader will contain the entire XML document's information making it possible to also gather element values for example. Returns: A list of DOM nodes or atomic values representing the XPath results, never null. Since: 14
### setXMLReader

public void setXMLReader([XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) xmlReader)

Set the [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) used for creating a SAX source. The content completion proposals for XSD and XSL documents are obtained by running XPath queries on this SAX source.
  Parameters: xmlReader - The new [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html).
### setAdditionalContextInformationProvider

public void setAdditionalContextInformationProvider(ro.sync.contentcompletion.xml.AdditionalContextInformationProvider infoProvider)

Set the AdditionalContextInformationProvider used for creating a SAX source and other useful stuff.
  Parameters: infoProvider - The new AdditionalContextInformationProvider.
### pushContextElement

public void pushContextElement([ContextElement](ContextElement.md) element, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContextElement](ContextElement.md)> previousSiblingElements)

Updates the context by adding the given element in the context. The new context can be used to get what elements can be added in the given element after the given previous children.
  Parameters: element - Context element to be added. previousSiblingElements - Previous siblings for the new insert position. They are children of the given element and the insertion position is after them.
### clone

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone()
  Overrides: [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.clone()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone())

### setIdValuesList

public void setIdValuesList([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValuesList)
  Parameters: idValuesList - The list of string values representing all ID's collected from the XML document.
### getIdValuesList

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> getIdValuesList()
  Returns: Returns a list of string values representing all ID's collected from the XML document.
### getSystemID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSystemID()

Get the system ID of the current document for which the context has been built..
  Returns: The system ID of the current document Since: 14.1
### computeContextXPathExpression

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeContextXPathExpression()

Takes the position in the document where the content completion was invoked and converts it to an XPath expression that contains the path of elements. /TEI[1]/body[1]/p[2]
  Returns: An XPath expression that when executed on the document it will return the element in which the content completion was invoked.
### getDefaultAttributeValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultAttributeValue([ContextElement](ContextElement.md) elementContext, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)

Returns the default value for the specified attribute and context element.
  Parameters: elementContext - The context element. attributeName - The name of the attribute. Returns: The default value of the attribute. Can be null
### getProxyNamespaceMapping

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getProxyNamespaceMapping([Context](Context.md) context)

Create the proxy-namespace mapping based on the current context.
  Parameters: context - The context where the handler is invoked. Returns: An array containing the prefixes on even positions and the corresponding namespace URI on the following odd position.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
