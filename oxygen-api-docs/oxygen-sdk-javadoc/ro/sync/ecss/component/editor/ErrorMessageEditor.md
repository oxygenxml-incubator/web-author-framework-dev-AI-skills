Package [ro.sync.ecss.component.editor](package-summary.md)

# Class ErrorMessageEditor

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.component.editor.ErrorMessageEditor
   All Implemented Interfaces: [InplaceEditor](../../extensions/api/editor/InplaceEditor.md), [Extension](../../extensions/api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class ErrorMessageEditor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [InplaceEditor](../../extensions/api/editor/InplaceEditor.md)
If there are errors obtaining the editor we will use this editor just to present the error.

## Constructor Summary
 Constructors
Constructor

Description
 [ErrorMessageEditor](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addEditingListener](#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))([InplaceEditingListener](../../extensions/api/editor/InplaceEditingListener.md) editingListener)
Adds a listener to receive edit notifications: - [InplaceEditingListener.editingCanceled()](../../extensions/api/editor/InplaceEditingListener.md#editingCanceled()) to remove the editor and cancel the edit operation.
  void [cancelEditing](#cancelEditing())()
Cancels the editing process.
  void [commitValue](#commitValue())()
Commit the given value inside the document without stopping the editing.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getEditorComponent](#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point))([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) context, [Rectangle](../../../exml/view/graphics/Rectangle.md) allocation, [Point](../../../exml/view/graphics/Point.md) mouseLocation)
Prepare and return the editor component.
  [Rectangle](../../../exml/view/graphics/Rectangle.md) [getScrollRectangle](#getScrollRectangle())()
Returns a rectangle that should be made visible after the editor is shown.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getValue](#getValue())()
Gets the value that the user entered.
  boolean [insertContent](#insertContent(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlContent)
An insert text event was received by the author page and redirected to this currently active form control.
  void [refresh](#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) context)
While this editor is inside an editing session a document change was detected that didn't originated form this editor.
  void [removeEditingListener](#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))([InplaceEditingListener](../../extensions/api/editor/InplaceEditingListener.md) editingListener)
Removes a listener that receives editing events.
  void [requestFocus](#requestFocus())()
Requests focus inside the editing component.
  void [stopEditing](#stopEditing())()
Stops the editing and commits the current value.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.editor.[InplaceEditor](../../extensions/api/editor/InplaceEditor.md)
 [allowsRepostingEvents](../../extensions/api/editor/InplaceEditor.md#allowsRepostingEvents())
## Constructor Details

### ErrorMessageEditor

public ErrorMessageEditor()

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../extensions/api/Extension.md#getDescription()) in interface [Extension](../../extensions/api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../extensions/api/Extension.md#getDescription())

### getEditorComponent

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getEditorComponent([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) context, [Rectangle](../../../exml/view/graphics/Rectangle.md) allocation, [Point](../../../exml/view/graphics/Point.md) mouseLocation)
 Description copied from interface: [InplaceEditor](../../extensions/api/editor/InplaceEditor.md#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point))
Prepare and return the editor component.
  Specified by: [getEditorComponent](../../extensions/api/editor/InplaceEditor.md#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point)) in interface [InplaceEditor](../../extensions/api/editor/InplaceEditor.md) Parameters: context - The context where the editor will be used. allocation - The bounds where the editor will be shown. This is normally the bounds of the box in which the value being edited is rendered. If the editor requires to be presented in different bounds it should alter this parameter. The X,Y coordinates are relative to the parent in which the editor will be added. mouseLocation - if the editor was requested using the mouse this parameter represents the X,Y location where the event took place. It is relative to the parent in which the editor will be added. null if the editor wasn't requested through mouse interaction.   **OBS**: This is the very first call received by an editor. This ensures that the editor is properly initialized for the subsequent calls (like a [InplaceEditor.requestFocus()](../../extensions/api/editor/InplaceEditor.md#requestFocus()) call).  **OBS**: An editor implementation will have to add listeners onto itself like:
        * a [KeyListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/KeyListener.html) for handling key events like: ENTER to stop editing (by calling [InplaceEditingListener.editingStopped(EditingEvent)](../../extensions/api/editor/InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))) and ESCAPE to cancel it (by calling [InplaceEditingListener.editingCanceled()](../../extensions/api/editor/InplaceEditingListener.md#editingCanceled())).
        * a [FocusListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/FocusListener.html) to stop editing when the focus is given to a component that is not part of the editor (by calling [InplaceEditingListener.editingStopped(EditingEvent)](../../extensions/api/editor/InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))).
        * a [DocumentListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/DocumentListener.html) to fire [InplaceEditingListener.editingOccured()](../../extensions/api/editor/InplaceEditingListener.md#editingOccured()) events (If the editor has a document).
 Returns: The component that performs the editing. For the Standalone distribution this should be a java.awt.JComponent implementation. For the Eclipse plugin distribution, an org.eclipse.swt.widgets.Control is expected. See Also:
        * [InplaceEditor.getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext, ro.sync.exml.view.graphics.Rectangle, ro.sync.exml.view.graphics.Point)](../../extensions/api/editor/InplaceEditor.md#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point))

### addEditingListener

public void addEditingListener([InplaceEditingListener](../../extensions/api/editor/InplaceEditingListener.md) editingListener)
 Description copied from interface: [InplaceEditor](../../extensions/api/editor/InplaceEditor.md#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))
Adds a listener to receive edit notifications: - [InplaceEditingListener.editingCanceled()](../../extensions/api/editor/InplaceEditingListener.md#editingCanceled()) to remove the editor and cancel the edit operation. - [InplaceEditingListener.editingOccured()](../../extensions/api/editor/InplaceEditingListener.md#editingOccured()) to signal modification in the editor. This event marks the editor as dirty and it's value will be committed when a [InplaceEditingListener.editingStopped(EditingEvent)](../../extensions/api/editor/InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))is received. - [InplaceEditingListener.editingStopped(EditingEvent)](../../extensions/api/editor/InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) to end editing and commit it's value if needed. The value is usually committed ONLY if a [InplaceEditingListener.editingOccured()](../../extensions/api/editor/InplaceEditingListener.md#editingOccured()) was fired. See [InplaceEditingListener.editingStopped(EditingEvent)](../../extensions/api/editor/InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) for more information.
  Specified by: [addEditingListener](../../extensions/api/editor/InplaceEditor.md#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)) in interface [InplaceEditor](../../extensions/api/editor/InplaceEditor.md) Parameters: editingListener - Editing listener. See Also:
        * [InplaceEditor.addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)](../../extensions/api/editor/InplaceEditor.md#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))

### requestFocus

public void requestFocus()
 Description copied from interface: [InplaceEditor](../../extensions/api/editor/InplaceEditor.md#requestFocus())
Requests focus inside the editing component.
  Specified by: [requestFocus](../../extensions/api/editor/InplaceEditor.md#requestFocus()) in interface [InplaceEditor](../../extensions/api/editor/InplaceEditor.md) See Also:
        * [InplaceEditor.requestFocus()](../../extensions/api/editor/InplaceEditor.md#requestFocus())

### getValue

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getValue()
 Description copied from interface: [InplaceEditor](../../extensions/api/editor/InplaceEditor.md#getValue())
Gets the value that the user entered.
  Specified by: [getValue](../../extensions/api/editor/InplaceEditor.md#getValue()) in interface [InplaceEditor](../../extensions/api/editor/InplaceEditor.md) Returns: The value that the user entered. See Also:
        * [InplaceEditor.getValue()](../../extensions/api/editor/InplaceEditor.md#getValue())

### stopEditing

public void stopEditing()
 Description copied from interface: [InplaceEditor](../../extensions/api/editor/InplaceEditor.md#stopEditing())
Stops the editing and commits the current value. The editor should release any held resources and notify [InplaceEditingListener.editingStopped(EditingEvent)](../../extensions/api/editor/InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)). OBS: The current value will be committed only if at least one [InplaceEditingListener.editingOccured()](../../extensions/api/editor/InplaceEditingListener.md#editingOccured()) event was issued before this moment.
  Specified by: [stopEditing](../../extensions/api/editor/InplaceEditor.md#stopEditing()) in interface [InplaceEditor](../../extensions/api/editor/InplaceEditor.md) See Also:
        * [InplaceEditor.stopEditing()](../../extensions/api/editor/InplaceEditor.md#stopEditing())

### cancelEditing

public void cancelEditing()
 Description copied from interface: [InplaceEditor](../../extensions/api/editor/InplaceEditor.md#cancelEditing())
Cancels the editing process. The editor should release any held resources and notify [InplaceEditingListener.editingCanceled()](../../extensions/api/editor/InplaceEditingListener.md#editingCanceled()).
  Specified by: [cancelEditing](../../extensions/api/editor/InplaceEditor.md#cancelEditing()) in interface [InplaceEditor](../../extensions/api/editor/InplaceEditor.md) See Also:
        * [InplaceEditor.cancelEditing()](../../extensions/api/editor/InplaceEditor.md#cancelEditing())

### removeEditingListener

public void removeEditingListener([InplaceEditingListener](../../extensions/api/editor/InplaceEditingListener.md) editingListener)
 Description copied from interface: [InplaceEditor](../../extensions/api/editor/InplaceEditor.md#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))
Removes a listener that receives editing events.
  Specified by: [removeEditingListener](../../extensions/api/editor/InplaceEditor.md#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)) in interface [InplaceEditor](../../extensions/api/editor/InplaceEditor.md) Parameters: editingListener - Editing listener. See Also:
        * [InplaceEditor.removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)](../../extensions/api/editor/InplaceEditor.md#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))

### getScrollRectangle

public [Rectangle](../../../exml/view/graphics/Rectangle.md) getScrollRectangle()
 Description copied from interface: [InplaceEditor](../../extensions/api/editor/InplaceEditor.md#getScrollRectangle())
Returns a rectangle that should be made visible after the editor is shown. The coordinate should be relative to the editor itself. The default behavior is to make the entire editor visible but if the editor is bigger than the viewport the visible part might not be the right one. For example is the editor is a text field the caret might not be visible. This is when this method is useful. The caret rectangle should be returned so that the part of the editor with the caret is presented.
  Specified by: [getScrollRectangle](../../extensions/api/editor/InplaceEditor.md#getScrollRectangle()) in interface [InplaceEditor](../../extensions/api/editor/InplaceEditor.md) Returns: A rectangle to be made visible or null to make the entire editor visible. See Also:
        * [InplaceEditor.getScrollRectangle()](../../extensions/api/editor/InplaceEditor.md#getScrollRectangle())

### refresh

public void refresh([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) context)
 Description copied from interface: [InplaceEditor](../../extensions/api/editor/InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))
While this editor is inside an editing session a document change was detected that didn't originated form this editor. In this situation it might be good for the editor to refresh the presented data. Currently this method is called if:
        * This editor edits an attribute and the same attribute was externally modified. In this situation is recommended for the editor to update the current value.

  Specified by: [refresh](../../extensions/api/editor/InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)) in interface [InplaceEditor](../../extensions/api/editor/InplaceEditor.md) Parameters: context - An updated editing context for this editor. See Also:
        * [InplaceEditor.refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)](../../extensions/api/editor/InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))

### insertContent

public boolean insertContent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlContent)
 Description copied from interface: [InplaceEditor](../../extensions/api/editor/InplaceEditor.md#insertContent(java.lang.String))
An insert text event was received by the author page and redirected to this currently active form control. The form control should insert this text as it sees fit. For example a text field might insert it at the caret position. An example when this event comes is when the user uses the Character Map Dialog to insert characters directly into a form control.
  Specified by: [insertContent](../../extensions/api/editor/InplaceEditor.md#insertContent(java.lang.String)) in interface [InplaceEditor](../../extensions/api/editor/InplaceEditor.md) Parameters: xmlContent - Content to be inserted. Returns: true if the event was handled or false if the form control can do nothing with the string. For example a text field can insert the text inside it but a check box form control can do nothing with it. If false is returned the form control editing session will be stopped and the author page will handle the event instead. See Also:
        * [InplaceEditor.insertContent(java.lang.String)](../../extensions/api/editor/InplaceEditor.md#insertContent(java.lang.String))

### commitValue

public void commitValue()
 Description copied from interface: [InplaceEditor](../../extensions/api/editor/InplaceEditor.md#commitValue())
Commit the given value inside the document without stopping the editing. Will only commit if a new string value is provided and only if the value that must be committed is different from the current value.
  Specified by: [commitValue](../../extensions/api/editor/InplaceEditor.md#commitValue()) in interface [InplaceEditor](../../extensions/api/editor/InplaceEditor.md) See Also:
        * [InplaceEditor.commitValue()](../../extensions/api/editor/InplaceEditor.md#commitValue())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
