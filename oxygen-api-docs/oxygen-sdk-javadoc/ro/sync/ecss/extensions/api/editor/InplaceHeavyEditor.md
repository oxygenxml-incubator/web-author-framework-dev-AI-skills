Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Interface InplaceHeavyEditor
    All Superinterfaces: [Extension](../Extension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface InplaceHeavyEditorextends [Extension](../Extension.md)
A form control that appears inside the author page. It differs from the classic form control by the fact that it is placed in the component hierarchy from the very beginning.
  Since: 18.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [deactivate](#deactivate())()
An event that comes when the page that presents this form control is no longer active.
  void [dispose](#dispose())()
The editor was removed from the layout and it will not be used anymore.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getEditorComponent](#getEditorComponent(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext,ro.sync.exml.view.graphics.Rectangle))([AuthorInplaceContext](AuthorInplaceContext.md) context, [Rectangle](../../../../exml/view/graphics/Rectangle.md) allocation)
Prepare and return the editor component.
  [RendererLayoutInfo](RendererLayoutInfo.md) [getRenderingInfo](#getRenderingInfo(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](AuthorInplaceContext.md) context)
Returns the rendering layout info.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../Extension.md)
 [getDescription](../Extension.md#getDescription())
## Method Details

### getRenderingInfo

[RendererLayoutInfo](RendererLayoutInfo.md) getRenderingInfo([AuthorInplaceContext](AuthorInplaceContext.md) context)

Returns the rendering layout info. This contains information about the baseline and the size in a certain context. The baseline is measured from the top of the component. **Because a renderer is reused, when this call is received, the renderer must re-initialize itself from the given context.**
  Parameters: context - The editing context. Returns: The rendering layout info.
### getEditorComponent

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getEditorComponent([AuthorInplaceContext](AuthorInplaceContext.md) context, [Rectangle](../../../../exml/view/graphics/Rectangle.md) allocation)

Prepare and return the editor component.
  Parameters: context - The context where the editor will be used. allocation - The bounds where the form control will be presented. Returns: The component that performs the editing. For the Standalone distribution, this should be a java.awt.JComponent implementation. For the Eclipse plugin distribution, an org.eclipse.swt.widgets.Control is expected.
### dispose

void dispose()

The editor was removed from the layout and it will not be used anymore. This is the time to dispose any resources allocated with it.

### deactivate

void deactivate()

An event that comes when the page that presents this form control is no longer active. For example another editor was selected. For example, if a media player form control that is playing receives this event it should pause.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
