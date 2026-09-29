Package [ro.sync.syntaxhighlight.marker](package-summary.md)

# Class TokenMarkerFactory

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.syntaxhighlight.marker.TokenMarkerFactory
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public final class TokenMarkerFactory extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Factory for the TokenMarkers.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static com.google.common.collect.ImmutableMap<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Class](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Class.html)> [getContentTypesToMarkersMap](#getContentTypesToMarkersMap())()
Get the content types to markers map.
  static boolean [hasMarkerFor](#hasMarkerFor(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
See if there is a marker for the content type.
  static boolean [isJSONTokenMarker](#isJSONTokenMarker(ro.sync.syntaxhighlight.marker.TokenMarker))(ro.sync.syntaxhighlight.marker.TokenMarker tokenMarker)
Check if the provided token marker is a JSON tokenMarker.
  static boolean [isXmlTokenMarker](#isXmlTokenMarker(ro.sync.syntaxhighlight.marker.TokenMarker))(ro.sync.syntaxhighlight.marker.TokenMarker tokenMarker)
Check if the provided token marker is an XML tokenMarker
  static boolean [isYAMLTokenMarker](#isYAMLTokenMarker(ro.sync.syntaxhighlight.marker.TokenMarker))(ro.sync.syntaxhighlight.marker.TokenMarker tokenMarker)
Check if the provided token marker is a YAML tokenMarker.
  static ro.sync.syntaxhighlight.marker.TokenMarker [newTokenMarker](#newTokenMarker(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
Creates a new token marker for the specified content type.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### getContentTypesToMarkersMap

public static com.google.common.collect.ImmutableMap<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Class](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Class.html)> getContentTypesToMarkersMap()

Get the content types to markers map.
  Returns: The map with markers.
### newTokenMarker

public static ro.sync.syntaxhighlight.marker.TokenMarker newTokenMarker([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)

Creates a new token marker for the specified content type.
  Parameters: contentType - The content type. It can be: "text/xml", "text/xsl", "text/wsdl", "text/xsd", "text/dtd", "text/rng", "text/plain", "text/java", "text/javascript", "text/c", "text/cc", "text/batch", "text/shell", "text/properties", "text/sql", "text/php", "text/perl, "text/css"", "text/python", "text/xquery", "text/xpath", "text/markdown". Returns: A token marker for that content type, or null if there is none.
### hasMarkerFor

public static boolean hasMarkerFor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)

See if there is a marker for the content type.
  Parameters: contentType - The content type. Returns: True if has marker for that content type.
### isXmlTokenMarker

public static boolean isXmlTokenMarker(ro.sync.syntaxhighlight.marker.TokenMarker tokenMarker)

Check if the provided token marker is an XML tokenMarker
  Parameters: tokenMarker - to be checked Returns: true if the specified tokenMarker is an XML tokenMarker
### isJSONTokenMarker

public static boolean isJSONTokenMarker(ro.sync.syntaxhighlight.marker.TokenMarker tokenMarker)

Check if the provided token marker is a JSON tokenMarker.
  Parameters: tokenMarker - The token marker to be checked Returns: true if the specified tokenMarker is a JSON tokenMarker
### isYAMLTokenMarker

public static boolean isYAMLTokenMarker(ro.sync.syntaxhighlight.marker.TokenMarker tokenMarker)

Check if the provided token marker is a YAML tokenMarker.
  Parameters: tokenMarker - The token marker to be checked Returns: true if the specified tokenMarker is a YAML tokenMarker
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
