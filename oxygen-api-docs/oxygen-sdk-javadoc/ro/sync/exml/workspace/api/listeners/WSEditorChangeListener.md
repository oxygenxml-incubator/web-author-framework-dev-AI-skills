Package [ro.sync.exml.workspace.api.listeners](package-summary.md)

# Class WSEditorChangeListener

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.listeners.WSEditorChangeListener
   @API(type=EXTENDABLE, src=PUBLIC) public class WSEditorChangeListener extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Notified when an editor is added, removed or the editor page is changed
  Since: 11.2
## Constructor Summary
 Constructors
Constructor

Description
 [WSEditorChangeListener](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [editorAboutToBeClosed](#editorAboutToBeClosed(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
An editor will be closed.
  void [editorAboutToBeOpened](#editorAboutToBeOpened(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
An editor will be opened.
  boolean [editorAboutToBeOpenedVeto](#editorAboutToBeOpenedVeto(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
An editor will be opened.
  void [editorActivated](#editorActivated(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
An editor was activated.
  void [editorClosed](#editorClosed(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
An editor was closed.
  void [editorDeactivated](#editorDeactivated(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
An editor was de-activated.
  void [editorOpened](#editorOpened(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
An editor was opened.
  void [editorPageChanged](#editorPageChanged(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
The current page for an editor has changed.
  void [editorRelocated](#editorRelocated(java.net.URL,java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) previousEditorLocation, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) newEditorLocation)
An editor was relocated to a new location.
  boolean [editorsAboutToBeClosed](#editorsAboutToBeClosed(java.net.URL%5B%5D))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] editorLocations)
A group of opened documents will be closed by using a batch close operation (like "Close All" or "Close Others").
  void [editorSelected](#editorSelected(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
An editor was selected in the tabbed pane.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WSEditorChangeListener

public WSEditorChangeListener()

## Method Details

### editorAboutToBeOpenedVeto

public boolean editorAboutToBeOpenedVeto([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

An editor will be opened. You can reject the opening of the editor by returning false. If the open is not rejected then the [editorAboutToBeOpened(URL)](#editorAboutToBeOpened(java.net.URL)) and then [editorOpened(URL)](#editorOpened(java.net.URL)) methods will be called. If you want to open another file instead, you must start a thread which calls the API to open the other file and then return false. Calling API to open another resource directly on this callback will block Oxygen. This method is not called in the Eclipse plugin.
  Parameters: editorLocation - The editor's location. Returns: true to proceed with the open, false to reject the open of the editor. Since: 12.2
### editorAboutToBeOpened

public void editorAboutToBeOpened([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

An editor will be opened. If the open does not fail, then the [editorOpened(URL)](#editorOpened(java.net.URL)) method will be called.
  Parameters: editorLocation - The editor's location Since: 12.1
### editorOpened

public void editorOpened([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

An editor was opened.
  Parameters: editorLocation - The editor's location
### editorClosed

public void editorClosed([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

An editor was closed.
  Parameters: editorLocation - The editor's location
### editorSelected

public void editorSelected([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

An editor was selected in the tabbed pane.
  Parameters: editorLocation - The editor's location. Can be null if no editor is opened or a switch between editors is pending.
### editorPageChanged

public void editorPageChanged([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

The current page for an editor has changed. This means the user switched for example from the **Text** to the **Author** page. An XML Editor usually has 3 pages: **Text**, **Grid** and **Author**.
  Parameters: editorLocation - The editor's location
### editorActivated

public void editorActivated([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

An editor was activated. It is the selected editor but also the editor in which the focus is present.
  Parameters: editorLocation - The editor's location Since: 12.2
### editorDeactivated

public void editorDeactivated([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

An editor was de-activated. Focus is no longer present in it. Maybe the editor was already closed.
  Parameters: editorLocation - The editor's location Since: 12.2
### editorAboutToBeClosed

public boolean editorAboutToBeClosed([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

An editor will be closed. You can reject the close of the editor by returning false.
  Parameters: editorLocation - The editor's location Returns: true to proceed with the close, false to reject the close of the editor. This method is not called in the Eclipse plugin. Since: 12.2
### editorRelocated

public void editorRelocated([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) previousEditorLocation, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) newEditorLocation)

An editor was relocated to a new location. Probably **Save As** was called on the opened editor.
  Parameters: previousEditorLocation - The previous editor's location newEditorLocation - The current editor's location In the standalone Oxygen version the listener is usually called after the end user has used the "Save as" or "Save to URL" actions and saved the editor contents somewhere else. This method is not called in the Eclipse plugin. Since: 12.2
### editorsAboutToBeClosed

public boolean editorsAboutToBeClosed([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] editorLocations)

A group of opened documents will be closed by using a batch close operation (like "Close All" or "Close Others"). This event is triggered before the application will try to check which of these editors are modified and to show a batch save dialog for them. You can reject the close of the editor by returning false. If the callback is not rejected, you will also receive individual "editorAboutToBeClosed" and "editorClosed" callbacks for each of the editors while they are being individually closed. This callback is only received in the Oxygen standalone application so it is not received in the Oxygen Eclipse Plugin.
  Parameters: editorLocations - The locations of the editors which will be batch closed. Returns: true to proceed with the close, false to reject the close of the editor. This method is not called in the Eclipse plugin. Since: 18
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
