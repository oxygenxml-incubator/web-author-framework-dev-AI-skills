Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorActionEventDetails

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorActionEventDetails
   @API(type=EXTENDABLE, src=PUBLIC) public class AuthorActionEventDetails extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Class offering details about an author action event.
  Since: 23
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorActionEventDetails](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType,boolean))([AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) eventType, boolean showContentCompletionWindowOnEnter)
Class containing information on an author action event.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) [getEventType](#getEventType())()

 boolean [isShowContentCompletionWindowOnEnter](#isShowContentCompletionWindowOnEnter())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorActionEventDetails

public AuthorActionEventDetails([AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) eventType, boolean showContentCompletionWindowOnEnter)

Class containing information on an author action event.
  Parameters: eventType - the event type. showContentCompletionWindowOnEnter - true if the content completion window should be shown when ENTER is pressed.
## Method Details

### getEventType

public [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) getEventType()
  Returns: Returns the eventType.
### isShowContentCompletionWindowOnEnter

public boolean isShowContentCompletionWindowOnEnter()
  Returns: Returns true if the content completion window will be shown when ENTER is pressed. This setting is controlled by the "Press ENTER to show available content completion proposals" checkbox.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
