Package [ro.sync.ecss.extensions.api.webapp.plugin.servlet.http](package-summary.md)

# Interface HttpServletResponse
    All Superinterfaces: [ServletResponse](../ServletResponse.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface HttpServletResponseextends [ServletResponse](../ServletResponse.md)
Response interface inspired from HTTP Servlet 5.0.
  Since: 26
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [SC_ACCEPTED](#SC_ACCEPTED)
Status code (202) indicating that a request was accepted for processing, but was not completed.
  static final int [SC_BAD_GATEWAY](#SC_BAD_GATEWAY)
Status code (502) indicating that the HTTP server received an invalid response from a server it consulted when acting as a proxy or gateway.
  static final int [SC_BAD_REQUEST](#SC_BAD_REQUEST)
Status code (400) indicating the request sent by the client was syntactically incorrect.
  static final int [SC_CONFLICT](#SC_CONFLICT)
Status code (409) indicating that the request could not be completed due to a conflict with the current state of the resource.
  static final int [SC_CONTINUE](#SC_CONTINUE)
Status code (100) indicating the client can continue.
  static final int [SC_CREATED](#SC_CREATED)
Status code (201) indicating the request succeeded and created a new resource on the server.
  static final int [SC_EXPECTATION_FAILED](#SC_EXPECTATION_FAILED)
Status code (417) indicating that the server could not meet the expectation given in the Expect request header.
  static final int [SC_FORBIDDEN](#SC_FORBIDDEN)
Status code (403) indicating the server understood the request but refused to fulfill it.
  static final int [SC_FOUND](#SC_FOUND)
Status code (302) indicating that the resource reside temporarily under a different URI.
  static final int [SC_GATEWAY_TIMEOUT](#SC_GATEWAY_TIMEOUT)
Status code (504) indicating that the server did not receive a timely response from the upstream server while acting as a gateway or proxy.
  static final int [SC_GONE](#SC_GONE)
Status code (410) indicating that the resource is no longer available at the server and no forwarding address is known.
  static final int [SC_HTTP_VERSION_NOT_SUPPORTED](#SC_HTTP_VERSION_NOT_SUPPORTED)
Status code (505) indicating that the server does not support or refuses to support the HTTP protocol version that was used in the request message.
  static final int [SC_INTERNAL_SERVER_ERROR](#SC_INTERNAL_SERVER_ERROR)
Status code (500) indicating an error inside the HTTP server which prevented it from fulfilling the request.
  static final int [SC_LENGTH_REQUIRED](#SC_LENGTH_REQUIRED)
Status code (411) indicating that the request cannot be handled without a defined Content-Length.
  static final int [SC_METHOD_NOT_ALLOWED](#SC_METHOD_NOT_ALLOWED)
Status code (405) indicating that the method specified in the Request-Line is not allowed for the resource identified by the Request-URI.
  static final int [SC_MOVED_PERMANENTLY](#SC_MOVED_PERMANENTLY)
Status code (301) indicating that the resource has permanently moved to a new location, and that future references should use a new URI with their requests.
  static final int [SC_MOVED_TEMPORARILY](#SC_MOVED_TEMPORARILY)
Status code (302) indicating that the resource has temporarily moved to another location, but that future references should still use the original URI to access the resource.
  static final int [SC_MULTIPLE_CHOICES](#SC_MULTIPLE_CHOICES)
Status code (300) indicating that the requested resource corresponds to any one of a set of representations, each with its own specific location.
  static final int [SC_NO_CONTENT](#SC_NO_CONTENT)
Status code (204) indicating that the request succeeded but that there was no new information to return.
  static final int [SC_NON_AUTHORITATIVE_INFORMATION](#SC_NON_AUTHORITATIVE_INFORMATION)
Status code (203) indicating that the meta information presented by the client did not originate from the server.
  static final int [SC_NOT_ACCEPTABLE](#SC_NOT_ACCEPTABLE)
Status code (406) indicating that the resource identified by the request is only capable of generating response entities which have content characteristics not acceptable according to the accept headers sent in the request.
  static final int [SC_NOT_FOUND](#SC_NOT_FOUND)
Status code (404) indicating that the requested resource is not available.
  static final int [SC_NOT_IMPLEMENTED](#SC_NOT_IMPLEMENTED)
Status code (501) indicating the HTTP server does not support the functionality needed to fulfill the request.
  static final int [SC_NOT_MODIFIED](#SC_NOT_MODIFIED)
Status code (304) indicating that a conditional GET operation found that the resource was available and not modified.
  static final int [SC_OK](#SC_OK)
Status code (200) indicating the request succeeded normally.
  static final int [SC_PARTIAL_CONTENT](#SC_PARTIAL_CONTENT)
Status code (206) indicating that the server has fulfilled the partial GET request for the resource.
  static final int [SC_PAYMENT_REQUIRED](#SC_PAYMENT_REQUIRED)
Status code (402) reserved for future use.
  static final int [SC_PRECONDITION_FAILED](#SC_PRECONDITION_FAILED)
Status code (412) indicating that the precondition given in one or more of the request-header fields evaluated to false when it was tested on the server.
  static final int [SC_PROXY_AUTHENTICATION_REQUIRED](#SC_PROXY_AUTHENTICATION_REQUIRED)
Status code (407) indicating that the client MUST first authenticate itself with the proxy.
  static final int [SC_REQUEST_ENTITY_TOO_LARGE](#SC_REQUEST_ENTITY_TOO_LARGE)
Status code (413) indicating that the server is refusing to process the request because the request entity is larger than the server is willing or able to process.
  static final int [SC_REQUEST_TIMEOUT](#SC_REQUEST_TIMEOUT)
Status code (408) indicating that the client did not produce a request within the time that the server was prepared to wait.
  static final int [SC_REQUEST_URI_TOO_LONG](#SC_REQUEST_URI_TOO_LONG)
Status code (414) indicating that the server is refusing to service the request because the Request-URI is longer than the server is willing to interpret.
  static final int [SC_REQUESTED_RANGE_NOT_SATISFIABLE](#SC_REQUESTED_RANGE_NOT_SATISFIABLE)
Status code (416) indicating that the server cannot serve the requested byte range.
  static final int [SC_RESET_CONTENT](#SC_RESET_CONTENT)
Status code (205) indicating that the agent SHOULD reset the document view which caused the request to be sent.
  static final int [SC_SEE_OTHER](#SC_SEE_OTHER)
Status code (303) indicating that the response to the request can be found under a different URI.
  static final int [SC_SERVICE_UNAVAILABLE](#SC_SERVICE_UNAVAILABLE)
Status code (503) indicating that the HTTP server is temporarily overloaded, and unable to handle the request.
  static final int [SC_SWITCHING_PROTOCOLS](#SC_SWITCHING_PROTOCOLS)
Status code (101) indicating the server is switching protocols according to Upgrade header.
  static final int [SC_TEMPORARY_REDIRECT](#SC_TEMPORARY_REDIRECT)
Status code (307) indicating that the requested resource resides temporarily under a different URI.
  static final int [SC_UNAUTHORIZED](#SC_UNAUTHORIZED)
Status code (401) indicating that the request requires HTTP authentication.
  static final int [SC_UNSUPPORTED_MEDIA_TYPE](#SC_UNSUPPORTED_MEDIA_TYPE)
Status code (415) indicating that the server is refusing to service the request because the entity of the request is in a format not supported by the requested resource for the requested method.
  static final int [SC_USE_PROXY](#SC_USE_PROXY)
Status code (305) indicating that the requested resource MUST be accessed through the proxy given by the Location field.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addCookie](#addCookie(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.Cookie))([Cookie](Cookie.md) cookie)
Adds the specified cookie to the response.
  void [addDateHeader](#addDateHeader(java.lang.String,long))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, long date)
Adds a response header with the given name and date-value.
  void [addHeader](#addHeader(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Adds a response header with the given name and value.
  void [addIntHeader](#addIntHeader(java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int value)
Adds a response header with the given name and integer value.
  boolean [containsHeader](#containsHeader(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns a boolean indicating whether the named response header has already been set.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [encodeRedirectURL](#encodeRedirectURL(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)
Encodes the specified URL for use in the sendRedirect method or, if encoding is not needed, returns the URL unchanged.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [encodeURL](#encodeURL(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)
Encodes the specified URL by including the session ID, or, if encoding is not needed, returns the URL unchanged.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHeader](#getHeader(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Gets the value of the response header with the given name.
  [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getHeaderNames](#getHeaderNames())()
Gets the names of the headers of this response.
  [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getHeaders](#getHeaders(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Gets the values of the response header with the given name.
  int [getStatus](#getStatus())()
Gets the current status code of this response.
  void [sendError](#sendError(int))(int sc)
Sends an error response to the client using the specified status code and clears the buffer.
  void [sendError](#sendError(int,java.lang.String))(int sc, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) msg)
Sends an error response to the client using the specified status and clears the buffer.
  void [sendRedirect](#sendRedirect(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) location)
Sends a temporary redirect response to the client using the specified redirect location URL and clears the buffer.
  void [setDateHeader](#setDateHeader(java.lang.String,long))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, long date)
Sets a response header with the given name and date-value.
  void [setHeader](#setHeader(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Sets a response header with the given name and value.
  void [setIntHeader](#setIntHeader(java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int value)
Sets a response header with the given name and integer value.
  void [setStatus](#setStatus(int))(int sc)
Sets the status code for this response.

### Methods inherited from interface ro.sync.ecss.extensions.api.webapp.plugin.servlet.[ServletResponse](../ServletResponse.md)
 [flushBuffer](../ServletResponse.md#flushBuffer()), [getBufferSize](../ServletResponse.md#getBufferSize()), [getCharacterEncoding](../ServletResponse.md#getCharacterEncoding()), [getContentType](../ServletResponse.md#getContentType()), [getLocale](../ServletResponse.md#getLocale()), [getOutputStream](../ServletResponse.md#getOutputStream()), [getWriter](../ServletResponse.md#getWriter()), [isCommitted](../ServletResponse.md#isCommitted()), [reset](../ServletResponse.md#reset()), [resetBuffer](../ServletResponse.md#resetBuffer()), [setBufferSize](../ServletResponse.md#setBufferSize(int)), [setCharacterEncoding](../ServletResponse.md#setCharacterEncoding(java.lang.String)), [setCharacterEncoding](../ServletResponse.md#setCharacterEncoding(java.nio.charset.Charset)), [setContentLength](../ServletResponse.md#setContentLength(int)), [setContentLengthLong](../ServletResponse.md#setContentLengthLong(long)), [setContentType](../ServletResponse.md#setContentType(java.lang.String)), [setLocale](../ServletResponse.md#setLocale(java.util.Locale))
## Field Details

### SC_CONTINUE

static final int SC_CONTINUE

Status code (100) indicating the client can continue.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_CONTINUE)

### SC_SWITCHING_PROTOCOLS

static final int SC_SWITCHING_PROTOCOLS

Status code (101) indicating the server is switching protocols according to Upgrade header.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_SWITCHING_PROTOCOLS)

### SC_OK

static final int SC_OK

Status code (200) indicating the request succeeded normally.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_OK)

### SC_CREATED

static final int SC_CREATED

Status code (201) indicating the request succeeded and created a new resource on the server.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_CREATED)

### SC_ACCEPTED

static final int SC_ACCEPTED

Status code (202) indicating that a request was accepted for processing, but was not completed.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_ACCEPTED)

### SC_NON_AUTHORITATIVE_INFORMATION

static final int SC_NON_AUTHORITATIVE_INFORMATION

Status code (203) indicating that the meta information presented by the client did not originate from the server.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_NON_AUTHORITATIVE_INFORMATION)

### SC_NO_CONTENT

static final int SC_NO_CONTENT

Status code (204) indicating that the request succeeded but that there was no new information to return.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_NO_CONTENT)

### SC_RESET_CONTENT

static final int SC_RESET_CONTENT

Status code (205) indicating that the agent SHOULD reset the document view which caused the request to be sent.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_RESET_CONTENT)

### SC_PARTIAL_CONTENT

static final int SC_PARTIAL_CONTENT

Status code (206) indicating that the server has fulfilled the partial GET request for the resource.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_PARTIAL_CONTENT)

### SC_MULTIPLE_CHOICES

static final int SC_MULTIPLE_CHOICES

Status code (300) indicating that the requested resource corresponds to any one of a set of representations, each with its own specific location.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_MULTIPLE_CHOICES)

### SC_MOVED_PERMANENTLY

static final int SC_MOVED_PERMANENTLY

Status code (301) indicating that the resource has permanently moved to a new location, and that future references should use a new URI with their requests.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_MOVED_PERMANENTLY)

### SC_MOVED_TEMPORARILY

static final int SC_MOVED_TEMPORARILY

Status code (302) indicating that the resource has temporarily moved to another location, but that future references should still use the original URI to access the resource. This definition is being retained for backwards compatibility. SC_FOUND is now the preferred definition.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_MOVED_TEMPORARILY)

### SC_FOUND

static final int SC_FOUND

Status code (302) indicating that the resource reside temporarily under a different URI. Since the redirection might be altered on occasion, the client should continue to use the Request-URI for future requests.(HTTP/1.1) To represent the status code (302), it is recommended to use this variable.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_FOUND)

### SC_SEE_OTHER

static final int SC_SEE_OTHER

Status code (303) indicating that the response to the request can be found under a different URI.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_SEE_OTHER)

### SC_NOT_MODIFIED

static final int SC_NOT_MODIFIED

Status code (304) indicating that a conditional GET operation found that the resource was available and not modified.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_NOT_MODIFIED)

### SC_USE_PROXY

static final int SC_USE_PROXY

Status code (305) indicating that the requested resource MUST be accessed through the proxy given by the Location field.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_USE_PROXY)

### SC_TEMPORARY_REDIRECT

static final int SC_TEMPORARY_REDIRECT

Status code (307) indicating that the requested resource resides temporarily under a different URI. The temporary URI SHOULD be given by the Location field in the response.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_TEMPORARY_REDIRECT)

### SC_BAD_REQUEST

static final int SC_BAD_REQUEST

Status code (400) indicating the request sent by the client was syntactically incorrect.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_BAD_REQUEST)

### SC_UNAUTHORIZED

static final int SC_UNAUTHORIZED

Status code (401) indicating that the request requires HTTP authentication.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_UNAUTHORIZED)

### SC_PAYMENT_REQUIRED

static final int SC_PAYMENT_REQUIRED

Status code (402) reserved for future use.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_PAYMENT_REQUIRED)

### SC_FORBIDDEN

static final int SC_FORBIDDEN

Status code (403) indicating the server understood the request but refused to fulfill it.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_FORBIDDEN)

### SC_NOT_FOUND

static final int SC_NOT_FOUND

Status code (404) indicating that the requested resource is not available.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_NOT_FOUND)

### SC_METHOD_NOT_ALLOWED

static final int SC_METHOD_NOT_ALLOWED

Status code (405) indicating that the method specified in the Request-Line is not allowed for the resource identified by the Request-URI.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_METHOD_NOT_ALLOWED)

### SC_NOT_ACCEPTABLE

static final int SC_NOT_ACCEPTABLE

Status code (406) indicating that the resource identified by the request is only capable of generating response entities which have content characteristics not acceptable according to the accept headers sent in the request.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_NOT_ACCEPTABLE)

### SC_PROXY_AUTHENTICATION_REQUIRED

static final int SC_PROXY_AUTHENTICATION_REQUIRED

Status code (407) indicating that the client MUST first authenticate itself with the proxy.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_PROXY_AUTHENTICATION_REQUIRED)

### SC_REQUEST_TIMEOUT

static final int SC_REQUEST_TIMEOUT

Status code (408) indicating that the client did not produce a request within the time that the server was prepared to wait.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_REQUEST_TIMEOUT)

### SC_CONFLICT

static final int SC_CONFLICT

Status code (409) indicating that the request could not be completed due to a conflict with the current state of the resource.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_CONFLICT)

### SC_GONE

static final int SC_GONE

Status code (410) indicating that the resource is no longer available at the server and no forwarding address is known. This condition SHOULD be considered permanent.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_GONE)

### SC_LENGTH_REQUIRED

static final int SC_LENGTH_REQUIRED

Status code (411) indicating that the request cannot be handled without a defined Content-Length.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_LENGTH_REQUIRED)

### SC_PRECONDITION_FAILED

static final int SC_PRECONDITION_FAILED

Status code (412) indicating that the precondition given in one or more of the request-header fields evaluated to false when it was tested on the server.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_PRECONDITION_FAILED)

### SC_REQUEST_ENTITY_TOO_LARGE

static final int SC_REQUEST_ENTITY_TOO_LARGE

Status code (413) indicating that the server is refusing to process the request because the request entity is larger than the server is willing or able to process.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_REQUEST_ENTITY_TOO_LARGE)

### SC_REQUEST_URI_TOO_LONG

static final int SC_REQUEST_URI_TOO_LONG

Status code (414) indicating that the server is refusing to service the request because the Request-URI is longer than the server is willing to interpret.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_REQUEST_URI_TOO_LONG)

### SC_UNSUPPORTED_MEDIA_TYPE

static final int SC_UNSUPPORTED_MEDIA_TYPE

Status code (415) indicating that the server is refusing to service the request because the entity of the request is in a format not supported by the requested resource for the requested method.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_UNSUPPORTED_MEDIA_TYPE)

### SC_REQUESTED_RANGE_NOT_SATISFIABLE

static final int SC_REQUESTED_RANGE_NOT_SATISFIABLE

Status code (416) indicating that the server cannot serve the requested byte range.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_REQUESTED_RANGE_NOT_SATISFIABLE)

### SC_EXPECTATION_FAILED

static final int SC_EXPECTATION_FAILED

Status code (417) indicating that the server could not meet the expectation given in the Expect request header.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_EXPECTATION_FAILED)

### SC_INTERNAL_SERVER_ERROR

static final int SC_INTERNAL_SERVER_ERROR

Status code (500) indicating an error inside the HTTP server which prevented it from fulfilling the request.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_INTERNAL_SERVER_ERROR)

### SC_NOT_IMPLEMENTED

static final int SC_NOT_IMPLEMENTED

Status code (501) indicating the HTTP server does not support the functionality needed to fulfill the request.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_NOT_IMPLEMENTED)

### SC_BAD_GATEWAY

static final int SC_BAD_GATEWAY

Status code (502) indicating that the HTTP server received an invalid response from a server it consulted when acting as a proxy or gateway.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_BAD_GATEWAY)

### SC_SERVICE_UNAVAILABLE

static final int SC_SERVICE_UNAVAILABLE

Status code (503) indicating that the HTTP server is temporarily overloaded, and unable to handle the request.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_SERVICE_UNAVAILABLE)

### SC_GATEWAY_TIMEOUT

static final int SC_GATEWAY_TIMEOUT

Status code (504) indicating that the server did not receive a timely response from the upstream server while acting as a gateway or proxy.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_GATEWAY_TIMEOUT)

### SC_HTTP_VERSION_NOT_SUPPORTED

static final int SC_HTTP_VERSION_NOT_SUPPORTED

Status code (505) indicating that the server does not support or refuses to support the HTTP protocol version that was used in the request message.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse.SC_HTTP_VERSION_NOT_SUPPORTED)

## Method Details

### addCookie

void addCookie([Cookie](Cookie.md) cookie)

Adds the specified cookie to the response. This method can be called multiple times to set more than one cookie.
  Parameters: cookie - the Cookie to return to the client
### containsHeader

boolean containsHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns a boolean indicating whether the named response header has already been set.
  Parameters: name - the header name Returns: true if the named response header has already been set; false otherwise
### encodeURL

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) encodeURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)

Encodes the specified URL by including the session ID, or, if encoding is not needed, returns the URL unchanged. The implementation of this method includes the logic to determine whether the session ID needs to be encoded in the URL. For example, if the browser supports cookies, or session tracking is turned off, URL encoding is unnecessary.
For robust session tracking, all URLs emitted by a servlet should be run through this method. Otherwise, URL rewriting cannot be used with browsers which do not support cookies.

If the URL is relative, it is always relative to the current HttpServletRequest.

  Parameters: url - the url to be encoded. Returns: the encoded URL if encoding is needed; the unchanged URL otherwise. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if the url is not valid
### encodeRedirectURL

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) encodeRedirectURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)

Encodes the specified URL for use in the sendRedirect method or, if encoding is not needed, returns the URL unchanged. The implementation of this method includes the logic to determine whether the session ID needs to be encoded in the URL. For example, if the browser supports cookies, or session tracking is turned off, URL encoding is unnecessary. Because the rules for making this determination can differ from those used to decide whether to encode a normal link, this method is separated from the encodeURL method.
All URLs sent to the HttpServletResponse.sendRedirect method should be run through this method. Otherwise, URL rewriting cannot be used with browsers which do not support cookies.

If the URL is relative, it is always relative to the current HttpServletRequest.

  Parameters: url - the url to be encoded. Returns: the encoded URL if encoding is needed; the unchanged URL otherwise. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if the url is not valid See Also:
        * [sendRedirect(java.lang.String)](#sendRedirect(java.lang.String))

### sendError

void sendError(int sc, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) msg)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Sends an error response to the client using the specified status and clears the buffer. The server defaults to creating the response to look like an HTML-formatted server error page containing the specified message, setting the content type to "text/html". The caller is not responsible for escaping or re-encoding the message to ensure it is safe with respect to the current response encoding and content type. This aspect of safety is the responsibility of the container, as it is generating the error page containing the message. The server will preserve cookies and may clear or update any headers needed to serve the error page as a valid response.

If an error-page declaration has been made for the web application corresponding to the status code passed in, it will be served back in preference to the suggested msg parameter and the msg parameter will be ignored.

If the response has already been committed, this method throws an IllegalStateException. After using this method, the response should be considered to be committed and should not be written to.
  Parameters: sc - the error status code msg - the descriptive message Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If an input or output exception occurs [IllegalStateException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalStateException.html) - If the response was committed
### sendError

void sendError(int sc)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Sends an error response to the client using the specified status code and clears the buffer. The server will preserve cookies and may clear or update any headers needed to serve the error page as a valid response. If an error-page declaration has been made for the web application corresponding to the status code passed in, it will be served back the error page
If the response has already been committed, this method throws an IllegalStateException. After using this method, the response should be considered to be committed and should not be written to.

  Parameters: sc - the error status code Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If an input or output exception occurs [IllegalStateException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalStateException.html) - If the response was committed before this method call
### sendRedirect

void sendRedirect([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) location)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Sends a temporary redirect response to the client using the specified redirect location URL and clears the buffer. The buffer will be replaced with the data set by this method. Calling this method sets the status code to [SC_FOUND](#SC_FOUND) 302 (Found). This method can accept relative URLs;the servlet container must convert the relative URL to an absolute URL before sending the response to the client. If the location is relative without a leading '/' the container interprets it as relative to the current request URI. If the location is relative with a leading '/' the container interprets it as relative to the servlet container root. If the location is relative with two leading '/' the container interprets it as a network-path reference (see [ RFC 3986: Uniform Resource Identifier (URI): Generic Syntax](http://www.ietf.org/rfc/rfc3986.txt), section 4.2 "Relative Reference").
If the response has already been committed, this method throws an IllegalStateException. After using this method, the response should be considered to be committed and should not be written to.

  Parameters: location - the redirect location URL Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If an input or output exception occurs [IllegalStateException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalStateException.html) - If the response was committed or if a partial URL is given and cannot be converted into a valid URL
### setDateHeader

void setDateHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, long date)

Sets a response header with the given name and date-value. The date is specified in terms of milliseconds since the epoch. If the header had already been set, the new value overwrites the previous one. The containsHeadermethod can be used to test for the presence of a header before setting its value.
  Parameters: name - the name of the header to set date - the assigned date value See Also:
        * [containsHeader(java.lang.String)](#containsHeader(java.lang.String))
        * [addDateHeader(java.lang.String, long)](#addDateHeader(java.lang.String,long))

### addDateHeader

void addDateHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, long date)

Adds a response header with the given name and date-value. The date is specified in terms of milliseconds since the epoch. This method allows response headers to have multiple values.
  Parameters: name - the name of the header to set date - the additional date value See Also:
        * [setDateHeader(java.lang.String, long)](#setDateHeader(java.lang.String,long))

### setHeader

void setHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Sets a response header with the given name and value. If the header had already been set, the new value overwrites the previous one. The containsHeader method can be used to test for the presence of a header before setting its value.
  Parameters: name - the name of the header value - the header value If it contains octet string, it should be encoded according to RFC 2047 (http://www.ietf.org/rfc/rfc2047.txt) See Also:
        * [containsHeader(java.lang.String)](#containsHeader(java.lang.String))
        * [addHeader(java.lang.String, java.lang.String)](#addHeader(java.lang.String,java.lang.String))

### addHeader

void addHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Adds a response header with the given name and value. This method allows response headers to have multiple values.
  Parameters: name - the name of the header value - the additional header value If it contains octet string, it should be encoded according to RFC 2047 (http://www.ietf.org/rfc/rfc2047.txt) See Also:
        * [setHeader(java.lang.String, java.lang.String)](#setHeader(java.lang.String,java.lang.String))

### setIntHeader

void setIntHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int value)

Sets a response header with the given name and integer value. If the header had already been set, the new value overwrites the previous one. The containsHeader method can be used to test for the presence of a header before setting its value.
  Parameters: name - the name of the header value - the assigned integer value See Also:
        * [containsHeader(java.lang.String)](#containsHeader(java.lang.String))
        * [addIntHeader(java.lang.String, int)](#addIntHeader(java.lang.String,int))

### addIntHeader

void addIntHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int value)

Adds a response header with the given name and integer value. This method allows response headers to have multiple values.
  Parameters: name - the name of the header value - the assigned integer value See Also:
        * [setIntHeader(java.lang.String, int)](#setIntHeader(java.lang.String,int))

### setStatus

void setStatus(int sc)

Sets the status code for this response.
This method is used to set the return status code when there is no error (for example, for the SC_OK or SC_MOVED_TEMPORARILY status codes).

If this method is used to set an error code, then the container's error page mechanism will not be triggered. If there is an error and the caller wishes to invoke an error page defined in the web application, then [sendError(int, java.lang.String)](#sendError(int,java.lang.String)) must be used instead.

This method preserves any cookies and other response headers.

Valid status codes are those in the 2XX, 3XX, 4XX, and 5XX ranges. Other status codes are treated as container specific.

  Parameters: sc - the status code See Also:
        * [sendError(int, java.lang.String)](#sendError(int,java.lang.String))

### getStatus

int getStatus()

Gets the current status code of this response.
  Returns: the current status code of this response
### getHeader

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Gets the value of the response header with the given name.
If a response header with the given name exists and contains multiple values, the value that was added first will be returned.

This method considers only response headers set or added via [setHeader(java.lang.String, java.lang.String)](#setHeader(java.lang.String,java.lang.String)), [addHeader(java.lang.String, java.lang.String)](#addHeader(java.lang.String,java.lang.String)), [setDateHeader(java.lang.String, long)](#setDateHeader(java.lang.String,long)), [addDateHeader(java.lang.String, long)](#addDateHeader(java.lang.String,long)), [setIntHeader(java.lang.String, int)](#setIntHeader(java.lang.String,int)), or [addIntHeader(java.lang.String, int)](#addIntHeader(java.lang.String,int)), respectively.

  Parameters: name - the name of the response header whose value to return Returns: the value of the response header with the given name, or null if no header with the given name has been set on this response
### getHeaders

[Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getHeaders([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Gets the values of the response header with the given name.
This method considers only response headers set or added via [setHeader(java.lang.String, java.lang.String)](#setHeader(java.lang.String,java.lang.String)), [addHeader(java.lang.String, java.lang.String)](#addHeader(java.lang.String,java.lang.String)), [setDateHeader(java.lang.String, long)](#setDateHeader(java.lang.String,long)), [addDateHeader(java.lang.String, long)](#addDateHeader(java.lang.String,long)), [setIntHeader(java.lang.String, int)](#setIntHeader(java.lang.String,int)), or [addIntHeader(java.lang.String, int)](#addIntHeader(java.lang.String,int)), respectively.

Any changes to the returned Collection must not affect this HttpServletResponse.

  Parameters: name - the name of the response header whose values to return Returns: a (possibly empty) Collection of the values of the response header with the given name
### getHeaderNames

[Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getHeaderNames()

Gets the names of the headers of this response.
This method considers only response headers set or added via [setHeader(java.lang.String, java.lang.String)](#setHeader(java.lang.String,java.lang.String)), [addHeader(java.lang.String, java.lang.String)](#addHeader(java.lang.String,java.lang.String)), [setDateHeader(java.lang.String, long)](#setDateHeader(java.lang.String,long)), [addDateHeader(java.lang.String, long)](#addDateHeader(java.lang.String,long)), [setIntHeader(java.lang.String, int)](#setIntHeader(java.lang.String,int)), or [addIntHeader(java.lang.String, int)](#addIntHeader(java.lang.String,int)), respectively.

Any changes to the returned Collection must not affect this HttpServletResponse.

  Returns: a (possibly empty) Collection of the names of the headers of this response
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
