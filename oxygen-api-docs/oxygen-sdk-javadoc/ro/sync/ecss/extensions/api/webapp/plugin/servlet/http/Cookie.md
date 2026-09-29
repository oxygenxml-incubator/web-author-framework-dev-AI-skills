Package [ro.sync.ecss.extensions.api.webapp.plugin.servlet.http](package-summary.md)

# Interface Cookie
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface Cookie
Cookie interface inspired from HTTP Servlet 5.0.
  Since: 26
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getComment](#getComment())()
Returns the comment describing the purpose of this cookie, or null if the cookie has no comment.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDomain](#getDomain())()
Gets the domain name of this Cookie.
  int [getMaxAge](#getMaxAge())()
Gets the maximum age in seconds of this Cookie.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Returns the name of the cookie.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPath](#getPath())()
Returns the path on the server to which the browser returns this cookie.
  boolean [getSecure](#getSecure())()
Returns true if the browser is sending cookies only over a secure protocol, or false if the browser can send cookies using any protocol.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getValue](#getValue())()
Gets the current value of this Cookie.
  int [getVersion](#getVersion())()
Returns the version of the protocol this cookie complies with.
  boolean [isHttpOnly](#isHttpOnly())()
Checks whether this Cookie has been marked as *HttpOnly*.
  void [setComment](#setComment(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) purpose)
Specifies a comment that describes a cookie's purpose.
  void [setDomain](#setDomain(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) domain)
Specifies the domain within which this cookie should be presented.
  void [setHttpOnly](#setHttpOnly(boolean))(boolean isHttpOnly)
Marks or unmarks this Cookie as *HttpOnly*.
  void [setMaxAge](#setMaxAge(int))(int expiry)
Sets the maximum age in seconds for this Cookie.
  void [setPath](#setPath(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri)
Specifies a path for the cookie to which the client should return the cookie.
  void [setSecure](#setSecure(boolean))(boolean flag)
Indicates to the browser whether the cookie should only be sent using a secure protocol, such as HTTPS or SSL.
  void [setValue](#setValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newValue)
Assigns a new value to this Cookie.
  void [setVersion](#setVersion(int))(int v)
Sets the version of the cookie protocol that this Cookie complies with.

## Method Details

### setComment

void setComment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) purpose)

Specifies a comment that describes a cookie's purpose. The comment is useful if the browser presents the cookie to the user. Comments are not supported by Netscape Version 0 cookies.
  Parameters: purpose - a String specifying the comment to display to the user See Also:
        * [getComment()](#getComment())

### getComment

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getComment()

Returns the comment describing the purpose of this cookie, or null if the cookie has no comment.
  Returns: the comment of the cookie, or null if unspecified See Also:
        * [setComment(java.lang.String)](#setComment(java.lang.String))

### setDomain

void setDomain([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) domain)

Specifies the domain within which this cookie should be presented.
The form of the domain name is specified by RFC 2109. A domain name begins with a dot (.foo.com) and means that the cookie is visible to servers in a specified Domain Name System (DNS) zone (for example, www.foo.com, but not a.b.foo.com). By default, cookies are only returned to the server that sent them.

  Parameters: domain - the domain name within which this cookie is visible; form is according to RFC 2109 See Also:
        * [getDomain()](#getDomain())

### getDomain

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDomain()

Gets the domain name of this Cookie.
Domain names are formatted according to RFC 2109.

  Returns: the domain name of this Cookie See Also:
        * [setDomain(java.lang.String)](#setDomain(java.lang.String))

### setMaxAge

void setMaxAge(int expiry)

Sets the maximum age in seconds for this Cookie.
A positive value indicates that the cookie will expire after that many seconds have passed. Note that the value is the *maximum* age when the cookie will expire, not the cookie's current age.

A negative value means that the cookie is not stored persistently and will be deleted when the Web browser exits. A zero value causes the cookie to be deleted.

  Parameters: expiry - an integer specifying the maximum age of the cookie in seconds; if negative, means the cookie is not stored; if zero, deletes the cookie See Also:
        * [getMaxAge()](#getMaxAge())

### getMaxAge

int getMaxAge()

Gets the maximum age in seconds of this Cookie.
By default, -1 is returned, which indicates that the cookie will persist until browser shutdown.

  Returns: an integer specifying the maximum age of the cookie in seconds; if negative, means the cookie persists until browser shutdown See Also:
        * [setMaxAge(int)](#setMaxAge(int))

### setPath

void setPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uri)

Specifies a path for the cookie to which the client should return the cookie.
The cookie is visible to all the pages in the directory you specify, and all the pages in that directory's subdirectories. A cookie's path must include the servlet that set the cookie, for example, */catalog*, which makes the cookie visible to all directories on the server under */catalog*.

Consult RFC 2109 (available on the Internet) for more information on setting path names for cookies.

  Parameters: uri - a String specifying a path See Also:
        * [getPath()](#getPath())

### getPath

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPath()

Returns the path on the server to which the browser returns this cookie. The cookie is visible to all subpaths on the server.
  Returns: a String specifying a path that contains a servlet name, for example, */catalog* See Also:
        * [setPath(java.lang.String)](#setPath(java.lang.String))

### setSecure

void setSecure(boolean flag)

Indicates to the browser whether the cookie should only be sent using a secure protocol, such as HTTPS or SSL.
The default value is false.

  Parameters: flag - if true, sends the cookie from the browser to the server only when using a secure protocol; if false, sent on any protocol See Also:
        * [getSecure()](#getSecure())

### getSecure

boolean getSecure()

Returns true if the browser is sending cookies only over a secure protocol, or false if the browser can send cookies using any protocol.
  Returns: true if the browser uses a secure protocol, false otherwise See Also:
        * [setSecure(boolean)](#setSecure(boolean))

### getName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

Returns the name of the cookie. The name cannot be changed after creation.
  Returns: the name of the cookie
### setValue

void setValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newValue)

Assigns a new value to this Cookie.
If you use a binary value, you may want to use BASE64 encoding.

With Version 0 cookies, values should not contain white space, brackets, parentheses, equals signs, commas, double quotes, slashes, question marks, at signs, colons, and semicolons. Empty values may not behave the same way on all browsers.

  Parameters: newValue - the new value of the cookie See Also:
        * [getValue()](#getValue())

### getValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getValue()

Gets the current value of this Cookie.
  Returns: the current value of this Cookie See Also:
        * [setValue(java.lang.String)](#setValue(java.lang.String))

### getVersion

int getVersion()

Returns the version of the protocol this cookie complies with. Version 1 complies with RFC 2109, and version 0 complies with the original cookie specification drafted by Netscape. Cookies provided by a browser use and identify the browser's cookie version.
  Returns: 0 if the cookie complies with the original Netscape specification; 1 if the cookie complies with RFC 2109 See Also:
        * [setVersion(int)](#setVersion(int))

### setVersion

void setVersion(int v)

Sets the version of the cookie protocol that this Cookie complies with.
Version 0 complies with the original Netscape cookie specification. Version 1 complies with RFC 2109.

Since RFC 2109 is still somewhat new, consider version 1 as experimental; do not use it yet on production sites.

  Parameters: v - 0 if the cookie should comply with the original Netscape specification; 1 if the cookie should comply with RFC 2109 See Also:
        * [getVersion()](#getVersion())

### setHttpOnly

void setHttpOnly(boolean isHttpOnly)

Marks or unmarks this Cookie as *HttpOnly*.
If isHttpOnly is set to true, this cookie is marked as *HttpOnly*, by adding the HttpOnly attribute to it.

 *HttpOnly* cookies are not supposed to be exposed to client-side scripting code, and may therefore help mitigate certain kinds of cross-site scripting attacks.

  Parameters: isHttpOnly - true if this cookie is to be marked as *HttpOnly*, false otherwise
### isHttpOnly

boolean isHttpOnly()

Checks whether this Cookie has been marked as *HttpOnly*.
  Returns: true if this Cookie has been marked as *HttpOnly*, false otherwise
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
