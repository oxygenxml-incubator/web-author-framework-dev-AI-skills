Package [ro.sync.exml.plugin.workspace.security](package-summary.md)

# Enum Class CspDirective

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[CspDirective](CspDirective.md)>
        * ro.sync.exml.plugin.workspace.security.CspDirective
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[CspDirective](CspDirective.md)>, [Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public enum CspDirective extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[CspDirective](CspDirective.md)>
Enum for Content Security Policy (CSP) directives. These directives control various resource types that can be loaded or executed in the context of a web page.
  Since: 26.1.1  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.
 See Also:
* [Content-Security-Policy directives](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Security-Policy#directives)

## Nested Class Summary

## Nested classes/interfaces inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [Enum.EnumDesc](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html) extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)>>
## Enum Constant Summary
 Enum Constants
Enum Constant

Description
 [CONNECT_SRC](#CONNECT_SRC)
Specifies valid sources for AJAX, WebSockets, and EventSource.
  [DEFAULT_SRC](#DEFAULT_SRC)
Defines the default policy for fetching resources such as JavaScript, Images, CSS, Fonts, AJAX requests, Frames, HTML5 Media.
  [FONT_SRC](#FONT_SRC)
Specifies valid sources for fonts loaded using font-face.
  [FRAME_SRC](#FRAME_SRC)
Specifies valid sources for <iframe> and <frame> elements.
  [IMG_SRC](#IMG_SRC)
Specifies valid sources of images.
  [MEDIA_SRC](#MEDIA_SRC)
Specifies valid sources of audio and video.
  [OBJECT_SRC](#OBJECT_SRC)
Specifies valid sources for the <object>, <embed>, and <applet> elements.
  [SANDBOX](#SANDBOX)
Applies extra restrictions to the content security policy of the page.
  [SCRIPT_SRC](#SCRIPT_SRC)
Specifies valid sources for JavaScript.
  [STYLE_SRC](#STYLE_SRC)
Specifies valid sources for stylesheets.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [CspDirective](CspDirective.md) [valueOf](#valueOf(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the enum constant of this class with the specified name.
  static [CspDirective](CspDirective.md)[] [values](#values())()
Returns an array containing the constants of this enum class, in the order they are declared.

### Methods inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#clone()), [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#compareTo(E)), [describeConstable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#describeConstable()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#finalize()), [getDeclaringClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#getDeclaringClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#hashCode()), [name](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#name()), [ordinal](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#ordinal()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#toString()), [valueOf](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#valueOf(java.lang.Class,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Enum Constant Details

### DEFAULT_SRC

public static final [CspDirective](CspDirective.md) DEFAULT_SRC

Defines the default policy for fetching resources such as JavaScript, Images, CSS, Fonts, AJAX requests, Frames, HTML5 Media.

### SCRIPT_SRC

public static final [CspDirective](CspDirective.md) SCRIPT_SRC

Specifies valid sources for JavaScript.

### STYLE_SRC

public static final [CspDirective](CspDirective.md) STYLE_SRC

Specifies valid sources for stylesheets.

### IMG_SRC

public static final [CspDirective](CspDirective.md) IMG_SRC

Specifies valid sources of images.

### CONNECT_SRC

public static final [CspDirective](CspDirective.md) CONNECT_SRC

Specifies valid sources for AJAX, WebSockets, and EventSource.

### FONT_SRC

public static final [CspDirective](CspDirective.md) FONT_SRC

Specifies valid sources for fonts loaded using font-face.

### OBJECT_SRC

public static final [CspDirective](CspDirective.md) OBJECT_SRC

Specifies valid sources for the <object>, <embed>, and <applet> elements.

### MEDIA_SRC

public static final [CspDirective](CspDirective.md) MEDIA_SRC

Specifies valid sources of audio and video.

### FRAME_SRC

public static final [CspDirective](CspDirective.md) FRAME_SRC

Specifies valid sources for <iframe> and <frame> elements.

### SANDBOX

public static final [CspDirective](CspDirective.md) SANDBOX

Applies extra restrictions to the content security policy of the page. Values are boolean flags (e.g., 'allow-forms', 'allow-scripts').

## Method Details

### values

public static [CspDirective](CspDirective.md)[] values()

Returns an array containing the constants of this enum class, in the order they are declared.
  Returns: an array containing the constants of this enum class, in the order they are declared
### valueOf

public static [CspDirective](CspDirective.md) valueOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the enum constant of this class with the specified name. The string must match *exactly* an identifier used to declare an enum constant in this class. (Extraneous whitespace characters are not permitted.)
  Parameters: name - the name of the enum constant to be returned. Returns: the enum constant with the specified name Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if this enum class has no constant with the specified name [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the argument is null
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
