Package [ro.sync.ecss.extensions.api.webapp.plugin.servlet](package-summary.md)

# Interface ServletResponse
    All Known Subinterfaces: [HttpServletResponse](http/HttpServletResponse.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ServletResponse
ServletResponse interface inspired from HTTP Servlet 5.0.
  Since: 26
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 void [flushBuffer](#flushBuffer())()
Forces any content in the buffer to be written to the client.
  int [getBufferSize](#getBufferSize())()
Returns the actual buffer size used for the response.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCharacterEncoding](#getCharacterEncoding())()
Returns the name of the character encoding (MIME charset) used for the body sent in this response.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContentType](#getContentType())()
Returns the content type used for the MIME body sent in this response.
  [Locale](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Locale.html) [getLocale](#getLocale())()
Returns the locale specified for this response using the [setLocale(java.util.Locale)](#setLocale(java.util.Locale)) method.
  [ServletOutputStream](ServletOutputStream.md) [getOutputStream](#getOutputStream())()
Returns a [ServletOutputStream](ServletOutputStream.md) suitable for writing binary data in the response.
  [PrintWriter](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/PrintWriter.html) [getWriter](#getWriter())()
Returns a PrintWriter object that can send character text to the client.
  boolean [isCommitted](#isCommitted())()
Returns a boolean indicating if the response has been committed.
  void [reset](#reset())()
Clears any data that exists in the buffer as well as the status code, headers.
  void [resetBuffer](#resetBuffer())()
Clears the content of the underlying buffer in the response without clearing headers or status code.
  void [setBufferSize](#setBufferSize(int))(int size)
Sets the preferred buffer size for the body of the response.
  void [setCharacterEncoding](#setCharacterEncoding(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) encoding)
Sets the character encoding (MIME charset) of the response being sent to the client, for example, to UTF-8.
  default void [setCharacterEncoding](#setCharacterEncoding(java.nio.charset.Charset))([Charset](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/nio/charset/Charset.html) encoding)
Sets the character encoding (MIME charset) of the response being sent to the client, for example, to UTF-8.
  void [setContentLength](#setContentLength(int))(int len)
Sets the length of the content body in the response In HTTP servlets, this method sets the HTTP Content-Length header.
  void [setContentLengthLong](#setContentLengthLong(long))(long len)
Sets the length of the content body in the response In HTTP servlets, this method sets the HTTP Content-Length header.
  void [setContentType](#setContentType(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) type)
Sets the content type of the response being sent to the client, if the response has not been committed yet.
  void [setLocale](#setLocale(java.util.Locale))([Locale](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Locale.html) loc)
Sets the locale of the response, if the response has not been committed yet.

## Method Details

### getCharacterEncoding

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCharacterEncoding()

Returns the name of the character encoding (MIME charset) used for the body sent in this response. The following methods for specifying the response character encoding are consulted, in decreasing order of priority: per request, perweb-app (using ServletContext#setResponseCharacterEncoding, deployment descriptor), and per container (for all web applications deployed in that container, using vendor specific configuration). The first one of these methods that yields a result is returned. Per-request, the charset for the response can be specified explicitly using the [setCharacterEncoding(String)](#setCharacterEncoding(java.lang.String)), [setCharacterEncoding(Charset)](#setCharacterEncoding(java.nio.charset.Charset)) and [setContentType(java.lang.String)](#setContentType(java.lang.String)) methods, or implicitly using the setLocale(java.util.Locale) method. Explicit specifications take precedence over implicit specifications. Calls made to these methods after getWriter has been called or after the response has been committed have no effect on the character encoding. If no character encoding has been specified, ISO-8859-1 is returned.
See RFC 2047 (http://www.ietf.org/rfc/rfc2047.txt) for more information about character encoding and MIME.

  Returns: a String specifying the name of the character encoding, for example, UTF-8
### getContentType

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContentType()

Returns the content type used for the MIME body sent in this response. The content type proper must have been specified using [setContentType(java.lang.String)](#setContentType(java.lang.String)) before the response is committed. If no content type has been specified, this method returns null. If a content type has been specified, and a character encoding has been explicitly or implicitly specified as described in [getCharacterEncoding()](#getCharacterEncoding()) or [getWriter()](#getWriter()) has been called, the charset parameter is included in the string returned. If no character encoding has been specified, the charset parameter is omitted.
  Returns: a String specifying the content type, for example, text/html; charset=UTF-8, or null
### getOutputStream

[ServletOutputStream](ServletOutputStream.md) getOutputStream() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Returns a [ServletOutputStream](ServletOutputStream.md) suitable for writing binary data in the response. The servlet container does not encode the binary data.
Calling flush() on the ServletOutputStream commits the response. Either this method or [getWriter()](#getWriter()) may be called to write the body, not both, except when [reset()](#reset()) has been called.

  Returns: a [ServletOutputStream](ServletOutputStream.md) for writing binary data Throws: [IllegalStateException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalStateException.html) - if the getWriter method has been called on this response [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - if an input or output exception occurred See Also:
        * [getWriter()](#getWriter())
        * [reset()](#reset())

### getWriter

[PrintWriter](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/PrintWriter.html) getWriter() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Returns a PrintWriter object that can send character text to the client. The PrintWriteruses the character encoding returned by [getCharacterEncoding()](#getCharacterEncoding()). If the response's character encoding has not been specified as described in getCharacterEncoding (i.e., the method just returns the default value ISO-8859-1), getWriter updates it to ISO-8859-1.
Calling flush() on the PrintWriter commits the response.

Either this method or [getOutputStream()](#getOutputStream()) may be called to write the body, not both, except when [reset()](#reset())has been called.

  Returns: a PrintWriter object that can return character data to the client Throws: [UnsupportedEncodingException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/UnsupportedEncodingException.html) - if the character encoding returned by getCharacterEncoding cannot be used [IllegalStateException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalStateException.html) - if the getOutputStream method has already been called for this response object [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - if an input or output exception occurred See Also:
        * [getOutputStream()](#getOutputStream())
        * [setCharacterEncoding(java.lang.String)](#setCharacterEncoding(java.lang.String))
        * [reset()](#reset())

### setCharacterEncoding

void setCharacterEncoding([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) encoding)

Sets the character encoding (MIME charset) of the response being sent to the client, for example, to UTF-8. If the response character encoding has already been set by ServletContext#setResponseCharacterEncoding, the deployment descriptor, or using the [setCharacterEncoding(Charset)](#setCharacterEncoding(java.nio.charset.Charset)), [setContentType(java.lang.String)](#setContentType(java.lang.String)) or [setLocale(java.util.Locale)](#setLocale(java.util.Locale)) methods, the value set in this method overrides all of those values. Calling [setContentType(java.lang.String)](#setContentType(java.lang.String)) with the String of text/html and calling this method with the String of UTF-8 is equivalent to calling [setContentType(java.lang.String)](#setContentType(java.lang.String)) with the String of text/html; charset=UTF-8.
This method can be called repeatedly to change the character encoding. This method has no effect if it is called after getWriter has been called or after the response has been committed.

If calling this method has an effect (as per the previous paragraph), calling this method with null clears any character encoding set via a previous call to this method, [setCharacterEncoding(Charset)](#setCharacterEncoding(java.nio.charset.Charset)), [setContentType(java.lang.String)](#setContentType(java.lang.String)) or [setLocale(java.util.Locale)](#setLocale(java.util.Locale)) but does not affect any default character encoding configured via ServletContext#setResponseCharacterEncoding or the deployment descriptor.

If this method is called with an invalid or unrecognised character encoding, then a subsequent call to [getWriter()](#getWriter()) will throw a [UnsupportedEncodingException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/UnsupportedEncodingException.html). Content for an unknown encoding can be sent with the [ServletOutputStream](ServletOutputStream.md) returned from [getOutputStream()](#getOutputStream()).

Containers may choose to log calls to this method that use an invalid or unrecognised character encoding.

Containers must communicate the character encoding used for the servlet response's writer to the client if the protocol provides a way for doing so. In the case of HTTP, the character encoding is communicated as part of the Content-Type header for text media types. Note that the character encoding cannot be communicated via HTTP headers if the servlet does not specify a content type; however, it is still used to encode text written via the servlet response's writer.

  Parameters: encoding - a String specifying only the character set defined by IANA Character Sets (http://www.iana.org/assignments/character-sets) or null See Also:
        * [setCharacterEncoding(Charset)](#setCharacterEncoding(java.nio.charset.Charset))
        * [setContentType(java.lang.String)](#setContentType(java.lang.String))
        * [setLocale(java.util.Locale)](#setLocale(java.util.Locale))

### setCharacterEncoding

default void setCharacterEncoding([Charset](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/nio/charset/Charset.html) encoding)

Sets the character encoding (MIME charset) of the response being sent to the client, for example, to UTF-8. If the response character encoding has already been set by ServletContext#setResponseCharacterEncoding, the deployment descriptor, or using the [setCharacterEncoding(String)](#setCharacterEncoding(java.lang.String)), [setContentType(java.lang.String)](#setContentType(java.lang.String)) or [setLocale(java.util.Locale)](#setLocale(java.util.Locale)) methods, the value set in this method overrides all of those values. Calling [setContentType(java.lang.String)](#setContentType(java.lang.String)) with the String of text/html and calling this method with [StandardCharsets.UTF_8](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/nio/charset/StandardCharsets.html#UTF_8) is equivalent to calling [setContentType(java.lang.String)](#setContentType(java.lang.String)) with the String of text/html; charset=UTF-8.
This method can be called repeatedly to change the character encoding. This method has no effect if it is called after getWriter has been called or after the response has been committed.

If calling this method has an effect (as per the previous paragraph), calling this method with null clears any character encoding set via a previous call to this method, [setCharacterEncoding(String)](#setCharacterEncoding(java.lang.String)), [setContentType(java.lang.String)](#setContentType(java.lang.String)) or [setLocale(java.util.Locale)](#setLocale(java.util.Locale)) but does not affect any default character encoding configured via ServletContext#setResponseCharacterEncoding or the deployment descriptor.

Containers must communicate the character encoding used for the servlet response's writer to the client if the protocol provides a way for doing so. In the case of HTTP, the character encoding is communicated as part of the Content-Type header for text media types. Note that the character encoding cannot be communicated via HTTP headers if the servlet does not specify a content type; however, it is still used to encode text written via the servlet response's writer.

Implementations are strongly encouraged to override this default method and provide a more efficient implementation.

  Parameters: encoding - a Charset instance representing the encoding to use or null See Also:
        * [setCharacterEncoding(String)](#setCharacterEncoding(java.lang.String))
        * [setContentType(java.lang.String)](#setContentType(java.lang.String))
        * [setLocale(java.util.Locale)](#setLocale(java.util.Locale))

### setContentLength

void setContentLength(int len)

Sets the length of the content body in the response In HTTP servlets, this method sets the HTTP Content-Length header.
This method may be called repeatedly to change the content length. This method has no effect if called after the response has been committed.

  Parameters: len - an integer specifying the length of the content being returned to the client; sets the Content-Length header
### setContentLengthLong

void setContentLengthLong(long len)

Sets the length of the content body in the response In HTTP servlets, this method sets the HTTP Content-Length header.
This method may be called repeatedly to change the content length. This method has no effect if called after the response has been committed.

  Parameters: len - a long specifying the length of the content being returned to the client; sets the Content-Length header
### setContentType

void setContentType([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) type)

Sets the content type of the response being sent to the client, if the response has not been committed yet. The given content type may include a character encoding specification, for example, text/html;charset=UTF-8. The response's character encoding is only set from the given content type if this method is called before [getWriter()](#getWriter()) is called.
This method may be called repeatedly to change content type and character encoding. This method has no effect if called after the response has been committed. It does not set the response's character encoding if it is called after getWriter has been called or after the response has been committed.

If calling this method has an effect (as per the previous paragraph), calling this method with null clears any content type set via a previous call to this method and clears any character encoding set via a previous call to this method, [setCharacterEncoding(String)](#setCharacterEncoding(java.lang.String)), [setCharacterEncoding(Charset)](#setCharacterEncoding(java.nio.charset.Charset)) or [setLocale(java.util.Locale)](#setLocale(java.util.Locale)) but does not affect any default character encoding configured via ServletContext#setResponseCharacterEncoding or the deployment descriptor.

If this method is called with an invalid or unrecognised character encoding, then a subsequent call to [getWriter()](#getWriter()) will throw a [UnsupportedEncodingException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/UnsupportedEncodingException.html). Content for an unknown encoding can be sent with the [ServletOutputStream](ServletOutputStream.md) returned from [getOutputStream()](#getOutputStream()).

Containers may choose to log calls to this method that use an invalid or unrecognised character encoding.

Containers must communicate the content type and the character encoding used for the servlet response's writer to the client if the protocol provides a way for doing so. In the case of HTTP, the Content-Type header is used.

  Parameters: type - a String specifying the MIME type of the content or null See Also:
        * [setLocale(java.util.Locale)](#setLocale(java.util.Locale))
        * [setCharacterEncoding(String)](#setCharacterEncoding(java.lang.String))
        * [setCharacterEncoding(Charset)](#setCharacterEncoding(java.nio.charset.Charset))
        * [getOutputStream()](#getOutputStream())
        * [getWriter()](#getWriter())

### setBufferSize

void setBufferSize(int size)

Sets the preferred buffer size for the body of the response. The servlet container will use a buffer at least as large as the size requested. The actual buffer size used can be found using getBufferSize.
A larger buffer allows more content to be written before anything is actually sent, thus providing the servlet with more time to set appropriate status codes and headers. A smaller buffer decreases server memory load and allows the client to start receiving data more quickly.

This method must be called before any response body content is written; if content has been written or the response object has been committed, this method throws an IllegalStateException.

  Parameters: size - the preferred buffer size Throws: [IllegalStateException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalStateException.html) - if this method is called after content has been written See Also:
        * [getBufferSize()](#getBufferSize())
        * [flushBuffer()](#flushBuffer())
        * [isCommitted()](#isCommitted())
        * [reset()](#reset())

### getBufferSize

int getBufferSize()

Returns the actual buffer size used for the response. If no buffering is used, this method returns 0.
  Returns: the actual buffer size used See Also:
        * [setBufferSize(int)](#setBufferSize(int))
        * [flushBuffer()](#flushBuffer())
        * [isCommitted()](#isCommitted())
        * [reset()](#reset())

### flushBuffer

void flushBuffer() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Forces any content in the buffer to be written to the client. A call to this method automatically commits the response, meaning the status code and headers will be written.
  Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - if the act of flushing the buffer cannot be completed. See Also:
        * [setBufferSize(int)](#setBufferSize(int))
        * [getBufferSize()](#getBufferSize())
        * [isCommitted()](#isCommitted())
        * [reset()](#reset())

### resetBuffer

void resetBuffer()

Clears the content of the underlying buffer in the response without clearing headers or status code. If the response has been committed, this method throws an IllegalStateException.
  See Also:
        * [setBufferSize(int)](#setBufferSize(int))
        * [getBufferSize()](#getBufferSize())
        * [isCommitted()](#isCommitted())
        * [reset()](#reset())

### isCommitted

boolean isCommitted()

Returns a boolean indicating if the response has been committed. A committed response has already had its status code and headers written.
  Returns: a boolean indicating if the response has been committed See Also:
        * [setBufferSize(int)](#setBufferSize(int))
        * [getBufferSize()](#getBufferSize())
        * [flushBuffer()](#flushBuffer())
        * [reset()](#reset())

### reset

void reset()

Clears any data that exists in the buffer as well as the status code, headers. The state of calling [getWriter()](#getWriter()) or [getOutputStream()](#getOutputStream()) is also cleared. It is legal, for instance, to call [getWriter()](#getWriter()), [reset()](#reset()) and then [getOutputStream()](#getOutputStream()). If [getWriter()](#getWriter()) or [getOutputStream()](#getOutputStream()) have been called before this method, then the corrresponding returned Writer or OutputStream will be staled and the behavior of using the stale object is undefined. If the response has been committed, this method throws an IllegalStateException.
  Throws: [IllegalStateException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalStateException.html) - if the response has already been committed See Also:
        * [setBufferSize(int)](#setBufferSize(int))
        * [getBufferSize()](#getBufferSize())
        * [flushBuffer()](#flushBuffer())
        * [isCommitted()](#isCommitted())

### setLocale

void setLocale([Locale](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Locale.html) loc)

Sets the locale of the response, if the response has not been committed yet. It also sets the response's character encoding appropriately for the locale, if the character encoding has not been explicitly set using [setContentType(java.lang.String)](#setContentType(java.lang.String)), [setCharacterEncoding(String)](#setCharacterEncoding(java.lang.String)) or [setCharacterEncoding(Charset)](#setCharacterEncoding(java.nio.charset.Charset)), getWriter hasn't been called yet, and the response hasn't been committed yet. If the deployment descriptor contains a locale-encoding-mapping-list element, and that element provides a mapping for the given locale, that mapping is used. Otherwise, the mapping from locale to character encoding is container dependent.
This method may be called repeatedly to change locale and character encoding. The method has no effect if called after the response has been committed. It does not set the response's character encoding if it is called after [setContentType(java.lang.String)](#setContentType(java.lang.String)) has been called with a charset specification, after [setCharacterEncoding(String)](#setCharacterEncoding(java.lang.String)) has been called, after [setCharacterEncoding(Charset)](#setCharacterEncoding(java.nio.charset.Charset)) has been called, after getWriter has been called, or after the response has been committed.

If calling this method has an effect on the locale (as per the previous paragraph), calling this method with null clears any locale set via a previous call to this method. If calling this method has an effect on the character encoding, calling this method with null clears the previously set character encoding.

Containers must communicate the locale and the character encoding used for the servlet response's writer to the client if the protocol provides a way for doing so. In the case of HTTP, the locale is communicated via the Content-Language header, the character encoding as part of the Content-Type header for text media types. Note that the character encoding cannot be communicated via HTTP headers if the servlet does not specify a content type; however, it is still used to encode text written via the servlet response's writer.

  Parameters: loc - the locale of the response or {code @null} See Also:
        * [getLocale()](#getLocale())
        * [setContentType(java.lang.String)](#setContentType(java.lang.String))
        * [setCharacterEncoding(String)](#setCharacterEncoding(java.lang.String))
        * [setCharacterEncoding(Charset)](#setCharacterEncoding(java.nio.charset.Charset))

### getLocale

[Locale](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Locale.html) getLocale()

Returns the locale specified for this response using the [setLocale(java.util.Locale)](#setLocale(java.util.Locale)) method. Calls made to setLocale after the response is committed have no effect. If no locale has been specified, the container's default locale is returned.
  Returns: the Locale for this response. See Also:
        * [setLocale(java.util.Locale)](#setLocale(java.util.Locale))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
