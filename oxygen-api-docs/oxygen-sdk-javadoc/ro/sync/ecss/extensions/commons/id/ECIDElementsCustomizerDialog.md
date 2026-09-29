Package [ro.sync.ecss.extensions.commons.id](package-summary.md)

# Class ECIDElementsCustomizerDialog

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * org.eclipse.jface.window.Window
        * org.eclipse.jface.dialogs.Dialog
            * org.eclipse.jface.dialogs.TrayDialog
                * ro.sync.ecss.extensions.commons.id.ECIDElementsCustomizerDialog
   All Implemented Interfaces: org.eclipse.jface.window.IShellProvider   @API(type=INTERNAL, src=PUBLIC) public class ECIDElementsCustomizerDialog extends org.eclipse.jface.dialogs.TrayDialog
Dialog used to customize DITA elements which have auto ID generation. It will be also used when the IDs are generated manually. It is used on standalone implementation.

## Nested Class Summary

## Nested classes/interfaces inherited from class org.eclipse.jface.window.Window
 org.eclipse.jface.window.Window.IExceptionHandler
## Field Summary

### Fields inherited from class org.eclipse.jface.dialogs.Dialog
 blockedHandler, buttonBar, DIALOG_DEFAULT_BOUNDS, DIALOG_PERSISTLOCATION, DIALOG_PERSISTSIZE, dialogArea, DLG_IMG_ERROR, DLG_IMG_HELP, DLG_IMG_INFO, DLG_IMG_MESSAGE_ERROR, DLG_IMG_MESSAGE_INFO, DLG_IMG_MESSAGE_WARNING, DLG_IMG_QUESTION, DLG_IMG_WARNING, ELLIPSIS
### Fields inherited from class org.eclipse.jface.window.Window
 CANCEL, OK, resizeHasOccurred
## Constructor Summary
 Constructors
Constructor

Description
 [ECIDElementsCustomizerDialog](#%3Cinit%3E(org.eclipse.swt.widgets.Shell,java.lang.String,ro.sync.ecss.extensions.api.AuthorResourceBundle,boolean))(org.eclipse.swt.widgets.Shell parentShell, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listMessage, [AuthorResourceBundle](../../api/AuthorResourceBundle.md) authorResourceBundle, boolean isDocBook)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [configureShell](#configureShell(org.eclipse.swt.widgets.Shell))(org.eclipse.swt.widgets.Shell newShell)

 protected org.eclipse.swt.widgets.Control [createDialogArea](#createDialogArea(org.eclipse.swt.widgets.Composite))(org.eclipse.swt.widgets.Composite parent)

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID())()
Get the ID of the help page which will be called by the end user.
  protected void [okPressed](#okPressed())()

 [GenerateIDElementsInfo](GenerateIDElementsInfo.md) [showDialog](#showDialog(ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo))([GenerateIDElementsInfo](GenerateIDElementsInfo.md) info)

### Methods inherited from class org.eclipse.jface.dialogs.TrayDialog
 closeTray, createButtonBar, createHelpControl, getLayout, getTray, handleShellCloseEvent, isDialogHelpAvailable, isHelpAvailable, openTray, setDialogHelpAvailable, setHelpAvailable
### Methods inherited from class org.eclipse.jface.dialogs.Dialog
 applyDialogFont, buttonPressed, cancelPressed, close, convertHeightInCharsToPixels, convertHeightInCharsToPixels, convertHorizontalDLUsToPixels, convertHorizontalDLUsToPixels, convertVerticalDLUsToPixels, convertVerticalDLUsToPixels, convertWidthInCharsToPixels, convertWidthInCharsToPixels, create, createButton, createButtonsForButtonBar, createContents, dialogFontIsDefault, getBlockedHandler, getButton, getButtonBar, getCancelButton, getDialogArea, getDialogBoundsSettings, getDialogBoundsStrategy, getImage, getInitialLocation, getInitialSize, getOKButton, initializeBounds, initializeDialogUnits, isResizable, setBlockedHandler, setButtonLayoutData, setButtonLayoutFormData, shortenText
### Methods inherited from class org.eclipse.jface.window.Window
 canHandleShellCloseEvent, constrainShellSize, createShell, getConstrainedShellBounds, getContents, getDefaultImage, getDefaultImages, getDefaultOrientation, getParentShell, getReturnCode, getShell, getShellListener, getShellStyle, getWindowManager, handleFontChange, open, setBlockOnOpen, setDefaultImage, setDefaultImages, setDefaultModalParent, setDefaultOrientation, setExceptionHandler, setParentShell, setReturnCode, setShellStyle, setWindowManager
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ECIDElementsCustomizerDialog

public ECIDElementsCustomizerDialog(org.eclipse.swt.widgets.Shell parentShell, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listMessage, [AuthorResourceBundle](../../api/AuthorResourceBundle.md) authorResourceBundle, boolean isDocBook)

Constructor.
  Parameters: parentShell - The parent shell for the dialog. listMessage - The message label used on the list. authorResourceBundle - The author resource bundle. isDocBook - true if we are in DocBook.
## Method Details

### configureShell

protected void configureShell(org.eclipse.swt.widgets.Shell newShell)
  Overrides: configureShell in class org.eclipse.jface.window.Window See Also:
        * Window.configureShell(org.eclipse.swt.widgets.Shell)

### createDialogArea

protected org.eclipse.swt.widgets.Control createDialogArea(org.eclipse.swt.widgets.Composite parent)
  Overrides: createDialogArea in class org.eclipse.jface.dialogs.Dialog See Also:
        * Dialog.createDialogArea(org.eclipse.swt.widgets.Composite)

### okPressed

protected void okPressed()
  Overrides: okPressed in class org.eclipse.jface.dialogs.Dialog See Also:
        * Dialog.okPressed()

### showDialog

public [GenerateIDElementsInfo](GenerateIDElementsInfo.md) showDialog([GenerateIDElementsInfo](GenerateIDElementsInfo.md) info)
  Parameters: info - The initial information Returns: The new information or null if canceled.
### getHelpPageID

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID()

Get the ID of the help page which will be called by the end user.
  Returns: the ID of the help page which will be called by the end user or null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
