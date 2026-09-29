Package [ro.sync.ecss.extensions.api.webapp.attributes](package-summary.md)

# Interface AttributesManager
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AttributesManager
Offers support for element attributes operations.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../../../contentcompletion/xml/CIAttribute.md)> [getAllAttributes](#getAllAttributes(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../node/AuthorElement.md) element)
Returns all possible attributes for a specific element.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../../../contentcompletion/xml/CIValue.md)> [getPossibleCIValues](#getPossibleCIValues(ro.sync.ecss.extensions.api.node.AuthorElement,ro.sync.contentcompletion.xml.CIAttribute))([AuthorElement](../../node/AuthorElement.md) element, [CIAttribute](../../../../../contentcompletion/xml/CIAttribute.md) attribute)
Get list of all possible values as CIValues.

## Method Details

### getAllAttributes

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../../../../contentcompletion/xml/CIAttribute.md)> getAllAttributes([AuthorElement](../../node/AuthorElement.md) element)

Returns all possible attributes for a specific element.
  Parameters: element - The author element. Returns: All possible attributes for a specific element.
### getPossibleCIValues

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../../../../contentcompletion/xml/CIValue.md)> getPossibleCIValues([AuthorElement](../../node/AuthorElement.md) element, [CIAttribute](../../../../../contentcompletion/xml/CIAttribute.md) attribute)

Get list of all possible values as CIValues.
  Parameters: element - The current element. attribute - The attribute to determine current allowed values for. Returns: A list of all possible values as CIValues.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
