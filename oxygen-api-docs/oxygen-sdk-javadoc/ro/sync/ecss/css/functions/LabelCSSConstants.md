Package [ro.sync.ecss.css.functions](package-summary.md)

# Interface LabelCSSConstants
    @API(type=EXTENDABLE, src=PUBLIC) public interface LabelCSSConstants
Processed arguments of the oxy_label function.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [BACKGROUND_COLOR_PROPERTY](#BACKGROUND_COLOR_PROPERTY)
A background color for the label.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [BASE_SYSTEM_ID](#BASE_SYSTEM_ID)
Base system id to be used to resolve imports from [STYLES_PROPERTY](#STYLES_PROPERTY).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [COLOR_PROPERTY](#COLOR_PROPERTY)
A foreground color for the text.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [STYLES_PROPERTY](#STYLES_PROPERTY)
Possibility to specify CSS rules for this label.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TEXT_ALIGN_PROPERTY](#TEXT_ALIGN_PROPERTY)
The alignment of the label.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TEXT_PROPERTY](#TEXT_PROPERTY)
The text that will be displayed as a label.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [WIDTH_PROPERTY](#WIDTH_PROPERTY)
The width of the label.

## Field Details

### TEXT_PROPERTY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TEXT_PROPERTY

The text that will be displayed as a label. A string value.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.css.functions.LabelCSSConstants.TEXT_PROPERTY)

### WIDTH_PROPERTY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) WIDTH_PROPERTY

The width of the label. An [RelativeLength](../RelativeLength.md).
**Note:** In case you don't have the possibility to build a [RelativeLength](../RelativeLength.md) then you can use the [STYLES_PROPERTY](#STYLES_PROPERTY) to give the width as a string: \* { width:100px; }

  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.css.functions.LabelCSSConstants.WIDTH_PROPERTY)

### TEXT_ALIGN_PROPERTY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TEXT_ALIGN_PROPERTY

The alignment of the label. A string value: left, right or center.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.css.functions.LabelCSSConstants.TEXT_ALIGN_PROPERTY)

### COLOR_PROPERTY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) COLOR_PROPERTY

A foreground color for the text. A [Color](../../../exml/view/graphics/Color.md).
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.css.functions.LabelCSSConstants.COLOR_PROPERTY)

### BACKGROUND_COLOR_PROPERTY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) BACKGROUND_COLOR_PROPERTY

A background color for the label. A [Color](../../../exml/view/graphics/Color.md).
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.css.functions.LabelCSSConstants.BACKGROUND_COLOR_PROPERTY)

### STYLES_PROPERTY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) STYLES_PROPERTY

Possibility to specify CSS rules for this label.

Example: \* { text-align:right; color:red; }
The selectors are ignored, all rules are considered to match.
You can also specify as CSS something like: @import 'label_styles.css';Relative imports will be resolved relative to [BASE_SYSTEM_ID](#BASE_SYSTEM_ID). This approach is useful to easily reuse the same styles for more oxy_labels.
 **The following properties are handled:**
        * font-weight, font-size, font-style, font
        * text-align, text-decoration
        * width
        * color, background-color

  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.css.functions.LabelCSSConstants.STYLES_PROPERTY)

### BASE_SYSTEM_ID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) BASE_SYSTEM_ID

Base system id to be used to resolve imports from [STYLES_PROPERTY](#STYLES_PROPERTY). This normally is the system ID of the CSS file in which the oxy_label was encountered.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.css.functions.LabelCSSConstants.BASE_SYSTEM_ID)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
