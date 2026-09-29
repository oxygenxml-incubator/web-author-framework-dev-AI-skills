Package [ro.sync.exml.view.graphics](package-summary.md)

# Class Font

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.view.graphics.Font
   @API(type=EXTENDABLE, src=PRIVATE) public class Font extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Font common class.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [BOLD](#BOLD)
The bold style constant.
  static final int [ITALIC](#ITALIC)
The italicized style constant.
  static final int [PLAIN](#PLAIN)
The plain style constant.

## Constructor Summary
 Constructors
Constructor

Description
 [Font](#%3Cinit%3E(java.lang.String,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int style, int size)
Creates a new Font from the specified name, style and point size.
  [Font](#%3Cinit%3E(java.lang.String,int,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int style, int size, int letterSpacing)
Creates a new Font from the specified name, style and point size.
  [Font](#%3Cinit%3E(java.lang.String,int,int,int,java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int style, int size, int letterSpacing, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] fontFamilies)
Creates a new Font from the specified name, style and point size.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static [Font](Font.md) [decodeFont](#decodeFont(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Decodes a font property value, having the format "name,style,size"
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [encodeFont](#encodeFont(ro.sync.exml.view.graphics.Font))([Font](Font.md) font)
Encodes a font as: "name,style,size"
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
Checks if the two colors have the same RGB value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getFontNames](#getFontNames())()
Get the array of font names.
  int [getLetterSpacing](#getLetterSpacing())()
Get the letter spacing.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()

 int [getSize](#getSize())()

 int [getStyle](#getStyle())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [hash](#hash())()

 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [hash](#hash(java.lang.String%5B%5D,int,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] fontNames, int style, int size, int letterSpacing)
Hash the font
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [hash](#hash(java.lang.String,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int style, int size)
Hash the font
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [hash](#hash(java.lang.String,int,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fontFamily, int style, int size, int letterSpacing)
Hash the font
  int [hashCode](#hashCode())()

 boolean [isBold](#isBold())()
Indicates whether or not this Font object's style is BOLD.
  boolean [isItalic](#isItalic())()
Indicates whether or not this Font object's style is ITALIC.
  boolean [isPlain](#isPlain())()
Indicates whether or not this Font object's style is PLAIN.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()
Converts this Font object to a Stringrepresentation.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### PLAIN

public static final int PLAIN

The plain style constant.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Font.PLAIN)

### BOLD

public static final int BOLD

The bold style constant. This can be combined with the other style constants (except PLAIN) for mixed styles.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Font.BOLD)

### ITALIC

public static final int ITALIC

The italicized style constant. This can be combined with the other style constants (except PLAIN) for mixed styles.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.view.graphics.Font.ITALIC)

## Constructor Details

### Font

public Font([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int style, int size)

Creates a new Font from the specified name, style and point size.
  Parameters: name - the font name. This can be a logical font name or a font face name. A logical name must be either: Dialog, DialogInput, Monospaced, Serif, or SansSerif. If name is null, the name of the new Font is set to the name "Default". style - the style constant for the FontThe style argument is an integer bitmask that may be PLAIN, or a bitwise union of BOLD and/or ITALIC (for example, ITALIC or BOLD|ITALIC). size - the point size of the Font
### Font

public Font([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int style, int size, int letterSpacing)

Creates a new Font from the specified name, style and point size.
  Parameters: name - the font name. This can be a logical font name or a font face name. A logical name must be either: Dialog, DialogInput, Monospaced, Serif, or SansSerif. If name is null, the name of the new Font is set to the name "Default". style - the style constant for the FontThe style argument is an integer bitmask that may be PLAIN, or a bitwise union of BOLD and/or ITALIC (for example, ITALIC or BOLD|ITALIC). size - the point size of the Font letterSpacing - MThe amount of advance pixels. Default is "0".
### Font

public Font([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int style, int size, int letterSpacing, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] fontFamilies)

Creates a new Font from the specified name, style and point size.
  Parameters: name - the font name. This can be a logical font name or a font face name. A logical name must be either: Dialog, DialogInput, Monospaced, Serif, or SansSerif. If name is null, the name of the new Font is set to the name "Default". style - the style constant for the FontThe style argument is an integer bitmask that may be PLAIN, or a bitwise union of BOLD and/or ITALIC (for example, ITALIC or BOLD|ITALIC). size - the point size of the Font letterSpacing - MThe amount of advance pixels. Default is "0". fontFamilies - The array of font families. The first entry from the array should be the same as the name parameter (the main font family name). The next entries are fallback family names, used when the main font does not support all the glyphs. This is cloned, for immutability.
## Method Details

### getName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()
  Returns: The name
### getSize

public int getSize()
  Returns: The size
### getStyle

public int getStyle()
  Returns: The style
### getLetterSpacing

public int getLetterSpacing()

Get the letter spacing.
  Returns: Returns the letterSpacing.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()

Converts this Font object to a Stringrepresentation.
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Returns: a String representation of this Font object.
### isPlain

public boolean isPlain()

Indicates whether or not this Font object's style is PLAIN.
  Returns: true if this Font has a PLAIN sytle; false otherwise. See Also:
        * [Font.getStyle()](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Font.html#getStyle())

### isBold

public boolean isBold()

Indicates whether or not this Font object's style is BOLD.
  Returns: true if this Font object's style is BOLD; false otherwise. See Also:
        * [Font.getStyle()](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Font.html#getStyle())

### isItalic

public boolean isItalic()

Indicates whether or not this Font object's style is ITALIC.
  Returns: true if this Font object's style is ITALIC; false otherwise. See Also:
        * [Font.getStyle()](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Font.html#getStyle())

### hash

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hash()
  Returns: A hash of the font
### hash

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hash([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int style, int size)

Hash the font
  Parameters: name - The the font main family one style - Style size - Size Returns: The hash
### hash

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hash([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fontFamily, int style, int size, int letterSpacing)

Hash the font
  Parameters: fontFamily - The the font main family one style - Style size - Size letterSpacing - Letter spacing in pixels Returns: The hash
### hash

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hash([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] fontNames, int style, int size, int letterSpacing)

Hash the font
  Parameters: fontNames - The list of font names, the main one and the fallback ones. style - Style size - Size letterSpacing - Letter spacing in pixels Returns: The hash
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

Checks if the two colors have the same RGB value. The alpha is also taken into account.
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### encodeFont

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) encodeFont([Font](Font.md) font)

Encodes a font as: "name,style,size"
  Parameters: font - The font to be encoded. Returns: The encoded value.
### decodeFont

public static [Font](Font.md) decodeFont([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Decodes a font property value, having the format "name,style,size"
  Parameters: value - The value to be decoded. Returns: The font.
### getFontNames

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getFontNames()

Get the array of font names. The first entry from the array should be the same as the name parameter (the main font family name). The next entries are fallback family names, used when the main font does not support all the glyphs.
  Returns: The entire list of font names, including the main one (on the first position), and the fallback ones.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
