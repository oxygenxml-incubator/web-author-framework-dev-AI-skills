Package [ro.sync.net.protocol.http](package-summary.md)

# Class HttpExceptionWithDetails

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html)
        * [java.lang.Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
            * [java.io.IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
                * ro.sync.basic.net.http.HttpException
                    * ro.sync.net.protocol.http.HttpExceptionWithDetails
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class HttpExceptionWithDetails extends ro.sync.basic.net.http.HttpException
HTTP Exception with details.
  Since: 25.0 See Also:
* [Serialized Form](../../../../../serialized-form.md#ro.sync.net.protocol.http.HttpExceptionWithDetails)

## Constructor Summary
 Constructors
Constructor

Description
 [HttpExceptionWithDetails](#%3Cinit%3E(java.lang.String,int,java.lang.String,java.net.URL))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, int reasonCode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reason, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL)
Constructor
  [HttpExceptionWithDetails](#%3Cinit%3E(java.lang.String,int,java.lang.String,java.net.URL,ro.sync.net.protocol.http.abstraction.HttpResponse))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, int reasonCode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reason, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, ro.sync.net.protocol.http.abstraction.HttpResponse httpResponse)
Constructor

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getBaseURL](#getBaseURL())()
Gets the base URL.
  ro.sync.net.protocol.http.abstraction.HttpResponse [getHttpResponse](#getHttpResponse())()
Gets the httpResponse.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReason](#getReason())()

 void [setBaseURL](#setBaseURL(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL)
Set the URL for which the message is reported.
  void [setHttpResponse](#setHttpResponse(ro.sync.net.protocol.http.abstraction.HttpResponse))(ro.sync.net.protocol.http.abstraction.HttpResponse httpResponse)
Sets the httpResponse.

### Methods inherited from class ro.sync.basic.net.http.HttpException
 getReasonCode, setReason, setReasonCode
### Methods inherited from class java.lang.[Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html)
 [addSuppressed](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#addSuppressed(java.lang.Throwable)), [fillInStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#fillInStackTrace()), [getCause](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getCause()), [getLocalizedMessage](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getLocalizedMessage()), [getMessage](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getMessage()), [getStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getStackTrace()), [getSuppressed](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getSuppressed()), [initCause](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#initCause(java.lang.Throwable)), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace()), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace(java.io.PrintStream)), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace(java.io.PrintWriter)), [setStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#setStackTrace(java.lang.StackTraceElement%5B%5D)), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#toString())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### HttpExceptionWithDetails

public HttpExceptionWithDetails([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, int reasonCode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reason, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL)

Constructor
  Parameters: message - The message. reasonCode - The reason status code. reason - The reason text. baseURL - The URL for which the message is reported.
### HttpExceptionWithDetails

public HttpExceptionWithDetails([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, int reasonCode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reason, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, ro.sync.net.protocol.http.abstraction.HttpResponse httpResponse)

Constructor
  Parameters: message - The message. reasonCode - The reason status code. reason - The reason text. baseURL - The URL for which the message is reported. httpResponse - The httpResponse of the request that threw this HttpException.
## Method Details

### setBaseURL

public void setBaseURL([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL)

Set the URL for which the message is reported.
  Parameters: baseURL - The URL for which the message is reported.
### getBaseURL

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getBaseURL()

Gets the base URL.
  Returns: The base URL.
### setHttpResponse

public void setHttpResponse(ro.sync.net.protocol.http.abstraction.HttpResponse httpResponse)

Sets the httpResponse.
  Parameters: httpResponse - The httpResponse to set.
### getHttpResponse

public ro.sync.net.protocol.http.abstraction.HttpResponse getHttpResponse()

Gets the httpResponse.
  Returns: Returns the httpResponse.
### getReason

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReason()
  Overrides: getReason in class ro.sync.basic.net.http.HttpException Returns: Returns the reason given by the server.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
