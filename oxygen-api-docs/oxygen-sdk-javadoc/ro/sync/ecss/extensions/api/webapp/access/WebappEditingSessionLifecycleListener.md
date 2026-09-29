Package [ro.sync.ecss.extensions.api.webapp.access](package-summary.md)

# Class WebappEditingSessionLifecycleListener

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.access.WebappEditingSessionLifecycleListener
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class WebappEditingSessionLifecycleListener extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Listener for the main lifecycle events of an editing session. The lifecycle is influenced by the fact that we cannot safely detect when the users closed the application and that the users may have a lot of instances of the application open. In order to optimize memory consumption, we serialize editing sessions to disk sometimes (after periods of inactivity or if there are too many concurrent sessions). However, the moment when the session gets serialized can be configured separately. This listener can be registered on [WebappPluginWorkspace](WebappPluginWorkspace.md).
  Since: 17
## Constructor Summary
 Constructors
Constructor

Description
 [WebappEditingSessionLifecycleListener](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [editingSessionAboutToBeSerialized](#editingSessionAboutToBeSerialized(java.lang.String,ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editingSessionId, [AuthorDocumentModel](../AuthorDocumentModel.md) documentModel)
The editing session was serialized to disk in order to free memory space.
  void [editingSessionAboutToBeStarted](#editingSessionAboutToBeStarted(java.lang.String,java.lang.String,java.net.URL,java.util.Map))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editingSessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) licenseeId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemId, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> options)
Method called when a new editing session is about to be started.
  void [editingSessionClosed](#editingSessionClosed(java.lang.String,ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editingSessionId, [AuthorDocumentModel](../AuthorDocumentModel.md) documentModel)
The session was closed by the user.
  void [editingSessionDeserialized](#editingSessionDeserialized(java.lang.String,ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editingSessionId, [AuthorDocumentModel](../AuthorDocumentModel.md) documentModel)
The editing session was deserialized because the user made some changes to it.
  void [editingSessionFailedToStart](#editingSessionFailedToStart(java.lang.String,java.lang.String,java.net.URL,java.util.Map))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editingSessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) licenseeId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemId, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> options)
Method called when a new editing session failed to start.
  void [editingSessionStarted](#editingSessionStarted(java.lang.String,ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editingSessionId, [AuthorDocumentModel](../AuthorDocumentModel.md) documentModel)
Method called when the editing session has already started.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WebappEditingSessionLifecycleListener

public WebappEditingSessionLifecycleListener()

## Method Details

### editingSessionAboutToBeStarted

public void editingSessionAboutToBeStarted([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editingSessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) licenseeId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemId, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> options)throws [EditingSessionOpenVetoException](EditingSessionOpenVetoException.md)

Method called when a new editing session is about to be started. If it throws a EditingSessionOpenVetoException, the details in the exception will be presented to the user.
  Parameters: editingSessionId - The id of the editing session in which the editing of the opened document happens. licenseeId - The id of the user or browser that uses a license. If the application cannot authenticate the user, it allocates the license to a specific browser. systemId - The system id of the XML document about to be opened. options - The options containing - the cookies used for the document load request - the key is the cookie name prefixed with 'cookie-' - the value is a String - the other HTTP headers - the key is the header name prefixed with "header-" - the value is a list of strings. - the session id set by the Servlet container with the key: "session-id". - options set explicitly by the client JS code, the value being a string. Throws: [EditingSessionOpenVetoException](EditingSessionOpenVetoException.md) - When implementation decides that the editing session should not be started.
### editingSessionFailedToStart

public void editingSessionFailedToStart([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editingSessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) licenseeId, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) systemId, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> options)

Method called when a new editing session failed to start.
  Parameters: editingSessionId - The id of the editing session in which the editing was supposed to happen. licenseeId - The licensee id of the user that opened the document. systemId - The system id of the XML document about to be opened. options - The options passed on the [editingSessionAboutToBeStarted(String, String, URL, Map)](#editingSessionAboutToBeStarted(java.lang.String,java.lang.String,java.net.URL,java.util.Map)) method. Since: 23
### editingSessionStarted

public void editingSessionStarted([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editingSessionId, [AuthorDocumentModel](../AuthorDocumentModel.md) documentModel)

Method called when the editing session has already started.
  Parameters: editingSessionId - The if of the editing session. documentModel - The model of the edited document. From it one can derive the URL and the options used to open it. For the URL : documentModel.getAuthorDocumentController().getAuthorDocumentNode().getSystemID() For the editing session options: documentModel.getAuthorAccess().getEditorAccess().getEditingContext() This document model may change during the lifetime of the session as it is inactivated and activated back.
### editingSessionClosed

public void editingSessionClosed([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editingSessionId, [AuthorDocumentModel](../AuthorDocumentModel.md) documentModel)

The session was closed by the user. Note that on some platforms, the user may close the browser without triggering this event.
  Parameters: editingSessionId - The id of the editing session. documentModel - The model of the edited document.
### editingSessionAboutToBeSerialized

public void editingSessionAboutToBeSerialized([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editingSessionId, [AuthorDocumentModel](../AuthorDocumentModel.md) documentModel)

The editing session was serialized to disk in order to free memory space. After this method is called, the document model given as a parameter cannot be used anymore.
  Parameters: editingSessionId - The id of the editing session. documentModel - The model of edited document.
### editingSessionDeserialized

public void editingSessionDeserialized([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editingSessionId, [AuthorDocumentModel](../AuthorDocumentModel.md) documentModel)

The editing session was deserialized because the user made some changes to it.
  Parameters: editingSessionId - The id of the editing session. documentModel - The document model may not be the same as the one created when the editing session was opened.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
