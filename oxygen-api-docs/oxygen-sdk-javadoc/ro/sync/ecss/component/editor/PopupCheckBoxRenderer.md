Package [ro.sync.ecss.component.editor](package-summary.md)

# Class PopupCheckBoxRenderer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.component.editor.PopupCheckBoxRenderer
   All Implemented Interfaces: ro.sync.ecss.component.editor.LoggableInplaceRenderer, [InplaceRenderer](../../extensions/api/editor/InplaceRenderer.md), [Extension](../../extensions/api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class PopupCheckBoxRenderer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [InplaceRenderer](../../extensions/api/editor/InplaceRenderer.md), ro.sync.ecss.component.editor.LoggableInplaceRenderer
Presents a simple or a composed value (multiple values separated by a separator) using a JLabel.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EMPTY_LABEL](#EMPTY_LABEL)
The text to render for empty labels.
  protected static final ro.sync.i18n.MessageBundle [messages](#messages)
The messages resource bundle.

## Constructor Summary
 Constructors
Constructor

Description
 [PopupCheckBoxRenderer](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [dump](#dump(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,java.lang.StringBuilder))([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) inplaceContext, [StringBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/StringBuilder.html) builder)

 [CursorType](../../extensions/api/CursorType.md) [getCursorType](#getCursorType(int,int))(int x, int y)
Get a cursor to be used when the user hovers with the mouse over this renderer.
  [CursorType](../../extensions/api/CursorType.md) [getCursorType](#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) context, int x, int y)
Get a cursor to be used when the user hovers with the mouse over this renderer.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getRendererComponent](#getRendererComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) context)
Initialize the renderer with the given context and returns the component.
  [RendererLayoutInfo](../../extensions/api/editor/RendererLayoutInfo.md) [getRenderingInfo](#getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) context)
Returns the rendering layout info.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTooltipText](#getTooltipText(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) context, int x, int y)
Gets a tooltip text to be presented when the cursor is over this renderer.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### messages

protected static final ro.sync.i18n.MessageBundle messages

The messages resource bundle.

### EMPTY_LABEL

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EMPTY_LABEL

The text to render for empty labels.

## Constructor Details

### PopupCheckBoxRenderer

public PopupCheckBoxRenderer()

Constructor.

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../extensions/api/Extension.md#getDescription()) in interface [Extension](../../extensions/api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../extensions/api/Extension.md#getDescription())

### getRendererComponent

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getRendererComponent([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) context)
 Description copied from interface: [InplaceRenderer](../../extensions/api/editor/InplaceRenderer.md#getRendererComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))
Initialize the renderer with the given context and returns the component. It's up to the caller to use the renderer to paint.
  Specified by: [getRendererComponent](../../extensions/api/editor/InplaceRenderer.md#getRendererComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)) in interface [InplaceRenderer](../../extensions/api/editor/InplaceRenderer.md) Parameters: context - The editing context. Returns: The renderer. A java.awt.Component implementation. See Also:
        * [InplaceRenderer.getRendererComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)](../../extensions/api/editor/InplaceRenderer.md#getRendererComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))

### getRenderingInfo

public [RendererLayoutInfo](../../extensions/api/editor/RendererLayoutInfo.md) getRenderingInfo([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) context)
 Description copied from interface: [InplaceRenderer](../../extensions/api/editor/InplaceRenderer.md#getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))
Returns the rendering layout info. This contains information about the baseline and the size in a certain context. The baseline is measured from the top of the component. **Because a renderer is reused, when this call is received, the renderer must re-initialize itself from the given context.**
  Specified by: [getRenderingInfo](../../extensions/api/editor/InplaceRenderer.md#getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)) in interface [InplaceRenderer](../../extensions/api/editor/InplaceRenderer.md) Parameters: context - The editing context. Returns: The rendering layout info. See Also:
        * [InplaceRenderer.getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)](../../extensions/api/editor/InplaceRenderer.md#getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))

### getTooltipText

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTooltipText([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) context, int x, int y)
 Description copied from interface: [InplaceRenderer](../../extensions/api/editor/InplaceRenderer.md#getTooltipText(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))
Gets a tooltip text to be presented when the cursor is over this renderer. **Because a renderer is reused, when this called is received, the renderer must re-initialize itself from the given context.**
  Specified by: [getTooltipText](../../extensions/api/editor/InplaceRenderer.md#getTooltipText(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int)) in interface [InplaceRenderer](../../extensions/api/editor/InplaceRenderer.md) Parameters: context - The editing context. x - The x coordinate relative to the renderer bounds. y - The y coordinate relative to the renderer bounds. Returns: A tooltip text or null if no tooltip. See Also:
        * [InplaceRenderer.getTooltipText(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext, int, int)](../../extensions/api/editor/InplaceRenderer.md#getTooltipText(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))

### getCursorType

public [CursorType](../../extensions/api/CursorType.md) getCursorType([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) context, int x, int y)
 Description copied from interface: [InplaceRenderer](../../extensions/api/editor/InplaceRenderer.md#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))
Get a cursor to be used when the user hovers with the mouse over this renderer. For a more complex renderer, the given X,Y coordinates can be used to decide what cursor to return.
  Specified by: [getCursorType](../../extensions/api/editor/InplaceRenderer.md#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int)) in interface [InplaceRenderer](../../extensions/api/editor/InplaceRenderer.md) Parameters: context - The editing context. Useful if the renderer is a more complex one, like a text field with an associated button and wants to provide different cursors when the cursor is over the textfield or over the button. In this case the renderer will have to initialize itself with this context in order to decide what the cursor is hovering. x - The x coordinate relative to the renderer bounds. y - The y coordinate relative to the renderer bounds. Returns: The type of cursor to be used or null to let the viewport decide. See Also:
        * [InplaceRenderer.getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext, int, int)](../../extensions/api/editor/InplaceRenderer.md#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int))

### getCursorType

public [CursorType](../../extensions/api/CursorType.md) getCursorType(int x, int y)
 Description copied from interface: [InplaceRenderer](../../extensions/api/editor/InplaceRenderer.md#getCursorType(int,int))
Get a cursor to be used when the user hovers with the mouse over this renderer. For a more complex renderer, the given X,Y coordinates can be used to decide what cursor to return. We recommend using [InplaceRenderer.getCursorType(AuthorInplaceContext, int, int)](../../extensions/api/editor/InplaceRenderer.md#getCursorType(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,int,int)) as you can use the provided context to get additional information.
  Specified by: [getCursorType](../../extensions/api/editor/InplaceRenderer.md#getCursorType(int,int)) in interface [InplaceRenderer](../../extensions/api/editor/InplaceRenderer.md) Parameters: x - The x coordinate relative to the renderer bounds. y - The y coordinate relative to the renderer bounds. Returns: The type of cursor to be used or null to let the viewport decide. See Also:
        * [InplaceRenderer.getCursorType(int, int)](../../extensions/api/editor/InplaceRenderer.md#getCursorType(int,int))

### dump

public void dump([AuthorInplaceContext](../../extensions/api/editor/AuthorInplaceContext.md) inplaceContext, [StringBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/StringBuilder.html) builder)
  Specified by: dump in interface ro.sync.ecss.component.editor.LoggableInplaceRenderer See Also:
        * LoggableInplaceRenderer.dump(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext, java.lang.StringBuilder)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
