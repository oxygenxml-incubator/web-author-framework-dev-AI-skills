Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Class InplaceEditorRendererAdapter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.editor.InplaceEditorRendererAdapter
   All Implemented Interfaces: [InplaceEditor](InplaceEditor.md), [InplaceRenderer](InplaceRenderer.md), [Extension](../Extension.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class InplaceEditorRendererAdapter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [InplaceRenderer](InplaceRenderer.md), [InplaceEditor](InplaceEditor.md)
Convenience implementation of the [InplaceRenderer](InplaceRenderer.md) and [InplaceEditor](InplaceEditor.md). By extending this adapter you are protected if any new methods are added inside [InplaceRenderer](InplaceRenderer.md) or [InplaceEditor](InplaceEditor.md).
  Since: 14.1
## Constructor Summary
 Constructors
Constructor

Description
 [InplaceEditorRendererAdapter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addEditingListener](#addEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))([InplaceEditingListener](InplaceEditingListener.md) editingListener)
Adds a listener to receive edit notifications: - [InplaceEditingListener.editingCanceled()](InplaceEditingListener.md#editingCanceled()) to remove the editor and cancel the edit operation.
  void [cancelEditing](#cancelEditing())()
Cancels the editing process.
  void [commitValue](#commitValue())()
Commit the given value inside the document without stopping the editing.
  [CursorType](../CursorType.md) [getCursorType](#getCursorType(int,int))(int x, int y)
Get a cursor to be used when the user hovers with the mouse over this renderer.
  [CursorType](../CursorType.md) [getCursorType](#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))([AuthorInplaceContext](AuthorInplaceContext.md) context, int x, int y)
Get a cursor to be used when the user hovers with the mouse over this renderer.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getEditorComponent](#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point))([AuthorInplaceContext](AuthorInplaceContext.md) context, [Rectangle](../../../../exml/view/graphics/Rectangle.md) allocation, [Point](../../../../exml/view/graphics/Point.md) mouseLocation)
Prepare and return the editor component.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getRendererComponent](#getRendererComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](AuthorInplaceContext.md) context)
Initialize the renderer with the given context and returns the component.
  [RendererLayoutInfo](RendererLayoutInfo.md) [getRenderingInfo](#getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](AuthorInplaceContext.md) context)
Returns the rendering layout info.
  [Rectangle](../../../../exml/view/graphics/Rectangle.md) [getScrollRectangle](#getScrollRectangle())()
Returns a rectangle that should be made visible after the editor is shown.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTooltipText](#getTooltipText(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))([AuthorInplaceContext](AuthorInplaceContext.md) context, int x, int y)
Gets a tooltip text to be presented when the cursor is over this renderer.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getValue](#getValue())()
Gets the value that the user entered.
  void [removeEditingListener](#removeEditingListener(ro.sync.ecss.extensions.api.editor.InplaceEditingListener))([InplaceEditingListener](InplaceEditingListener.md) editingListener)
Removes a listener that receives editing events.
  void [requestFocus](#requestFocus())()
Requests focus inside the editing component.
  void [stopEditing](#stopEditing())()
Stops the editing and commits the current value.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.editor.[InplaceEditor](InplaceEditor.md)
 [allowsRepostingEvents](InplaceEditor.md#allowsRepostingEvents()), [insertContent](InplaceEditor.md#insertContent(java.lang.String)), [refresh](InplaceEditor.md#refresh(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))
## Constructor Details

### InplaceEditorRendererAdapter

public InplaceEditorRendererAdapter()

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../Extension.md#getDescription()) in interface [Extension](../Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../Extension.md#getDescription())

### getRendererComponent

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getRendererComponent([AuthorInplaceContext](AuthorInplaceContext.md) context)
 Description copied from interface: [InplaceRenderer](InplaceRenderer.md#getRendererComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))
Initialize the renderer with the given context and returns the component. It's up to the caller to use the renderer to paint.
  Specified by: [getRendererComponent](InplaceRenderer.md#getRendererComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)) in interface [InplaceRenderer](InplaceRenderer.md) Parameters: context - The editing context. Returns: The renderer. A java.awt.Component implementation. See Also:
        * [InplaceRenderer.getRendererComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)](InplaceRenderer.md#getRendererComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))

### getRenderingInfo

public [RendererLayoutInfo](RendererLayoutInfo.md) getRenderingInfo([AuthorInplaceContext](AuthorInplaceContext.md) context)
 Description copied from interface: [InplaceRenderer](InplaceRenderer.md#getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))
Returns the rendering layout info. This contains information about the baseline and the size in a certain context. The baseline is measured from the top of the component. **Because a renderer is reused, when this call is received, the renderer must re-initialize itself from the given context.**
  Specified by: [getRenderingInfo](InplaceRenderer.md#getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)) in interface [InplaceRenderer](InplaceRenderer.md) Parameters: context - The editing context. Returns: The rendering layout info. See Also:
        * [InplaceRenderer.getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)](InplaceRenderer.md#getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))

### getTooltipText

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTooltipText([AuthorInplaceContext](AuthorInplaceContext.md) context, int x, int y)
 Description copied from interface: [InplaceRenderer](InplaceRenderer.md#getTooltipText(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))
Gets a tooltip text to be presented when the cursor is over this renderer. **Because a renderer is reused, when this called is received, the renderer must re-initialize itself from the given context.**
  Specified by: [getTooltipText](InplaceRenderer.md#getTooltipText(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int)) in interface [InplaceRenderer](InplaceRenderer.md) Parameters: context - The editing context. x - The x coordinate relative to the renderer bounds. y - The y coordinate relative to the renderer bounds. Returns: A tooltip text or null if no tooltip. See Also:
        * [InplaceRenderer.getTooltipText(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext, int, int)](InplaceRenderer.md#getTooltipText(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))

### getEditorComponent

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getEditorComponent([AuthorInplaceContext](AuthorInplaceContext.md) context, [Rectangle](../../../../exml/view/graphics/Rectangle.md) allocation, [Point](../../../../exml/view/graphics/Point.md) mouseLocation)
 Description copied from interface: [InplaceEditor](InplaceEditor.md#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point))
Prepare and return the editor component.
  Specified by: [getEditorComponent](InplaceEditor.md#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle,ro.sync.exml.view.graphics.Point)) in interface [InplaceEditor](InplaceEditor.md) Parameters: context - The context where the editor will be used. allocation - The bounds where the editor will be shown. This is normally the bounds of the box in which the value being edited is rendered. If the editor requires to be presented in different bounds it should alter this parameter. The X,Y coordinates are relative to the parent in which the editor will be added. mouseLocation - if the editor was requested using the mouse this parameter represents the X,Y location where the event took place. It is relative to the parent in which the editor will be added. null if the editor wasn't requested through mouse interaction.   **OBS**: This is the very first call received by an editor. This ensures that the editor is properly initialized for the subsequent calls (like a [InplaceEditor.requestFocus()](InplaceEditor.md#requestFocus()) call).  **OBS**: An editor implementation will have to add listeners onto itself like:
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

### getCursorType

public [CursorType](../CursorType.md) getCursorType([AuthorInplaceContext](AuthorInplaceContext.md) context, int x, int y)
 Description copied from interface: [InplaceRenderer](InplaceRenderer.md#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))
Get a cursor to be used when the user hovers with the mouse over this renderer. For a more complex renderer, the given X,Y coordinates can be used to decide what cursor to return.
  Specified by: [getCursorType](InplaceRenderer.md#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int)) in interface [InplaceRenderer](InplaceRenderer.md) Parameters: context - The editing context. Useful if the renderer is a more complex one, like a text field with an associated button and wants to provide different cursors when the cursor is over the textfield or over the button. In this case the renderer will have to initialize itself with this context in order to decide what the cursor is hovering. x - The x coordinate relative to the renderer bounds. y - The y coordinate relative to the renderer bounds. Returns: The type of cursor to be used or null to let the viewport decide. See Also:
        * [InplaceRenderer.getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext, int, int)](InplaceRenderer.md#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))

### getCursorType

public [CursorType](../CursorType.md) getCursorType(int x, int y)
 Description copied from interface: [InplaceRenderer](InplaceRenderer.md#getCursorType(int,int))
Get a cursor to be used when the user hovers with the mouse over this renderer. For a more complex renderer, the given X,Y coordinates can be used to decide what cursor to return. We recommend using [InplaceRenderer.getCursorType(AuthorInplaceContext, int, int)](InplaceRenderer.md#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int)) as you can use the provided context to get additional information.
  Specified by: [getCursorType](InplaceRenderer.md#getCursorType(int,int)) in interface [InplaceRenderer](InplaceRenderer.md) Parameters: x - The x coordinate relative to the renderer bounds. y - The y coordinate relative to the renderer bounds. Returns: The type of cursor to be used or null to let the viewport decide. See Also:
        * [InplaceRenderer.getCursorType(int, int)](InplaceRenderer.md#getCursorType(int,int))

### commitValue

public void commitValue()
 Description copied from interface: [InplaceEditor](InplaceEditor.md#commitValue())
Commit the given value inside the document without stopping the editing. Will only commit if a new string value is provided and only if the value that must be committed is different from the current value.
  Specified by: [commitValue](InplaceEditor.md#commitValue()) in interface [InplaceEditor](InplaceEditor.md) See Also:
        * [InplaceEditor.commitValue()](InplaceEditor.md#commitValue())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
