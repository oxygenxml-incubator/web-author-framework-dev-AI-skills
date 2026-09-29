Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorAttributesController
    All Known Subinterfaces: [AuthorDocumentController](AuthorDocumentController.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorAttributesController
Helper used to set attributes

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [setAttribute](#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AttrValue](node/AttrValue.md) value, [AuthorElement](node/AuthorElement.md) element)
Sets the value of an attribute in the specified element.

## Method Details

### setAttribute

void setAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AttrValue](node/AttrValue.md) value, [AuthorElement](node/AuthorElement.md) element)

Sets the value of an attribute in the specified element. Attributes set in this manner (as opposed to calling [AuthorElement.setAttribute(String, AttrValue)](node/AuthorElement.md#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue)) directly) will be subject to undo/redo.
  Parameters: attributeName - Name of the attribute being changed. value - New [AttrValue](node/AttrValue.md) for the attribute. If null, the attribute is removed from the element. element - The [AuthorElement](node/AuthorElement.md) whose attribute is changing.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
