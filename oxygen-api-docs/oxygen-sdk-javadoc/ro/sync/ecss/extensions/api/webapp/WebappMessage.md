Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Class WebappMessage

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.WebappMessage
   Direct Known Subclasses: [UserActionRequiredMessage](plugin/UserActionRequiredMessage.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class WebappMessage extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Webapp server message that is presented on client side.
  Since: 16.0
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [MESSAGE_TYPE_CUSTOM](#MESSAGE_TYPE_CUSTOM)
A message type that is the lowest designed to be intercepted by the plugin code on the client side and displayed in a custom way.
  static final int [MESSAGE_TYPE_ERROR](#MESSAGE_TYPE_ERROR)
Message type error.
  static final int [MESSAGE_TYPE_INFO](#MESSAGE_TYPE_INFO)
Message type info.
  static final int [MESSAGE_TYPE_RESULT_VALUE](#MESSAGE_TYPE_RESULT_VALUE)
This message represents a return value from an WebappAuthorOperation.
  static final int [MESSAGE_TYPE_SYSTEM_APPLICATION](#MESSAGE_TYPE_SYSTEM_APPLICATION)
A message type that should be handled by the webapp to open the url in the system application as it cannot be opened server-side.
  static final int [MESSAGE_TYPE_WARN](#MESSAGE_TYPE_WARN)
Message type warning.

## Constructor Summary
 Constructors
Constructor

Description
 [WebappMessage](#%3Cinit%3E(int,java.lang.String,java.lang.String,boolean))(int type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, boolean isUserGenerated)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessage](#getMessage())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTitle](#getTitle())()

 int [getType](#getType())()

 int [hashCode](#hashCode())()

 boolean [isUserGenerated](#isUserGenerated())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### MESSAGE_TYPE_RESULT_VALUE

public static final int MESSAGE_TYPE_RESULT_VALUE

This message represents a return value from an WebappAuthorOperation.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.WebappMessage.MESSAGE_TYPE_RESULT_VALUE)

### MESSAGE_TYPE_SYSTEM_APPLICATION

public static final int MESSAGE_TYPE_SYSTEM_APPLICATION

A message type that should be handled by the webapp to open the url in the system application as it cannot be opened server-side.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.WebappMessage.MESSAGE_TYPE_SYSTEM_APPLICATION)

### MESSAGE_TYPE_INFO

public static final int MESSAGE_TYPE_INFO

Message type info.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.WebappMessage.MESSAGE_TYPE_INFO)

### MESSAGE_TYPE_WARN

public static final int MESSAGE_TYPE_WARN

Message type warning.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.WebappMessage.MESSAGE_TYPE_WARN)

### MESSAGE_TYPE_ERROR

public static final int MESSAGE_TYPE_ERROR

Message type error.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.WebappMessage.MESSAGE_TYPE_ERROR)

### MESSAGE_TYPE_CUSTOM

public static final int MESSAGE_TYPE_CUSTOM

A message type that is the lowest designed to be intercepted by the plugin code on the client side and displayed in a custom way. All message types larger than this one are not handled by default by the webapp, but passed to the plugin code handlers.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.WebappMessage.MESSAGE_TYPE_CUSTOM)

## Constructor Details

### WebappMessage

public WebappMessage(int type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, boolean isUserGenerated)

Constructor.
  Parameters: type - Message type. title - Message title. message - Message body. isUserGenerated - true if the message was generated by the user and should be presented in UI.
## Method Details

### getMessage

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessage()
  Returns: Returns the message.
### getTitle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTitle()
  Returns: Returns the title.
### getType

public int getType()
  Returns: Returns the type.
### isUserGenerated

public boolean isUserGenerated()
  Returns: Returns the isUserGenerated.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
