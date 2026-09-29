Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class CustomAttributeValueEditor

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.CustomAttributeValueEditor
   All Implemented Interfaces: [Extension](Extension.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class CustomAttributeValueEditor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Extension](Extension.md)
A custom editor which gets invoked to edit the value for an attribute.
  Since: 15
## Constructor Summary
 Constructors
Constructor

Description
 [CustomAttributeValueEditor](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeValue](#getAttributeValue(ro.sync.ecss.extensions.api.EditedAttribute,java.lang.Object))([EditedAttribute](EditedAttribute.md) attribute, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentComponent)
Get a value for the current attribute.
  [TooltipIconInfo](TooltipIconInfo.md) [getTooltipButtonInfo](#getTooltipButtonInfo(ro.sync.ecss.extensions.api.EditedAttribute))([EditedAttribute](EditedAttribute.md) attribute)
Get the information(tooltip and button) that describes the handle of the given attribute.
  abstract boolean [shouldHandleAttribute](#shouldHandleAttribute(ro.sync.ecss.extensions.api.EditedAttribute))([EditedAttribute](EditedAttribute.md) attribute)
Ask the custom editor if it wants to handle editing for a certain attribute.
  boolean [shouldHandleAttribute](#shouldHandleAttribute(ro.sync.ecss.extensions.api.EditedAttribute,ro.sync.ecss.extensions.api.CustomAttributeValueEditingContext))([EditedAttribute](EditedAttribute.md) attribute, [CustomAttributeValueEditingContext](CustomAttributeValueEditingContext.md) editContext)
Ask the custom editor if it wants to handle editing for a certain attribute in a certain context.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Constructor Details

### CustomAttributeValueEditor

public CustomAttributeValueEditor()

## Method Details

### getAttributeValue

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeValue([EditedAttribute](EditedAttribute.md) attribute, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentComponent)throws [CancelledByUserException](CancelledByUserException.md)

Get a value for the current attribute.
  Parameters: attribute - The attribute to be edited. parentComponent - The parent component, usually the table in which the user double clicked the value. Used for example to find the parent window/shell when creating dialogs. It is very important to set the parent of the dialog used as custom editor when showing it from oXygen's in-place attribute-editing dialog in the Author page. This needs to be done in order for oXygen's in-place attribute editor not to disappear when presenting the custom attribute value editor.The code that creates a simple input dialog as a custom editor, with the proper parent dialog, for the stand-alone oXygen, looks as following:
```

 public String getAttributeValue(EditedAttribute attribute, Object parentComponent)
     throws CancelledByUserException {
   String attrValue = null;
   PluginWorkspace pluginWorkspace = PluginWorkspaceProvider.getPluginWorkspace();
   Platform platform = pluginWorkspace.getPlatform();
   if (platform == Platform.STANDALONE) {
     // Find the parent window
     Component parent = (Component) parentComponent;
     while (!(parent instanceof Window)) {
       parent = parent.getParent();
     }
     attrValue = JOptionPane.showInputDialog(
         parent,
         "Set a new value for \"" + attribute.getAttributeQName() + "\":");
   }
   return attrValue;
 }

```
For the Eclipse plug-in, the code changes into:
```

 public String getAttributeValue(EditedAttribute attribute, Object parentComponent)
     throws CancelledByUserException {
   String attrValue = null;
   PluginWorkspace pluginWorkspace = PluginWorkspaceProvider.getPluginWorkspace();
   Platform platform = pluginWorkspace.getPlatform();
   if (platform == Platform.ECLIPSE) {
     // Find the parent shell
     Control parent = (Control) parentComponent;
     while (!(parent instanceof Shell)) {
       parent = parent.getParent();
     }
     InputDialog inputDialog = new InputDialog(
         (Shell) parent,
         "Edit attribute",
         "Set a new value for \"" + attribute.getAttributeQName() + "\":",
         null,
         null);
     if (inputDialog.open() == org.eclipse.jface.window.Window.OK) {
       // OK pressed. Get the value.
       attrValue = inputDialog.getValue();
     }
   }
   return attrValue;
 }

```
 Returns: The proposed value. Returning the empty string will commit it as a value, returning null will remove the attribute, while throwing a [CancelledByUserException](CancelledByUserException.md) will cancel the editing. Throws: [CancelledByUserException](CancelledByUserException.md) - When the user cancels the editing.
### shouldHandleAttribute

public abstract boolean shouldHandleAttribute([EditedAttribute](EditedAttribute.md) attribute)

Ask the custom editor if it wants to handle editing for a certain attribute.
  Parameters: attribute - The attribute. Returns: true if this custom editor's "getAttributeValue" method should be invoked for that certain attribute.
### shouldHandleAttribute

public boolean shouldHandleAttribute([EditedAttribute](EditedAttribute.md) attribute, [CustomAttributeValueEditingContext](CustomAttributeValueEditingContext.md) editContext)

Ask the custom editor if it wants to handle editing for a certain attribute in a certain context.
  Parameters: attribute - The attribute. editContext - The context from the editing is invoked. Can be [CustomAttributeValueEditingContext.ATTRIBUTES_TABLE_CELL_CONTEXT](CustomAttributeValueEditingContext.md#ATTRIBUTES_TABLE_CELL_CONTEXT) or [CustomAttributeValueEditingContext.CUSTOM_EDIT_BUTTON_CONTEXT](CustomAttributeValueEditingContext.md#CUSTOM_EDIT_BUTTON_CONTEXT) Returns: true if this custom editor's "getAttributeValue" method should be invoked for that certain attribute. Since: 21
### getTooltipButtonInfo

public [TooltipIconInfo](TooltipIconInfo.md) getTooltipButtonInfo([EditedAttribute](EditedAttribute.md) attribute)

Get the information(tooltip and button) that describes the handle of the given attribute.
  Parameters: attribute - The attribute to be edited. Returns: The proposed information. Returning null if isn't a proposed info for the attribute. Since: 21
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
