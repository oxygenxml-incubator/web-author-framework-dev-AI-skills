Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Class InplaceEditorAdapter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.editor.InplaceEditorAdapter
   All Implemented Interfaces: [InplaceEditor](InplaceEditor.md), [Extension](../Extension.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class InplaceEditorAdapter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [InplaceEditor](InplaceEditor.md)
Convenience implementation of the [InplaceEditor](InplaceEditor.md). By extending this adapter you are protected if any new methods are added inside [InplaceEditor](InplaceEditor.md).
  Since: 14.1
## Constructor Summary
 Constructors
Constructor

Description
 [InplaceEditorAdapter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addEditingListener](#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))([InplaceEditingListener](InplaceEditingListener.md) editingListener)
Adds a listener to receive edit notifications: - [InplaceEditingListener.editingCanceled()](InplaceEditingListener.md#editingCanceled()) to remove the editor and cancel the edit operation.
  void [cancelEditing](#cancelEditing())()
Cancels the editing process.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getEditorComponent](#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point))([AuthorInplaceContext](AuthorInplaceContext.md) context, [Rectangle](../../../../exml/view/graphics/Rectangle.md) allocation, [Point](../../../../exml/view/graphics/Point.md) mouseInvocationLocation)
Prepare and return the editor component.
  [Rectangle](../../../../exml/view/graphics/Rectangle.md) [getScrollRectangle](#getScrollRectangle())()
Returns a rectangle that should be made visible after the editor is shown.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getValue](#getValue())()
Gets the value that the user entered.
  void [refresh](#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](AuthorInplaceContext.md) context)
While this editor is inside an editing session a document change was detected that didn't originated form this editor.
  void [removeEditingListener](#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))([InplaceEditingListener](InplaceEditingListener.md) editingListener)
Removes a listener that receives editing events.
  void [requestFocus](#requestFocus())()
Requests focus inside the editing component.
  void [stopEditing](#stopEditing())()
Stops the editing and commits the current value.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.editor.[InplaceEditor](InplaceEditor.md)
 [allowsRepostingEvents](InplaceEditor.md#allowsRepostingEvents()), [commitValue](InplaceEditor.md#commitValue()), [insertContent](InplaceEditor.md#insertContent(java.lang.String))
## Constructor Details

### InplaceEditorAdapter

public InplaceEditorAdapter()

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../Extension.md#getDescription()) in interface [Extension](../Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../Extension.md#getDescription())

### getEditorComponent

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getEditorComponent([AuthorInplaceContext](AuthorInplaceContext.md) context, [Rectangle](../../../../exml/view/graphics/Rectangle.md) allocation, [Point](../../../../exml/view/graphics/Point.md) mouseInvocationLocation)
 Description copied from interface: [InplaceEditor](InplaceEditor.md#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point))
Prepare and return the editor component.
  Specified by: [getEditorComponent](InplaceEditor.md#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point)) in interface [InplaceEditor](InplaceEditor.md) Parameters: context - The context where the editor will be used. allocation - The bounds where the editor will be shown. This is normally the bounds of the box in which the value being edited is rendered. If the editor requires to be presented in different bounds it should alter this parameter. The X,Y coordinates are relative to the parent in which the editor will be added. mouseInvocationLocation - if the editor was requested using the mouse this parameter represents the X,Y location where the event took place. It is relative to the parent in which the editor will be added. null if the editor wasn't requested through mouse interaction.   **OBS**: This is the very first call received by an editor. This ensures that the editor is properly initialized for the subsequent calls (like a [InplaceEditor.requestFocus()](InplaceEditor.md#requestFocus()) call).  **OBS**: An editor implementation will have to add listeners onto itself like:
        * a [KeyListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/KeyListener.html) for handling key events like: ENTER to stop editing (by calling [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))) and ESCAPE to cancel it (by calling [InplaceEditingListener.editingCanceled()](InplaceEditingListener.md#editingCanceled())).
        * a [FocusListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/FocusListener.html) to stop editing when the focus is given to a component that is not part of the editor (by calling [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))).
        * a [DocumentListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/DocumentListener.html) to fire [InplaceEditingListener.editingOccured()](InplaceEditingListener.md#editingOccured()) events (If the editor has a document).
 Returns: The component that performs the editing. For the Standalone distribution this should be a java.awt.JComponent implementation. For the Eclipse plugin distribution, an org.eclipse.swt.widgets.Control is expected. See Also:
        * [InplaceEditor.getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext, ro.sync.exml.view.graphics.Rectangle, ro.sync.exml.view.graphics.Point)](InplaceEditor.md#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point))

### getScrollRectangle

public [Rectangle](../../../../exml/view/graphics/Rectangle.md) getScrollRectangle()
 Description copied from interface: [InplaceEditor](InplaceEditor.md#getScrollRectangle())
Returns a rectangle that should be made visible after the editor is shown. The coordinate should be relative to the editor itself. The default behavior is to make the entire editor visible but if the editor is bigger than the viewport the visible part might not be the right one. For example is the editor is a text field the caret might not be visible. This is when this method is useful. The caret rectangle should be returned so that the part of the editor with the caret is presented.
  Specified by: [getScrollRectangle](InplaceEditor.md#getScrollRectangle()) in interface [InplaceEditor](InplaceEditor.md) Returns: A rectangle to be made visible or null to make the entire editor visible. See Also:
        * [InplaceEditor.getScrollRectangle()](InplaceEditor.md#getScrollRectangle())

### addEditingListener

public void addEditingListener([InplaceEditingListener](InplaceEditingListener.md) editingListener)
 Description copied from interface: [InplaceEditor](InplaceEditor.md#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))
Adds a listener to receive edit notifications: - [InplaceEditingListener.editingCanceled()](InplaceEditingListener.md#editingCanceled()) to remove the editor and cancel the edit operation. - [InplaceEditingListener.editingOccured()](InplaceEditingListener.md#editingOccured()) to signal modification in the editor. This event marks the editor as dirty and it's value will be committed when a [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))is received. - [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) to end editing and commit it's value if needed. The value is usually committed ONLY if a [InplaceEditingListener.editingOccured()](InplaceEditingListener.md#editingOccured()) was fired. See [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) for more information.
  Specified by: [addEditingListener](InplaceEditor.md#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)) in interface [InplaceEditor](InplaceEditor.md) Parameters: editingListener - Editing listener. See Also:
        * [InplaceEditor.addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)](InplaceEditor.md#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))

### requestFocus

public void requestFocus()
 Description copied from interface: [InplaceEditor](InplaceEditor.md#requestFocus())
Requests focus inside the editing component.
  Specified by: [requestFocus](InplaceEditor.md#requestFocus()) in interface [InplaceEditor](InplaceEditor.md) See Also:
        * [InplaceEditor.requestFocus()](InplaceEditor.md#requestFocus())

### getValue

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getValue()
 Description copied from interface: [InplaceEditor](InplaceEditor.md#getValue())
Gets the value that the user entered.
  Specified by: [getValue](InplaceEditor.md#getValue()) in interface [InplaceEditor](InplaceEditor.md) Returns: The value that the user entered. See Also:
        * [InplaceEditor.getValue()](InplaceEditor.md#getValue())

### stopEditing

public void stopEditing()
 Description copied from interface: [InplaceEditor](InplaceEditor.md#stopEditing())
Stops the editing and commits the current value. The editor should release any held resources and notify [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)). OBS: The current value will be committed only if at least one [InplaceEditingListener.editingOccured()](InplaceEditingListener.md#editingOccured()) event was issued before this moment.
  Specified by: [stopEditing](InplaceEditor.md#stopEditing()) in interface [InplaceEditor](InplaceEditor.md) See Also:
        * [InplaceEditor.stopEditing()](InplaceEditor.md#stopEditing())

### cancelEditing

public void cancelEditing()
 Description copied from interface: [InplaceEditor](InplaceEditor.md#cancelEditing())
Cancels the editing process. The editor should release any held resources and notify [InplaceEditingListener.editingCanceled()](InplaceEditingListener.md#editingCanceled()).
  Specified by: [cancelEditing](InplaceEditor.md#cancelEditing()) in interface [InplaceEditor](InplaceEditor.md) See Also:
        * [InplaceEditor.cancelEditing()](InplaceEditor.md#cancelEditing())

### removeEditingListener

public void removeEditingListener([InplaceEditingListener](InplaceEditingListener.md) editingListener)
 Description copied from interface: [InplaceEditor](InplaceEditor.md#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))
Removes a listener that receives editing events.
  Specified by: [removeEditingListener](InplaceEditor.md#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)) in interface [InplaceEditor](InplaceEditor.md) Parameters: editingListener - Editing listener. See Also:
        * [InplaceEditor.removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)](InplaceEditor.md#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))

### refresh

public void refresh([AuthorInplaceContext](AuthorInplaceContext.md) context)
 Description copied from interface: [InplaceEditor](InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))
While this editor is inside an editing session a document change was detected that didn't originated form this editor. In this situation it might be good for the editor to refresh the presented data. Currently this method is called if:
        * This editor edits an attribute and the same attribute was externally modified. In this situation is recommended for the editor to update the current value.

  Specified by: [refresh](InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)) in interface [InplaceEditor](InplaceEditor.md) Parameters: context - An updated editing context for this editor. See Also:
        * [InplaceEditor.refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)](InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
