Package [ro.sync.ecss.extensions.api.webapp.plugin.servlet](package-summary.md)

# Interface ServletRequest
    All Known Subinterfaces: [HttpServletRequest](http/HttpServletRequest.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ServletRequest
ServletRequest interface inspired from HTTP Servlet 5.0.
  Since: 26
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getAttribute](#getAttribute(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the value of the named attribute as an Object, or null if no attribute of the given name exists.
  [Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getAttributeNames](#getAttributeNames())()
Returns an Enumeration containing the names of the attributes available to this request.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCharacterEncoding](#getCharacterEncoding())()
Returns the name of the character encoding used in the body of this request.
  int [getContentLength](#getContentLength())()
Returns the length, in bytes, of the request body and made available by the input stream, or -1 if the length is not known or is greater than Integer.MAX_VALUE.
  long [getContentLengthLong](#getContentLengthLong())()
Returns the length, in bytes, of the request body and made available by the input stream, or -1 if the length is not known.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContentType](#getContentType())()
Returns the MIME type of the body of the request, or null if the type is not known.
  [ServletInputStream](ServletInputStream.md) [getInputStream](#getInputStream())()
Retrieves the body of the request as binary data using a ServletInputStream.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLocalAddr](#getLocalAddr())()
Returns the Internet Protocol (IP) address representing the interface on which the request was received.
  [Locale](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Locale.html) [getLocale](#getLocale())()
Returns the preferred Locale that the client will accept content in, based on the Accept-Language header.
  [Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[Locale](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Locale.html)> [getLocales](#getLocales())()
Returns an Enumeration of Locale objects indicating, in decreasing order starting with the preferred locale, the locales that are acceptable to the client based on the Accept-Language header.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLocalName](#getLocalName())()
Returns the fully qualified name of the address returned by #getLocalAddr().
  int [getLocalPort](#getLocalPort())()
Returns the Internet Protocol (IP) port number representing the interface on which the request was received.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getParameter](#getParameter(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the value of a request parameter as a String, or null if the parameter does not exist.
  [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[]> [getParameterMap](#getParameterMap())()
Returns a java.util.Map of the parameters of this request.
  [Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getParameterNames](#getParameterNames())()
Returns an Enumeration of String objects containing the names of the parameters contained in this request.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getParameterValues](#getParameterValues(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns an array of String objects containing all of the values the given request parameter has, or null if the parameter does not exist.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getProtocol](#getProtocol())()
Returns the name and version of the protocol the request uses in the form *protocol/majorVersion.minorVersion*, for example, HTTP/1.1.
  [BufferedReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/BufferedReader.html) [getReader](#getReader())()
Retrieves the body of the request as character data using a BufferedReader.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRemoteAddr](#getRemoteAddr())()
Returns the Internet Protocol (IP) of the remote end of the connection on which the request was received.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRemoteHost](#getRemoteHost())()
Returns the fully qualified name of the address returned by #getRemoteAddr().
  int [getRemotePort](#getRemotePort())()
Returns the Internet Protocol (IP) source port the remote end of the connection on which the request was received.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getScheme](#getScheme())()
Returns the name of the scheme used to make this request, for example, http, https, or ftp.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getServerName](#getServerName())()
Returns the host name of the server to which the request was sent.
  int [getServerPort](#getServerPort())()
Returns the port number to which the request was sent.
  [ServletContext](ServletContext.md) [getServletContext](#getServletContext())()
Gets the servlet context to which this ServletRequest was last dispatched.
  boolean [isSecure](#isSecure())()
Returns a boolean indicating whether this request was made using a secure channel, such as HTTPS.
  void [removeAttribute](#removeAttribute(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Removes an attribute from this request.
  void [setAttribute](#setAttribute(java.lang.String,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) o)
Stores an attribute in this request.
  void [setCharacterEncoding](#setCharacterEncoding(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) encoding)
Overrides the name of the character encoding used in the body of this request.
  default void [setCharacterEncoding](#setCharacterEncoding(java.nio.charset.Charset))([Charset](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/nio/charset/Charset.html) encoding)
Overrides the character encoding used in the body of this request.

## Method Details

### getAttribute

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the value of the named attribute as an Object, or null if no attribute of the given name exists.
Attributes can be set two ways. The servlet container may set attributes to make available custom information about a request. For example, for requests made using HTTPS, the attribute jakarta.servlet.request.X509Certificate can be used to retrieve information on the certificate of the client. Attributes can also be set programmatically using ServletRequest#setAttribute. This allows information to be embedded into a request before a RequestDispatcher call.

Attribute names should follow the same conventions as package names. The Jakarta Servlet specification reserves names matching jakarta.\*.

  Parameters: name - a String specifying the name of the attribute Returns: an Object containing the value of the attribute, or null if the attribute does not exist
### getAttributeNames

[Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getAttributeNames()

Returns an Enumeration containing the names of the attributes available to this request. This method returns an empty Enumeration if the request has no attributes available to it.
  Returns: an Enumeration of strings containing the names of the request's attributes
### getCharacterEncoding

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCharacterEncoding()

Returns the name of the character encoding used in the body of this request. This method returns null if no request encoding character encoding has been specified. The following methods for specifying the request character encoding are consulted, in decreasing order of priority: per request, per web app (using ServletContext#setRequestCharacterEncoding, deployment descriptor), and per container (for all web applications deployed in that container, using vendor specific configuration).
  Returns: a String containing the name of the character encoding, or null if the request does not specify a character encoding
### setCharacterEncoding

void setCharacterEncoding([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) encoding)throws [UnsupportedEncodingException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/UnsupportedEncodingException.html)

Overrides the name of the character encoding used in the body of this request. This method must be called prior to reading request parameters or reading input using getReader(). Otherwise, it has no effect.
  Parameters: encoding - String containing the name of the character encoding. Throws: [UnsupportedEncodingException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/UnsupportedEncodingException.html) - if this ServletRequest is still in a state where a character encoding may be set, but the specified encoding is invalid
### setCharacterEncoding

default void setCharacterEncoding([Charset](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/nio/charset/Charset.html) encoding)

Overrides the character encoding used in the body of this request. This method must be called prior to reading request parameters or reading input using getReader(). Otherwise, it has no effect.
Implementations are strongly encouraged to override this default method and provide a more efficient implementation.

  Parameters: encoding - Charset representing the character encoding.
### getContentLength

int getContentLength()

Returns the length, in bytes, of the request body and made available by the input stream, or -1 if the length is not known or is greater than Integer.MAX_VALUE.
  Returns: an integer containing the length of the request body or -1 if the length is not known or is greater than Integer.MAX_VALUE.
### getContentLengthLong

long getContentLengthLong()

Returns the length, in bytes, of the request body and made available by the input stream, or -1 if the length is not known.
  Returns: a long containing the length of the request body or -1L if the length is not known
### getContentType

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContentType()

Returns the MIME type of the body of the request, or null if the type is not known.
  Returns: a String containing the name of the MIME type of the request, or null if the type is not known
### getInputStream

[ServletInputStream](ServletInputStream.md) getInputStream() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Retrieves the body of the request as binary data using a ServletInputStream. Either this method or #getReader may be called to read the body, not both.
  Returns: a ServletInputStream object containing the body of the request Throws: [IllegalStateException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalStateException.html) - if the #getReader method has already been called for this request [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - if an input or output exception occurred
### getParameter

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getParameter([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the value of a request parameter as a String, or null if the parameter does not exist. Request parameters are extra information sent with the request. For HTTP servlets, parameters are contained in the query string or posted form data.
You should only use this method when you are sure the parameter has only one value. If the parameter might have more than one value, use #getParameterValues.

If you use this method with a multivalued parameter, the value returned is equal to the first value in the array returned by getParameterValues.

If the parameter data was sent in the request body, such as occurs with an HTTP POST request, then reading the body directly via #getInputStream or #getReader can interfere with the execution of this method.

  Parameters: name - a String specifying the name of the parameter Returns: a String representing the single value of the parameter See Also:
        * [getParameterValues(java.lang.String)](#getParameterValues(java.lang.String))

### getParameterNames

[Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getParameterNames()

Returns an Enumeration of String objects containing the names of the parameters contained in this request. If the request has no parameters, the method returns an empty Enumeration.
  Returns: an Enumeration of String objects, each String containing the name of a request parameter; or an empty Enumeration if the request has no parameters
### getParameterValues

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getParameterValues([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns an array of String objects containing all of the values the given request parameter has, or null if the parameter does not exist.
If the parameter has a single value, the array has a length of 1.

  Parameters: name - a String containing the name of the parameter whose value is requested Returns: an array of String objects containing the parameter's values See Also:
        * [getParameter(java.lang.String)](#getParameter(java.lang.String))

### getParameterMap

[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[]> getParameterMap()

Returns a java.util.Map of the parameters of this request.
Request parameters are extra information sent with the request. For HTTP servlets, parameters are contained in the query string or posted form data.

  Returns: an immutable java.util.Map containing parameter names as keys and parameter values as map values. The keys in the parameter map are of type String. The values in the parameter map are of type String array.
### getProtocol

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getProtocol()

Returns the name and version of the protocol the request uses in the form *protocol/majorVersion.minorVersion*, for example, HTTP/1.1.
  Returns: a String containing the protocol name and version number
### getScheme

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getScheme()

Returns the name of the scheme used to make this request, for example, http, https, or ftp. Different schemes have different rules for constructing URLs, as noted in RFC 1738.
  Returns: a String containing the name of the scheme used to make this request
### getServerName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getServerName()

Returns the host name of the server to which the request was sent. It may be derived from a protocol specific mechanism, such as the Host header, or the HTTP/2 authority, or [RFC 7239](https://tools.ietf.org/html/rfc7239), otherwise the resolved server name or the server IP address.
  Returns: a String containing the name of the server
### getServerPort

int getServerPort()

Returns the port number to which the request was sent. It may be derived from a protocol specific mechanism, such as the Host header, or HTTP authority, or [RFC 7239](https://tools.ietf.org/html/rfc7239), otherwise the server port where the client connection was accepted on.
  Returns: an integer specifying the port number
### getReader

[BufferedReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/BufferedReader.html) getReader() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Retrieves the body of the request as character data using a BufferedReader. The reader translates the character data according to the character encoding used on the body. Either this method or #getInputStreammay be called to read the body, not both.
  Returns: a BufferedReader containing the body of the request Throws: [UnsupportedEncodingException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/UnsupportedEncodingException.html) - if the character set encoding used is not supported and the text cannot be decoded [IllegalStateException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalStateException.html) - if #getInputStream method has been called on this request [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - if an input or output exception occurred See Also:
        * [getInputStream()](#getInputStream())

### getRemoteAddr

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRemoteAddr()

Returns the Internet Protocol (IP) of the remote end of the connection on which the request was received. By default this is either the address of the client or last proxy that sent the request. In some cases a protocol specific mechanism, such as [RFC 7239](https://tools.ietf.org/html/rfc7239), may be used to obtain an address different to that of the actual TCP/IP connection.
  Returns: a String containing an IP address
### getRemoteHost

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRemoteHost()

Returns the fully qualified name of the address returned by #getRemoteAddr(). If the engine cannot or chooses not to resolve the hostname (to improve performance), this method returns the IP address.
  Returns: a String containing a fully qualified name or IP address.
### setAttribute

void setAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) o)

Stores an attribute in this request. Attributes are reset between requests. This method is most often used in conjunction with RequestDispatcher.
Attribute names should follow the same conventions as package names. If the object passed in is null, the effect is the same as calling #removeAttribute. It is warned that when the request is dispatched from the servlet resides in a different web application by RequestDispatcher, the object set by this method may not be correctly retrieved in the caller servlet.

  Parameters: name - a String specifying the name of the attribute o - the Object to be stored
### removeAttribute

void removeAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Removes an attribute from this request. This method is not generally needed as attributes only persist as long as the request is being handled.
Attribute names should follow the same conventions as package names. Names beginning with jakarta.\* are reserved for use by the Jakarta Servlet specification.

  Parameters: name - a String specifying the name of the attribute to remove
### getLocale

[Locale](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Locale.html) getLocale()

Returns the preferred Locale that the client will accept content in, based on the Accept-Language header. If the client request doesn't provide an Accept-Language header, this method returns the default locale for the server.
  Returns: the preferred Locale for the client
### getLocales

[Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[Locale](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Locale.html)> getLocales()

Returns an Enumeration of Locale objects indicating, in decreasing order starting with the preferred locale, the locales that are acceptable to the client based on the Accept-Language header. If the client request doesn't provide an Accept-Language header, this method returns an Enumeration containing one Locale, the default locale for the server.
  Returns: an Enumeration of preferred Locale objects for the client
### isSecure

boolean isSecure()

Returns a boolean indicating whether this request was made using a secure channel, such as HTTPS.
  Returns: a boolean indicating if the request was made using a secure channel
### getRemotePort

int getRemotePort()

Returns the Internet Protocol (IP) source port the remote end of the connection on which the request was received. By default this is either the port of the client or last proxy that sent the request. In some cases, protocol specific mechanisms such as [RFC 7239](https://tools.ietf.org/html/rfc7239) may be used to obtain a port different to that of the actual TCP/IP connection.
  Returns: an integer specifying the port number
### getLocalName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLocalName()

Returns the fully qualified name of the address returned by #getLocalAddr(). If the engine cannot or chooses not to resolve the hostname (to improve performance), this method returns the IP address.
  Returns: a String containing the host name of the IP on which the request was received.
### getLocalAddr

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLocalAddr()

Returns the Internet Protocol (IP) address representing the interface on which the request was received. In some cases a protocol specific mechanism, such as [RFC 7239](https://tools.ietf.org/html/rfc7239), may be used to obtain an address different to that of the actual TCP/IP connection.
  Returns: a String containing an IP address.
### getLocalPort

int getLocalPort()

Returns the Internet Protocol (IP) port number representing the interface on which the request was received. In some cases, a protocol specific mechanism such as [RFC 7239](https://tools.ietf.org/html/rfc7239) may be used to obtain an address different to that of the actual TCP/IP connection.
  Returns: an integer specifying a port number
### getServletContext

[ServletContext](ServletContext.md) getServletContext()

Gets the servlet context to which this ServletRequest was last dispatched.
  Returns: the servlet context to which this ServletRequest was last dispatched
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
