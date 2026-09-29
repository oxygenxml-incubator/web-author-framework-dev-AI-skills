Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class ECTableSplitCustomizerDialog

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * org.eclipse.jface.window.Window
        * org.eclipse.jface.dialogs.Dialog
            * org.eclipse.jface.dialogs.TrayDialog
                * ro.sync.ecss.extensions.commons.table.operations.ECTableSplitCustomizerDialog
   All Implemented Interfaces: org.eclipse.jface.window.IShellProvider   @API(type=INTERNAL, src=PUBLIC) public class ECTableSplitCustomizerDialog extends org.eclipse.jface.dialogs.TrayDialog
Dialog that allows the user to choose the information necessary for the Split operation.

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
 [ECTableSplitCustomizerDialog](#%3Cinit%3E(java.lang.Object,ro.sync.ecss.extensions.api.AuthorResourceBundle,int,int,java.lang.String))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int maxColumns, int maxRows, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) helpPageID)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [configureShell](#configureShell(org.eclipse.swt.widgets.Shell))(org.eclipse.swt.widgets.Shell newShell)

 protected org.eclipse.swt.widgets.Control [createDialogArea](#createDialogArea(org.eclipse.swt.widgets.Composite))(org.eclipse.swt.widgets.Composite parent)

 int[] [getSplitInformation](#getSplitInformation())()
Obtain the number of cells on split.

### Methods inherited from class org.eclipse.jface.dialogs.TrayDialog
 closeTray, createButtonBar, createHelpControl, getLayout, getTray, handleShellCloseEvent, isDialogHelpAvailable, isHelpAvailable, openTray, setDialogHelpAvailable, setHelpAvailable
### Methods inherited from class org.eclipse.jface.dialogs.Dialog
 applyDialogFont, buttonPressed, cancelPressed, close, convertHeightInCharsToPixels, convertHeightInCharsToPixels, convertHorizontalDLUsToPixels, convertHorizontalDLUsToPixels, convertVerticalDLUsToPixels, convertVerticalDLUsToPixels, convertWidthInCharsToPixels, convertWidthInCharsToPixels, create, createButton, createButtonsForButtonBar, createContents, dialogFontIsDefault, getBlockedHandler, getButton, getButtonBar, getCancelButton, getDialogArea, getDialogBoundsSettings, getDialogBoundsStrategy, getImage, getInitialLocation, getInitialSize, getOKButton, initializeBounds, initializeDialogUnits, isResizable, okPressed, setBlockedHandler, setButtonLayoutData, setButtonLayoutFormData, shortenText
### Methods inherited from class org.eclipse.jface.window.Window
 canHandleShellCloseEvent, constrainShellSize, createShell, getConstrainedShellBounds, getContents, getDefaultImage, getDefaultImages, getDefaultOrientation, getParentShell, getReturnCode, getShell, getShellListener, getShellStyle, getWindowManager, handleFontChange, open, setBlockOnOpen, setDefaultImage, setDefaultImages, setDefaultModalParent, setDefaultOrientation, setExceptionHandler, setParentShell, setReturnCode, setShellStyle, setWindowManager
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ECTableSplitCustomizerDialog

public ECTableSplitCustomizerDialog([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentFrame, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int maxColumns, int maxRows, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) helpPageID)

Constructor.
  Parameters: parentFrame - The parent frame of the dialog. authorResourceBundle - The author resource bundle.It is used for translations. maxColumns - The maximum number of columns in which the current cell can be split. maxRows - The maximum number of rows in which the current cell can be split. helpPageID - The help page ID.
## Method Details

### configureShell

protected void configureShell(org.eclipse.swt.widgets.Shell newShell)
  Overrides: configureShell in class org.eclipse.jface.window.Window See Also:
        * Window.configureShell(org.eclipse.swt.widgets.Shell)

### createDialogArea

protected org.eclipse.swt.widgets.Control createDialogArea(org.eclipse.swt.widgets.Composite parent)
  Overrides: createDialogArea in class org.eclipse.jface.dialogs.Dialog See Also:
        * Dialog.createDialogArea(org.eclipse.swt.widgets.Composite)

### getSplitInformation

public int[] getSplitInformation()

Obtain the number of cells on split. (horizontally and vertically)
  Returns: The first element contains the number of columns and the second element contains the number of rows.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
