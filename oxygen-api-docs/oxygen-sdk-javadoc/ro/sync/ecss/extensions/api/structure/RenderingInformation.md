Package [ro.sync.ecss.extensions.api.structure](package-summary.md)

# Class RenderingInformation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.workspace.api.node.customizer.BasicRenderingInformation](../../../../exml/workspace/api/node/customizer/BasicRenderingInformation.md)
        * ro.sync.ecss.extensions.api.structure.RenderingInformation
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class RenderingInformation extends [BasicRenderingInformation](../../../../exml/workspace/api/node/customizer/BasicRenderingInformation.md)
The rendering information used to render a node in the outliner and bread crumb.
  Since: 11.2
## Constructor Summary
 Constructors
Constructor

Description
 [RenderingInformation](#%3Cinit%3E(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String))([AuthorNode](../node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) renderedText, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalRenderedText, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tooltipText)

 [RenderingInformation](#%3Cinit%3E(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String,java.lang.String,java.lang.String))([AuthorNode](../node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) renderedText, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalRenderedText, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalRenderedAttributeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tooltipText)

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAdditionalRenderedAttributeValue](#getAdditionalRenderedAttributeValue())()
Get the additional rendered attribute value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAdditionalRenderedText](#getAdditionalRenderedText())()
The additional rendered text.
  [AuthorNode](../node/AuthorNode.md) [getNode](#getNode())()

 boolean [isIgnoreNodeFromDisplay](#isIgnoreNodeFromDisplay())()
Check if this node should be ignored for display, used only on the breadcrumb.
  void [setAdditionalRenderedAttributeValue](#setAdditionalRenderedAttributeValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalRenderedAttributeValue)
Set the additional rendered attribute value.
  void [setAdditionalRenderedText](#setAdditionalRenderedText(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalRenderedText)
The additional rendered text.
  void [setIgnoreNodeFromDisplay](#setIgnoreNodeFromDisplay(boolean))(boolean ignoreNodeFromDisplay)
Set this to true to ignore this node from being displayed.

### Methods inherited from class ro.sync.exml.workspace.api.node.customizer.[BasicRenderingInformation](../../../../exml/workspace/api/node/customizer/BasicRenderingInformation.md)
 [getIconPath](../../../../exml/workspace/api/node/customizer/BasicRenderingInformation.md#getIconPath()), [getRenderedText](../../../../exml/workspace/api/node/customizer/BasicRenderingInformation.md#getRenderedText()), [getTooltipText](../../../../exml/workspace/api/node/customizer/BasicRenderingInformation.md#getTooltipText()), [setIconPath](../../../../exml/workspace/api/node/customizer/BasicRenderingInformation.md#setIconPath(java.lang.String)), [setRenderedText](../../../../exml/workspace/api/node/customizer/BasicRenderingInformation.md#setRenderedText(java.lang.String)), [setTooltipText](../../../../exml/workspace/api/node/customizer/BasicRenderingInformation.md#setTooltipText(java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### RenderingInformation

public RenderingInformation([AuthorNode](../node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) renderedText, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalRenderedText, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tooltipText)
  Parameters: node - The node to render renderedText - The rendered text. This will be used both in the Outliner and the Bread Crumb. By default it is usually the node name. additionalRenderedText - The additional rendered text. This will be used only in the Outliner. By default it shows some node text content. tooltipText - The tooltip text which will appear in the tooltip associated with the node
### RenderingInformation

public RenderingInformation([AuthorNode](../node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) renderedText, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalRenderedText, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalRenderedAttributeValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tooltipText)
  Parameters: node - The node to render renderedText - The rendered text. This will be used both in the Outliner and the Bread Crumb. By default it is usually the node name. additionalRenderedText - The additional rendered text. This will be used only in the Outliner. By default it shows some node text content . additionalRenderedAttributeValue - The additional rendered attribute value. This will be used only in the Outliner. By default it shows the value of the first attribute. tooltipText - The tooltip text which will appear in the tooltip associated with the node
## Method Details

### setAdditionalRenderedText

public void setAdditionalRenderedText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalRenderedText)

The additional rendered text. This will be used only in the Outliner. By default it shows some node text content.
  Parameters: additionalRenderedText - The additional rendered text. This will be used only in the Outliner. By default it shows some node text content.
### setAdditionalRenderedAttributeValue

public void setAdditionalRenderedAttributeValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalRenderedAttributeValue)

Set the additional rendered attribute value. This will be used only in the Outliner. By default it shows the value of the first attribute.
  Parameters: additionalRenderedAttributeValue - The additional rendered attribute value.
### getAdditionalRenderedText

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAdditionalRenderedText()

The additional rendered text. This will be used only in the Outliner. By default it shows some node text content.
  Returns: Returns the additional rendered text. This will be used only in the Outliner. By default it shows the value of the first attribute and some text.
### getAdditionalRenderedAttributeValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAdditionalRenderedAttributeValue()

Get the additional rendered attribute value. This will be used only in the Outliner. By default it shows the value of the first attribute.
  Returns: Returns the the additional rendered attribute value. This will be used only in the Outliner. By default it shows the value of the first attribute.
### getNode

public [AuthorNode](../node/AuthorNode.md) getNode()
  Returns: Returns the node to render information for.
### setIgnoreNodeFromDisplay

public void setIgnoreNodeFromDisplay(boolean ignoreNodeFromDisplay)

Set this to true to ignore this node from being displayed. This takes effect only on the Breadcrumb Customizer.
  Parameters: ignoreNodeFromDisplay - Set this to true to ignore this node from being displayed. Since: 12.1
### isIgnoreNodeFromDisplay

public boolean isIgnoreNodeFromDisplay()

Check if this node should be ignored for display, used only on the breadcrumb.
  Returns: Returns true to ignore this node from being displayed.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
