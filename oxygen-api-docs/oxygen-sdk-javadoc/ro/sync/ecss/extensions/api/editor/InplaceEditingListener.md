Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Interface InplaceEditingListener
    All Superinterfaces: [InplaceEditingTraversalListener](InplaceEditingTraversalListener.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface InplaceEditingListenerextends [InplaceEditingTraversalListener](InplaceEditingTraversalListener.md)
Gets notified about edit events:
* [editingStopped(EditingEvent)](#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) - a request to stop the editing and commit the value from the editor. **Unless a [editingOccured()](#editingOccured()) is received the value will not be committed.**
* [editingOccured()](#editingOccured()) - signals an edit event inside the editor. This will mark the value from the editor as being dirty and requiring committing.
* [editingCanceled()](#editingCanceled()) - a request to hide the editor without any commit.
An editor implementation will have to add listeners onto itself like:
* a [KeyListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/KeyListener.html) for handling key events like: ENTER to stop editing and ESCAPE to cancel it.
* a [FocusListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/FocusListener.html) to stop editing when the focus is given to a component that is not part of the editor.
* a [DocumentListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/DocumentListener.html) to fire [editingOccured()](#editingOccured()) events (If the editor has a document).

  Since: 14.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [commitValue](#commitValue(ro.sync.ecss.extensions.api.editor.EditingEvent))([EditingEvent](EditingEvent.md) event)
Commit the given value inside the document without stopping the editing.
  void [editingCanceled](#editingCanceled())()
An editing canceled request.
  void [editingOccured](#editingOccured())()
An edit happened in the inplace editor which could result in a document modification if the new value will be committed.
  void [editingStopped](#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))([EditingEvent](EditingEvent.md) event)
An editing stopped request.

### Methods inherited from interface ro.sync.ecss.extensions.api.editor.[InplaceEditingTraversalListener](InplaceEditingTraversalListener.md)
 [nextEditLocationRequested](InplaceEditingTraversalListener.md#nextEditLocationRequested()), [previousEditLocationRequested](InplaceEditingTraversalListener.md#previousEditLocationRequested())
## Method Details

### editingStopped

void editingStopped([EditingEvent](EditingEvent.md) event)

An editing stopped request. This will commit the value into the document **ONLY if the following conditions apply**:
        * an [editingOccured()](#editingOccured()) event was received prior to this event.
        * the value that must be committed is different from the old value. The old value taken into account is either [InplaceEditorArgumentKeys.INITIAL_VALUE](InplaceEditorArgumentKeys.md#INITIAL_VALUE) or, if missing, [InplaceEditorArgumentKeys.DEFAULT_VALUE](InplaceEditorArgumentKeys.md#DEFAULT_VALUE).
        *  **OBS:** Before or after firing this event, the editor should release any held resources. For example a SWT editor will have to dispose() any created images, fonts or controls.

  Parameters: event - Provides information about the editing. If null we should handle this as a cancel event.
### editingCanceled

void editingCanceled()

An editing canceled request.  **OBS:** Before or after firing this event, the editor should release any held resources. For example a SWT editor will have to dispose() any created images, fonts or controls.

### editingOccured

void editingOccured()

An edit happened in the inplace editor which could result in a document modification if the new value will be committed. OBS: THIS EVENT IS VERY IMPORTANT. If no [editingOccured()](#editingOccured()) event is received, the value from the editor will not be committed when the editing is stopped. See [editingStopped(EditingEvent)](#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) for more information.

### commitValue

void commitValue([EditingEvent](EditingEvent.md) event)

Commit the given value inside the document without stopping the editing. Will only commit if a new string value is provided and only if the value that must be committed is different from the current value. Normally, this kind of event should be preceded by an [editingOccured()](#editingOccured()) event.
  Parameters: event - Editing event. Currently only the string value from within is of interest. Also in case of custom form controls any given [EditingEvent.customEdit](EditingEvent.md#customEdit) will also be executed.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
