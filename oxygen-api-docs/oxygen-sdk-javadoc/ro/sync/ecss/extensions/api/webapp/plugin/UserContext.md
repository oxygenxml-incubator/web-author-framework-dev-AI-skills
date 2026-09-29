Package [ro.sync.ecss.extensions.api.webapp.plugin](package-summary.md)

# Class UserContext

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.plugin.UserContext
   @API(src=PUBLIC, type=NOT_EXTENDABLE) public class UserContext extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The context of the user that opened the URL.
  Since: 17
## Constructor Summary
 Constructors
Constructor

Description
 [UserContext](#%3Cinit%3E(java.util.Map,java.lang.String))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> headersMap, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId)

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getCookies](#getCookies())()

 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getHeaders](#getHeaders())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSessionId](#getSessionId())()

 boolean [isServiceAccount](#isServiceAccount())()
UserContext is used both for real users connected with their web browser and for plugins that try to open an URL on their own behalf.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### UserContext

public UserContext([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> headersMap, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId)
  Parameters: headersMap - The cookies that are part of the context of this URL. sessionId - The session ID of the user.
## Method Details

### getCookies

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getCookies()
  Returns: Returns the cookies.
### getHeaders

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getHeaders()
  Returns: the an immutable request headers map.
### getSessionId

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSessionId()
  Returns: The id of the session of the user maintained by the Servlet container.
### isServiceAccount

public boolean isServiceAccount()

UserContext is used both for real users connected with their web browser and for plugins that try to open an URL on their own behalf. For example, in a concurrent editing session, users join and leave. In order to have a robust way to save changes, a plugin may choose to use a dedicated set of credentials that do not belong to any of those users. Such credentials belong to a "service account".
  Returns: false if the user context represents a real user connected with their web browser.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
