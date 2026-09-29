Package [ro.sync.ecss.extensions.commons.sort](package-summary.md)

# Class ECSortCustomizerDialog

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * org.eclipse.jface.window.Window
        * org.eclipse.jface.dialogs.Dialog
            * org.eclipse.jface.dialogs.TrayDialog
                * ro.sync.ecss.extensions.commons.sort.ECSortCustomizerDialog
   All Implemented Interfaces: org.eclipse.jface.window.IShellProvider, [KeysController](KeysController.md), [SortCustomizer](SortCustomizer.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class ECSortCustomizerDialog extends org.eclipse.jface.dialogs.TrayDialog implements [SortCustomizer](SortCustomizer.md), [KeysController](KeysController.md)
Eclipse implementation of the customizer used to select the criterion information used when sorting.

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
 [ECSortCustomizerDialog](#%3Cinit%3E(org.eclipse.swt.widgets.Shell,ro.sync.ecss.extensions.api.AuthorResourceBundle,java.lang.String,java.lang.String))(org.eclipse.swt.widgets.Shell parentFrame, [AuthorResourceBundle](../../api/AuthorResourceBundle.md) authorResourceBundle, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) selectedElemensString, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) allElementsString)
Constructor.
  [ECSortCustomizerDialog](#%3Cinit%3E(org.eclipse.swt.widgets.Shell,ro.sync.ecss.extensions.api.AuthorResourceBundle,java.lang.String,java.lang.String,java.lang.String))(org.eclipse.swt.widgets.Shell parentFrame, [AuthorResourceBundle](../../api/AuthorResourceBundle.md) authorResourceBundle, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) selectedElemensString, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) allElementsString, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) helpPageID)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [configureShell](#configureShell(org.eclipse.swt.widgets.Shell))(org.eclipse.swt.widgets.Shell newShell)

 protected org.eclipse.swt.widgets.Control [createDialogArea](#createDialogArea(org.eclipse.swt.widgets.Composite))(org.eclipse.swt.widgets.Composite parent)

 [SortCriteriaInformation](SortCriteriaInformation.md) [getSortInformation](#getSortInformation(java.util.List,boolean,boolean))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> criteriaInformation, boolean hasSelectedSortableElements, boolean cannotSortAllElements)
Obtain the sort information given some initial sort criteria.
  protected boolean [isResizable](#isResizable())()

 protected void [okPressed](#okPressed())()

 void [selectionChanged](#selectionChanged(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newSelection, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) oldSelection)
Method which controls the change of the selected key.

### Methods inherited from class org.eclipse.jface.dialogs.TrayDialog
 closeTray, createButtonBar, createHelpControl, getLayout, getTray, handleShellCloseEvent, isDialogHelpAvailable, isHelpAvailable, openTray, setDialogHelpAvailable, setHelpAvailable
### Methods inherited from class org.eclipse.jface.dialogs.Dialog
 applyDialogFont, buttonPressed, cancelPressed, close, convertHeightInCharsToPixels, convertHeightInCharsToPixels, convertHorizontalDLUsToPixels, convertHorizontalDLUsToPixels, convertVerticalDLUsToPixels, convertVerticalDLUsToPixels, convertWidthInCharsToPixels, convertWidthInCharsToPixels, create, createButton, createButtonsForButtonBar, createContents, dialogFontIsDefault, getBlockedHandler, getButton, getButtonBar, getCancelButton, getDialogArea, getDialogBoundsSettings, getDialogBoundsStrategy, getImage, getInitialLocation, getInitialSize, getOKButton, initializeBounds, initializeDialogUnits, setBlockedHandler, setButtonLayoutData, setButtonLayoutFormData, shortenText
### Methods inherited from class org.eclipse.jface.window.Window
 canHandleShellCloseEvent, constrainShellSize, createShell, getConstrainedShellBounds, getContents, getDefaultImage, getDefaultImages, getDefaultOrientation, getParentShell, getReturnCode, getShell, getShellListener, getShellStyle, getWindowManager, handleFontChange, open, setBlockOnOpen, setDefaultImage, setDefaultImages, setDefaultModalParent, setDefaultOrientation, setExceptionHandler, setParentShell, setReturnCode, setShellStyle, setWindowManager
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ECSortCustomizerDialog

public ECSortCustomizerDialog(org.eclipse.swt.widgets.Shell parentFrame, [AuthorResourceBundle](../../api/AuthorResourceBundle.md) authorResourceBundle, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) selectedElemensString, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) allElementsString)

Constructor.
  Parameters: parentFrame - The parent shell. authorResourceBundle - The author resource bundle. selectedElemensString - The name of the "selected elements" radio combo. allElementsString - The name of the "all elements" radio combo.
### ECSortCustomizerDialog

public ECSortCustomizerDialog(org.eclipse.swt.widgets.Shell parentFrame, [AuthorResourceBundle](../../api/AuthorResourceBundle.md) authorResourceBundle, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) selectedElemensString, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) allElementsString, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) helpPageID)

Constructor.
  Parameters: parentFrame - The parent shell. authorResourceBundle - The author resource bundle. selectedElemensString - The name of the "selected elements" radio combo. allElementsString - The name of the "all elements" radio combo. helpPageID - Help page ID
## Method Details

### createDialogArea

protected org.eclipse.swt.widgets.Control createDialogArea(org.eclipse.swt.widgets.Composite parent)
  Overrides: createDialogArea in class org.eclipse.jface.dialogs.Dialog See Also:
        * Dialog.createDialogArea(org.eclipse.swt.widgets.Composite)

### configureShell

protected void configureShell(org.eclipse.swt.widgets.Shell newShell)
  Overrides: configureShell in class org.eclipse.jface.window.Window See Also:
        * Window.configureShell(org.eclipse.swt.widgets.Shell)

### getSortInformation

public [SortCriteriaInformation](SortCriteriaInformation.md) getSortInformation([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> criteriaInformation, boolean hasSelectedSortableElements, boolean cannotSortAllElements)
 Description copied from interface: [SortCustomizer](SortCustomizer.md#getSortInformation(java.util.List,boolean,boolean))
Obtain the sort information given some initial sort criteria.
  Specified by: [getSortInformation](SortCustomizer.md#getSortInformation(java.util.List,boolean,boolean)) in interface [SortCustomizer](SortCustomizer.md) Parameters: criteriaInformation - The information about the available sorting criteria. hasSelectedSortableElements - true when elements selected in the document can be sorted. cannotSortAllElements - true when all the elements from the parent of the sort operation cannot be sorted. for example when the selected rows from a table can be sorted but the whole table cannot because it contains, outside the selected rows, some rows with multiple rowspan cells. Returns: The sort information, about criteria and the sort scope. See Also:
        * [SortCustomizer.getSortInformation(java.util.List, boolean, boolean)](SortCustomizer.md#getSortInformation(java.util.List,boolean,boolean))

### okPressed

protected void okPressed()
  Overrides: okPressed in class org.eclipse.jface.dialogs.Dialog See Also:
        * Dialog.okPressed()

### isResizable

protected boolean isResizable()
  Overrides: isResizable in class org.eclipse.jface.dialogs.Dialog See Also:
        * Dialog.isResizable()

### selectionChanged

public void selectionChanged([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newSelection, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) oldSelection)
 Description copied from interface: [KeysController](KeysController.md#selectionChanged(java.lang.String,java.lang.String))
Method which controls the change of the selected key.
  Specified by: [selectionChanged](KeysController.md#selectionChanged(java.lang.String,java.lang.String)) in interface [KeysController](KeysController.md) Parameters: newSelection - The new selected key. oldSelection - The old selected key. See Also:
        * [KeysController.selectionChanged(java.lang.String, java.lang.String)](KeysController.md#selectionChanged(java.lang.String,java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
