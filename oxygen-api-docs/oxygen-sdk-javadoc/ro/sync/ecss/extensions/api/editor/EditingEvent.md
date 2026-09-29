Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Class EditingEvent

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.editor.EditingEvent
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class EditingEvent extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The in-place editing was stopped. It will provide the committed value if such a value exists for the current type of editor. For example a [InplaceEditorCSSConstants.TYPE_BUTTON](InplaceEditorCSSConstants.md#TYPE_BUTTON) doesn't give such a value. In this case when the notification is received we will just invoke the action associated with the button. A custom form control that wants to perform more custom operation can wrap these on a [Runnable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Runnable.html) and give then on the [customEdit](#customEdit)field. This is the recommended way for performing custom changes.
  Since: 14.1
## Field Summary
 Fields
Modifier and Type

Field

Description
 final [Runnable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Runnable.html) [customEdit](#customEdit)
If the form control performs custom editing([InplaceEditorCSSConstants.EDIT_CUSTOM](InplaceEditorCSSConstants.md#EDIT_CUSTOM)) it can give this custom editing wrapped inside this runnable.
  boolean [requestFocusInHost](#requestFocusInHost)
true if the focus should be requested inside the author component.
  [IAuthorExtensionAction](IAuthorExtensionAction.md) [toInvoke](#toInvoke)
The action to be invoked as a result for the edit event.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [val](#val)
The value that the user accepted when the editing stopped.

## Constructor Summary
 Constructors
Constructor

Description
 [EditingEvent](#%3Cinit%3E(java.lang.Runnable,boolean))([Runnable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Runnable.html) toInvoke, boolean requestFocus)
Constructor.
  [EditingEvent](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) val)
Constructor.
  [EditingEvent](#%3Cinit%3E(java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean requestFocus)
Constructor.
  [EditingEvent](#%3Cinit%3E(ro.sync.ecss.extensions.api.editor.IAuthorExtensionAction))([IAuthorExtensionAction](IAuthorExtensionAction.md) toInvoke)
Constructor.

## Method Summary

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### val

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) val

The value that the user accepted when the editing stopped. If the type of editor used can provide such a value. When editing an attribute value, an empty string will result in deleting the attribute.

### toInvoke

public [IAuthorExtensionAction](IAuthorExtensionAction.md) toInvoke

The action to be invoked as a result for the edit event.

### requestFocusInHost

public boolean requestFocusInHost

true if the focus should be requested inside the author component. Depending on how the editing was stopped it might be necessary to skip requesting focus inside the author component. For example if the cause of the stop editing was a focus lost event, we should skip requesting focus since the focus has already a destination.

### customEdit

public final [Runnable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Runnable.html) customEdit

If the form control performs custom editing([InplaceEditorCSSConstants.EDIT_CUSTOM](InplaceEditorCSSConstants.md#EDIT_CUSTOM)) it can give this custom editing wrapped inside this runnable. This will ensure a more seamless integration by letting Oxygen decide when to make the custom changes.

## Constructor Details

### EditingEvent

public EditingEvent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) val)

Constructor.
  Parameters: val - The value that the user accepted when the editing stopped.
### EditingEvent

public EditingEvent([Runnable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Runnable.html) toInvoke, boolean requestFocus)

Constructor.
  Parameters: toInvoke - The action to be invoked as a result for the edit event. requestFocus - true if the focus should be requested inside the author component. Depending on how the editing was stopped it might be necessary to skip requesting focus inside the author component. For example if the cause of the stop editing was a focus lost event, we should skip requesting focus since the focus has already a destination.
### EditingEvent

public EditingEvent([IAuthorExtensionAction](IAuthorExtensionAction.md) toInvoke)

Constructor.
  Parameters: toInvoke - The action to be invoked as a result for the edit event.
### EditingEvent

public EditingEvent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean requestFocus)

Constructor.
  Parameters: value - The value that the user accepted when the editing stopped. requestFocus - true if the focus should be requested inside the author component. Depending on how the editing was stopped it might be necessary to skip requesting focus inside the author component. For example if the cause of the stop editing was a focus lost event, we should skip requesting focus since the focus has already a destination.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
