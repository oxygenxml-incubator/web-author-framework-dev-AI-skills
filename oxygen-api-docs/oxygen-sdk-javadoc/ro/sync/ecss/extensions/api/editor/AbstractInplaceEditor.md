Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Class AbstractInplaceEditor

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.editor.AbstractInplaceEditor
   All Implemented Interfaces: [InplaceEditor](InplaceEditor.md), [Extension](../Extension.md)   Direct Known Subclasses: [ButtonEditor](../../../component/editor/ButtonEditor.md), [ButtonGroupEditor](../../../component/editor/ButtonGroupEditor.md), [CheckBoxEditor](../../../component/editor/CheckBoxEditor.md), [ComboBoxEditor](../../../component/editor/ComboBoxEditor.md), [DatePickerEditor](../../../component/editor/DatePickerEditor.md), [HtmlContentEditor](../../../component/editor/HtmlContentEditor.md), [InputURLEditor](../../../component/editor/InputURLEditor.md), [PopupCheckBoxEditor](../../../component/editor/PopupCheckBoxEditor.md), [PopupListEditor](../../../component/editor/PopupListEditor.md), [SimpleURLChooserEditor](../../commons/editor/SimpleURLChooserEditor.md), [TextFieldEditor](../../../component/editor/TextFieldEditor.md), [URLChooserEditorSWT](../../commons/editor/URLChooserEditorSWT.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AbstractInplaceEditor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [InplaceEditor](InplaceEditor.md)
An abstract implementation that handles listeners fire.
  Since: 14.1
## Constructor Summary
 Constructors
Constructor

Description
 [AbstractInplaceEditor](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 final void [addEditingListener](#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))([InplaceEditingListener](InplaceEditingListener.md) editingListener)
Adds a listener to receive edit notifications: - [InplaceEditingListener.editingCanceled()](InplaceEditingListener.md#editingCanceled()) to remove the editor and cancel the edit operation.
  void [commitValue](#commitValue())()
Commit the given value inside the document without stopping the editing.
  protected void [fireCommitValue](#fireCommitValue(ro.sync.ecss.extensions.api.editor.EditingEvent))([EditingEvent](EditingEvent.md) event)
Notify the interested listeners that the current value must be committed.
  protected void [fireEditingCanceled](#fireEditingCanceled())()
Notify the interested listeners that the editing was canceled.
  protected void [fireEditingOccured](#fireEditingOccured())()
Notify the interested listeners that an edit occurred inside the editor.
  protected void [fireEditingStopped](#fireEditingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))([EditingEvent](EditingEvent.md) event)
Notify the interested listeners that the editing stopped.
  protected void [fireNextEditLocationRequested](#fireNextEditLocationRequested())()
Notify the interested listeners that the next edit position was requested.
  protected void [firePreviousEditLocationRequested](#firePreviousEditLocationRequested())()
Notify the interested listeners that the previous edit position was requested.
  protected [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) [getBoolean](#getBoolean(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,java.lang.String))([AuthorInplaceContext](AuthorInplaceContext.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
Gets a boolean from the properties set on the form control.
  boolean [insertContent](#insertContent(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) content)
An insert text event was received by the author page and redirected to this currently active form control.
  void [refresh](#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](AuthorInplaceContext.md) context)
While this editor is inside an editing session a document change was detected that didn't originated form this editor.
  final void [removeEditingListener](#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))([InplaceEditingListener](InplaceEditingListener.md) editingListener)
Removes a listener that receives editing events.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../Extension.md)
 [getDescription](../Extension.md#getDescription())
### Methods inherited from interface ro.sync.ecss.extensions.api.editor.[InplaceEditor](InplaceEditor.md)
 [allowsRepostingEvents](InplaceEditor.md#allowsRepostingEvents()), [cancelEditing](InplaceEditor.md#cancelEditing()), [getEditorComponent](InplaceEditor.md#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point)), [getScrollRectangle](InplaceEditor.md#getScrollRectangle()), [getValue](InplaceEditor.md#getValue()), [requestFocus](InplaceEditor.md#requestFocus()), [stopEditing](InplaceEditor.md#stopEditing())
## Constructor Details

### AbstractInplaceEditor

public AbstractInplaceEditor()

## Method Details

### fireEditingStopped

protected void fireEditingStopped([EditingEvent](EditingEvent.md) event)

Notify the interested listeners that the editing stopped.
  Parameters: event - Editing event.
### fireEditingCanceled

protected void fireEditingCanceled()

Notify the interested listeners that the editing was canceled.

### fireEditingOccured

protected void fireEditingOccured()

Notify the interested listeners that an edit occurred inside the editor.

### fireNextEditLocationRequested

protected void fireNextEditLocationRequested()

Notify the interested listeners that the next edit position was requested.

### firePreviousEditLocationRequested

protected void firePreviousEditLocationRequested()

Notify the interested listeners that the previous edit position was requested.

### addEditingListener

public final void addEditingListener([InplaceEditingListener](InplaceEditingListener.md) editingListener)
 Description copied from interface: [InplaceEditor](InplaceEditor.md#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))
Adds a listener to receive edit notifications: - [InplaceEditingListener.editingCanceled()](InplaceEditingListener.md#editingCanceled()) to remove the editor and cancel the edit operation. - [InplaceEditingListener.editingOccured()](InplaceEditingListener.md#editingOccured()) to signal modification in the editor. This event marks the editor as dirty and it's value will be committed when a [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))is received. - [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) to end editing and commit it's value if needed. The value is usually committed ONLY if a [InplaceEditingListener.editingOccured()](InplaceEditingListener.md#editingOccured()) was fired. See [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) for more information.
  Specified by: [addEditingListener](InplaceEditor.md#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)) in interface [InplaceEditor](InplaceEditor.md) Parameters: editingListener - Editing listener. See Also:
        * [InplaceEditor.addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)](InplaceEditor.md#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))

### removeEditingListener

public final void removeEditingListener([InplaceEditingListener](InplaceEditingListener.md) editingListener)
 Description copied from interface: [InplaceEditor](InplaceEditor.md#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))
Removes a listener that receives editing events.
  Specified by: [removeEditingListener](InplaceEditor.md#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)) in interface [InplaceEditor](InplaceEditor.md) Parameters: editingListener - Editing listener. See Also:
        * [InplaceEditor.removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)](InplaceEditor.md#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))

### fireCommitValue

protected void fireCommitValue([EditingEvent](EditingEvent.md) event)

Notify the interested listeners that the current value must be committed.
  Parameters: event - Editing event.
### getBoolean

protected [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) getBoolean([AuthorInplaceContext](AuthorInplaceContext.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

Gets a boolean from the properties set on the form control.
  Parameters: context - The context. key - The property key. Returns: [Boolean.TRUE](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html#TRUE), [Boolean.FALSE](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html#FALSE), or null if the property is not set.
### refresh

public void refresh([AuthorInplaceContext](AuthorInplaceContext.md) context)
 Description copied from interface: [InplaceEditor](InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))
While this editor is inside an editing session a document change was detected that didn't originated form this editor. In this situation it might be good for the editor to refresh the presented data. Currently this method is called if:
        * This editor edits an attribute and the same attribute was externally modified. In this situation is recommended for the editor to update the current value.

  Specified by: [refresh](InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)) in interface [InplaceEditor](InplaceEditor.md) Parameters: context - An updated editing context for this editor. See Also:
        * [InplaceEditor.refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)](InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))

### insertContent

public boolean insertContent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) content)
 Description copied from interface: [InplaceEditor](InplaceEditor.md#insertContent(java.lang.String))
An insert text event was received by the author page and redirected to this currently active form control. The form control should insert this text as it sees fit. For example a text field might insert it at the caret position. An example when this event comes is when the user uses the Character Map Dialog to insert characters directly into a form control.
  Specified by: [insertContent](InplaceEditor.md#insertContent(java.lang.String)) in interface [InplaceEditor](InplaceEditor.md) Parameters: content - Content to be inserted. Returns: true if the event was handled or false if the form control can do nothing with the string. For example a text field can insert the text inside it but a check box form control can do nothing with it. If false is returned the form control editing session will be stopped and the author page will handle the event instead. See Also:
        * [InplaceEditor.insertContent(java.lang.String)](InplaceEditor.md#insertContent(java.lang.String))

### commitValue

public void commitValue()
 Description copied from interface: [InplaceEditor](InplaceEditor.md#commitValue())
Commit the given value inside the document without stopping the editing. Will only commit if a new string value is provided and only if the value that must be committed is different from the current value.
  Specified by: [commitValue](InplaceEditor.md#commitValue()) in interface [InplaceEditor](InplaceEditor.md) See Also:
        * [InplaceEditor.commitValue()](InplaceEditor.md#commitValue())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
