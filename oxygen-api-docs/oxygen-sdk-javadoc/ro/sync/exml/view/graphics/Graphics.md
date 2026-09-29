Package [ro.sync.exml.view.graphics](package-summary.md)

# Interface Graphics
    @API(type=NOT_EXTENDABLE, src=PRIVATE) public interface Graphics
The graphics interface used to draw Author and Schema Diagram.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [FILL_PATTERN_SQUARE](#FILL_PATTERN_SQUARE)
A pattern of squares (of size 1).
  static final int [FILL_PATTERN_SQUARE_BIG](#FILL_PATTERN_SQUARE_BIG)
A pattern of big squares (of size 2).
  static final int [ICON_COMMENT_TREE](#ICON_COMMENT_TREE)
Icon code for comment nodes.
  static final int [ICON_PROCESSING_INSTRUCTION_TREE](#ICON_PROCESSING_INSTRUCTION_TREE)
Icon code for processing instruction nodes.
  static final int [ICON_TEXT_TREE](#ICON_TEXT_TREE)
Icon code for text nodes.
  static final int [IMAGE_EXPANSION_BAR_BOTTOM](#IMAGE_EXPANSION_BAR_BOTTOM)
Image representing the bottom arrow of the expansion bar.
  static final int [IMAGE_EXPANSION_BAR_COLLAPSED](#IMAGE_EXPANSION_BAR_COLLAPSED)
Image representing an arrow for the collapsed expansion bar.
  static final int [IMAGE_EXPANSION_BAR_MIDDLE_GRADIENT](#IMAGE_EXPANSION_BAR_MIDDLE_GRADIENT)
Image representing the middle of the expansion bar gradient.
  static final int [IMAGE_EXPANSION_BAR_TOP](#IMAGE_EXPANSION_BAR_TOP)
Image representing the top arrow of the expansion bar.
  static final int [STROKE_DASHED](#STROKE_DASHED)
Dotted stroke
  static final int [STROKE_DOT_DASH](#STROKE_DOT_DASH)
Dot-dash stroke
  static final int [STROKE_DOT_DOT_DASH](#STROKE_DOT_DOT_DASH)
Dot-dot-dash stroke
  static final int [STROKE_DOTTED](#STROKE_DOTTED)
Dotted stroke
  static final int [STROKE_NORMAL](#STROKE_NORMAL)
Normal stroke
  static final int [STROKE_WAVY](#STROKE_WAVY)
Wavy stroke with endings.
  static final int [STROKE_WAVY_NO_ENDINGS](#STROKE_WAVY_NO_ENDINGS)
Wavy stroke without endings.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [activateAntialiasing](#activateAntialiasing())()
Activate the antialiasing mode.
  [Font](Font.md) [deriveSize](#deriveSize(ro.sync.exml.view.graphics.Font,int))([Font](Font.md) current, int size)
Derive the size of the font
  [Font](Font.md) [deriveStyle](#deriveStyle(ro.sync.exml.view.graphics.Font,int))([Font](Font.md) current, int style)
Derive the style of the font
  void [disableAntialiasing](#disableAntialiasing())()
Disable the antialiasing mode.
  void [drawArc](#drawArc(int,int,int,int,int,int))(int x, int y, int width, int height, int startAngle, int arcAngle)
draws an arc.
  void [drawIcon](#drawIcon(java.lang.Object,int,int,int))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) hostComponent, int iconCode, int x, int y)
Draw the icon at (x,y) coordinates.
  void [drawImage](#drawImage(java.lang.Object,int,int))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) image, int x, int y)
Draw an image object depending on the platform
  void [drawImage](#drawImage(java.lang.Object,int,int,int,int))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) image, int x, int y, int width, int height)
Draw an image object depending on the platform.
  void [drawImage](#drawImage(java.lang.Object,int,int,int,int,int,int,int,int))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) img, int dx1, int dy1, int dx2, int dy2, int sx1, int sy1, int sx2, int sy2)
Draws as much of the specified area of the specified image as is currently available, scaling it on the fly to fit inside the specified area of the destination drawable surface.
  void [drawLine](#drawLine(int,int,int,int))(int x1, int y1, int x2, int y2)
Draw a line from (x1, y1) to (x2, y2).
  void [drawOval](#drawOval(int,int,int,int))(int x, int y, int width, int height)
Draw an oval.
  void [drawPolygon](#drawPolygon(int%5B%5D,int%5B%5D,int))(int[] xPoints, int[] yPoints, int nPoints)
Draw a closed polygon defined by arrays of *x* and *y* coordinates.
  void [drawPolyline](#drawPolyline(int%5B%5D,int%5B%5D,int))(int[] xpoints, int[] ypoints, int npoints)
Draws a polyline which is not closed if the last point differs from the first.
  void [drawRect](#drawRect(int,int,int,int))(int x, int y, int width, int height)
Draw a rect with (x,y) top-left corner.
  void [drawRoundRect](#drawRoundRect(int,int,int,int,int,int))(int x, int y, int width, int height, int arcWidth, int arcHeight)
Draws an outlined round-cornered rectangle using this graphics context's current color.
  void [drawShadow](#drawShadow(ro.sync.exml.view.graphics.Shape,int))([Shape](Shape.md) shape, int displacement)
Draws a shadow using the shape of the polygon.
  void [drawShape](#drawShape(ro.sync.exml.view.graphics.Shape))([Shape](Shape.md) shape)
Draw a shape
  void [drawString](#drawString(java.lang.String,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, int x, int y)
Draw a string.
  void [drawWrappedString](#drawWrappedString(ro.sync.exml.view.graphics.AttributedString,int,int,int))([AttributedString](AttributedString.md) aStr, int x, int y, int wrappingWidth)
Draws a string at the specified coordinates.
  void [drawWrappedString](#drawWrappedString(ro.sync.exml.view.graphics.AttributedString,int,int,int,boolean))([AttributedString](AttributedString.md) aStr, int x, int y, int wrappingWidth, boolean drawAtBaseLine)
Draws a string at the specified coordinates.
  void [fillArc](#fillArc(int,int,int,int,int,int))(int x, int y, int width, int height, int startAngle, int arcAngle)
Fills an arc.
  void [fillOval](#fillOval(int,int,int,int))(int x, int y, int width, int height)
Fill an oval with curent fill color.
  void [fillPolygon](#fillPolygon(int%5B%5D,int%5B%5D,int))(int[] xPoints, int[] yPoints, int nPoints)
Fills a closed polygon defined by arrays of *x* and *y* coordinates.
  void [fillRect](#fillRect(int,int,int,int))(int x, int y, int width, int height)
Fill a rect with (x,y) top-left corner.
  void [fillRect](#fillRect(int,int,int,int,int,ro.sync.exml.view.graphics.Color))(int x, int y, int width, int height, int fillPattern, [Color](Color.md) fillColor)
Fills a rectangle with a pattern.
  void [fillRect](#fillRect(ro.sync.exml.view.graphics.Rectangle))([Rectangle](Rectangle.md) rectangle)
Fill a rectangle.
  void [fillRoundRect](#fillRoundRect(int,int,int,int,int,int))(int x, int y, int width, int height, int arcWidth, int arcHeight)
Fills the specified rounded corner rectangle.
  void [fillShape](#fillShape(ro.sync.exml.view.graphics.Shape))([Shape](Shape.md) shape)
Fill a shape
  void [fillWithGradient](#fillWithGradient(ro.sync.exml.view.graphics.Ellipse,ro.sync.exml.view.graphics.Color,ro.sync.exml.view.graphics.Color,boolean))([Ellipse](Ellipse.md) ellipse, [Color](Color.md) startColorCode, [Color](Color.md) endColorCode, boolean isVertical)

 void [fillWithGradient](#fillWithGradient(ro.sync.exml.view.graphics.Polygon,ro.sync.exml.view.graphics.Color,ro.sync.exml.view.graphics.Color,boolean))([Polygon](Polygon.md) polygon, [Color](Color.md) startColorCode, [Color](Color.md) endColorCode, boolean isVertical)

 void [fillWithGradient](#fillWithGradient(ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Color,ro.sync.exml.view.graphics.Color,boolean))([Rectangle](Rectangle.md) rect, [Color](Color.md) startColorCode, [Color](Color.md) endColorCode, boolean isVertical)

 void [fillWithGradient](#fillWithGradient(ro.sync.exml.view.graphics.Shape,ro.sync.exml.view.graphics.Color,ro.sync.exml.view.graphics.Color,boolean))([Shape](Shape.md) shape, [Color](Color.md) startColorCode, [Color](Color.md) endColorCode, boolean isVertical)

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getAntialiasing](#getAntialiasing())()

 [Rectangle](Rectangle.md) [getClipBounds](#getClipBounds())()

 [Color](Color.md) [getDrawColor](#getDrawColor())()
Get the current color code.
  [Color](Color.md) [getFillColor](#getFillColor())()
Get the color code for fill shapes.
  [Font](Font.md) [getFont](#getFont())()
Get current font.
  [FontMetrics](FontMetrics.md) [getFontMetrics](#getFontMetrics(ro.sync.exml.view.graphics.Font))([Font](Font.md) font)

 int [getStrokeType](#getStrokeType())()

 int [getStrokeWidth](#getStrokeWidth())()

 void [plainDrawString](#plainDrawString(java.lang.String,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, int x, int y)
Draw a string directly using the graphics, without creating a text layout.
  void [setAntialiasing](#setAntialiasing(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)

 void [setClipBounds](#setClipBounds(ro.sync.exml.view.graphics.Rectangle))([Rectangle](Rectangle.md) clip)
Set cliping for the graphics.
  void [setDrawColor](#setDrawColor(ro.sync.exml.view.graphics.Color))([Color](Color.md) colorCode)
Set the color for draw methods.
  void [setFillColor](#setFillColor(ro.sync.exml.view.graphics.Color))([Color](Color.md) colorCode)
Set the color for fill methods.
  void [setFont](#setFont(ro.sync.exml.view.graphics.Font))([Font](Font.md) font)
Set the new font.
  void [setStroke](#setStroke(int,int))(int width, int type)
Sets the line width for the stroke.

## Field Details

### ICON_TEXT_TREE

static final int ICON_TEXT_TREE

Icon code for text nodes.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.ICON_TEXT_TREE)

### ICON_COMMENT_TREE

static final int ICON_COMMENT_TREE

Icon code for comment nodes.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.ICON_COMMENT_TREE)

### ICON_PROCESSING_INSTRUCTION_TREE

static final int ICON_PROCESSING_INSTRUCTION_TREE

Icon code for processing instruction nodes.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.ICON_PROCESSING_INSTRUCTION_TREE)

### IMAGE_EXPANSION_BAR_TOP

static final int IMAGE_EXPANSION_BAR_TOP

Image representing the top arrow of the expansion bar.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.IMAGE_EXPANSION_BAR_TOP)

### IMAGE_EXPANSION_BAR_BOTTOM

static final int IMAGE_EXPANSION_BAR_BOTTOM

Image representing the bottom arrow of the expansion bar.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.IMAGE_EXPANSION_BAR_BOTTOM)

### IMAGE_EXPANSION_BAR_MIDDLE_GRADIENT

static final int IMAGE_EXPANSION_BAR_MIDDLE_GRADIENT

Image representing the middle of the expansion bar gradient.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.IMAGE_EXPANSION_BAR_MIDDLE_GRADIENT)

### IMAGE_EXPANSION_BAR_COLLAPSED

static final int IMAGE_EXPANSION_BAR_COLLAPSED

Image representing an arrow for the collapsed expansion bar.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.IMAGE_EXPANSION_BAR_COLLAPSED)

### STROKE_NORMAL

static final int STROKE_NORMAL

Normal stroke
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.STROKE_NORMAL)

### STROKE_DOTTED

static final int STROKE_DOTTED

Dotted stroke
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.STROKE_DOTTED)

### STROKE_DASHED

static final int STROKE_DASHED

Dotted stroke
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.STROKE_DASHED)

### STROKE_WAVY

static final int STROKE_WAVY

Wavy stroke with endings.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.STROKE_WAVY)

### STROKE_WAVY_NO_ENDINGS

static final int STROKE_WAVY_NO_ENDINGS

Wavy stroke without endings.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.STROKE_WAVY_NO_ENDINGS)

### STROKE_DOT_DASH

static final int STROKE_DOT_DASH

Dot-dash stroke
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.STROKE_DOT_DASH)

### STROKE_DOT_DOT_DASH

static final int STROKE_DOT_DOT_DASH

Dot-dot-dash stroke
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.STROKE_DOT_DOT_DASH)

### FILL_PATTERN_SQUARE

static final int FILL_PATTERN_SQUARE

A pattern of squares (of size 1).
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.FILL_PATTERN_SQUARE)

### FILL_PATTERN_SQUARE_BIG

static final int FILL_PATTERN_SQUARE_BIG

A pattern of big squares (of size 2).
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Graphics.FILL_PATTERN_SQUARE_BIG)

## Method Details

### setFont

void setFont([Font](Font.md) font)

Set the new font.
  Parameters: font - The font to be used.
### fillPolygon

void fillPolygon(int[] xPoints, int[] yPoints, int nPoints)

Fills a closed polygon defined by arrays of *x* and *y* coordinates.
  Parameters: xPoints - a an array of x coordinates. yPoints - a an array of y coordinates. nPoints - a the total number of points.
### drawPolygon

void drawPolygon(int[] xPoints, int[] yPoints, int nPoints)

Draw a closed polygon defined by arrays of *x* and *y* coordinates.
  Parameters: xPoints - a an array of x coordinates. yPoints - a an array of y coordinates. nPoints - a the total number of points.
### getFont

[Font](Font.md) getFont()

Get current font.
  Returns: The current font.
### drawString

void drawString([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, int x, int y)

Draw a string.
  Parameters: text - The text to be drawn. x - The x coordinate. y - The y coordinate(top-left).
### plainDrawString

void plainDrawString([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, int x, int y)

Draw a string directly using the graphics, without creating a text layout.
  Parameters: text - The text to be drawn. x - The x coordinate. y - The y coordinate(top-left).
### getDrawColor

[Color](Color.md) getDrawColor()

Get the current color code.
  Returns: The current color code.
### drawLine

void drawLine(int x1, int y1, int x2, int y2)

Draw a line from (x1, y1) to (x2, y2).
  Parameters: x1 - x of first point. y1 - y of first point. x2 - x of second point. y2 - y of second point.
### fillRect

void fillRect(int x, int y, int width, int height)

Fill a rect with (x,y) top-left corner.
  Parameters: x - The x coordinate. y - The y coordinate. width - The rect width. height - The rect height.
### fillRect

void fillRect([Rectangle](Rectangle.md) rectangle)

Fill a rectangle.
  Parameters: rectangle - The rectangle.
### drawRect

void drawRect(int x, int y, int width, int height)

Draw a rect with (x,y) top-left corner.
  Parameters: x - The x coordinate. y - The y coordinate. width - The rect width. height - The rect height.
### drawRoundRect

void drawRoundRect(int x, int y, int width, int height, int arcWidth, int arcHeight)

Draws an outlined round-cornered rectangle using this graphics context's current color. The left and right edges of the rectangle are at x and x + width, respectively. The top and bottom edges of the rectangle are at y and y + height.
  Parameters: x - the *x* coordinate of the rectangle to be drawn. y - the *y* coordinate of the rectangle to be drawn. width - the width of the rectangle to be drawn. height - the height of the rectangle to be drawn. arcWidth - the horizontal diameter of the arc at the four corners. arcHeight - the vertical diameter of the arc at the four corners.
### fillRoundRect

void fillRoundRect(int x, int y, int width, int height, int arcWidth, int arcHeight)

Fills the specified rounded corner rectangle.
  Parameters: x - the *x* coordinate of the rectangle to be filled. y - the *y* coordinate of the rectangle to be filled. width - the width of the rectangle to be filled. height - the height of the rectangle to be filled. arcWidth - the horizontal diameter of the arc at the four corners. arcHeight - the vertical diameter of the arc at the four corners.
### drawPolyline

void drawPolyline(int[] xpoints, int[] ypoints, int npoints)

Draws a polyline which is not closed if the last point differs from the first.
  Parameters: xpoints - The xpoints array. ypoints - The ypoints array. npoints - The number of points.
### drawArc

void drawArc(int x, int y, int width, int height, int startAngle, int arcAngle)

draws an arc.
  Parameters: x - the *x* coordinate of the upper-left corner of the arc to be drawn. y - the *y* coordinate of the upper-left corner of the arc to be drawn. width - the width of the arc to be drawn. height - the height of the arc to be drawn. startAngle - the beginning angle. arcAngle - the angular extent of the arc, relative to the start angle.
### fillArc

void fillArc(int x, int y, int width, int height, int startAngle, int arcAngle)

Fills an arc.
  Parameters: x - the *x* coordinate of the upper-left corner of the arc to be drawn. y - the *y* coordinate of the upper-left corner of the arc to be drawn. width - the width of the arc to be drawn. height - the height of the arc to be drawn. startAngle - the beginning angle. arcAngle - the angular extent of the arc, relative to the start angle.
### setStroke

void setStroke(int width, int type)

Sets the line width for the stroke. The line is solid, no dashes.
  Parameters: width - The width value. type - The stroke type.
### getStrokeWidth

int getStrokeWidth()
  Returns: the value of the stroke width.
### getStrokeType

int getStrokeType()
  Returns: the value of the stroke type.
### getClipBounds

[Rectangle](Rectangle.md) getClipBounds()
  Returns: the clipping rectangle.
### setClipBounds

void setClipBounds([Rectangle](Rectangle.md) clip)

Set cliping for the graphics.
  Parameters: clip - The clip bounds to be set.
### setFillColor

void setFillColor([Color](Color.md) colorCode)

Set the color for fill methods.
  Parameters: colorCode - The color code used by fill methods.
### setDrawColor

void setDrawColor([Color](Color.md) colorCode)

Set the color for draw methods.
  Parameters: colorCode - The color code used by draw methods.
### drawIcon

void drawIcon([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) hostComponent, int iconCode, int x, int y)

Draw the icon at (x,y) coordinates.
  Parameters: hostComponent - Icon implementations may use the HostComponent argument to get properties useful for painting, e.g. the foreground or background color. iconCode - The icon code. x - The x coordinate. y - The y coordinate.
### drawOval

void drawOval(int x, int y, int width, int height)

Draw an oval.
  Parameters: x - The x coordinate. y - The y coordinate. width - The width. height - The height.
### getFillColor

[Color](Color.md) getFillColor()

Get the color code for fill shapes.
  Returns: The color code for fill shapes.
### fillOval

void fillOval(int x, int y, int width, int height)

Fill an oval with curent fill color.
  Parameters: x - The x coordinate. y - The y coordinate. width - The width. height - The height.
### fillWithGradient

void fillWithGradient([Rectangle](Rectangle.md) rect, [Color](Color.md) startColorCode, [Color](Color.md) endColorCode, boolean isVertical)
  Parameters: rect - The rect to fill with a gradient startColorCode - Start color of gradient endColorCode - End color of gradient. isVertical - True if the gradient should be vertical.
### fillWithGradient

void fillWithGradient([Polygon](Polygon.md) polygon, [Color](Color.md) startColorCode, [Color](Color.md) endColorCode, boolean isVertical)
  Parameters: polygon - The polygon to fill with a gradient startColorCode - Start color of gradient endColorCode - End color of gradient. isVertical - True if the gradient should be vertical.
### fillShape

void fillShape([Shape](Shape.md) shape)

Fill a shape
  Parameters: shape - The shape
### drawShape

void drawShape([Shape](Shape.md) shape)

Draw a shape
  Parameters: shape - The shape
### getFontMetrics

[FontMetrics](FontMetrics.md) getFontMetrics([Font](Font.md) font)
  Parameters: font - The font Returns: The font metrics
### deriveStyle

[Font](Font.md) deriveStyle([Font](Font.md) current, int style)

Derive the style of the font
  Parameters: current - Current font style - New style Returns: The new font
### deriveSize

[Font](Font.md) deriveSize([Font](Font.md) current, int size)

Derive the size of the font
  Parameters: current - Current font size - New size Returns: The new font
### drawImage

void drawImage([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) image, int x, int y)

Draw an image object depending on the platform
  Parameters: image - The image data x - image X y - image Y
### drawImage

void drawImage([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) image, int x, int y, int width, int height)

Draw an image object depending on the platform. The image is scaled to the width and height specified.
  Parameters: image - The image data x - image X y - image Y width - image width height - image height
### drawImage

void drawImage([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) img, int dx1, int dy1, int dx2, int dy2, int sx1, int sy1, int sx2, int sy2)

Draws as much of the specified area of the specified image as is currently available, scaling it on the fly to fit inside the specified area of the destination drawable surface. Transparent pixels do not affect whatever pixels are already there.
  Parameters: img - the specified image to be drawn. This method does nothing if img is null. dx1 - the *x* coordinate of the first corner of the destination rectangle. dy1 - the *y* coordinate of the first corner of the destination rectangle. dx2 - the *x* coordinate of the second corner of the destination rectangle. dy2 - the *y* coordinate of the second corner of the destination rectangle. sx1 - the *x* coordinate of the first corner of the source rectangle. sy1 - the *y* coordinate of the first corner of the source rectangle. sx2 - the *x* coordinate of the second corner of the source rectangle. sy2 - the *y* coordinate of the second corner of the source rectangle. Since: 14.0
### fillRect

void fillRect(int x, int y, int width, int height, int fillPattern, [Color](Color.md) fillColor)

Fills a rectangle with a pattern.
  Parameters: x - The left corner x coordinate. y - The left corner y coordinate width - The width of the rectangle. height - The hight of the rectangle. fillPattern - One this class constants that begin with FILL_PATTERN_ fillColor - The color for building the pattern.
### drawShadow

void drawShadow([Shape](Shape.md) shape, int displacement)

Draws a shadow using the shape of the polygon. The shadow will move to the right and down, with the size of the shadow.
  Parameters: shape - The shape of the real object. displacement - The size of the shadow. This is the displacement to the original object, on X and Y.
### fillWithGradient

void fillWithGradient([Ellipse](Ellipse.md) ellipse, [Color](Color.md) startColorCode, [Color](Color.md) endColorCode, boolean isVertical)
  Parameters: ellipse - The ellipse to fill with a gradient startColorCode - Start color of gradient endColorCode - End color of gradient. isVertical - True if the gradient should be vertical.
### fillWithGradient

void fillWithGradient([Shape](Shape.md) shape, [Color](Color.md) startColorCode, [Color](Color.md) endColorCode, boolean isVertical)
  Parameters: shape - The shape to fill with a gradient startColorCode - Start color of gradient endColorCode - End color of gradient. isVertical - True if the gradient should be vertical.
### setAntialiasing

void setAntialiasing([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)
  Parameters: value - The antialising value to be set depending on the platform.
### getAntialiasing

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getAntialiasing()
  Returns: The antialising value to be set depending on the platform.
### activateAntialiasing

void activateAntialiasing()

Activate the antialiasing mode.

### disableAntialiasing

void disableAntialiasing()

Disable the antialiasing mode.

### drawWrappedString

void drawWrappedString([AttributedString](AttributedString.md) aStr, int x, int y, int wrappingWidth, boolean drawAtBaseLine)

Draws a string at the specified coordinates. Takes into account the wrapping width and newline characters.
  Parameters: aStr - The text, as an attributed string. x - The x coordinate. y - The y coordinate. wrappingWidth - The maximum width of the wrapped text. drawAtBaseLine - true if we should draw directly at the specified Y
### drawWrappedString

void drawWrappedString([AttributedString](AttributedString.md) aStr, int x, int y, int wrappingWidth)

Draws a string at the specified coordinates. Takes into account the wrapping width and newline characters.
  Parameters: aStr - The text, as an attributed string. x - The x coordinate. y - The y coordinate. wrappingWidth - The maximum width of the wrapped text.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
