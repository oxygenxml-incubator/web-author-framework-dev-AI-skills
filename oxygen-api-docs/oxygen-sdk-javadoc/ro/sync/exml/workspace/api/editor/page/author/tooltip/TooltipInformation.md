Package [ro.sync.exml.workspace.api.editor.page.author.tooltip](package-summary.md)

# Class TooltipInformation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.author.tooltip.TooltipInformation
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class TooltipInformation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Information about the tooltip.
  Since: 18
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ORIGIN_CALLOUTS](#ORIGIN_CALLOUTS)
The tooltip describes information when hovering callouts.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ORIGIN_CHANGE_MARKERS](#ORIGIN_CHANGE_MARKERS)
Hovering over comment change tracking.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ORIGIN_ERROR_NODE](#ORIGIN_ERROR_NODE)
Tooltip computed when hovering over an error node.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ORIGIN_FORM_CONTROLS](#ORIGIN_FORM_CONTROLS)
Tooltip computed when hovering form controls.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ORIGIN_IMAGE](#ORIGIN_IMAGE)
Tooltip computed when hovering over an image.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ORIGIN_LINK](#ORIGIN_LINK)
Tooltip computed when hovering a link.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ORIGIN_PROFILING_CONDITIONS](#ORIGIN_PROFILING_CONDITIONS)
Tooltip computed when an element with profiling attributes is hovered.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ORIGIN_SCHEMA_DESCRIPTION](#ORIGIN_SCHEMA_DESCRIPTION)
Tooltip computed by looking in the associated schema for annotations on that particular element.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ORIGIN_VALIDATION_ERROR](#ORIGIN_VALIDATION_ERROR)
Validation error.

## Constructor Summary
 Constructors
Constructor

Description
 [TooltipInformation](#%3Cinit%3E(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description, [AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) hoveredNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tooltipOriginInformation, int mouseX, int mouseY)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()
Get the current description which will be used for the tooltip.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHoveredErrorOriginInformation](#getHoveredErrorOriginInformation())()
Get information about the originator for the tooltip (for example if it is given by hovering an error message or by hovering an image or so on).
  [AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) [getHoveredNode](#getHoveredNode())()
Get the hovered node, can be null.
  int [getMouseX](#getMouseX())()
Get mouse X coordinates
  int [getMouseY](#getMouseY())()
Get mouse Y coordinates
  void [setDescription](#setDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description)
Set a description to be used on the tooltip.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### ORIGIN_CALLOUTS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ORIGIN_CALLOUTS

The tooltip describes information when hovering callouts.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.author.tooltip.TooltipInformation.ORIGIN_CALLOUTS)

### ORIGIN_FORM_CONTROLS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ORIGIN_FORM_CONTROLS

Tooltip computed when hovering form controls.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.author.tooltip.TooltipInformation.ORIGIN_FORM_CONTROLS)

### ORIGIN_LINK

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ORIGIN_LINK

Tooltip computed when hovering a link.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.author.tooltip.TooltipInformation.ORIGIN_LINK)

### ORIGIN_PROFILING_CONDITIONS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ORIGIN_PROFILING_CONDITIONS

Tooltip computed when an element with profiling attributes is hovered.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.author.tooltip.TooltipInformation.ORIGIN_PROFILING_CONDITIONS)

### ORIGIN_SCHEMA_DESCRIPTION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ORIGIN_SCHEMA_DESCRIPTION

Tooltip computed by looking in the associated schema for annotations on that particular element.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.author.tooltip.TooltipInformation.ORIGIN_SCHEMA_DESCRIPTION)

### ORIGIN_IMAGE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ORIGIN_IMAGE

Tooltip computed when hovering over an image.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.author.tooltip.TooltipInformation.ORIGIN_IMAGE)

### ORIGIN_ERROR_NODE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ORIGIN_ERROR_NODE

Tooltip computed when hovering over an error node.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.author.tooltip.TooltipInformation.ORIGIN_ERROR_NODE)

### ORIGIN_VALIDATION_ERROR

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ORIGIN_VALIDATION_ERROR

Validation error.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.author.tooltip.TooltipInformation.ORIGIN_VALIDATION_ERROR)

### ORIGIN_CHANGE_MARKERS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ORIGIN_CHANGE_MARKERS

Hovering over comment change tracking.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.author.tooltip.TooltipInformation.ORIGIN_CHANGE_MARKERS)

## Constructor Details

### TooltipInformation

public TooltipInformation([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description, [AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) hoveredNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tooltipOriginInformation, int mouseX, int mouseY)

Constructor.
  Parameters: description - Original tooltip description. Can be null hoveredNode - The hovered node. Can be null tooltipOriginInformation - Details about where the hovered error came from. Can be null mouseX - Mouse X coordinate. mouseY - Mouse Y coordinate.
## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()

Get the current description which will be used for the tooltip.
  Returns: Returns the description which will be displayed for the tooltip.
### setDescription

public void setDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description)

Set a description to be used on the tooltip. The description can also be in HTML format.
  Parameters: description - The description.
### getMouseX

public int getMouseX()

Get mouse X coordinates
  Returns: Returns the mouse X coordinates.
### getMouseY

public int getMouseY()

Get mouse Y coordinates
  Returns: Returns the mouse Y coordinates.
### getHoveredNode

public [AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) getHoveredNode()

Get the hovered node, can be null.
  Returns: Returns the hovered node, can be null.
### getHoveredErrorOriginInformation

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHoveredErrorOriginInformation()

Get information about the originator for the tooltip (for example if it is given by hovering an error message or by hovering an image or so on). Can be null.
  Returns: Returns information about the originator for the tooltip.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
