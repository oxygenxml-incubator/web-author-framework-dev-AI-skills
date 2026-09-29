Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Interface InplaceRenderer
    All Superinterfaces: [Extension](../Extension.md)   All Known Implementing Classes: [ButtonEditor](../../../component/editor/ButtonEditor.md), [ButtonGroupEditor](../../../component/editor/ButtonGroupEditor.md), [CheckBoxEditor](../../../component/editor/CheckBoxEditor.md), [DatePickerEditor](../../../component/editor/DatePickerEditor.md), [HtmlContentEditor](../../../component/editor/HtmlContentEditor.md), [InplaceEditorRendererAdapter](InplaceEditorRendererAdapter.md), [InplaceRendererAdapter](InplaceRendererAdapter.md), [InputURLEditor](../../../component/editor/InputURLEditor.md), [PopupCheckBoxRenderer](../../../component/editor/PopupCheckBoxRenderer.md), [SimpleURLChooserEditor](../../commons/editor/SimpleURLChooserEditor.md), [TextFieldEditor](../../../component/editor/TextFieldEditor.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface InplaceRendererextends [Extension](../Extension.md)
An author in-place renderer. Subclasses contain implementation based on real SWT or Swing components like combo boxes, text fields, check boxes, buttons etc.
A renderer is associated with an oxy_editor CSS function and it's the instance that handles the painting of the value that the [InplaceEditor](InplaceEditor.md) will edit.

It is recommended to extend the adapter class [InplaceEditorRendererAdapter](InplaceEditorRendererAdapter.md)or [InplaceRendererAdapter](InplaceRendererAdapter.md) in order to be protected from future API additions.

A renderer of a certain type will be reused to render in different contexts so the renderer must initialize itself for the given [AuthorInplaceContext](AuthorInplaceContext.md) on each of its called methods. Example: For the following CSS, the same **combo** renderer (same instance) will be used for both attributes. So for each callback it must prepare itself for the current context.

```

 code {
   content: 
     "Attr1: " oxy_editor(type, combo, edit, '@attr1')
     "Attr2: " oxy_editor(type, combo, edit, '@attr2')
  }

```

 For a custom implementation property [InplaceEditorCSSConstants.PROPERTY_RENDERER_CLASS_NAME](InplaceEditorCSSConstants.md#PROPERTY_RENDERER_CLASS_NAME)must be used. The same implementation will be used in Standalone or Eclipse plugin environment:

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

In the previous example, the renderer class com.custom.editors.CustomRenderer must be added in the Classpath of the document type associated with the edited document.

  Since: 14.1 See Also:
* [SimpleURLChooserEditor](../../commons/editor/SimpleURLChooserEditor.md)

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [CursorType](../CursorType.md) [getCursorType](#getCursorType(int,int))(int x, int y)
Get a cursor to be used when the user hovers with the mouse over this renderer.
  [CursorType](../CursorType.md) [getCursorType](#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))([AuthorInplaceContext](AuthorInplaceContext.md) context, int x, int y)
Get a cursor to be used when the user hovers with the mouse over this renderer.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getRendererComponent](#getRendererComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](AuthorInplaceContext.md) context)
Initialize the renderer with the given context and returns the component.
  [RendererLayoutInfo](RendererLayoutInfo.md) [getRenderingInfo](#getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](AuthorInplaceContext.md) context)
Returns the rendering layout info.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTooltipText](#getTooltipText(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))([AuthorInplaceContext](AuthorInplaceContext.md) context, int x, int y)
Gets a tooltip text to be presented when the cursor is over this renderer.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../Extension.md)
 [getDescription](../Extension.md#getDescription())
## Method Details

### getRendererComponent

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getRendererComponent([AuthorInplaceContext](AuthorInplaceContext.md) context)

Initialize the renderer with the given context and returns the component. It's up to the caller to use the renderer to paint.
  Parameters: context - The editing context. Returns: The renderer. A java.awt.Component implementation.
### getCursorType

[CursorType](../CursorType.md) getCursorType([AuthorInplaceContext](AuthorInplaceContext.md) context, int x, int y)

Get a cursor to be used when the user hovers with the mouse over this renderer. For a more complex renderer, the given X,Y coordinates can be used to decide what cursor to return.
  Parameters: context - The editing context. Useful if the renderer is a more complex one, like a text field with an associated button and wants to provide different cursors when the cursor is over the textfield or over the button. In this case the renderer will have to initialize itself with this context in order to decide what the cursor is hovering. x - The x coordinate relative to the renderer bounds. y - The y coordinate relative to the renderer bounds. Returns: The type of cursor to be used or null to let the viewport decide.
### getCursorType

[CursorType](../CursorType.md) getCursorType(int x, int y)

Get a cursor to be used when the user hovers with the mouse over this renderer. For a more complex renderer, the given X,Y coordinates can be used to decide what cursor to return. We recommend using [getCursorType(AuthorInplaceContext, int, int)](#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int)) as you can use the provided context to get additional information.
  Parameters: x - The x coordinate relative to the renderer bounds. y - The y coordinate relative to the renderer bounds. Returns: The type of cursor to be used or null to let the viewport decide.
### getTooltipText

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTooltipText([AuthorInplaceContext](AuthorInplaceContext.md) context, int x, int y)

Gets a tooltip text to be presented when the cursor is over this renderer. **Because a renderer is reused, when this called is received, the renderer must re-initialize itself from the given context.**
  Parameters: context - The editing context. x - The x coordinate relative to the renderer bounds. y - The y coordinate relative to the renderer bounds. Returns: A tooltip text or null if no tooltip.
### getRenderingInfo

[RendererLayoutInfo](RendererLayoutInfo.md) getRenderingInfo([AuthorInplaceContext](AuthorInplaceContext.md) context)

Returns the rendering layout info. This contains information about the baseline and the size in a certain context. The baseline is measured from the top of the component. **Because a renderer is reused, when this call is received, the renderer must re-initialize itself from the given context.**
  Parameters: context - The editing context. Returns: The rendering layout info.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
