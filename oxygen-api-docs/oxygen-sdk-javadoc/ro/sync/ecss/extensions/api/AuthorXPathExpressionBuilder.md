Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorXPathExpressionBuilder
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorXPathExpressionBuilder
Generates an XPath expression for an XML node.
  Since: 24
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorXPathExpressionBuilder](AuthorXPathExpressionBuilder.md) [avoidNamespacePrefixes](#avoidNamespacePrefixes())()
Do not generate namespace prefixes.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXpathExpresion](#getXpathExpresion())()
Get the XPath expression for the specified node.
  [AuthorXPathExpressionBuilder](AuthorXPathExpressionBuilder.md) [processChanges](#processChanges(boolean))(boolean processChanges)

## Method Details

### processChanges

[AuthorXPathExpressionBuilder](AuthorXPathExpressionBuilder.md) processChanges(boolean processChanges)
  Parameters: processChanges - If true the delete changes will be ignored. Returns: This instance for chaining.
### avoidNamespacePrefixes

[AuthorXPathExpressionBuilder](AuthorXPathExpressionBuilder.md) avoidNamespacePrefixes()

Do not generate namespace prefixes.
For example, intead of generating an expression like the one below that uses namespace prefixes

```
/db:article/db:sect1
```

Generate an expression that use the full namespace URI for the element.

```
/*[namespace-uri()='http://docbook.org/ns/docbook' and local-name()='article']/*[namespace-uri()='http://docbook.org/ns/docbook' and local-name()='sect1'][1]
```

  Returns: this instance for chaining.
### getXpathExpresion

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXpathExpresion()

Get the XPath expression for the specified node.
  Returns: XPath expression of the element for the current Node. Empty string if no XPath expression could be computed.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
