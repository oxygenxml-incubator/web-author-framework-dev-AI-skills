Package [ro.sync.exml.workspace.api.standalone](package-summary.md)

# Interface AttributeEditingContextDescription
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AttributeEditingContextDescription
Provides language-independent information about the element and attribute name for which the value is edited.
  Since: 15
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCurrentEditedAttributeValue](#getCurrentEditedAttributeValue())()
Get the current value of the edited attribute as it appears in the Value combo box.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getEditedAttributeName](#getEditedAttributeName())()
Get the name of the edited attribute.
  [NodeContext](../node/NodeContext.md) [getElementContext](#getElementContext())()
Get the context in which we are editing, information about the current element on which we are editing an attribute value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getElementName](#getElementName())()
Get the qname of the element for which the attribute is edited.

## Method Details

### getEditedAttributeName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getEditedAttributeName()

Get the name of the edited attribute.
  Returns: the name of the edited attribute.
### getCurrentEditedAttributeValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCurrentEditedAttributeValue()

Get the current value of the edited attribute as it appears in the Value combo box.
  Returns: the value of the edited attribute. Since: 15.2
### getElementName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getElementName()

Get the qname of the element for which the attribute is edited.
  Returns: the qname of the element for which the attribute is edited.
### getElementContext

[NodeContext](../node/NodeContext.md) getElementContext()

Get the context in which we are editing, information about the current element on which we are editing an attribute value.
  Returns: The element for which we are currently editing attributes. Since: 15.2
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
