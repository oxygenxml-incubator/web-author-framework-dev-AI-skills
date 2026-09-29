# Package ro.sync.ecss.extensions.api.editor

package ro.sync.ecss.extensions.api.editor
    Related Packages
Package

Description
 [ro.sync.ecss.extensions.api](../package-summary.md)
Main API package used for controlling the Author page (making modifications, adding listeners).
      All Classes and InterfacesInterfacesClasses
Class

Description
 [AbstractInplaceEditor](AbstractInplaceEditor.md)
An abstract implementation that handles listeners fire.
  [AbstractInplaceEditorWrapper](AbstractInplaceEditorWrapper.md)
It can be used when more than one editor types are needed depending on the received context and it can choose at runtime an appropriate editor implementation.
  [AuthorExtensionAskAction](AuthorExtensionAskAction.md)
An author action created over an author operation who does not handle the ask variables expansion.
  [AuthorInplaceContext](AuthorInplaceContext.md)
Context where an edit component will be used.
  [DynamicPropertyEvaluator](DynamicPropertyEvaluator.md)
Some form control properties can't be evaluated at the time the CSS is compiled.
  [EditingEvent](EditingEvent.md)
The in-place editing was stopped.
  [IAuthorExtensionAction](IAuthorExtensionAction.md)
An author action created over an author operation.
  [InplaceEditingListener](InplaceEditingListener.md)
Gets notified about edit events: [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) - a request to stop the editing and commit the value from the editor.
  [InplaceEditingTraversalListener](InplaceEditingTraversalListener.md)
Gets notified about focus traversal keys TAB and SHIFT-TAB.
  [InplaceEditor](InplaceEditor.md)
An author in-place editor.
  [InplaceEditorAdapter](InplaceEditorAdapter.md)
Convenience implementation of the [InplaceEditor](InplaceEditor.md).
  [InplaceEditorArgumentKeys](InplaceEditorArgumentKeys.md)
Properties of the oxy_editor function extended with other computed properties that the renderer/editor might need.
  [InplaceEditorCSSConstants](InplaceEditorCSSConstants.md)
Arguments of the oxy_editor function as well as built-in values for some of these arguments.
  [InplaceEditorRendererAdapter](InplaceEditorRendererAdapter.md)
Convenience implementation of the [InplaceRenderer](InplaceRenderer.md) and [InplaceEditor](InplaceEditor.md).
  [InplaceHeavyEditor](InplaceHeavyEditor.md)
A form control that appears inside the author page.
  [InplaceRenderer](InplaceRenderer.md)
An author in-place renderer.
  [InplaceRendererAdapter](InplaceRendererAdapter.md)
Convenience implementation of the [InplaceRenderer](InplaceRenderer.md).

[LazyValue](LazyValue.md)<T>

This class enables one to give a form control property that isn't constructed until the first time it's looked up with AuthorInplaceContext#getArguments().get(key) method.
  [RendererLayoutInfo](RendererLayoutInfo.md)
Class which contains rendering information about a renderer, information like the baseline and the size.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
