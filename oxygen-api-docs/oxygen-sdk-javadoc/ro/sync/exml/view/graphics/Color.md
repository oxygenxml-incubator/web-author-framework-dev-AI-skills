Package [ro.sync.exml.view.graphics](package-summary.md)

# Class Color

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.view.graphics.Color
   @API(type=EXTENDABLE, src=PRIVATE) public class Color extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The class used to represent a Color. WARNING: This class is immutable. Its values are sometimes cached in class StyleSheet.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [ALPHA_CHANNEL_DEFAULT_VALUE](#ALPHA_CHANNEL_DEFAULT_VALUE)
Default value for the alpha channel, when not specified.Fully opaque color.
  static final [Color](Color.md) [COLOR_AUTOCORRECT_HIGHLIGHT_YELLOW_FOR_DARK_THEME](#COLOR_AUTOCORRECT_HIGHLIGHT_YELLOW_FOR_DARK_THEME)
The AutoCorrect highlight color.
  static final [Color](Color.md) [COLOR_BLACK](#COLOR_BLACK)
Black color constant.
  static final [Color](Color.md) [COLOR_BLACK_ALPHA](#COLOR_BLACK_ALPHA)
Black color with alpha constant.
  static final [Color](Color.md) [COLOR_BLUE](#COLOR_BLUE)
Blue color constant.
  static final [Color](Color.md) [COLOR_DARK_GRAY](#COLOR_DARK_GRAY)
Dark gray color constant.
  static final [Color](Color.md) [COLOR_DARK_GREEN](#COLOR_DARK_GREEN)
Darker green color constant.
  static final [Color](Color.md) [COLOR_DARK_YELLOW](#COLOR_DARK_YELLOW)
A dark yellow color.
  static final [Color](Color.md) [COLOR_GRAY](#COLOR_GRAY)
Gray color constant.
  static final [Color](Color.md) [COLOR_LIGHT_GRAY](#COLOR_LIGHT_GRAY)
Light gray color constant.
  static final [Color](Color.md) [COLOR_LIGHT_GRAY_ALPHA](#COLOR_LIGHT_GRAY_ALPHA)
Gray with alpha color constant.
  static final [Color](Color.md) [COLOR_LIGHT_GREEN](#COLOR_LIGHT_GREEN)
Light green color constant.
  static final [Color](Color.md) [COLOR_LIGHT_YELLOW](#COLOR_LIGHT_YELLOW)
Light yellow color constant.
  static final [Color](Color.md) [COLOR_LIGHTER_BLUE](#COLOR_LIGHTER_BLUE)
Lighter blue color constant.
  static final [Color](Color.md) [COLOR_LIGHTER_GRAY](#COLOR_LIGHTER_GRAY)
Lighter gray color constant.
  static final [Color](Color.md) [COLOR_ORANGE](#COLOR_ORANGE)
Orange color constant.
  static final [Color](Color.md) [COLOR_PASTE_HIGHLIGHT_YELLOW](#COLOR_PASTE_HIGHLIGHT_YELLOW)
The paste highlight color.
  static final [Color](Color.md) [COLOR_RED](#COLOR_RED)
Red color constant.
  static final [Color](Color.md) [COLOR_RED_DARKER](#COLOR_RED_DARKER)
Red darker color constant.
  static final [Color](Color.md) [COLOR_TRANSPARENT](#COLOR_TRANSPARENT)
A transparent color.
  static final [Color](Color.md) [COLOR_WHITE](#COLOR_WHITE)
White color constant.
  static final [Color](Color.md) [COLOR_WHITE_ALPHA](#COLOR_WHITE_ALPHA)
Light gray with alpha color constant.
  static final [Color](Color.md) [COLOR_YELLOW](#COLOR_YELLOW)
A yellow color.

## Constructor Summary
 Constructors
Constructor

Description
 [Color](#%3Cinit%3E(int))(int rgba)
Creates an sRGB color from the specified RGBa color value.
  [Color](#%3Cinit%3E(int%5B%5D))(int[] rgba)
Creates a color from a given RGBa array.
  [Color](#%3Cinit%3E(int,int,int))(int r, int g, int b)
Creates an opaque sRGB color with the specified red, green, and blue values in the range [0 - 255].
  [Color](#%3Cinit%3E(int,int,int,int))(int r, int g, int b, int a)
Creates an sRGB color with the specified red, green, blue, and alpha values in the range [0 - 255].

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static [Color](Color.md) [alphaComposite](#alphaComposite(ro.sync.exml.view.graphics.Color,ro.sync.exml.view.graphics.Color))([Color](Color.md) color, [Color](Color.md) background)
Used to simulate an alpha composition between a color and a background color.
  static [Color](Color.md) [brighter](#brighter(ro.sync.exml.view.graphics.Color))([Color](Color.md) color)
Increase brightness of the color.
  static int [changeBrightnessAndSaturation](#changeBrightnessAndSaturation(int,float,float))(int rgba, float brightness, float saturation)
Change brightness and saturation of the color.
  static [Color](Color.md) [darker](#darker(ro.sync.exml.view.graphics.Color))([Color](Color.md) color)
Decrease the brightness of the color.
  static [Color](Color.md) [darker](#darker(ro.sync.exml.view.graphics.Color,float))([Color](Color.md) color, float percent)
Decrease the brightness of the color.
  static [Color](Color.md) [decodeColor](#decodeColor(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colorString)
Method used to decode the given string to a color.
  static [Color](Color.md) [desaturate](#desaturate(ro.sync.exml.view.graphics.Color,double))([Color](Color.md) fillColor, double percent)
Used for decrease the color saturation with the given percent.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
Checks if the two colors have the same RGB value.
  int [getAlpha](#getAlpha())()
Returns the alpha component in the range 0-255.
  int [getBlue](#getBlue())()
Returns the blue component in the range 0-255 in the default sRGB space.
  float [getBrightness](#getBrightness())()
Gets the L component form the HSL spectrum of the color.
  int [getGreen](#getGreen())()
Returns the green component in the range 0-255 in the default sRGB space.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHexColor](#getHexColor(ro.sync.exml.view.graphics.Color))([Color](Color.md) color)
Get the hexadecimal value for the given color.
  int [getRed](#getRed())()
Returns the red component in the range 0-255 in the default sRGB space.
  int [getRGB](#getRGB())()
Returns the RGB value representing the color in the default sRGB (Bits 24-31 are alpha, 16-23 are red, 8-15 are green, 0-7 are blue).
  static int [getRGB](#getRGB(int,int,int,int))(int red, int green, int blue, int alpha)
Gets the RGBa value for a color.
  int [hashCode](#hashCode())()

 static int [HSBtoRGB](#HSBtoRGB(float,float,float,int))(float hue, float saturation, float brightness, int alpha)
Converts the components of a color, as specified by the HSB model, to an equivalent set of values for the default RGB model.
  static [Color](Color.md) [hslToColor](#hslToColor(float,float,float,int))(float H, float S, float L, int alpha)
HSL color space to RGB convert method.
  static [Color](Color.md) [hslToRGB](#hslToRGB(float,float,float))(float H, float S, float L)
HSL color space to RGB convert method.
  static int [normalize](#normalize(int))(int value)
Normalizes a value according to the range of values a sRGB color component can have - [0-255].
  static [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Color](Color.md)> [parseColor](#parseColor(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colorString)
Parses a RGBa color's [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) representation to create a [Color](Color.md) from it.
  static float[] [RGBtoHSB](#RGBtoHSB(int,int,int,float%5B%5D))(int r, int g, int b, float[] hsbvals)
Converts the components of a color, as specified by the default RGB model, to an equivalent set of values for hue, saturation, and brightness that are the three components of the HSB model.
  static float[] [rgbTohsl](#rgbTohsl(int,int,int))(int r, int g, int b)
RGB to HSl space convert method.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()
Returns a string representation of this Color.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### COLOR_WHITE_ALPHA

public static final [Color](Color.md) COLOR_WHITE_ALPHA

Light gray with alpha color constant. The RGB values are: (192, 192, 192, 128).

### COLOR_LIGHT_GRAY

public static final [Color](Color.md) COLOR_LIGHT_GRAY

Light gray color constant. The RGB values are: (192, 192, 192).

### COLOR_LIGHT_GRAY_ALPHA

public static final [Color](Color.md) COLOR_LIGHT_GRAY_ALPHA

Gray with alpha color constant. The RGB values are: (192, 192, 192, 50).

### COLOR_WHITE

public static final [Color](Color.md) COLOR_WHITE

White color constant. The RGB values are: (255, 255, 255).

### COLOR_BLACK

public static final [Color](Color.md) COLOR_BLACK

Black color constant. The RGB values are: (0, 0, 0).

### COLOR_BLACK_ALPHA

public static final [Color](Color.md) COLOR_BLACK_ALPHA

Black color with alpha constant. The RGB values are: (0, 0, 0, 40).

### COLOR_RED

public static final [Color](Color.md) COLOR_RED

Red color constant. The RGB values are: (255, 0, 0).

### COLOR_RED_DARKER

public static final [Color](Color.md) COLOR_RED_DARKER

Red darker color constant. The RGB values are: (178, 0, 0).

### COLOR_DARK_GRAY

public static final [Color](Color.md) COLOR_DARK_GRAY

Dark gray color constant. The RGB values are: (64, 64, 64).

### COLOR_BLUE

public static final [Color](Color.md) COLOR_BLUE

Blue color constant. The RGB values are: (0, 0, 255).

### COLOR_GRAY

public static final [Color](Color.md) COLOR_GRAY

Gray color constant. The RGB values are: (128, 128, 128).

### COLOR_LIGHT_GREEN

public static final [Color](Color.md) COLOR_LIGHT_GREEN

Light green color constant. The RGB values are: (230, 255, 230).

### COLOR_ORANGE

public static final [Color](Color.md) COLOR_ORANGE

Orange color constant. The RGB values are: (255, 200, 0).

### COLOR_LIGHTER_GRAY

public static final [Color](Color.md) COLOR_LIGHTER_GRAY

Lighter gray color constant. The RGB values are: (240, 240, 240).

### COLOR_LIGHTER_BLUE

public static final [Color](Color.md) COLOR_LIGHTER_BLUE

Lighter blue color constant. The RGB values are: (247, 250, 252).

### COLOR_DARK_GREEN

public static final [Color](Color.md) COLOR_DARK_GREEN

Darker green color constant. The RGB values are: (0, 128, 0).

### COLOR_LIGHT_YELLOW

public static final [Color](Color.md) COLOR_LIGHT_YELLOW

Light yellow color constant. The RGB values are: (255, 255, 230).

### COLOR_YELLOW

public static final [Color](Color.md) COLOR_YELLOW

A yellow color.

### COLOR_DARK_YELLOW

public static final [Color](Color.md) COLOR_DARK_YELLOW

A dark yellow color.

### COLOR_PASTE_HIGHLIGHT_YELLOW

public static final [Color](Color.md) COLOR_PASTE_HIGHLIGHT_YELLOW

The paste highlight color.

### COLOR_AUTOCORRECT_HIGHLIGHT_YELLOW_FOR_DARK_THEME

public static final [Color](Color.md) COLOR_AUTOCORRECT_HIGHLIGHT_YELLOW_FOR_DARK_THEME

The AutoCorrect highlight color.

### COLOR_TRANSPARENT

public static final [Color](Color.md) COLOR_TRANSPARENT

A transparent color.

### ALPHA_CHANNEL_DEFAULT_VALUE

public static final int ALPHA_CHANNEL_DEFAULT_VALUE

Default value for the alpha channel, when not specified.Fully opaque color.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Color.ALPHA_CHANNEL_DEFAULT_VALUE)

## Constructor Details

### Color

public Color(int r, int g, int b, int a)

Creates an sRGB color with the specified red, green, blue, and alpha values in the range [0 - 255].
  Parameters: r - the red component. g - the green component. b - the blue component. a - the alpha component.
### Color

public Color(int rgba)

Creates an sRGB color from the specified RGBa color value.
  Parameters: rgba - The value of the RGBa color. Bits 24-31 are alpha, 16-23 are red, 8-15 are green, 0-7 are blue.
### Color

public Color(int[] rgba)

Creates a color from a given RGBa array.
  Parameters: rgba - A color's RGBa components. The alpha channel can be missing, will default to 255 (fully opaque color).
### Color

public Color(int r, int g, int b)

Creates an opaque sRGB color with the specified red, green, and blue values in the range [0 - 255]. The actual color used in rendering depends on finding the best match given the color space available for a given output device. Alpha is defaulted to 255.
  Parameters: r - the red component. g - the green component. b - the blue component.
## Method Details

### normalize

public static int normalize(int value)

Normalizes a value according to the range of values a sRGB color component can have - [0-255].
  Parameters: value - The value to be checked and normalized. Returns: The same value, if value is in the [0-255] range. 0 if value is < 0. 255 if value is > 255.
### getRGB

public static int getRGB(int red, int green, int blue, int alpha)

Gets the RGBa value for a color.
  Parameters: red - Red value. green - Green value. blue - Blue value alpha - Alpha value. Returns: The representation of the given values as an int.
### getRed

public int getRed()

Returns the red component in the range 0-255 in the default sRGB space.
  Returns: The red component.
### getGreen

public int getGreen()

Returns the green component in the range 0-255 in the default sRGB space.
  Returns: The green component.
### getBlue

public int getBlue()

Returns the blue component in the range 0-255 in the default sRGB space.
  Returns: The blue component.
### getAlpha

public int getAlpha()

Returns the alpha component in the range 0-255.
  Returns: The alpha component.
### getRGB

public int getRGB()

Returns the RGB value representing the color in the default sRGB (Bits 24-31 are alpha, 16-23 are red, 8-15 are green, 0-7 are blue).
  Returns: the RGB value of the color in the default sRGB ColorModel.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()

Returns a string representation of this Color. This method is intended to be used only for debugging purposes. The content and format of the returned string might vary between implementations. The returned string might be empty but cannot be null.
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Returns: A string representation of this Color.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

Checks if the two colors have the same RGB value. The alpha is also taken into account.
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### desaturate

public static [Color](Color.md) desaturate([Color](Color.md) fillColor, double percent)

Used for decrease the color saturation with the given percent.
  Parameters: fillColor - The color to be darkened. percent - The percent to be used for decrease the color saturation. Returns: The modified color.
### alphaComposite

public static [Color](Color.md) alphaComposite([Color](Color.md) color, [Color](Color.md) background)

Used to simulate an alpha composition between a color and a background color.
  Parameters: color - The transparent color. background - The background color. Returns: The resulted color. See Also:
        * "http://en.wikipedia.org/wiki/Alpha_compositing"

### decodeColor

public static [Color](Color.md) decodeColor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colorString)

Method used to decode the given string to a color.
  Parameters: colorString - The string representation of the color. Returns: The decoded color if possible, black otherwise.
### parseColor

public static [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Color](Color.md)> parseColor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colorString)throws ro.sync.basic.util.NumberFormatException

Parses a RGBa color's [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) representation to create a [Color](Color.md) from it.
  Parameters: colorString - A RGBa color's String representation. Returns: The corresponding Color.Can be null if colorString is null, the empty string, or it cannot be properly tokenized to identify the 3 or 4 components of a RGBa color (red, green and blue channels; alpha channel is optional). Throws: ro.sync.basic.util.NumberFormatException - If invalid values for color channels R, G, B or alpha. See Also:
        * [normalize(int)](#normalize(int))

### rgbTohsl

public static float[] rgbTohsl(int r, int g, int b)

RGB to HSl space convert method. Copied from: http://www.easyrgb.com/math.php?MATH=M19#text19
  Parameters: r - Red (0 -> 255) g - Green (0 -> 255) b - Blue (0 -> 255) Returns: The HSL array of values between 0.0f and 1.0f
### hslToColor

public static [Color](Color.md) hslToColor(float H, float S, float L, int alpha)

HSL color space to RGB convert method. Copied from: http://www.easyrgb.com/math.php?MATH=M19#text19
  Parameters: H - (between 0.0 and 1.0) S - (between 0.0 and 1.0) L - (between 0.0 and 1.0) alpha - The alpha tone. Returns: The RGB color.
### hslToRGB

public static [Color](Color.md) hslToRGB(float H, float S, float L)

HSL color space to RGB convert method. Copied from: http://www.easyrgb.com/math.php?MATH=M19#text19
  Parameters: H - (between 0.0 and 1.0) S - (between 0.0 and 1.0) L - (between 0.0 and 1.0) Returns: The RGB color.
### darker

public static [Color](Color.md) darker([Color](Color.md) color)

Decrease the brightness of the color.
  Parameters: color - The color to be modified. Returns: The color with decreased brightness.
### darker

public static [Color](Color.md) darker([Color](Color.md) color, float percent)

Decrease the brightness of the color.
  Parameters: color - The color to be modified. percent - The percent to be used for darkening a color. Returns: The color with decreased brightness.
### brighter

public static [Color](Color.md) brighter([Color](Color.md) color)

Increase brightness of the color.
  Parameters: color - The color to be modified. Returns: The color with increased brightness.
### getBrightness

public float getBrightness()

Gets the L component form the HSL spectrum of the color.
  Returns: The brightness of the color. Between 0.0 and 1.0
### getHexColor

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHexColor([Color](Color.md) color)

Get the hexadecimal value for the given color.
  Parameters: color - The color to compute HEX value, Returns: The hexadecimal value for the given color.
### changeBrightnessAndSaturation

public static int changeBrightnessAndSaturation(int rgba, float brightness, float saturation)

Change brightness and saturation of the color.
  Parameters: rgba - The color to be modified. brightness - The factor for changing the brightness. saturation - The factor for changing the saturation. Returns: The modified color.
### RGBtoHSB

public static float[] RGBtoHSB(int r, int g, int b, float[] hsbvals)

Converts the components of a color, as specified by the default RGB model, to an equivalent set of values for hue, saturation, and brightness that are the three components of the HSB model.
If the hsbvals argument is null, then a new array is allocated to return the result. Otherwise, the method returns the array hsbvals, with the values put into that array. Copied from [Color.RGBtoHSB(int, int, int, float[])](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Color.html#RGBtoHSB(int,int,int,float%5B%5D))

  Parameters: r - the red component of the color g - the green component of the color b - the blue component of the color hsbvals - the array used to return the three HSB values, or null Returns: an array of three elements containing the hue, saturation, and brightness (in that order), of the color with the indicated red, green, and blue components. See Also:
        * [Color.getRGB()](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Color.html#getRGB())
        * [Color(int)](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Color.html#%3Cinit%3E(int))
        * [ColorModel.getRGBdefault()](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/image/ColorModel.html#getRGBdefault())

### HSBtoRGB

public static int HSBtoRGB(float hue, float saturation, float brightness, int alpha)

Converts the components of a color, as specified by the HSB model, to an equivalent set of values for the default RGB model.
The saturation and brightness components should be floating-point values between zero and one (numbers in the range 0.0-1.0). The hue component can be any floating-point number. The floor of this number is subtracted from it to create a fraction between 0 and 1. This fractional number is then multiplied by 360 to produce the hue angle in the HSB color model.

The integer that is returned by HSBtoRGB encodes the value of a color in bits 0-23 of an integer value that is the same format used by the method [getRGB](#getRGB()). This integer can be supplied as an argument to the Color constructor that takes a single integer argument. Copied from [Color.HSBtoRGB(float, float, float)](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Color.html#HSBtoRGB(float,float,float))

  Parameters: hue - the hue component of the color saturation - the saturation of the color brightness - the brightness of the color alpha - the alpha level. Returns: the RGB value of the color with the indicated hue, saturation, and brightness. See Also:
        * [Color.getRGB()](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Color.html#getRGB())
        * [Color(int)](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Color.html#%3Cinit%3E(int))
        * [ColorModel.getRGBdefault()](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/image/ColorModel.html#getRGBdefault())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
