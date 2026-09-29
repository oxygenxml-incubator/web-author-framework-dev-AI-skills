Package [ro.sync.exml.plugin.workspace.security](package-summary.md)

# Class Response

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.plugin.workspace.security.Response
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class Response extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
A response describing what this provider knows about this host.
  Since: 22
## Constructor Summary
 Constructors
Constructor

Description
 [Response](#%3Cinit%3E(ro.sync.ui.application.security.ResponseType))([ResponseType](../../../../ui/application/security/ResponseType.md) responseType)
Constructor.
  [Response](#%3Cinit%3E(ro.sync.ui.application.security.ResponseType,java.lang.String))([ResponseType](../../../../ui/application/security/ResponseType.md) responseType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reason)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReason](#getReason())()

 [ResponseType](../../../../ui/application/security/ResponseType.md) [getResponseType](#getResponseType())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### Response

public Response([ResponseType](../../../../ui/application/security/ResponseType.md) responseType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reason)

Constructor.
  Parameters: responseType - The response types. reason - A reason why this response was given for a particular host.
### Response

public Response([ResponseType](../../../../ui/application/security/ResponseType.md) responseType)

Constructor.
  Parameters: responseType - The response types.
## Method Details

### getReason

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReason()
  Returns: The reason why this response was given for a particular host.
### getResponseType

public [ResponseType](../../../../ui/application/security/ResponseType.md) getResponseType()
  Returns: Returns the responseType.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
