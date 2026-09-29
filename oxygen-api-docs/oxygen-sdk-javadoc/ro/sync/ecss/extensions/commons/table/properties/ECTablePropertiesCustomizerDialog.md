Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Class ECTablePropertiesCustomizerDialog

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * org.eclipse.jface.window.Window
        * org.eclipse.jface.dialogs.Dialog
            * org.eclipse.jface.dialogs.TrayDialog
                * ro.sync.ecss.extensions.commons.table.properties.ECTablePropertiesCustomizerDialog
   All Implemented Interfaces: org.eclipse.jface.window.IShellProvider   @API(type=INTERNAL, src=PUBLIC) public class ECTablePropertiesCustomizerDialog extends org.eclipse.jface.dialogs.TrayDialog
Dialog that allows the user to edit the table properties.

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
 [ECTablePropertiesCustomizerDialog](#%3Cinit%3E(org.eclipse.swt.widgets.Shell,ro.sync.ecss.extensions.api.AuthorResourceBundle,ro.sync.exml.workspace.api.util.ColorThemeUtilities))(org.eclipse.swt.widgets.Shell parentFrame, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, [ColorThemeUtilities](../../../../../exml/workspace/api/util/ColorThemeUtilities.md) colorThemeUtilities)
Constructor.
  [ECTablePropertiesCustomizerDialog](#%3Cinit%3E(org.eclipse.swt.widgets.Shell,ro.sync.ecss.extensions.api.AuthorResourceBundle,ro.sync.exml.workspace.api.util.ColorThemeUtilities,java.lang.String))(org.eclipse.swt.widgets.Shell parentFrame, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, [ColorThemeUtilities](../../../../../exml/workspace/api/util/ColorThemeUtilities.md) colorThemeUtilities, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) helpPageID)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [configureShell](#configureShell(org.eclipse.swt.widgets.Shell))(org.eclipse.swt.widgets.Shell newShell)

 protected org.eclipse.swt.widgets.Control [createDialogArea](#createDialogArea(org.eclipse.swt.widgets.Composite))(org.eclipse.swt.widgets.Composite parent)

 [EditedTablePropertiesInfo](EditedTablePropertiesInfo.md) [getTablePropertiesInformation](#getTablePropertiesInformation(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo))([EditedTablePropertiesInfo](EditedTablePropertiesInfo.md) editedTablePropertiesInfo)
Obtain the table information.
  protected void [okPressed](#okPressed())()

### Methods inherited from class org.eclipse.jface.dialogs.TrayDialog
 closeTray, createButtonBar, createHelpControl, getLayout, getTray, handleShellCloseEvent, isDialogHelpAvailable, isHelpAvailable, openTray, setDialogHelpAvailable, setHelpAvailable
### Methods inherited from class org.eclipse.jface.dialogs.Dialog
 applyDialogFont, buttonPressed, cancelPressed, close, convertHeightInCharsToPixels, convertHeightInCharsToPixels, convertHorizontalDLUsToPixels, convertHorizontalDLUsToPixels, convertVerticalDLUsToPixels, convertVerticalDLUsToPixels, convertWidthInCharsToPixels, convertWidthInCharsToPixels, create, createButton, createButtonsForButtonBar, createContents, dialogFontIsDefault, getBlockedHandler, getButton, getButtonBar, getCancelButton, getDialogArea, getDialogBoundsSettings, getDialogBoundsStrategy, getImage, getInitialLocation, getInitialSize, getOKButton, initializeBounds, initializeDialogUnits, isResizable, setBlockedHandler, setButtonLayoutData, setButtonLayoutFormData, shortenText
### Methods inherited from class org.eclipse.jface.window.Window
 canHandleShellCloseEvent, constrainShellSize, createShell, getConstrainedShellBounds, getContents, getDefaultImage, getDefaultImages, getDefaultOrientation, getParentShell, getReturnCode, getShell, getShellListener, getShellStyle, getWindowManager, handleFontChange, open, setBlockOnOpen, setDefaultImage, setDefaultImages, setDefaultModalParent, setDefaultOrientation, setExceptionHandler, setParentShell, setReturnCode, setShellStyle, setWindowManager
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ECTablePropertiesCustomizerDialog

public ECTablePropertiesCustomizerDialog(org.eclipse.swt.widgets.Shell parentFrame, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, [ColorThemeUtilities](../../../../../exml/workspace/api/util/ColorThemeUtilities.md) colorThemeUtilities)

Constructor.
  Parameters: parentFrame - The parent frame. The dialog will be created over the parent. authorResourceBundle - The author resource bundle. It is used to translate different information used inside the dialog. colorThemeUtilities - The color theme utilities.
### ECTablePropertiesCustomizerDialog

public ECTablePropertiesCustomizerDialog(org.eclipse.swt.widgets.Shell parentFrame, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, [ColorThemeUtilities](../../../../../exml/workspace/api/util/ColorThemeUtilities.md) colorThemeUtilities, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) helpPageID)

Constructor.
  Parameters: parentFrame - The parent frame. The dialog will be created over the parent. authorResourceBundle - The author resource bundle. It is used to translate different information used inside the dialog. colorThemeUtilities - The color theme utilities. helpPageID - The help page ID.
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

### getTablePropertiesInformation

public [EditedTablePropertiesInfo](EditedTablePropertiesInfo.md) getTablePropertiesInformation([EditedTablePropertiesInfo](EditedTablePropertiesInfo.md) editedTablePropertiesInfo)

Obtain the table information.
  Parameters: editedTablePropertiesInfo - The information used to customize the "Table Properties dialog" Returns: The table information if at least one of the properties was modified or null if none of the properties was modified or if the dialog was cancelled.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
