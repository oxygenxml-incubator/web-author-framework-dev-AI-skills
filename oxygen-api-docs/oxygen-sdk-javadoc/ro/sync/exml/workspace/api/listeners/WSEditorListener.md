Package [ro.sync.exml.workspace.api.listeners](package-summary.md)

# Class WSEditorListener

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.workspace.api.listeners.WSEditorPageChangedListener](WSEditorPageChangedListener.md)
        * ro.sync.exml.workspace.api.listeners.WSEditorListener
   @API(type=EXTENDABLE, src=PUBLIC) public class WSEditorListener extends [WSEditorPageChangedListener](WSEditorPageChangedListener.md)
WS Editor listener. The listener is added to a WSEditor and receives different callbacks.
  Since: 13
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [SAVE_AS_OPERATION](#SAVE_AS_OPERATION)
Operation type used to signal that an editor was saved as another resource.
  static final int [SAVE_OPERATION](#SAVE_OPERATION)
Operation type used to signal that an editor was saved.

## Constructor Summary
 Constructors
Constructor

Description
 [WSEditorListener](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [documentTypeExtensionsReconfigured](#documentTypeExtensionsReconfigured())()
The editor document type-specific functionality was refreshed.
  boolean [editorAboutToBeClosedVeto](#editorAboutToBeClosedVeto(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)
The editor is about to be closed.
  boolean [editorAboutToBeSavedVeto](#editorAboutToBeSavedVeto(int))(int operationType)
The editor is about to be saved.
  void [editorReloaded](#editorReloaded(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorURL)
The content of the document has been reloaded.
  void [editorSaved](#editorSaved(int))(int operationType)
The editor was saved.

### Methods inherited from class ro.sync.exml.workspace.api.listeners.[WSEditorPageChangedListener](WSEditorPageChangedListener.md)
 [editorPageAboutToBeChangedVeto](WSEditorPageChangedListener.md#editorPageAboutToBeChangedVeto(java.lang.String)), [editorPageChanged](WSEditorPageChangedListener.md#editorPageChanged())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### SAVE_OPERATION

public static final int SAVE_OPERATION

Operation type used to signal that an editor was saved.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.listeners.WSEditorListener.SAVE_OPERATION)

### SAVE_AS_OPERATION

public static final int SAVE_AS_OPERATION

Operation type used to signal that an editor was saved as another resource.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.listeners.WSEditorListener.SAVE_AS_OPERATION)

## Constructor Details

### WSEditorListener

public WSEditorListener()

## Method Details

### editorAboutToBeSavedVeto

public boolean editorAboutToBeSavedVeto(int operationType)

The editor is about to be saved.
  Parameters: operationType - The operation type. One of the constants [SAVE_AS_OPERATION](#SAVE_AS_OPERATION) or [SAVE_OPERATION](#SAVE_OPERATION). Returns: true to continue saving it, false to cancel the save operation.
### editorSaved

public void editorSaved(int operationType)

The editor was saved.
  Parameters: operationType - The operation type. One of the constants [SAVE_AS_OPERATION](#SAVE_AS_OPERATION) or [SAVE_OPERATION](#SAVE_OPERATION).
### documentTypeExtensionsReconfigured

public void documentTypeExtensionsReconfigured()

The editor document type-specific functionality was refreshed. For example after a document is opened, the application will re-configure the framework-specific toolbar. After this, the callback will be received. So if you are using code which for example tries to add a listener to one of the actions on the framework-specific toolbar, the code should re-add the listener when the callback is received.
  Since: 18
### editorAboutToBeClosedVeto

public boolean editorAboutToBeClosedVeto([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorLocation)

The editor is about to be closed. Decide if the closing should proceed or not.This method is not called from the Eclipse plug-in. It works only with the stand-alone application.
  Parameters: editorLocation - The URL of the editor. Returns: true to continue closing it, false to cancel the closing of the editor. Since: 19.1
### editorReloaded

public void editorReloaded([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) editorURL)

The content of the document has been reloaded. Probably F5 was pressed.
  Parameters: editorURL - The URL for which the content has been reloaded. Since: 22
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
