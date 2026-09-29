Package [ro.sync.ecss.extensions.api.webapp.plugin](package-summary.md)

# Class URLStreamHandlerWithContextUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.plugin.URLStreamHandlerWithContextUtil
   @API(src=PUBLIC, type=EXTENDABLE) public class URLStreamHandlerWithContextUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Utility class for adding/removing the user context id from the URLs. The context ID is typically added when the user asks the webapp to open an URL and is stripped before displaying a URL to the user.
  Since: 17
## Constructor Summary
 Constructors
Constructor

Description
 [URLStreamHandlerWithContextUtil](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [clearCacheForTC](#clearCacheForTC())()
Clears the handlers cache.
  void [copyContextId](#copyContextId(java.net.URL,java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) source, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) target)
Method called to copy the context ID of a source URL to a target one.
  static [URLStreamHandlerWithContextUtil](URLStreamHandlerWithContextUtil.md) [getInstance](#getInstance())()

 void [setUserContext](#setUserContext(ro.sync.ecss.extensions.api.webapp.plugin.UserContext,java.net.URL))([UserContext](UserContext.md) context, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Method called to set the context of an URL.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toStrippedExternalForm](#toStrippedExternalForm(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
If the URL contains a context id (set by a URLStreamHandlerWithContext), this method strips it, otherwise it simply returns the URL.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### URLStreamHandlerWithContextUtil

public URLStreamHandlerWithContextUtil()

Constructor.

## Method Details

### getInstance

public static [URLStreamHandlerWithContextUtil](URLStreamHandlerWithContextUtil.md) getInstance()
  Returns: Returns the singleton instance.
### setUserContext

public void setUserContext([UserContext](UserContext.md) context, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Method called to set the context of an URL. If the URL handler for this URL is an URLStreamHandlerWithContext, it is used to set the context for the URL, otherwise the URL is left unmodified. Note: If the URL already has a context, the newly set context must have the same id.
  Parameters: context - The context. url - The URL. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)
### copyContextId

public void copyContextId([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) source, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) target)

Method called to copy the context ID of a source URL to a target one. If the two URLs have different protocols, this method does nothing.
  Parameters: source - The URL from which to copy the user context id. target - The URL where to copy the user context id.
### toStrippedExternalForm

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toStrippedExternalForm([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

If the URL contains a context id (set by a URLStreamHandlerWithContext), this method strips it, otherwise it simply returns the URL.
  Parameters: url - The URL with the context id. Returns: The stripped URL.
### clearCacheForTC

public void clearCacheForTC()

Clears the handlers cache. Note: To be used only from TC.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
