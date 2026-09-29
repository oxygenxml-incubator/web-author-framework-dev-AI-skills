Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Class InplaceRendererAdapter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.editor.InplaceRendererAdapter
   All Implemented Interfaces: [InplaceRenderer](InplaceRenderer.md), [Extension](../Extension.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class InplaceRendererAdapter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [InplaceRenderer](InplaceRenderer.md)
Convenience implementation of the [InplaceRenderer](InplaceRenderer.md). By extending this adapter you are protected if any new methods are added inside [InplaceRenderer](InplaceRenderer.md).
  Since: 14.1
## Constructor Summary
 Constructors
Constructor

Description
 [InplaceRendererAdapter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [CursorType](../CursorType.md) [getCursorType](#getCursorType(int,int))(int x, int y)
Get a cursor to be used when the user hovers with the mouse over this renderer.
  [CursorType](../CursorType.md) [getCursorType](#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))([AuthorInplaceContext](AuthorInplaceContext.md) context, int x, int y)
Get a cursor to be used when the user hovers with the mouse over this renderer.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getRendererComponent](#getRendererComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](AuthorInplaceContext.md) context)
Initialize the renderer with the given context and returns the component.
  [RendererLayoutInfo](RendererLayoutInfo.md) [getRenderingInfo](#getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](AuthorInplaceContext.md) context)
Returns the rendering layout info.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTooltipText](#getTooltipText(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))([AuthorInplaceContext](AuthorInplaceContext.md) context, int x, int y)
Gets a tooltip text to be presented when the cursor is over this renderer.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### InplaceRendererAdapter

public InplaceRendererAdapter()

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

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
