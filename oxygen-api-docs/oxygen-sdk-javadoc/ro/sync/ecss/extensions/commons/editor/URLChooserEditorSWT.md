Package [ro.sync.ecss.extensions.commons.editor](package-summary.md)

# Class URLChooserEditorSWT

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.editor.AbstractInplaceEditor](../../api/editor/AbstractInplaceEditor.md)
        * ro.sync.ecss.extensions.commons.editor.URLChooserEditorSWT
   All Implemented Interfaces: org.eclipse.jface.text.ITextOperationTarget, [InplaceEditor](../../api/editor/InplaceEditor.md), [Extension](../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class URLChooserEditorSWT extends [AbstractInplaceEditor](../../api/editor/AbstractInplaceEditor.md)implements org.eclipse.jface.text.ITextOperationTarget
URL Chooser in-place editor on Eclipse.

## Field Summary

### Fields inherited from interface org.eclipse.jface.text.ITextOperationTarget
 COPY, CUT, DELETE, PASTE, PREFIX, PRINT, REDO, SELECT_ALL, SHIFT_LEFT, SHIFT_RIGHT, STRIP_PREFIX, UNDO
## Constructor Summary
 Constructors
Constructor

Description
 [URLChooserEditorSWT](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [cancelEditing](#cancelEditing())()
Cancels the editing process.
  boolean [canDoOperation](#canDoOperation(int))(int operation)

 void [commitValue](#commitValue())()
Commit the given value inside the document without stopping the editing.
  void [doOperation](#doOperation(int))(int operation)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getEditorComponent](#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point))([AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context, [Rectangle](../../../../exml/view/graphics/Rectangle.md) allocation, [Point](../../../../exml/view/graphics/Point.md) mouseInvocationLocation)
Prepare and return the editor component.
  [Rectangle](../../../../exml/view/graphics/Rectangle.md) [getScrollRectangle](#getScrollRectangle())()
Returns a rectangle that should be made visible after the editor is shown.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getValue](#getValue())()
Gets the value that the user entered.
  void [refresh](#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)
While this editor is inside an editing session a document change was detected that didn't originated form this editor.
  void [requestFocus](#requestFocus())()
Requests focus inside the editing component.
  void [stopEditing](#stopEditing())()
Stops the editing and commits the current value.

### Methods inherited from class ro.sync.ecss.extensions.api.editor.[AbstractInplaceEditor](../../api/editor/AbstractInplaceEditor.md)
 [addEditingListener](../../api/editor/AbstractInplaceEditor.md#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener)), [fireCommitValue](../../api/editor/AbstractInplaceEditor.md#fireCommitValue(ro.sync.ecss.extensions.api.editor.EditingEvent)), [fireEditingCanceled](../../api/editor/AbstractInplaceEditor.md#fireEditingCanceled()), [fireEditingOccured](../../api/editor/AbstractInplaceEditor.md#fireEditingOccured()), [fireEditingStopped](../../api/editor/AbstractInplaceEditor.md#fireEditingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)), [fireNextEditLocationRequested](../../api/editor/AbstractInplaceEditor.md#fireNextEditLocationRequested()), [firePreviousEditLocationRequested](../../api/editor/AbstractInplaceEditor.md#firePreviousEditLocationRequested()), [getBoolean](../../api/editor/AbstractInplaceEditor.md#getBoolean(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,java.lang.String)), [insertContent](../../api/editor/AbstractInplaceEditor.md#insertContent(java.lang.String)), [removeEditingListener](../../api/editor/AbstractInplaceEditor.md#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.editor.[InplaceEditor](../../api/editor/InplaceEditor.md)
 [allowsRepostingEvents](../../api/editor/InplaceEditor.md#allowsRepostingEvents())
## Constructor Details

### URLChooserEditorSWT

public URLChooserEditorSWT()

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../api/Extension.md#getDescription()) in interface [Extension](../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

### getEditorComponent

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getEditorComponent([AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context, [Rectangle](../../../../exml/view/graphics/Rectangle.md) allocation, [Point](../../../../exml/view/graphics/Point.md) mouseInvocationLocation)
 Description copied from interface: [InplaceEditor](../../api/editor/InplaceEditor.md#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point))
Prepare and return the editor component.
  Specified by: [getEditorComponent](../../api/editor/InplaceEditor.md#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point)) in interface [InplaceEditor](../../api/editor/InplaceEditor.md) Parameters: context - The context where the editor will be used. allocation - The bounds where the editor will be shown. This is normally the bounds of the box in which the value being edited is rendered. If the editor requires to be presented in different bounds it should alter this parameter. The X,Y coordinates are relative to the parent in which the editor will be added. mouseInvocationLocation - if the editor was requested using the mouse this parameter represents the X,Y location where the event took place. It is relative to the parent in which the editor will be added. null if the editor wasn't requested through mouse interaction.   **OBS**: This is the very first call received by an editor. This ensures that the editor is properly initialized for the subsequent calls (like a [InplaceEditor.requestFocus()](../../api/editor/InplaceEditor.md#requestFocus()) call).  **OBS**: An editor implementation will have to add listeners onto itself like:
        * a [KeyListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/KeyListener.html) for handling key events like: ENTER to stop editing (by calling [InplaceEditingListener.editingStopped(EditingEvent)](../../api/editor/InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))) and ESCAPE to cancel it (by calling [InplaceEditingListener.editingCanceled()](../../api/editor/InplaceEditingListener.md#editingCanceled())).
        * a [FocusListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/FocusListener.html) to stop editing when the focus is given to a component that is not part of the editor (by calling [InplaceEditingListener.editingStopped(EditingEvent)](../../api/editor/InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))).
        * a [DocumentListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/DocumentListener.html) to fire [InplaceEditingListener.editingOccured()](../../api/editor/InplaceEditingListener.md#editingOccured()) events (If the editor has a document).
 Returns: The component that performs the editing. For the Standalone distribution this should be a java.awt.JComponent implementation. For the Eclipse plugin distribution, an org.eclipse.swt.widgets.Control is expected. See Also:
        * [InplaceEditor.getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext, ro.sync.exml.view.graphics.Rectangle, ro.sync.exml.view.graphics.Point)](../../api/editor/InplaceEditor.md#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point))

### getScrollRectangle

public [Rectangle](../../../../exml/view/graphics/Rectangle.md) getScrollRectangle()
 Description copied from interface: [InplaceEditor](../../api/editor/InplaceEditor.md#getScrollRectangle())
Returns a rectangle that should be made visible after the editor is shown. The coordinate should be relative to the editor itself. The default behavior is to make the entire editor visible but if the editor is bigger than the viewport the visible part might not be the right one. For example is the editor is a text field the caret might not be visible. This is when this method is useful. The caret rectangle should be returned so that the part of the editor with the caret is presented.
  Specified by: [getScrollRectangle](../../api/editor/InplaceEditor.md#getScrollRectangle()) in interface [InplaceEditor](../../api/editor/InplaceEditor.md) Returns: A rectangle to be made visible or null to make the entire editor visible. See Also:
        * [InplaceEditor.getScrollRectangle()](../../api/editor/InplaceEditor.md#getScrollRectangle())

### requestFocus

public void requestFocus()
 Description copied from interface: [InplaceEditor](../../api/editor/InplaceEditor.md#requestFocus())
Requests focus inside the editing component.
  Specified by: [requestFocus](../../api/editor/InplaceEditor.md#requestFocus()) in interface [InplaceEditor](../../api/editor/InplaceEditor.md) See Also:
        * [InplaceEditor.requestFocus()](../../api/editor/InplaceEditor.md#requestFocus())

### getValue

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getValue()
 Description copied from interface: [InplaceEditor](../../api/editor/InplaceEditor.md#getValue())
Gets the value that the user entered.
  Specified by: [getValue](../../api/editor/InplaceEditor.md#getValue()) in interface [InplaceEditor](../../api/editor/InplaceEditor.md) Returns: The value that the user entered. See Also:
        * [InplaceEditor.getValue()](../../api/editor/InplaceEditor.md#getValue())

### stopEditing

public void stopEditing()
 Description copied from interface: [InplaceEditor](../../api/editor/InplaceEditor.md#stopEditing())
Stops the editing and commits the current value. The editor should release any held resources and notify [InplaceEditingListener.editingStopped(EditingEvent)](../../api/editor/InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)). OBS: The current value will be committed only if at least one [InplaceEditingListener.editingOccured()](../../api/editor/InplaceEditingListener.md#editingOccured()) event was issued before this moment.
  Specified by: [stopEditing](../../api/editor/InplaceEditor.md#stopEditing()) in interface [InplaceEditor](../../api/editor/InplaceEditor.md) See Also:
        * [InplaceEditor.stopEditing()](../../api/editor/InplaceEditor.md#stopEditing())

### commitValue

public void commitValue()
 Description copied from interface: [InplaceEditor](../../api/editor/InplaceEditor.md#commitValue())
Commit the given value inside the document without stopping the editing. Will only commit if a new string value is provided and only if the value that must be committed is different from the current value.
  Specified by: [commitValue](../../api/editor/InplaceEditor.md#commitValue()) in interface [InplaceEditor](../../api/editor/InplaceEditor.md) Overrides: [commitValue](../../api/editor/AbstractInplaceEditor.md#commitValue()) in class [AbstractInplaceEditor](../../api/editor/AbstractInplaceEditor.md) See Also:
        * [InplaceEditor.commitValue()](../../api/editor/InplaceEditor.md#commitValue())

### cancelEditing

public void cancelEditing()
 Description copied from interface: [InplaceEditor](../../api/editor/InplaceEditor.md#cancelEditing())
Cancels the editing process. The editor should release any held resources and notify [InplaceEditingListener.editingCanceled()](../../api/editor/InplaceEditingListener.md#editingCanceled()).
  Specified by: [cancelEditing](../../api/editor/InplaceEditor.md#cancelEditing()) in interface [InplaceEditor](../../api/editor/InplaceEditor.md) See Also:
        * [InplaceEditor.cancelEditing()](../../api/editor/InplaceEditor.md#cancelEditing())

### canDoOperation

public boolean canDoOperation(int operation)
  Specified by: canDoOperation in interface org.eclipse.jface.text.ITextOperationTarget See Also:
        * ITextOperationTarget.canDoOperation(int)

### doOperation

public void doOperation(int operation)
  Specified by: doOperation in interface org.eclipse.jface.text.ITextOperationTarget See Also:
        * ITextOperationTarget.doOperation(int)

### refresh

public void refresh([AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)
 Description copied from interface: [InplaceEditor](../../api/editor/InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))
While this editor is inside an editing session a document change was detected that didn't originated form this editor. In this situation it might be good for the editor to refresh the presented data. Currently this method is called if:
        * This editor edits an attribute and the same attribute was externally modified. In this situation is recommended for the editor to update the current value.

  Specified by: [refresh](../../api/editor/InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)) in interface [InplaceEditor](../../api/editor/InplaceEditor.md) Overrides: [refresh](../../api/editor/AbstractInplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)) in class [AbstractInplaceEditor](../../api/editor/AbstractInplaceEditor.md) Parameters: context - An updated editing context for this editor. See Also:
        * [InplaceEditor.refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)](../../api/editor/InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
