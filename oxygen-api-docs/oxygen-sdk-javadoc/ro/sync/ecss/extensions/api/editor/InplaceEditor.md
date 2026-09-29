Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Interface InplaceEditor
    All Superinterfaces: [Extension](../Extension.md)   All Known Implementing Classes: [AbstractInplaceEditor](AbstractInplaceEditor.md), [AbstractInplaceEditorWrapper](AbstractInplaceEditorWrapper.md), [ButtonEditor](../../../component/editor/ButtonEditor.md), [ButtonGroupEditor](../../../component/editor/ButtonGroupEditor.md), [CheckBoxEditor](../../../component/editor/CheckBoxEditor.md), [ComboBoxEditor](../../../component/editor/ComboBoxEditor.md), [DatePickerEditor](../../../component/editor/DatePickerEditor.md), [ErrorMessageEditor](../../../component/editor/ErrorMessageEditor.md), [HtmlContentEditor](../../../component/editor/HtmlContentEditor.md), [InplaceEditorAdapter](InplaceEditorAdapter.md), [InplaceEditorRendererAdapter](InplaceEditorRendererAdapter.md), [InputURLEditor](../../../component/editor/InputURLEditor.md), [PopupCheckBoxEditor](../../../component/editor/PopupCheckBoxEditor.md), [PopupListEditor](../../../component/editor/PopupListEditor.md), [SimpleURLChooserEditor](../../commons/editor/SimpleURLChooserEditor.md), [TextFieldEditor](../../../component/editor/TextFieldEditor.md), [URLChooserEditorSWT](../../commons/editor/URLChooserEditorSWT.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface InplaceEditorextends [Extension](../Extension.md)
An author in-place editor. Subclasses contain implementation based on real SWT or Swing components like combo boxes, text fields, check boxes, buttons etc.
An editor is associated with an oxy_editor CSS function and is invoked on user interaction. It only handles edit requests while the [InplaceRenderer](InplaceRenderer.md) will handle the painting of the value to edit.

An editor implementation is used through the oxy_editor function like this:

```

 code {
   content: 
     "Attr1: " oxy_editor(type, combo, edit, '@attr1')
     "Attr2: " oxy_editor(type, text, edit, '@attr2')
  }

```

In the previous example a predefined **combo** editor is requested for editing the value of attribute **attr1** and a predefined **text** editor for editing attribute **attr2**. For a custom implementation properties [InplaceEditorCSSConstants.PROPERTY_SWING_EDITOR_CLASS_NAME](InplaceEditorCSSConstants.md#PROPERTY_SWING_EDITOR_CLASS_NAME)and [InplaceEditorCSSConstants.PROPERTY_SWT_EDITOR_CLASS_NAME](InplaceEditorCSSConstants.md#PROPERTY_SWT_EDITOR_CLASS_NAME) must be used:

```

 myElement {
   content: oxy_editor(
       rendererClassName, "com.custom.editors.CustomRenderer",
       swingEditorClassName, "com.custom.editors.SwingCustomEditor",
       swtEditorClassName, "com.custom.editors.SwtCustomEditor",
       edit, "@my_attr"
       customProperty1, "customValue1",
       customProperty2, "customValue2"
   )
 }

```

In the previous example, the editor classes com.custom.editors.SwingCustomEditor and com.custom.editors.SwtCustomEditor must be added in the Classpath of the document type associated with the edited document.

It is recommended to extend the adapter class [InplaceEditorRendererAdapter](InplaceEditorRendererAdapter.md) or [InplaceEditorAdapter](InplaceEditorAdapter.md) in order to be protected from future API additions.

A SWT implementation should also implement org.eclipse.jface.text.ITextOperationTarget so that it will be delegated with events of UNDO, REDO, CUT, PASTE, SELECT ALL.

  Since: 14.1 See Also:
* [SimpleURLChooserEditor](../../commons/editor/SimpleURLChooserEditor.md)
* [URLChooserEditorSWT](../../commons/editor/URLChooserEditorSWT.md)

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 void [addEditingListener](#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))([InplaceEditingListener](InplaceEditingListener.md) editingListener)
Adds a listener to receive edit notifications: - [InplaceEditingListener.editingCanceled()](InplaceEditingListener.md#editingCanceled()) to remove the editor and cancel the edit operation.
  default boolean [allowsRepostingEvents](#allowsRepostingEvents())()

 void [cancelEditing](#cancelEditing())()
Cancels the editing process.
  void [commitValue](#commitValue())()
Commit the given value inside the document without stopping the editing.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getEditorComponent](#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point))([AuthorInplaceContext](AuthorInplaceContext.md) context, [Rectangle](../../../../exml/view/graphics/Rectangle.md) allocation, [Point](../../../../exml/view/graphics/Point.md) mouseInvocationLocation)
Prepare and return the editor component.
  [Rectangle](../../../../exml/view/graphics/Rectangle.md) [getScrollRectangle](#getScrollRectangle())()
Returns a rectangle that should be made visible after the editor is shown.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getValue](#getValue())()
Gets the value that the user entered.
  boolean [insertContent](#insertContent(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) content)
An insert text event was received by the author page and redirected to this currently active form control.
  void [refresh](#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](AuthorInplaceContext.md) context)
While this editor is inside an editing session a document change was detected that didn't originated form this editor.
  void [removeEditingListener](#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))([InplaceEditingListener](InplaceEditingListener.md) editingListener)
Removes a listener that receives editing events.
  void [requestFocus](#requestFocus())()
Requests focus inside the editing component.
  void [stopEditing](#stopEditing())()
Stops the editing and commits the current value.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../Extension.md)
 [getDescription](../Extension.md#getDescription())
## Method Details

### getEditorComponent

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getEditorComponent([AuthorInplaceContext](AuthorInplaceContext.md) context, [Rectangle](../../../../exml/view/graphics/Rectangle.md) allocation, [Point](../../../../exml/view/graphics/Point.md) mouseInvocationLocation)

Prepare and return the editor component.
  Parameters: context - The context where the editor will be used. allocation - The bounds where the editor will be shown. This is normally the bounds of the box in which the value being edited is rendered. If the editor requires to be presented in different bounds it should alter this parameter. The X,Y coordinates are relative to the parent in which the editor will be added. mouseInvocationLocation - if the editor was requested using the mouse this parameter represents the X,Y location where the event took place. It is relative to the parent in which the editor will be added. null if the editor wasn't requested through mouse interaction.   **OBS**: This is the very first call received by an editor. This ensures that the editor is properly initialized for the subsequent calls (like a [requestFocus()](#requestFocus()) call).  **OBS**: An editor implementation will have to add listeners onto itself like:
        * a [KeyListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/KeyListener.html) for handling key events like: ENTER to stop editing (by calling [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))) and ESCAPE to cancel it (by calling [InplaceEditingListener.editingCanceled()](InplaceEditingListener.md#editingCanceled())).
        * a [FocusListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/FocusListener.html) to stop editing when the focus is given to a component that is not part of the editor (by calling [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))).
        * a [DocumentListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/DocumentListener.html) to fire [InplaceEditingListener.editingOccured()](InplaceEditingListener.md#editingOccured()) events (If the editor has a document).
 Returns: The component that performs the editing. For the Standalone distribution this should be a java.awt.JComponent implementation. For the Eclipse plugin distribution, an org.eclipse.swt.widgets.Control is expected.
### getScrollRectangle

[Rectangle](../../../../exml/view/graphics/Rectangle.md) getScrollRectangle()

Returns a rectangle that should be made visible after the editor is shown. The coordinate should be relative to the editor itself. The default behavior is to make the entire editor visible but if the editor is bigger than the viewport the visible part might not be the right one. For example is the editor is a text field the caret might not be visible. This is when this method is useful. The caret rectangle should be returned so that the part of the editor with the caret is presented.
  Returns: A rectangle to be made visible or null to make the entire editor visible.
### addEditingListener

void addEditingListener([InplaceEditingListener](InplaceEditingListener.md) editingListener)

Adds a listener to receive edit notifications: - [InplaceEditingListener.editingCanceled()](InplaceEditingListener.md#editingCanceled()) to remove the editor and cancel the edit operation. - [InplaceEditingListener.editingOccured()](InplaceEditingListener.md#editingOccured()) to signal modification in the editor. This event marks the editor as dirty and it's value will be committed when a [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))is received. - [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) to end editing and commit it's value if needed. The value is usually committed ONLY if a [InplaceEditingListener.editingOccured()](InplaceEditingListener.md#editingOccured()) was fired. See [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) for more information.
  Parameters: editingListener - Editing listener.
### requestFocus

void requestFocus()

Requests focus inside the editing component.

### getValue

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getValue()

Gets the value that the user entered.
  Returns: The value that the user entered.
### stopEditing

void stopEditing()

Stops the editing and commits the current value. The editor should release any held resources and notify [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)). OBS: The current value will be committed only if at least one [InplaceEditingListener.editingOccured()](InplaceEditingListener.md#editingOccured()) event was issued before this moment.

### commitValue

void commitValue()

Commit the given value inside the document without stopping the editing. Will only commit if a new string value is provided and only if the value that must be committed is different from the current value.
  Since: 17.1
### cancelEditing

void cancelEditing()

Cancels the editing process. The editor should release any held resources and notify [InplaceEditingListener.editingCanceled()](InplaceEditingListener.md#editingCanceled()).

### removeEditingListener

void removeEditingListener([InplaceEditingListener](InplaceEditingListener.md) editingListener)

Removes a listener that receives editing events.
  Parameters: editingListener - Editing listener.
### refresh

void refresh([AuthorInplaceContext](AuthorInplaceContext.md) context)

While this editor is inside an editing session a document change was detected that didn't originated form this editor. In this situation it might be good for the editor to refresh the presented data. Currently this method is called if:
        * This editor edits an attribute and the same attribute was externally modified. In this situation is recommended for the editor to update the current value.

  Parameters: context - An updated editing context for this editor. Since: 16.1
### insertContent

boolean insertContent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) content)

An insert text event was received by the author page and redirected to this currently active form control. The form control should insert this text as it sees fit. For example a text field might insert it at the caret position. An example when this event comes is when the user uses the Character Map Dialog to insert characters directly into a form control.
  Parameters: content - Content to be inserted. Returns: true if the event was handled or false if the form control can do nothing with the string. For example a text field can insert the text inside it but a check box form control can do nothing with it. If false is returned the form control editing session will be stopped and the author page will handle the event instead. Since: 16.1
### allowsRepostingEvents

default boolean allowsRepostingEvents()
  Returns: true if the component allows receiving mouse events from the editor area if visible on screen.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
