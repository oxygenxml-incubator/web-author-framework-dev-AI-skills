Package [ro.sync.ecss.extensions.api.webapp.plugin.servlet.http](package-summary.md)

# Interface HttpServletRequest
    All Superinterfaces: [ServletRequest](../ServletRequest.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface HttpServletRequestextends [ServletRequest](../ServletRequest.md)
HTTP Request interface inspired from HTTP Servlet 5.0.
  Since: 26
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContextPath](#getContextPath())()
Returns the portion of the request URI that indicates the context of the request.
  [Cookie](Cookie.md)[] [getCookies](#getCookies())()
Returns an array containing all of the Cookie objects the client sent with this request.
  long [getDateHeader](#getDateHeader(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the value of the specified request header as a long value that represents a Dateobject.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHeader](#getHeader(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the value of the specified request header as a String.
  [Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getHeaderNames](#getHeaderNames())()
Returns an enumeration of all the header names this request contains.
  [Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getHeaders](#getHeaders(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns all the values of the specified request header as an Enumeration of String objects.
  int [getIntHeader](#getIntHeader(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the value of the specified request header as an int.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMethod](#getMethod())()
Returns the name of the HTTP method with which this request was made, for example, GET, POST, or PUT.
  [Part](Part.md) [getPart](#getPart(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Gets the [Part](Part.md) with the given name.
  [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[Part](Part.md)> [getParts](#getParts())()
Gets all the [Part](Part.md) components of this request, provided that it is of type multipart/form-data.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPathInfo](#getPathInfo())()
Returns any extra path information associated with the URL the client sent when it made this request.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPathTranslated](#getPathTranslated())()
Returns any extra path information after the servlet name but before the query string, and translates it to a real path.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getQueryString](#getQueryString())()
Returns the query string that is contained in the request URL after the path.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRequestURI](#getRequestURI())()
Returns the part of this request's URL from the protocol name up to the query string in the first line of the HTTP request.
  [StringBuffer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/StringBuffer.html) [getRequestURL](#getRequestURL())()
Reconstructs the URL the client used to make the request.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getServletPath](#getServletPath())()
Returns the part of this request's URL that calls the servlet.
  [HttpSession](HttpSession.md) [getSession](#getSession())()
Returns the current session associated with this request, or if the request does not have a session, creates one.
  [HttpSession](HttpSession.md) [getSession](#getSession(boolean))(boolean create)
Returns the current HttpSession associated with this request or, if there is no current session and create is true, returns a new session.

### Methods inherited from interface ro.sync.ecss.extensions.api.webapp.plugin.servlet.[ServletRequest](../ServletRequest.md)
 [getAttribute](../ServletRequest.md#getAttribute(java.lang.String)), [getAttributeNames](../ServletRequest.md#getAttributeNames()), [getCharacterEncoding](../ServletRequest.md#getCharacterEncoding()), [getContentLength](../ServletRequest.md#getContentLength()), [getContentLengthLong](../ServletRequest.md#getContentLengthLong()), [getContentType](../ServletRequest.md#getContentType()), [getInputStream](../ServletRequest.md#getInputStream()), [getLocalAddr](../ServletRequest.md#getLocalAddr()), [getLocale](../ServletRequest.md#getLocale()), [getLocales](../ServletRequest.md#getLocales()), [getLocalName](../ServletRequest.md#getLocalName()), [getLocalPort](../ServletRequest.md#getLocalPort()), [getParameter](../ServletRequest.md#getParameter(java.lang.String)), [getParameterMap](../ServletRequest.md#getParameterMap()), [getParameterNames](../ServletRequest.md#getParameterNames()), [getParameterValues](../ServletRequest.md#getParameterValues(java.lang.String)), [getProtocol](../ServletRequest.md#getProtocol()), [getReader](../ServletRequest.md#getReader()), [getRemoteAddr](../ServletRequest.md#getRemoteAddr()), [getRemoteHost](../ServletRequest.md#getRemoteHost()), [getRemotePort](../ServletRequest.md#getRemotePort()), [getScheme](../ServletRequest.md#getScheme()), [getServerName](../ServletRequest.md#getServerName()), [getServerPort](../ServletRequest.md#getServerPort()), [getServletContext](../ServletRequest.md#getServletContext()), [isSecure](../ServletRequest.md#isSecure()), [removeAttribute](../ServletRequest.md#removeAttribute(java.lang.String)), [setAttribute](../ServletRequest.md#setAttribute(java.lang.String,java.lang.Object)), [setCharacterEncoding](../ServletRequest.md#setCharacterEncoding(java.lang.String)), [setCharacterEncoding](../ServletRequest.md#setCharacterEncoding(java.nio.charset.Charset))
## Method Details

### getCookies

[Cookie](Cookie.md)[] getCookies()

Returns an array containing all of the Cookie objects the client sent with this request. This method returns null if no cookies were sent.
  Returns: an array of all the Cookies included with this request, or null if the request has no cookies
### getDateHeader

long getDateHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the value of the specified request header as a long value that represents a Dateobject. Use this method with headers that contain dates, such as If-Modified-Since.
The date is returned as the number of milliseconds since January 1, 1970 GMT. The header name is case insensitive.

If the request did not have a header of the specified name, this method returns -1. If there are multiple headers with the same name, this method returns the value of the first header in the request. If the header can't be converted to a date, the method throws an IllegalArgumentException.

  Parameters: name - a String specifying the name of the header Returns: a long value representing the date specified in the header expressed as the number of milliseconds since January 1, 1970 GMT, or -1 if the named header was not included with the request Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - If the header value can't be converted to a date
### getHeader

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the value of the specified request header as a String. If the request did not include a header of the specified name, this method returns null. If there are multiple headers with the same name, this method returns the value of the first header in the request. The header name is case insensitive. You can use this method with any request header.
  Parameters: name - a String specifying the header name Returns: a String containing the value of the requested header, or null if the request does not have a header of that name
### getHeaders

[Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getHeaders([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns all the values of the specified request header as an Enumeration of String objects.
Some headers, such as Accept-Language can be sent by clients as several headers each with a different value rather than sending the header as a comma separated list.

If the request did not include any headers of the specified name, this method returns an empty Enumeration. The header name is case insensitive. You can use this method with any request header.

  Parameters: name - a String specifying the header name Returns: an Enumeration containing the values of the requested header. If the request does not have any headers of that name return an empty enumeration. If the container does not allow access to header information, return null
### getHeaderNames

[Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getHeaderNames()

Returns an enumeration of all the header names this request contains. If the request has no headers, this method returns an empty enumeration.
Some servlet containers do not allow servlets to access headers using this method, in which case this method returns null

  Returns: an enumeration of all the header names sent with this request; if the request has no headers, an empty enumeration; if the servlet container does not allow servlets to use this method, null
### getIntHeader

int getIntHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the value of the specified request header as an int. If the request does not have a header of the specified name, this method returns -1. If there are multiple headers with the same name, this method returns the value of the first header in the request. If the header cannot be converted to an integer, this method throws a NumberFormatException.
The header name is case insensitive.

  Parameters: name - a String specifying the name of a request header Returns: an integer expressing the value of the request header or -1 if the request doesn't have a header of this name Throws: [NumberFormatException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NumberFormatException.html) - If the header value can't be converted to an int
### getMethod

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMethod()

Returns the name of the HTTP method with which this request was made, for example, GET, POST, or PUT.
  Returns: a String specifying the name of the method with which this request was made
### getPathInfo

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPathInfo()

Returns any extra path information associated with the URL the client sent when it made this request. The extra path information follows the servlet path but precedes the query string and will start with a "/" character.
This method returns null if there was no extra path information.

  Returns: a String specifying extra path information that comes after the servlet path but before the query string in the request URL; or null if the URL does not have any extra path information. The path will be canonicalized as per [Servlet 6.0, 3.5](https://jakarta.ee/specifications/servlet/6.0/jakarta-servlet-spec-6.0.html#request-uri-path-processing). This method will not return any encoded characters unless the container is configured specifically to allow them. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - In standard configuration, this method will never throw. However, a container may be configured to not reject some suspicious sequences identified by [Servlet 6.0, 3.5.2](https://jakarta.ee/specifications/servlet/6.0/jakarta-servlet-spec-6.0.html#uri-path-canonicalization)[]()[, furthermore the container may be configured to allow such paths to only be accessed via safer methods like ](https://jakarta.ee/specifications/servlet/6.0/jakarta-servlet-spec-6.0.html#uri-path-canonicalization)[getRequestURI()](#getRequestURI())[ and to throw IllegalArgumentException if this method is called for such suspicious paths.](https://jakarta.ee/specifications/servlet/6.0/jakarta-servlet-spec-6.0.html#uri-path-canonicalization)
### getPathTranslated

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPathTranslated()

Returns any extra path information after the servlet name but before the query string, and translates it to a real path.
If the URL does not have any extra path information, this method returns null or the servlet container cannot translate the virtual path to a real path for any reason (such as when the web application is executed from an archive). The web container does not decode this string.

  Returns: a String specifying the real path, or null if the URL does not have any extra path information
### getContextPath

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContextPath()

Returns the portion of the request URI that indicates the context of the request. The context path always comes first in a request URI. The path starts with a "/" character but does not end with a "/" character. For servlets in the default (root) context, this method returns "". The container does not decode this string.
It is possible that a servlet container may match a context by more than one context path. In such cases this method will return the actual context path used by the request and it may differ from the path returned by the [ServletContext.getContextPath()](../ServletContext.md#getContextPath()) method. The context path returned by [ServletContext.getContextPath()](../ServletContext.md#getContextPath()) should be considered as the prime or preferred context path of the application.

  Returns: a String specifying the portion of the request URI that indicates the context of the request. The path will be canonicalized as per [Servlet 6.0, 3.5](https://jakarta.ee/specifications/servlet/6.0/jakarta-servlet-spec-6.0.html#request-uri-path-processing). This method will not return any encoded characters unless the container is configured specifically to allow them. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - In standard configuration, this method will never throw. However, a container may be configured to not reject some suspicious sequences identified by [Servlet 6.0, 3.5.2](https://jakarta.ee/specifications/servlet/6.0/jakarta-servlet-spec-6.0.html#uri-path-canonicalization)[]()[, furthermore the container may be configured to allow such paths to only be accessed via safer methods like ](https://jakarta.ee/specifications/servlet/6.0/jakarta-servlet-spec-6.0.html#uri-path-canonicalization)[getRequestURI()](#getRequestURI())[ and to throw IllegalArgumentException if this method is called for such suspicious paths.](https://jakarta.ee/specifications/servlet/6.0/jakarta-servlet-spec-6.0.html#uri-path-canonicalization) See Also:
        * [ServletContext.getContextPath()](../ServletContext.md#getContextPath())

### getQueryString

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getQueryString()

Returns the query string that is contained in the request URL after the path. This method returns nullif the URL does not have a query string.
  Returns: a String containing the query string or null if the URL contains no query string. The value is not decoded by the container.
### getRequestURI

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRequestURI()

Returns the part of this request's URL from the protocol name up to the query string in the first line of the HTTP request. The web container does not decode this String. For example:
| -----------| -----------|
| First line of HTTP request | Returned Value |
| POST /some/path.html HTTP/1.1  |   | /some/path.html  |
| GET http://foo.bar/a.html HTTP/1.0  |   | /a.html  |
| HEAD /xyz?a=b HTTP/1.1  |   | /xyz  |

  Returns: a String containing the part of the URL from the protocol name up to the query string
### getRequestURL

[StringBuffer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/StringBuffer.html) getRequestURL()

Reconstructs the URL the client used to make the request. The returned URL contains a protocol, server name, port number, and server path, but it does not include query string parameters.
If this request has been forwarded using RequestDispatcher#forward, the server path in the reconstructed URL must reflect the path used to obtain the RequestDispatcher, and not the server path specified by the client.

Because this method returns a StringBuffer, not a string, you can modify the URL easily, for example, to append query parameters.

This method is useful for creating redirect messages and for reporting errors.

  Returns: a StringBuffer object containing the reconstructed URL
### getServletPath

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getServletPath()

Returns the part of this request's URL that calls the servlet. This path starts with a "/" character and includes the path to the servlet, but does not include any extra path information or a query string.
This method will return an empty string ("") if the servlet used to process this request was matched using the "/\*" pattern.

  Returns: a String containing the path of the servlet being called, as specified in the request URL, or an empty string if the servlet used to process the request is matched using the "/\*" pattern. The path will be canonicalized as per [Servlet 6.0, 3.5](https://jakarta.ee/specifications/servlet/6.0/jakarta-servlet-spec-6.0.html#request-uri-path-processing). This method will not return any encoded characters unless the container is configured specifically to allow them. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - In standard configuration, this method will never throw. However, a container may be configured to not reject some suspicious sequences identified by [Servlet 6.0, 3.5.2](https://jakarta.ee/specifications/servlet/6.0/jakarta-servlet-spec-6.0.html#uri-path-canonicalization)[]()[, furthermore the container may be configured to allow such paths to only be accessed via safer methods like ](https://jakarta.ee/specifications/servlet/6.0/jakarta-servlet-spec-6.0.html#uri-path-canonicalization)[getRequestURI()](#getRequestURI())[ and to throw IllegalArgumentException if this method is called for such suspicious paths.](https://jakarta.ee/specifications/servlet/6.0/jakarta-servlet-spec-6.0.html#uri-path-canonicalization)
### getSession

[HttpSession](HttpSession.md) getSession(boolean create)

Returns the current HttpSession associated with this request or, if there is no current session and create is true, returns a new session.
If create is false and the request has no valid HttpSession, this method returns null.

To make sure the session is properly maintained, you must call this method before the response is committed. If the container is using cookies to maintain session integrity and is asked to create a new session when the response is committed, an IllegalStateException is thrown.

  Parameters: create - true to create a new session for this request if necessary; false to return null if there's no current session Returns: the HttpSession associated with this request or null if create is false and the request has no valid session See Also:
        * [getSession()](#getSession())

### getSession

[HttpSession](HttpSession.md) getSession()

Returns the current session associated with this request, or if the request does not have a session, creates one.
  Returns: the HttpSession associated with this request See Also:
        * [getSession(boolean)](#getSession(boolean))

### getParts

[Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[Part](Part.md)> getParts() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [ServletException](../ServletException.md)

Gets all the [Part](Part.md) components of this request, provided that it is of type multipart/form-data.
If this request is of type multipart/form-data, but does not contain any Part components, the returned Collection will be empty.

Any changes to the returned Collection must not affect this HttpServletRequest.

  Returns: a (possibly empty) Collection of the Part components of this request Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - if an I/O error occurred during the retrieval of the [Part](Part.md) components of this request [ServletException](../ServletException.md) - if this request is not of type multipart/form-data [IllegalStateException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalStateException.html) - if the request body is larger than maxRequestSize, or any Part in the request is larger than maxFileSize, or there is no @MultipartConfig or multipart-config in deployment descriptors
### getPart

[Part](Part.md) getPart([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [ServletException](../ServletException.md)

Gets the [Part](Part.md) with the given name.
  Parameters: name - the name of the requested Part Returns: The Part with the given name, or null if this request is of type multipart/form-data, but does not contain the requested Part Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - if an I/O error occurred during the retrieval of the requested Part [ServletException](../ServletException.md) - if this request is not of type multipart/form-data [IllegalStateException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalStateException.html) - if the request body is larger than maxRequestSize, or any Part in the request is larger than maxFileSize, or there is no @MultipartConfig or multipart-config in deployment descriptors
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
