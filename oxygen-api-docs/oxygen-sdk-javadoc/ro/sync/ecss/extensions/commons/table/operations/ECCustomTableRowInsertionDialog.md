Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class ECCustomTableRowInsertionDialog

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * org.eclipse.jface.window.Window
        * org.eclipse.jface.dialogs.Dialog
            * org.eclipse.jface.dialogs.TrayDialog
                * ro.sync.ecss.extensions.commons.table.operations.ECCustomTableRowInsertionDialog
   All Implemented Interfaces: org.eclipse.jface.window.IShellProvider   @API(type=INTERNAL, src=PUBLIC) public class ECCustomTableRowInsertionDialog extends org.eclipse.jface.dialogs.TrayDialog
Dialog displayed when trying to insert multiple rows (using "Insert Rows..."). For Eclipse plugin.

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
 [ECCustomTableRowInsertionDialog](#%3Cinit%3E(org.eclipse.swt.widgets.Shell,ro.sync.ecss.extensions.api.AuthorResourceBundle))(org.eclipse.swt.widgets.Shell parentShell, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [configureShell](#configureShell(org.eclipse.swt.widgets.Shell))(org.eclipse.swt.widgets.Shell newShell)
Configure Shell.
  protected void [createButtonsForButtonBar](#createButtonsForButtonBar(org.eclipse.swt.widgets.Composite))(org.eclipse.swt.widgets.Composite parent)

 protected org.eclipse.swt.widgets.Control [createDialogArea](#createDialogArea(org.eclipse.swt.widgets.Composite))(org.eclipse.swt.widgets.Composite parent)
Create Dialog area.
  [TableRowsInfo](TableRowsInfo.md) [showDialog](#showDialog(ro.sync.ecss.extensions.commons.table.operations.TableRowsInfo))([TableRowsInfo](TableRowsInfo.md) previousTableRowsInfo)
Show the dialog to customize the row(s) insertion.

### Methods inherited from class org.eclipse.jface.dialogs.TrayDialog
 closeTray, createButtonBar, createHelpControl, getLayout, getTray, handleShellCloseEvent, isDialogHelpAvailable, isHelpAvailable, openTray, setDialogHelpAvailable, setHelpAvailable
### Methods inherited from class org.eclipse.jface.dialogs.Dialog
 applyDialogFont, buttonPressed, cancelPressed, close, convertHeightInCharsToPixels, convertHeightInCharsToPixels, convertHorizontalDLUsToPixels, convertHorizontalDLUsToPixels, convertVerticalDLUsToPixels, convertVerticalDLUsToPixels, convertWidthInCharsToPixels, convertWidthInCharsToPixels, create, createButton, createContents, dialogFontIsDefault, getBlockedHandler, getButton, getButtonBar, getCancelButton, getDialogArea, getDialogBoundsSettings, getDialogBoundsStrategy, getImage, getInitialLocation, getInitialSize, getOKButton, initializeBounds, initializeDialogUnits, isResizable, okPressed, setBlockedHandler, setButtonLayoutData, setButtonLayoutFormData, shortenText
### Methods inherited from class org.eclipse.jface.window.Window
 canHandleShellCloseEvent, constrainShellSize, createShell, getConstrainedShellBounds, getContents, getDefaultImage, getDefaultImages, getDefaultOrientation, getParentShell, getReturnCode, getShell, getShellListener, getShellStyle, getWindowManager, handleFontChange, open, setBlockOnOpen, setDefaultImage, setDefaultImages, setDefaultModalParent, setDefaultOrientation, setExceptionHandler, setParentShell, setReturnCode, setShellStyle, setWindowManager
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ECCustomTableRowInsertionDialog

public ECCustomTableRowInsertionDialog(org.eclipse.swt.widgets.Shell parentShell, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle)

Constructor.
  Parameters: parentShell - the parent shell. authorResourceBundle - the author resource bundle.
## Method Details

### configureShell

protected void configureShell(org.eclipse.swt.widgets.Shell newShell)

Configure Shell. Set a title to it.
  Overrides: configureShell in class org.eclipse.jface.window.Window Parameters: newShell - The new shell. See Also:
        * Window.configureShell(org.eclipse.swt.widgets.Shell)

### createDialogArea

protected org.eclipse.swt.widgets.Control createDialogArea(org.eclipse.swt.widgets.Composite parent)

Create Dialog area.
  Overrides: createDialogArea in class org.eclipse.jface.dialogs.Dialog Parameters: parent - The parent composite. Returns: The dialog control.
### showDialog

public [TableRowsInfo](TableRowsInfo.md) showDialog([TableRowsInfo](TableRowsInfo.md) previousTableRowsInfo)

Show the dialog to customize the row(s) insertion.
  Parameters: previousTableRowsInfo - the previous row(s) information. Returns: The information about the row(s) to be inserted, or null if the user canceled the insertion.
### createButtonsForButtonBar

protected void createButtonsForButtonBar(org.eclipse.swt.widgets.Composite parent)
  Overrides: createButtonsForButtonBar in class org.eclipse.jface.dialogs.Dialog See Also:
        * Dialog.createButtonsForButtonBar(org.eclipse.swt.widgets.Composite)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
