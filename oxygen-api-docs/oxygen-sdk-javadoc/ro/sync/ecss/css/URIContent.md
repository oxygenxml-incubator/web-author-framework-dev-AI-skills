Package [ro.sync.ecss.css](package-summary.md)

# Class URIContent

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.css.URIContent
   All Implemented Interfaces: [StaticContent](StaticContent.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class URIContent extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [StaticContent](StaticContent.md)
URI content

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected static final ro.sync.i18n.MessageBundle [messages](#messages)
The messages resource bundle.

### Fields inherited from interface ro.sync.ecss.css.[StaticContent](StaticContent.md)
 [CONTENT_CONTENT](StaticContent.md#CONTENT_CONTENT), [COUNTER_CONTENT](StaticContent.md#COUNTER_CONTENT), [COUNTERS_CONTENT](StaticContent.md#COUNTERS_CONTENT), [EDITOR_CONTENT](StaticContent.md#EDITOR_CONTENT), [LABEL_CONTENT](StaticContent.md#LABEL_CONTENT), [LEADER_CONTENT](StaticContent.md#LEADER_CONTENT), [STRING_FUNCTION_CONTENT](StaticContent.md#STRING_FUNCTION_CONTENT), [TARGET_COUNTER_CONTENT](StaticContent.md#TARGET_COUNTER_CONTENT), [TARGET_COUNTERS_CONTENT](StaticContent.md#TARGET_COUNTERS_CONTENT), [TEXT_CONTENT](StaticContent.md#TEXT_CONTENT), [URI_CONTENT](StaticContent.md#URI_CONTENT)
## Constructor Summary
 Constructors
Constructor

Description
 [URIContent](#%3Cinit%3E(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) base, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) href)  Deprecated.
Left only for backward compatibility.
   [URIContent](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) base, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) href, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cssSystemID)
Constructor

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static void [checkIfSafe](#checkIfSafe(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cssSystemID)
Connecting the an URI can be dangerous.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getBase](#getBase())()

 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getCatalogExpandedURL](#getCatalogExpandedURL())()
Returns the image URL after resolving it with the catalog.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getCatalogExpandedURL](#getCatalogExpandedURL(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) href, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) base)
Returns the image URL after resolving it with the catalog.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHref](#getHref())()

 int [getType](#getType())()
Gets the content type.
  int [hashCode](#hashCode())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### messages

protected static final ro.sync.i18n.MessageBundle messages

The messages resource bundle.

## Constructor Details

### URIContent

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public URIContent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) base, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) href)throws ro.sync.ecss.css.UnsecureContextException
 Deprecated.
Left only for backward compatibility.

Constructor.
  Parameters: base - Base system ID. href - Href. Throws: ro.sync.ecss.css.UnsecureContextException - Connecting the an URI can be dangerous. If the context is not safe we will reject the URI so a connection will not be opened.
### URIContent

public URIContent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) base, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) href, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cssSystemID)throws ro.sync.ecss.css.UnsecureContextException

Constructor
  Parameters: base - Base system ID. href - Href. cssSystemID - The location where this content was encountered. Can be null. Throws: ro.sync.ecss.css.UnsecureContextException - Connecting the an URI can be dangerous. If the context is not safe we will reject the URI so a connection will not be opened.
## Method Details

### checkIfSafe

public static void checkIfSafe([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cssSystemID)throws ro.sync.ecss.css.UnsecureContextException

Connecting the an URI can be dangerous. If the context is not safe we will reject the URI so a connection will not be opened.
```

 p:before {
   content: url('http://devel-new.sync.ro/?&file;')
 }

```

  Parameters: cssSystemID - Location in which this URI content was detected. Throws: ro.sync.ecss.css.UnsecureContextException - If the context is not safe we will reject the URI so a connection will not be opened.
### getType

public int getType()
 Description copied from interface: [StaticContent](StaticContent.md#getType())
Gets the content type.
  Specified by: [getType](StaticContent.md#getType()) in interface [StaticContent](StaticContent.md) Returns: The content type. See Also:
        * [StaticContent.getType()](StaticContent.md#getType())

### getHref

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHref()
  Returns: The href.
### getBase

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getBase()
  Returns: The Base URL
### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### getCatalogExpandedURL

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getCatalogExpandedURL() throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Returns the image URL after resolving it with the catalog. This methods should be used as a fallback for the extension bundle resolving.
  Returns: The expanded URL. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - if cannot build URL.
### getCatalogExpandedURL

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getCatalogExpandedURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) href, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) base)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Returns the image URL after resolving it with the catalog. This methods should be used as a fallback for the extension bundle resolving.
  Parameters: href - The href. base - The base. Returns: The expanded URL. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - if cannot build URL.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
