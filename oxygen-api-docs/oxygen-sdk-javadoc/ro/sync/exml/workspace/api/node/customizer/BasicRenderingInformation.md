Package [ro.sync.exml.workspace.api.node.customizer](package-summary.md)

# Class BasicRenderingInformation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.node.customizer.BasicRenderingInformation
   Direct Known Subclasses: [RenderingInformation](../../../../../ecss/extensions/api/structure/RenderingInformation.md)   @API(type=EXTENDABLE, src=PUBLIC) public class BasicRenderingInformation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The rendering information used to display a node in the Outline view, Author bread crumb, Content Completion popup window, Elements view and DITA Map view.
  Since: 13.2
## Constructor Summary
 Constructors
Constructor

Description
 [BasicRenderingInformation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getIconPath](#getIconPath())()
Get the path of the icon used to render a node.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRenderedText](#getRenderedText())()
Get the text to be rendered for a node.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTooltipText](#getTooltipText())()
The tooltip text which will appear in the tooltip associated with the node.
  void [setIconPath](#setIconPath(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) iconPath)
Set the path of the icon used to render a node.
  void [setRenderedText](#setRenderedText(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) renderedText)
Set the text to be rendered for a node.
  void [setTooltipText](#setTooltipText(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tooltipText)
The tooltip text which will appear in the tooltip associated with the node.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### BasicRenderingInformation

public BasicRenderingInformation()

## Method Details

### setRenderedText

public void setRenderedText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) renderedText)

Set the text to be rendered for a node. If the rendered text is null then the default node rendering will be used.
  Parameters: renderedText - The rendered text, usually the node name. If null the default text will be used for rendering.
### setTooltipText

public void setTooltipText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tooltipText)

The tooltip text which will appear in the tooltip associated with the node. If the tooltip text is null then the default tooltip text will be used for the node.
  Parameters: tooltipText - The tooltip text which will appear in the tooltip associated with the node. If null the default tooltip text will be used for the node.
### setIconPath

public void setIconPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) iconPath)

Set the path of the icon used to render a node. The path can be an icon file path, the string representation of an icon [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) or can contain editor variables as defined in the [EditorVariables](../../../../../util/editorvars/EditorVariables.md) class. The editor variables will be expanded at runtime. If the icon path is null the default icon will be used for the node. If the custom used images are located in the same **jar** file as the [XMLNodeRendererCustomizer](XMLNodeRendererCustomizer.md)then you can use as the return value for this function the following code sequence:  this.getClass().getResource("/images/Icon.gif").toExternalForm();  The previous sequence assumes that Icon.gif icon image is located in the images folder inside your **jar** file.
  Parameters: iconPath - The path of the icon. If null the default icon will be used for the node.
### getRenderedText

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRenderedText()

Get the text to be rendered for a node.
  Returns: Returns the rendered text.
### getTooltipText

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTooltipText()

The tooltip text which will appear in the tooltip associated with the node.
  Returns: the tooltip text which will appear in the tooltip associated with the node.
### getIconPath

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getIconPath()

Get the path of the icon used to render a node. The path can be an icon file path, the string representation of an icon [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) or can contain editor variables as defined in the [EditorVariables](../../../../../util/editorvars/EditorVariables.md) class. The editor variables will be expanded at runtime.
  Returns: Returns the path of the icon.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
