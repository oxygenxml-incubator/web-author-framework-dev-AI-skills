Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface CustomAttributeValueContext
    @API(type=EXTENDABLE, src=PUBLIC) public interface CustomAttributeValueContext
Context for a custom attribute.
  Since: 22
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeName](#getAttributeName())()
Get the attribute qname.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeValue](#getAttributeValue())()
Get the attribute value.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getBaseURL](#getBaseURL())()
Get the URL of the current document in which the attribute is defined.

## Method Details

### getAttributeName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeName()

Get the attribute qname.
  Returns: the attribute qname.
### getAttributeValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeValue()

Get the attribute value.
  Returns: the attribute value.
### getBaseURL

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getBaseURL()

Get the URL of the current document in which the attribute is defined.
  Returns: the URL of the current document in which the attribute is defined.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
