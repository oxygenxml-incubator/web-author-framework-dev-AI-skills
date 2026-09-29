Package [ro.sync.ecss.extensions.api.webapp.plugin](package-summary.md)

# Class URLStreamHandlerWithContext

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.net.URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html)
        * ro.sync.ecss.extensions.api.webapp.plugin.URLStreamHandlerWithContext
   @API(src=PUBLIC, type=EXTENDABLE) public abstract class URLStreamHandlerWithContext extends [URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html)
A base-class for URLStreamHandlers that need a context for the URL whose connection is to be opened. It is implemented by adding a user context id to the URL in the userInfo section. The context id should remain unchanged while the user edits a document. The user context contains information about the cookies and HTTP headers sent by the user. For openConnection calls, the context id passed along. You can use it to retrieve information about the user on behalf of which the request is made.
  Since: 17
## Constructor Summary
 Constructors
Modifier

Constructor

Description
 protected  [URLStreamHandlerWithContext](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContextId](#getContextId(ro.sync.ecss.extensions.api.webapp.plugin.UserContext))([UserContext](UserContext.md) context)
Computes the context id based on the user context.
  int [hashCode](#hashCode(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) u)

 protected boolean [hostsEqual](#hostsEqual(java.net.URL,java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) u1, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) u2)

 protected final [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) [openConnection](#openConnection(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) u)

 protected final [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) [openConnection](#openConnection(java.net.URL,java.net.Proxy))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) u, [Proxy](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/Proxy.html) p)

 protected abstract [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) [openConnectionInContext](#openConnectionInContext(java.lang.String,java.net.URL,java.net.Proxy))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Proxy](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/Proxy.html) proxy)
This method has the same purpose as openConnection() in a standard URLConnection except that the context is also passed in.

### Methods inherited from class java.net.[URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html)
 [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#equals(java.net.URL,java.net.URL)), [getDefaultPort](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#getDefaultPort()), [getHostAddress](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#getHostAddress(java.net.URL)), [parseURL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#parseURL(java.net.URL,java.lang.String,int,int)), [sameFile](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#sameFile(java.net.URL,java.net.URL)), [setURL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#setURL(java.net.URL,java.lang.String,java.lang.String,int,java.lang.String,java.lang.String)), [setURL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#setURL(java.net.URL,java.lang.String,java.lang.String,int,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String)), [toExternalForm](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#toExternalForm(java.net.URL))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### URLStreamHandlerWithContext

protected URLStreamHandlerWithContext()

Constructor. It uses the session cookie of the Servlet container as a context id.

## Method Details

### getContextId

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContextId([UserContext](UserContext.md) context)

Computes the context id based on the user context. By default, it uses the id of the session managed by the Servlet container.
  Parameters: context - The UserContext. Returns: The context id.
### openConnection

protected final [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) openConnection([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) u, [Proxy](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/Proxy.html) p)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
  Overrides: [openConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#openConnection(java.net.URL,java.net.Proxy)) in class [URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html) Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) See Also:
        * [URLStreamHandler.openConnection(java.net.URL, java.net.Proxy)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#openConnection(java.net.URL,java.net.Proxy))

### openConnection

protected final [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) openConnection([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) u)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
  Specified by: [openConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#openConnection(java.net.URL)) in class [URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html) Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) See Also:
        * [URLStreamHandler.openConnection(java.net.URL)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#openConnection(java.net.URL))

### openConnectionInContext

protected abstract [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) openConnectionInContext([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Proxy](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/Proxy.html) proxy)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

This method has the same purpose as openConnection() in a standard URLConnection except that the context is also passed in. If the connection, or one of the following IO operations on it need some user interaction like providing credentials, they should throw an IOException that also implements the UserActionRequiredException. The message of the IOException will still be rendered in different places, but the instance of WebappMessage found in the UserActionRequiredException will be used to present an authentication dialog to the users. This message needs to be handled in JavaScript by the plugin code. If no JS handler is registered, the message will just be displayed in the browser console.
  Parameters: contextId - The id of the context. url - The URL to connect to. proxy - The proxy to use. May be null. Returns: The connection. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the connection fails.
### hashCode

public int hashCode([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) u)
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#hashCode(java.net.URL)) in class [URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html) See Also:
        * [URLStreamHandler.hashCode(java.net.URL)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#hashCode(java.net.URL))

### hostsEqual

protected boolean hostsEqual([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) u1, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) u2)
  Overrides: [hostsEqual](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#hostsEqual(java.net.URL,java.net.URL)) in class [URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html) See Also:
        * [URLStreamHandler.hostsEqual(java.net.URL, java.net.URL)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html#hostsEqual(java.net.URL,java.net.URL))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
