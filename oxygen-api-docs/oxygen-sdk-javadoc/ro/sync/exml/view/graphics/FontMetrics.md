Package [ro.sync.exml.view.graphics](package-summary.md)

# Interface FontMetrics
    @API(type=NOT_EXTENDABLE, src=PRIVATE) public interface FontMetrics
Common font metrics

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 int [charsWidth](#charsWidth(char%5B%5D,int,int))(char[] chars, int off, int len)
Returns the total advance width for showing the specified array of characters in this Font.
  int [charWidth](#charWidth(char))(char c)
Get the char width
  int [getAscent](#getAscent())()
The font ascent is the distance from the font's baseline to the top of most alphanumeric characters.
  int [getCorrectedBreakYForWrappedString](#getCorrectedBreakYForWrappedString(ro.sync.exml.view.graphics.AttributedString,int,int))([AttributedString](AttributedString.md) aStr, int wrappingWidth, int initialBreak)
Gets the y coordinate where the given wrapped string bounds can be split without cutting off a text line.
  int [getDescent](#getDescent())()
The font descent is the distance from the font's baseline to the bottom of most alphanumeric characters with descenders.
  int [getHeight](#getHeight())()

 int [getLeading](#getLeading())()
Determines the standard leading of the Font described by this FontMetricsobject.
  default int [getMaxCharWidth](#getMaxCharWidth())()
Get the maximum character width, -1 if not implemented.
  [Rectangle](Rectangle.md) [getWrappedStringBounds](#getWrappedStringBounds(ro.sync.exml.view.graphics.AttributedString,int))([AttributedString](AttributedString.md) aStr, int wrappingWidth)
Gets the bounds of a string that is wrapped at the wrappingWidth.
  [AttributedString](AttributedString.md)[] [limitAttributedString](#limitAttributedString(ro.sync.exml.view.graphics.AttributedString,int,int))([AttributedString](AttributedString.md) aStr, int wrappingWidth, int maxLineCount)
Limit the given attributed string at a maximum number of lines.
  int [stringWidth](#stringWidth(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text)
Returns the total advance width for showing the specified String in this Font.

## Method Details

### charsWidth

int charsWidth(char[] chars, int off, int len)

Returns the total advance width for showing the specified array of characters in this Font.
  Parameters: chars - the array of characters to be measured off - the start offset of the characters in the array len - the number of characters to be measured from the array Returns: the advance width of the subarray of the specified char array in the font described by this FontMetrics object.
### getAscent

int getAscent()

The font ascent is the distance from the font's baseline to the top of most alphanumeric characters.
  Returns: The font ascent.
### getDescent

int getDescent()

The font descent is the distance from the font's baseline to the bottom of most alphanumeric characters with descenders.
  Returns: The ont descent.
### stringWidth

int stringWidth([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text)

Returns the total advance width for showing the specified String in this Font.
  Parameters: text - The text. Returns: The width of the text.
### getHeight

int getHeight()
  Returns: The font height
### charWidth

int charWidth(char c)

Get the char width
  Parameters: c - The char Returns: The char width
### getLeading

int getLeading()

Determines the standard leading of the Font described by this FontMetricsobject. The standard leading, or interline spacing, is the logical amount of space to be reserved between the descent of one line of text and the ascent of the next line. The height metric is calculated to include this extra space.
  Returns: the standard leading of the Font.
### getWrappedStringBounds

[Rectangle](Rectangle.md) getWrappedStringBounds([AttributedString](AttributedString.md) aStr, int wrappingWidth)

Gets the bounds of a string that is wrapped at the wrappingWidth. Takes into account newlines.
  Parameters: aStr - The text, as an attributed string. The {TextAttribute#FONT} and {TextAttribute#FOREGROUND} contain values that are instances of [Font](Font.md) and [Color](Color.md). wrappingWidth - The maximum width of the text. Returns: The bounds of the wrapped string.
### limitAttributedString

[AttributedString](AttributedString.md)[] limitAttributedString([AttributedString](AttributedString.md) aStr, int wrappingWidth, int maxLineCount)

Limit the given attributed string at a maximum number of lines.
  Parameters: aStr - The text, as an attributed string. The {TextAttribute#FONT} and {TextAttribute#FOREGROUND} contain values that are instances of [Font](Font.md) and [Color](Color.md). wrappingWidth - The maximum width of the text. maxLineCount - The maximum number of lines. Returns: The array of attributed strings, one for each line of text (if the given attributed string overflows the maximum number of lines) or the initial attributed string (if there is no overflow)
### getCorrectedBreakYForWrappedString

int getCorrectedBreakYForWrappedString([AttributedString](AttributedString.md) aStr, int wrappingWidth, int initialBreak)

Gets the y coordinate where the given wrapped string bounds can be split without cutting off a text line. If the given initial break Y is inside a text line, the resulting break will point to the top of the text line. Otherwise -1 is returned.
  Parameters: aStr - The text, as an attributed string. The {TextAttribute#FONT} and {TextAttribute#FOREGROUND} contain values that are instances of [Font](Font.md) and [Color](Color.md). wrappingWidth - The maximum width of the text. initialBreak - The initial break Y coordinate. Returns: The corrected Y break coordinate or -1 if the initial break is not placed inside a text line.
### getMaxCharWidth

default int getMaxCharWidth()

Get the maximum character width, -1 if not implemented.
  Returns: the maximum character width, -1 if not implemented.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
