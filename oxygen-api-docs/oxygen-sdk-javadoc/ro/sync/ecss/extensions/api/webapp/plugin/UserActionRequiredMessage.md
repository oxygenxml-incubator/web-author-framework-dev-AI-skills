Package [ro.sync.ecss.extensions.api.webapp.plugin](package-summary.md)

# Class UserActionRequiredMessage

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.webapp.WebappMessage](../WebappMessage.md)
        * ro.sync.ecss.extensions.api.webapp.plugin.UserActionRequiredMessage
   @API(src=PUBLIC, type=NOT_EXTENDABLE) public class UserActionRequiredMessage extends [WebappMessage](../WebappMessage.md)
Contains details for the server message that is presented on client side when a user action required exception is thrown.
  Since: 21
## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.api.webapp.[WebappMessage](../WebappMessage.md)
 [MESSAGE_TYPE_CUSTOM](../WebappMessage.md#MESSAGE_TYPE_CUSTOM), [MESSAGE_TYPE_ERROR](../WebappMessage.md#MESSAGE_TYPE_ERROR), [MESSAGE_TYPE_INFO](../WebappMessage.md#MESSAGE_TYPE_INFO), [MESSAGE_TYPE_RESULT_VALUE](../WebappMessage.md#MESSAGE_TYPE_RESULT_VALUE), [MESSAGE_TYPE_SYSTEM_APPLICATION](../WebappMessage.md#MESSAGE_TYPE_SYSTEM_APPLICATION), [MESSAGE_TYPE_WARN](../WebappMessage.md#MESSAGE_TYPE_WARN)
## Constructor Summary
 Constructors
Constructor

Description
 [UserActionRequiredMessage](#%3Cinit%3E(ro.sync.ecss.extensions.api.webapp.WebappMessage,java.lang.String))([WebappMessage](../WebappMessage.md) webappMessage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextUrl)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getUrl](#getUrl())()

### Methods inherited from class ro.sync.ecss.extensions.api.webapp.[WebappMessage](../WebappMessage.md)
 [equals](../WebappMessage.md#equals(java.lang.Object)), [getMessage](../WebappMessage.md#getMessage()), [getTitle](../WebappMessage.md#getTitle()), [getType](../WebappMessage.md#getType()), [hashCode](../WebappMessage.md#hashCode()), [isUserGenerated](../WebappMessage.md#isUserGenerated()), [toString](../WebappMessage.md#toString())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### UserActionRequiredMessage

public UserActionRequiredMessage([WebappMessage](../WebappMessage.md) webappMessage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextUrl)

Constructor.
  Parameters: webappMessage - The server message that is presented on client side contextUrl - The URL of the resource for which the user action required exception is thrown.
## Method Details

### getUrl

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getUrl()
  Returns: Returns the URL of the resource for which the user action required exception is thrown.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
