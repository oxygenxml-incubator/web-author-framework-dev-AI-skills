Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Class AuthorInplaceContext

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.editor.AuthorInplaceContext
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorInplaceContext extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Context where an edit component will be used. Contains all the information required to build the editor.
  Since: 14.1
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorInplaceContext](#%3Cinit%3E(java.util.Map,ro.sync.ecss.extensions.api.node.AuthorElement,ro.sync.ecss.css.Styles,ro.sync.ecss.extensions.api.AuthorSchemaManager,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.Object,ro.sync.ecss.extensions.api.editor.DynamicPropertyEvaluator))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> arguments, [AuthorElement](../node/AuthorElement.md) elem, [Styles](../../../css/Styles.md) styles, [AuthorSchemaManager](../AuthorSchemaManager.md) schemaManager, [AuthorAccess](../AuthorAccess.md) authorAccess, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentHost, [DynamicPropertyEvaluator](DynamicPropertyEvaluator.md) propsEvaluator)
The editor context.
  [AuthorInplaceContext](#%3Cinit%3E(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](AuthorInplaceContext.md) copy)
Copy constructor.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> [getArguments](#getArguments())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeToEdit](#getAttributeToEdit())()  Deprecated.
Use [getAttributeToEditQName()](#getAttributeToEditQName()) instead.
   static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeToEdit](#getAttributeToEdit(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toEdit)
Checks if the property [InplaceEditorCSSConstants.PROPERTY_EDIT](InplaceEditorCSSConstants.md#PROPERTY_EDIT) specifies an attribute to be edited.
  [QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html) [getAttributeToEditQName](#getAttributeToEditQName())()
The QName of the edited attribute.
  [AuthorAccess](../AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()

 [AuthorElement](../node/AuthorElement.md) [getElem](#getElem())()
Get the element being edited.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getErrorMessage](#getErrorMessage())()

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getParentHost](#getParentHost())()
The parent host in which the editor will be added or the renderer will be painted.
  [DynamicPropertyEvaluator](DynamicPropertyEvaluator.md) [getPropertyEvaluator](#getPropertyEvaluator())()
Some form control properties can't be evaluated at the time the CSS is compiled.
  [Point](../../../../exml/view/graphics/Point.md) [getRelativeMouseLocation](#getRelativeMouseLocation())()
If the mouse is currently hovering the area of this editor this represents the X,Y location relative to the editor bounds.
  [AuthorSchemaManager](../AuthorSchemaManager.md) [getSchemaManager](#getSchemaManager())()

 [Styles](../../../css/Styles.md) [getStyles](#getStyles())()

 boolean [isReadOnlyContext](#isReadOnlyContext())()
Checks if the form control is added in a context where changes are not permitted.
  void [setErrorMessage](#setErrorMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) errorMessage)
Sets an error message encountered while building the context.
  void [setParentHost](#setParentHost(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentHost)
The parent host in which the editor will be added or the renderer will be painted.
  void [setReadOnlyContext](#setReadOnlyContext(boolean))(boolean readOnlyContext)
Sets if the form control is added in a context where editing is not permitted.
  void [setRelativeMousePosition](#setRelativeMousePosition(ro.sync.exml.view.graphics.Point))([Point](../../../../exml/view/graphics/Point.md) relativeMousePosition)
If the mouse is currently hovering the area of this editor this represents the X,Y location relative to the editor bounds.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorInplaceContext

public AuthorInplaceContext([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> arguments, [AuthorElement](../node/AuthorElement.md) elem, [Styles](../../../css/Styles.md) styles, [AuthorSchemaManager](../AuthorSchemaManager.md) schemaManager, [AuthorAccess](../AuthorAccess.md) authorAccess, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentHost, [DynamicPropertyEvaluator](DynamicPropertyEvaluator.md) propsEvaluator)

The editor context.
  Parameters: arguments - The editor arguments elem - The element being edited. styles - The styles of the element where the editing takes place schemaManager - Provides support for obtaining information about what elements, attributes can be inserted in a given context. authorAccess - Provides access to different functions. parentHost - The parent host in which the editor will be added or the renderer will be painted. If we are in the stand-alone Oxygen version this will be a JPanel. If we are in the Oxygen Eclipse plug-in this will be a Composite. For SWT, an editor will require the parent in order to create itself. propsEvaluator - Some form control properties can't be evaluated at the time the CSS is compiled. This interface can be used by form controls to expand such properties.
### AuthorInplaceContext

public AuthorInplaceContext([AuthorInplaceContext](AuthorInplaceContext.md) copy)

Copy constructor.
  Parameters: copy - Another context object to copy from.
## Method Details

### getPropertyEvaluator

public [DynamicPropertyEvaluator](DynamicPropertyEvaluator.md) getPropertyEvaluator()

Some form control properties can't be evaluated at the time the CSS is compiled. This interface can be used by form controls to expand such properties.
  Returns: A property evaluator. Since: 16.1
### getArguments

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> getArguments()
  Returns: The arguments from the oxy_editor function as well as some others. The keys are the constants from class [InplaceEditorArgumentKeys](InplaceEditorArgumentKeys.md).
### getAttributeToEdit

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeToEdit()
 Deprecated.
Use [getAttributeToEditQName()](#getAttributeToEditQName()) instead. This method returns the attribute name as it was specified in the CSS. If a QName was specified then this QName might not be valid in the context of the current element. Property [InplaceEditorArgumentKeys.PROPERTY_EDIT_QUALIFIED](InplaceEditorArgumentKeys.md#PROPERTY_EDIT_QUALIFIED)should be used in these situations.
   Returns: The attribute being edited as extracted from the oxy_editor arguments. null no attribute was specified in which case the text should be edited.
### getAttributeToEditQName

public [QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html) getAttributeToEditQName()

The QName of the edited attribute.
  Returns: The QName of the edited attribute or null if not editing an attribute.
### getAttributeToEdit

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeToEdit([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toEdit)

Checks if the property [InplaceEditorCSSConstants.PROPERTY_EDIT](InplaceEditorCSSConstants.md#PROPERTY_EDIT) specifies an attribute to be edited.
  Parameters: toEdit - The value of the property [InplaceEditorCSSConstants.PROPERTY_EDIT](InplaceEditorCSSConstants.md#PROPERTY_EDIT) Returns: The attribute being edited as extracted from the oxy_editor arguments. null if no attribute name was specified.
### getElem

public [AuthorElement](../node/AuthorElement.md) getElem()

Get the element being edited.
  Returns: The element being edited. If a processing instruction is being edited, the returned object is an instance of ro.sync.ecss.extensions.api.node.ArtificialNode and you can obtain the wrapped PI from it.
### getSchemaManager

public [AuthorSchemaManager](../AuthorSchemaManager.md) getSchemaManager()
  Returns: Returns the schemaManager.
### getAuthorAccess

public [AuthorAccess](../AuthorAccess.md) getAuthorAccess()
  Returns: Provides access to different author functions.
### getParentHost

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getParentHost()

The parent host in which the editor will be added or the renderer will be painted. If we are in the stand-alone Oxygen version this will be a [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html). If we are in the Oxygen Eclipse plug-in, for [InplaceEditor](InplaceEditor.md) this will be a Compositeand for [InplaceRenderer](InplaceRenderer.md) it will be a [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html). For SWT, an editor will require the parent in order to create itself.
  Returns: The [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) or Composite of the author.
### setErrorMessage

public void setErrorMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) errorMessage)

Sets an error message encountered while building the context.
  Parameters: errorMessage - An error message encountered while building the context.
### getErrorMessage

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getErrorMessage()
  Returns: An error message encountered while building the context.
### getStyles

public [Styles](../../../css/Styles.md) getStyles()
  Returns: Returns the styles of the element where the editing takes place.
### setRelativeMousePosition

public void setRelativeMousePosition([Point](../../../../exml/view/graphics/Point.md) relativeMousePosition)

If the mouse is currently hovering the area of this editor this represents the X,Y location relative to the editor bounds. The editor might choose to render itself differently in this situation. For example a button editor might paint a special highlight as a feedback that an action can be performed. null if the mouse is not over the editor. This information is relevant only when the editor is painted. When editing is started the editor can just add mouse listeners onto itself.
  Parameters: relativeMousePosition - The mouse location if the mouse is over the editor.
### getRelativeMouseLocation

public [Point](../../../../exml/view/graphics/Point.md) getRelativeMouseLocation()

If the mouse is currently hovering the area of this editor this represents the X,Y location relative to the editor bounds. The editor might choose to render itself differently in this situation. For example a button editor might paint a special highlight as a feedback that an action can be performed. null if the mouse is not over the editor. This information is relevant only when the editor is painted. When editing is started the editor can just add mouse listeners onto itself.
  Returns: The mouse location if the mouse is over the editor.
### setReadOnlyContext

public void setReadOnlyContext(boolean readOnlyContext)

Sets if the form control is added in a context where editing is not permitted.
  Parameters: readOnlyContext - true if this form control is added in a context where changes are not permitted.
### isReadOnlyContext

public boolean isReadOnlyContext()

Checks if the form control is added in a context where changes are not permitted. In this situation the form control will automatically be rendered as disabled. A form control implementation might look to this flag to dynamically change things. For example a pop-up form control usually presents a message that says: "Click to edit....". In a read-only context this tooltip will not be presented anymore.
  Returns: true if this form control is added in a context where changes are not permitted.
### setParentHost

public void setParentHost([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentHost)

The parent host in which the editor will be added or the renderer will be painted. If we are in the stand-alone Oxygen version this will be a JPanel.
  Parameters: parentHost - The host to set.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
