Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Class ColorHighlightPainter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.highlights.ColorHighlightPainter
   All Implemented Interfaces: [HighlightPainter](HighlightPainter.md), [PrioritizableHighlightPainter](PrioritizableHighlightPainter.md), [TextForegroundHighlighterPainter](TextForegroundHighlighterPainter.md)   @API(type=EXTENDABLE, src=PUBLIC) public class ColorHighlightPainter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [TextForegroundHighlighterPainter](TextForegroundHighlighterPainter.md), [PrioritizableHighlightPainter](PrioritizableHighlightPainter.md)
Painter that can be used to customize the way that a highlight is displayed by setting custom text decoration, text decoration stroke, background color or stroke color.

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static enum  [ColorHighlightPainter.TextDecoration](ColorHighlightPainter.TextDecoration.md)
The decoration added to text.

## Nested classes/interfaces inherited from interface ro.sync.ecss.extensions.api.highlights.[PrioritizableHighlightPainter](PrioritizableHighlightPainter.md)
 [PrioritizableHighlightPainter.ZLayer](PrioritizableHighlightPainter.ZLayer.md)
## Constructor Summary
 Constructors
Constructor

Description
 [ColorHighlightPainter](#%3Cinit%3E())()
Default constructor.
  [ColorHighlightPainter](#%3Cinit%3E(ro.sync.exml.view.graphics.Color,int,int))([Color](../../../../exml/view/graphics/Color.md) color, int height, int totalHeight)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 [Color](../../../../exml/view/graphics/Color.md) [getBgColor](#getBgColor())()

 [Color](../../../../exml/view/graphics/Color.md) [getColor](#getColor())()

 protected int [getHighlightLength](#getHighlightLength(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo))([HighlightPainterInfo](HighlightPainterInfo.md) pi)
Get the length to highlight.
  [Color](../../../../exml/view/graphics/Color.md) [getTextForegroundColor](#getTextForegroundColor())()
Get the text foreground color.
  [PrioritizableHighlightPainter.ZLayer](PrioritizableHighlightPainter.ZLayer.md) [getZLayer](#getZLayer())()
All in the first layer.
  void [paint](#paint(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo))([HighlightPainterInfo](HighlightPainterInfo.md) pi)
Renders the highlight.
  void [setBgColor](#setBgColor(ro.sync.exml.view.graphics.Color))([Color](../../../../exml/view/graphics/Color.md) bgColor)

 void [setBgColor](#setBgColor(ro.sync.exml.view.graphics.Color,boolean))([Color](../../../../exml/view/graphics/Color.md) bgColor, boolean useLineBoxHeight)

 void [setColor](#setColor(ro.sync.exml.view.graphics.Color))([Color](../../../../exml/view/graphics/Color.md) c)
Set the color used for decoration (strike out or underline)
  void [setStrikeOut](#setStrikeOut(boolean))(boolean strikeOut)  Deprecated.
Use [setTextDecoration(TextDecoration)](#setTextDecoration(ro.sync.ecss.extensions.api.highlights.ColorHighlightPainter.TextDecoration)) instead.
   void [setTextDecoration](#setTextDecoration(ro.sync.ecss.extensions.api.highlights.ColorHighlightPainter.TextDecoration))([ColorHighlightPainter.TextDecoration](ColorHighlightPainter.TextDecoration.md) decoration)
Set the text decoration.
  void [setTextDecorationStroke](#setTextDecorationStroke(int))(int stroke)
Set the text decoration stroke.
  void [setTextForegroundColor](#setTextForegroundColor(ro.sync.exml.view.graphics.Color))([Color](../../../../exml/view/graphics/Color.md) foregroundColor)
Set the text foreground color.
  boolean [useBaseLineForUnderline](#useBaseLineForUnderline())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ColorHighlightPainter

public ColorHighlightPainter()

Default constructor. The color is red.

### ColorHighlightPainter

public ColorHighlightPainter([Color](../../../../exml/view/graphics/Color.md) color, int height, int totalHeight)

Constructor.
  Parameters: color - The color to use for highlight. height - The height of the highlight line. This may be smaller than the total height. If it is, the extra space will remain under the line. totalHeight - The height of the highlight.
## Method Details

### getZLayer

public [PrioritizableHighlightPainter.ZLayer](PrioritizableHighlightPainter.ZLayer.md) getZLayer()

All in the first layer.
  Specified by: [getZLayer](PrioritizableHighlightPainter.md#getZLayer()) in interface [PrioritizableHighlightPainter](PrioritizableHighlightPainter.md) Returns: the base layer. See Also:
        * [PrioritizableHighlightPainter.getZLayer()](PrioritizableHighlightPainter.md#getZLayer())

### paint

public void paint([HighlightPainterInfo](HighlightPainterInfo.md) pi)
 Description copied from interface: [HighlightPainter](HighlightPainter.md#paint(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo))
Renders the highlight.
  Specified by: [paint](HighlightPainter.md#paint(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo)) in interface [HighlightPainter](HighlightPainter.md) Parameters: pi - Information used by highlight See Also:
        * [HighlightPainter.paint(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo)](HighlightPainter.md#paint(ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo))

### getHighlightLength

protected int getHighlightLength([HighlightPainterInfo](HighlightPainterInfo.md) pi)

Get the length to highlight.
  Parameters: pi - The painter info. Returns: the length to highlight.
### setColor

public void setColor([Color](../../../../exml/view/graphics/Color.md) c)

Set the color used for decoration (strike out or underline)
  Parameters: c - The decoration color.
### setTextDecoration

public void setTextDecoration([ColorHighlightPainter.TextDecoration](ColorHighlightPainter.TextDecoration.md) decoration)

Set the text decoration. If is set to [ColorHighlightPainter.TextDecoration.NONE](ColorHighlightPainter.TextDecoration.md#NONE) no line will be drawn.
  Parameters: decoration - The new text decoration.
### setBgColor

public void setBgColor([Color](../../../../exml/view/graphics/Color.md) bgColor)
  Parameters: bgColor - The background color to set.
### setBgColor

public void setBgColor([Color](../../../../exml/view/graphics/Color.md) bgColor, boolean useLineBoxHeight)
  Parameters: bgColor - The background color to set. useLineBoxHeight - true to use the parent line height for drawing the background color.
### useBaseLineForUnderline

public boolean useBaseLineForUnderline()
  Returns: true if use the base line for underlining
### setTextDecorationStroke

public void setTextDecorationStroke(int stroke)

Set the text decoration stroke.
  Parameters: stroke - The new Stroke type. Constants are defined in [Graphics](../../../../exml/view/graphics/Graphics.md).
### setStrikeOut

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public void setStrikeOut(boolean strikeOut)
 Deprecated.
Use [setTextDecoration(TextDecoration)](#setTextDecoration(ro.sync.ecss.extensions.api.highlights.ColorHighlightPainter.TextDecoration)) instead.
   Parameters: strikeOut - Set this highlight as strike out.
### getBgColor

public [Color](../../../../exml/view/graphics/Color.md) getBgColor()
  Returns: Returns the background color.
### getColor

public [Color](../../../../exml/view/graphics/Color.md) getColor()
  Returns: Returns the color used for decoration (strike out or underline)
### setTextForegroundColor

public void setTextForegroundColor([Color](../../../../exml/view/graphics/Color.md) foregroundColor)

Set the text foreground color.
  Parameters: foregroundColor - The foreground color to set. Since: 13.2
### getTextForegroundColor

public [Color](../../../../exml/view/graphics/Color.md) getTextForegroundColor()

Get the text foreground color.
  Specified by: [getTextForegroundColor](TextForegroundHighlighterPainter.md#getTextForegroundColor()) in interface [TextForegroundHighlighterPainter](TextForegroundHighlighterPainter.md) Returns: the color for the text foreground. NULL for inhibiting this feature. Since: 13.2 See Also:
        * [TextForegroundHighlighterPainter.getTextForegroundColor()](TextForegroundHighlighterPainter.md#getTextForegroundColor())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
