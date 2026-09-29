Package [ro.sync.ecss.extensions.api.webapp.plugin](package-summary.md)

# Class UserActionRequiredException

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html)
        * [java.lang.Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
            * [java.io.IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
                * ro.sync.ecss.extensions.api.webapp.plugin.UserActionRequiredException
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)   @API(src=PUBLIC, type=NOT_EXTENDABLE) public class UserActionRequiredException extends [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
Class that extends an IOException with an WebappMessage that should be sent to the client-side code.
  Since: 17 See Also:
* [Serialized Form](../../../../../../../serialized-form.md#ro.sync.ecss.extensions.api.webapp.plugin.UserActionRequiredException)

## Constructor Summary
 Constructors
Constructor

Description
 [UserActionRequiredException](#%3Cinit%3E(ro.sync.ecss.extensions.api.webapp.WebappMessage))([WebappMessage](../WebappMessage.md) webappMessage)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [WebappMessage](../WebappMessage.md) [getUserMessage](#getUserMessage())()
The message to be sent to the client-side code.
  [UserActionRequiredMessage](UserActionRequiredMessage.md) [getUserMessage](#getUserMessage(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
The message to be sent to the client-side code.

### Methods inherited from class java.lang.[Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html)
 [addSuppressed](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#addSuppressed(java.lang.Throwable)), [fillInStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#fillInStackTrace()), [getCause](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getCause()), [getLocalizedMessage](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getLocalizedMessage()), [getMessage](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getMessage()), [getStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getStackTrace()), [getSuppressed](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getSuppressed()), [initCause](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#initCause(java.lang.Throwable)), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace()), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace(java.io.PrintStream)), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace(java.io.PrintWriter)), [setStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#setStackTrace(java.lang.StackTraceElement%5B%5D)), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#toString())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### UserActionRequiredException

public UserActionRequiredException([WebappMessage](../WebappMessage.md) webappMessage)

Constructor.
  Parameters: webappMessage - The webapp message.
## Method Details

### getUserMessage

public [WebappMessage](../WebappMessage.md) getUserMessage()

The message to be sent to the client-side code.
  Returns: The webapp message.
### getUserMessage

public [UserActionRequiredMessage](UserActionRequiredMessage.md) getUserMessage([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

The message to be sent to the client-side code.
  Parameters: url - The URL of the resource for which the user action required exception is thrown. Returns: The webapp message.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
