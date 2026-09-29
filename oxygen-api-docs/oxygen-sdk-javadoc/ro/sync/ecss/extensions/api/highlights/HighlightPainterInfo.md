Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Class HighlightPainterInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.highlights.HighlightPainterInfo
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class HighlightPainterInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Information needed by the painter.

## Constructor Summary
 Constructors
Constructor

Description
 [HighlightPainterInfo](#%3Cinit%3E(ro.sync.exml.view.graphics.Graphics,int,ro.sync.exml.view.graphics.Point,int,int,int,int,int,int,int,int,ro.sync.exml.view.graphics.Point,int,int,int))([Graphics](../../../../exml/view/graphics/Graphics.md) g, int currentBoxHeight, [Point](../../../../exml/view/graphics/Point.md) origin, int relativeX, int textYPadding, int length, int startOffset, int endOffset, int baseLine, int fontAscent, int fontSize, [Point](../../../../exml/view/graphics/Point.md) parentLineBoxOrigin, int parentLineBoxWidth, int parentLineBoxHeight, int viewEndOffset)
Renders the highlight.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getBaseLine](#getBaseLine())()
Returns the base line relative to top, relative to the box.
  int [getCurrentBoxHeight](#getCurrentBoxHeight())()
Current run of text/image height.
  int [getEndOffset](#getEndOffset())()
Returns the end offset in content.
  int [getFontAscent](#getFontAscent())()
Returns the font ascent.
  int [getFontSize](#getFontSize())()
Returns the font size.
  [Graphics](../../../../exml/view/graphics/Graphics.md) [getGraphics](#getGraphics())()
Returns the graphics used for paint.
  int [getLength](#getLength())()
Returns the length of highlight, in pixels.
  [Point](../../../../exml/view/graphics/Point.md) [getOrigin](#getOrigin())()
Returns the origin of box, relative to the upper corner of the editor.
  int [getParentLineBoxHight](#getParentLineBoxHight())()

 [Point](../../../../exml/view/graphics/Point.md) [getParentLineBoxOrigin](#getParentLineBoxOrigin())()

 int [getParentLineBoxWidth](#getParentLineBoxWidth())()

 int [getRelativeX](#getRelativeX())()
Returns the relative X from where highlight should start.
  int [getStartOffset](#getStartOffset())()
Returns the start offset in content.
  int [getTextYPadding](#getTextYPadding())()
Returns the relative Y position from box Y used to paint the text inside the box.
  int [getViewEndOffset](#getViewEndOffset())()

 boolean [isHighlightOverFormControl](#isHighlightOverFormControl())()
Check if we have a highlight over form controls
  boolean [isHighlightOverImage](#isHighlightOverImage())()

 boolean [isHighlightOverText](#isHighlightOverText())()
Returns true if the highlight is done over a text view.
  void [setHighlightOverFormControls](#setHighlightOverFormControls(boolean))(boolean isHighlightOverFormControl)
Set highlight over form controls.
  void [setHighlightOverImage](#setHighlightOverImage(boolean))(boolean isHighlightOverImage)
true if the highlight is over an image
  void [setHighlightOverText](#setHighlightOverText(boolean))(boolean isHighlightOverText)
It is set by the author layout, so that the painter knows the painted box is a text box.
  void [setLength](#setLength(int))(int length)
Set a new value for the length of the highlight, in pixels.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### HighlightPainterInfo

public HighlightPainterInfo([Graphics](../../../../exml/view/graphics/Graphics.md) g, int currentBoxHeight, [Point](../../../../exml/view/graphics/Point.md) origin, int relativeX, int textYPadding, int length, int startOffset, int endOffset, int baseLine, int fontAscent, int fontSize, [Point](../../../../exml/view/graphics/Point.md) parentLineBoxOrigin, int parentLineBoxWidth, int parentLineBoxHeight, int viewEndOffset)

Renders the highlight.
  Parameters: g - The graphics currentBoxHeight - The current box height. origin - Origin (upper left corner of the box in absolute coordinates) relativeX - The x relative to the origin where the highlight must start. textYPadding - The relative Y position from box Y used to paint the box. length - The length of the highlight, in pixels. startOffset - Start offset of highlight endOffset - End offset of highlight baseLine - The base line relative to the box start fontAscent - The font ascent fontSize - The font size parentLineBoxWidth - The width of the parent line box. Can be -1. parentLineBoxHeight - The height of the parent line box. Can be -1. parentLineBoxOrigin - The origin of the parent line box. Can be null. viewEndOffset - The end offset of the current view over which the highight is being painted.
## Method Details

### setHighlightOverText

public void setHighlightOverText(boolean isHighlightOverText)

It is set by the author layout, so that the painter knows the painted box is a text box.
  Parameters: isHighlightOverText - The isHighlightOverText to set.
### getGraphics

public [Graphics](../../../../exml/view/graphics/Graphics.md) getGraphics()

Returns the graphics used for paint.
  Returns: Returns the graphics used for paint.
### getCurrentBoxHeight

public int getCurrentBoxHeight()

Current run of text/image height. Usually the highlight should expand as high as the containing box.
  Returns: Current run of text/image height. Usually the highlight should expand as high as the containing box.
### getOrigin

public [Point](../../../../exml/view/graphics/Point.md) getOrigin()

Returns the origin of box, relative to the upper corner of the editor.
  Returns: Returns the origin of box, relative to the upper corner of the editor.
### getRelativeX

public int getRelativeX()

Returns the relative X from where highlight should start.
  Returns: Returns the relative X from where highlight should start.
### getTextYPadding

public int getTextYPadding()

Returns the relative Y position from box Y used to paint the text inside the box.
  Returns: The relative Y position from box Y used to paint the text inside the box.
### getLength

public int getLength()

Returns the length of highlight, in pixels.
  Returns: Returns the length of highlight, in pixels.
### setLength

public void setLength(int length)

Set a new value for the length of the highlight, in pixels.
  Parameters: length - the new value.
### getStartOffset

public int getStartOffset()

Returns the start offset in content.
  Returns: Returns the start offset in content.
### getEndOffset

public int getEndOffset()

Returns the end offset in content.
  Returns: Returns the end offset in content.
### getBaseLine

public int getBaseLine()

Returns the base line relative to top, relative to the box.
  Returns: Returns the base line relative to top, relative to the box.
### getFontAscent

public int getFontAscent()

Returns the font ascent.
  Returns: Returns the font ascent.
### getFontSize

public int getFontSize()

Returns the font size.
  Returns: Returns the font size.
### isHighlightOverText

public boolean isHighlightOverText()

Returns true if the highlight is done over a text view.
  Returns: Returns true if the highlight is done over a text view.
### getParentLineBoxHight

public int getParentLineBoxHight()
  Returns: Returns the height of parent line box. Can be -1.
### getParentLineBoxWidth

public int getParentLineBoxWidth()
  Returns: Returns the width of parent line box. Can be -1.
### getParentLineBoxOrigin

public [Point](../../../../exml/view/graphics/Point.md) getParentLineBoxOrigin()
  Returns: Returns the origin(absolute) of the parent line box. Can be null.
### setHighlightOverImage

public void setHighlightOverImage(boolean isHighlightOverImage)

true if the highlight is over an image
  Parameters: isHighlightOverImage - true if the highlight is over an image
### isHighlightOverImage

public boolean isHighlightOverImage()
  Returns: Returns true if the highlight is over an image
### setHighlightOverFormControls

public void setHighlightOverFormControls(boolean isHighlightOverFormControl)

Set highlight over form controls.
  Parameters: isHighlightOverFormControl - true if we have a highlight over form controls.
### isHighlightOverFormControl

public boolean isHighlightOverFormControl()

Check if we have a highlight over form controls
  Returns: Returns true if we have a highlight over form controls.
### getViewEndOffset

public int getViewEndOffset()
  Returns: The end offset of the current view over which the highight is being painted.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
