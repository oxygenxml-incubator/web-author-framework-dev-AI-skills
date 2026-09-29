Package [ro.sync.ecss.extensions.commons.table.operations.xhtml](package-summary.md)

# Class ECXHTMLTableCustomizerDialog

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * org.eclipse.jface.window.Window
        * org.eclipse.jface.dialogs.Dialog
            * org.eclipse.jface.dialogs.TrayDialog
                * [ro.sync.ecss.extensions.commons.table.operations.ECTableCustomizerDialog](../ECTableCustomizerDialog.md)
                    * ro.sync.ecss.extensions.commons.table.operations.xhtml.ECXHTMLTableCustomizerDialog
   All Implemented Interfaces: org.eclipse.jface.window.IShellProvider, [TableCustomizerConstants](../TableCustomizerConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class ECXHTMLTableCustomizerDialog extends [ECTableCustomizerDialog](../ECTableCustomizerDialog.md)
Dialog used to customize XHTML table creation. It is used on Eclipse platform implementation.

## Nested Class Summary

## Nested classes/interfaces inherited from class org.eclipse.jface.window.Window
 org.eclipse.jface.window.Window.IExceptionHandler
## Nested classes/interfaces inherited from interface ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](../TableCustomizerConstants.md)
 [TableCustomizerConstants.ColumnWidthsType](../TableCustomizerConstants.ColumnWidthsType.md)
## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[ECTableCustomizerDialog](../ECTableCustomizerDialog.md)
 [authorResourceBundle](../ECTableCustomizerDialog.md#authorResourceBundle), [selectedColWidthsType](../ECTableCustomizerDialog.md#selectedColWidthsType)
### Fields inherited from class org.eclipse.jface.dialogs.Dialog
 blockedHandler, buttonBar, DIALOG_DEFAULT_BOUNDS, DIALOG_PERSISTLOCATION, DIALOG_PERSISTSIZE, dialogArea, DLG_IMG_ERROR, DLG_IMG_HELP, DLG_IMG_INFO, DLG_IMG_MESSAGE_ERROR, DLG_IMG_MESSAGE_INFO, DLG_IMG_MESSAGE_WARNING, DLG_IMG_QUESTION, DLG_IMG_WARNING, ELLIPSIS
### Fields inherited from class org.eclipse.jface.window.Window
 CANCEL, OK, resizeHasOccurred
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](../TableCustomizerConstants.md)
 [CALS_WIDTHS_SPECIFICATIONS](../TableCustomizerConstants.md#CALS_WIDTHS_SPECIFICATIONS), [CENTER](../TableCustomizerConstants.md#CENTER), [CHAR](../TableCustomizerConstants.md#CHAR), [COLS_DYNAMIC](../TableCustomizerConstants.md#COLS_DYNAMIC), [COLS_FIXED](../TableCustomizerConstants.md#COLS_FIXED), [COLS_PROPORTIONAL](../TableCustomizerConstants.md#COLS_PROPORTIONAL), [DITA_CONREF](../TableCustomizerConstants.md#DITA_CONREF), [FIXED_COL_WIDTH_DEFAULT_VALUE](../TableCustomizerConstants.md#FIXED_COL_WIDTH_DEFAULT_VALUE), [FRAME_ABOVE](../TableCustomizerConstants.md#FRAME_ABOVE), [FRAME_ALL](../TableCustomizerConstants.md#FRAME_ALL), [FRAME_BELLOW](../TableCustomizerConstants.md#FRAME_BELLOW), [FRAME_BORDER](../TableCustomizerConstants.md#FRAME_BORDER), [FRAME_BOTTOM](../TableCustomizerConstants.md#FRAME_BOTTOM), [FRAME_BOX](../TableCustomizerConstants.md#FRAME_BOX), [FRAME_HSIDES](../TableCustomizerConstants.md#FRAME_HSIDES), [FRAME_LHS](../TableCustomizerConstants.md#FRAME_LHS), [FRAME_NONE](../TableCustomizerConstants.md#FRAME_NONE), [FRAME_RHS](../TableCustomizerConstants.md#FRAME_RHS), [FRAME_SIDES](../TableCustomizerConstants.md#FRAME_SIDES), [FRAME_TOP](../TableCustomizerConstants.md#FRAME_TOP), [FRAME_TOPBOT](../TableCustomizerConstants.md#FRAME_TOPBOT), [FRAME_VOID](../TableCustomizerConstants.md#FRAME_VOID), [FRAME_VSIDES](../TableCustomizerConstants.md#FRAME_VSIDES), [HTML_WIDTHS_SPECIFICATIONS](../TableCustomizerConstants.md#HTML_WIDTHS_SPECIFICATIONS), [JUSTIFY](../TableCustomizerConstants.md#JUSTIFY), [LEFT](../TableCustomizerConstants.md#LEFT), [REL_COL_WIDTH_DEFAULT_VALUE](../TableCustomizerConstants.md#REL_COL_WIDTH_DEFAULT_VALUE), [RIGHT](../TableCustomizerConstants.md#RIGHT), [SIMPLE_WIDTHS_SPECIFICATIONS](../TableCustomizerConstants.md#SIMPLE_WIDTHS_SPECIFICATIONS), [UNSPECIFIED](../TableCustomizerConstants.md#UNSPECIFIED)
## Constructor Summary
 Constructors
Constructor

Description
 [ECXHTMLTableCustomizerDialog](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,org.eclipse.swt.widgets.Shell,ro.sync.ecss.extensions.api.AuthorResourceBundle,int,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, [AuthorResourceBundle](../../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected org.eclipse.swt.widgets.Button [createTitleCheckbox](#createTitleCheckbox(org.eclipse.swt.widgets.Composite))(org.eclipse.swt.widgets.Composite parent)
Create a checkbox with an implementation specific title.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getAlignValues](#getAlignValues(int))(int tableModelType)
Compute the possible values for 'align' attribute.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getColsepValues](#getColsepValues(int))(int tableModelType)
Compute the possible values for 'colsep' attribute.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableCustomizerConstants.ColumnWidthsType](../TableCustomizerConstants.ColumnWidthsType.md)> [getColumnWidthsSpecifications](#getColumnWidthsSpecifications(int))(int tableModelType)
Compute the possible values for the column widths specifications.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultAlignValue](#getDefaultAlignValue(int))(int tableModelType)
Get the default align value.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultColsepValue](#getDefaultColsepValue(int))(int tableModelType)
Get the default column separator value.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultFrameValue](#getDefaultFrameValue(int))(int tableModelType)
Get the default frame value.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultRowsepValue](#getDefaultRowsepValue(int))(int tableModelType)
Get the default row separator value.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getFrameValues](#getFrameValues(int))(int tableModelType)
Compute the possible values for 'frame' attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID())()
Get the ID of the help page which will be called by the end user.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getRowsepValues](#getRowsepValues(int))(int tableModelType)
Compute the possible values for 'rowsep' attribute.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[ECTableCustomizerDialog](../ECTableCustomizerDialog.md)
 [configureShell](../ECTableCustomizerDialog.md#configureShell(org.eclipse.swt.widgets.Shell)), [createButtonsForButtonBar](../ECTableCustomizerDialog.md#createButtonsForButtonBar(org.eclipse.swt.widgets.Composite)), [createDialogArea](../ECTableCustomizerDialog.md#createDialogArea(org.eclipse.swt.widgets.Composite)), [showDialog](../ECTableCustomizerDialog.md#showDialog(ro.sync.ecss.extensions.commons.table.operations.TableInfo))
### Methods inherited from class org.eclipse.jface.dialogs.TrayDialog
 closeTray, createButtonBar, createHelpControl, getLayout, getTray, handleShellCloseEvent, isDialogHelpAvailable, isHelpAvailable, openTray, setDialogHelpAvailable, setHelpAvailable
### Methods inherited from class org.eclipse.jface.dialogs.Dialog
 applyDialogFont, buttonPressed, cancelPressed, close, convertHeightInCharsToPixels, convertHeightInCharsToPixels, convertHorizontalDLUsToPixels, convertHorizontalDLUsToPixels, convertVerticalDLUsToPixels, convertVerticalDLUsToPixels, convertWidthInCharsToPixels, convertWidthInCharsToPixels, create, createButton, createContents, dialogFontIsDefault, getBlockedHandler, getButton, getButtonBar, getCancelButton, getDialogArea, getDialogBoundsSettings, getDialogBoundsStrategy, getImage, getInitialLocation, getInitialSize, getOKButton, initializeBounds, initializeDialogUnits, isResizable, okPressed, setBlockedHandler, setButtonLayoutData, setButtonLayoutFormData, shortenText
### Methods inherited from class org.eclipse.jface.window.Window
 canHandleShellCloseEvent, constrainShellSize, createShell, getConstrainedShellBounds, getContents, getDefaultImage, getDefaultImages, getDefaultOrientation, getParentShell, getReturnCode, getShell, getShellListener, getShellStyle, getWindowManager, handleFontChange, open, setBlockOnOpen, setDefaultImage, setDefaultImages, setDefaultModalParent, setDefaultOrientation, setExceptionHandler, setParentShell, setReturnCode, setShellStyle, setWindowManager
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ECXHTMLTableCustomizerDialog

public ECXHTMLTableCustomizerDialog([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, [AuthorResourceBundle](../../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount)

Constructor.
  Parameters: authorAccess - The Author access. parentShell - The parent shell for the dialog. authorResourceBundle - The author resource bundle. predefinedRowsCount - The predefined number of rows. predefinedColumnsCount - The predefined number of columns.
## Method Details

### getFrameValues

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getFrameValues(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../ECTableCustomizerDialog.md#getFrameValues(int))
Compute the possible values for 'frame' attribute.
  Specified by: [getFrameValues](../ECTableCustomizerDialog.md#getFrameValues(int)) in class [ECTableCustomizerDialog](../ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for 'frame' attribute. See Also:
        * [ECTableCustomizerDialog.getFrameValues(int)](../ECTableCustomizerDialog.md#getFrameValues(int))

### getColumnWidthsSpecifications

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableCustomizerConstants.ColumnWidthsType](../TableCustomizerConstants.ColumnWidthsType.md)> getColumnWidthsSpecifications(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../ECTableCustomizerDialog.md#getColumnWidthsSpecifications(int))
Compute the possible values for the column widths specifications.
  Specified by: [getColumnWidthsSpecifications](../ECTableCustomizerDialog.md#getColumnWidthsSpecifications(int)) in class [ECTableCustomizerDialog](../ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for the column widths modifications. See Also:
        * [ECTableCustomizerDialog.getColumnWidthsSpecifications(int)](../ECTableCustomizerDialog.md#getColumnWidthsSpecifications(int))

### createTitleCheckbox

protected org.eclipse.swt.widgets.Button createTitleCheckbox(org.eclipse.swt.widgets.Composite parent)
 Description copied from class: [ECTableCustomizerDialog](../ECTableCustomizerDialog.md#createTitleCheckbox(org.eclipse.swt.widgets.Composite))
Create a checkbox with an implementation specific title.
  Specified by: [createTitleCheckbox](../ECTableCustomizerDialog.md#createTitleCheckbox(org.eclipse.swt.widgets.Composite)) in class [ECTableCustomizerDialog](../ECTableCustomizerDialog.md) Parameters: parent - The parent Composite. Returns: The title checkbox customized according to implementation. See Also:
        * [ECTableCustomizerDialog.createTitleCheckbox(org.eclipse.swt.widgets.Composite)](../ECTableCustomizerDialog.md#createTitleCheckbox(org.eclipse.swt.widgets.Composite))

### getDefaultFrameValue

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultFrameValue(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../ECTableCustomizerDialog.md#getDefaultFrameValue(int))
Get the default frame value.
  Specified by: [getDefaultFrameValue](../ECTableCustomizerDialog.md#getDefaultFrameValue(int)) in class [ECTableCustomizerDialog](../ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../TableInfo.md#TABLE_MODEL_HTML). Returns: The default frame value See Also:
        * [ECTableCustomizerDialog.getDefaultFrameValue(int)](../ECTableCustomizerDialog.md#getDefaultFrameValue(int))

### getRowsepValues

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getRowsepValues(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../ECTableCustomizerDialog.md#getRowsepValues(int))
Compute the possible values for 'rowsep' attribute.
  Specified by: [getRowsepValues](../ECTableCustomizerDialog.md#getRowsepValues(int)) in class [ECTableCustomizerDialog](../ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for 'rowsep' attribute. See Also:
        * [ECTableCustomizerDialog.getRowsepValues(int)](../ECTableCustomizerDialog.md#getRowsepValues(int))

### getColsepValues

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getColsepValues(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../ECTableCustomizerDialog.md#getColsepValues(int))
Compute the possible values for 'colsep' attribute.
  Specified by: [getColsepValues](../ECTableCustomizerDialog.md#getColsepValues(int)) in class [ECTableCustomizerDialog](../ECTableCustomizerDialog.md) Parameters: tableModelType - The table model. One of the constants: [TableInfo.TABLE_MODEL_CALS](../TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for 'colsep' attribute. See Also:
        * [ECTableCustomizerDialog.getColsepValues(int)](../ECTableCustomizerDialog.md#getColsepValues(int))

### getDefaultRowsepValue

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultRowsepValue(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../ECTableCustomizerDialog.md#getDefaultRowsepValue(int))
Get the default row separator value.
  Specified by: [getDefaultRowsepValue](../ECTableCustomizerDialog.md#getDefaultRowsepValue(int)) in class [ECTableCustomizerDialog](../ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../TableInfo.md#TABLE_MODEL_HTML). Returns: The default row separator value See Also:
        * [ECTableCustomizerDialog.getDefaultRowsepValue(int)](../ECTableCustomizerDialog.md#getDefaultRowsepValue(int))

### getDefaultColsepValue

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultColsepValue(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../ECTableCustomizerDialog.md#getDefaultColsepValue(int))
Get the default column separator value.
  Specified by: [getDefaultColsepValue](../ECTableCustomizerDialog.md#getDefaultColsepValue(int)) in class [ECTableCustomizerDialog](../ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../TableInfo.md#TABLE_MODEL_HTML). Returns: The default column separator value See Also:
        * [ECTableCustomizerDialog.getDefaultColsepValue(int)](../ECTableCustomizerDialog.md#getDefaultColsepValue(int))

### getAlignValues

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getAlignValues(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../ECTableCustomizerDialog.md#getAlignValues(int))
Compute the possible values for 'align' attribute.
  Specified by: [getAlignValues](../ECTableCustomizerDialog.md#getAlignValues(int)) in class [ECTableCustomizerDialog](../ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for 'align' attribute. See Also:
        * [ECTableCustomizerDialog.getAlignValues(int)](../ECTableCustomizerDialog.md#getAlignValues(int))

### getDefaultAlignValue

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultAlignValue(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../ECTableCustomizerDialog.md#getDefaultAlignValue(int))
Get the default align value.
  Specified by: [getDefaultAlignValue](../ECTableCustomizerDialog.md#getDefaultAlignValue(int)) in class [ECTableCustomizerDialog](../ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../TableInfo.md#TABLE_MODEL_HTML). Returns: The default align value See Also:
        * [ECTableCustomizerDialog.getDefaultAlignValue(int)](../ECTableCustomizerDialog.md#getDefaultAlignValue(int))

### getHelpPageID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID()
 Description copied from class: [ECTableCustomizerDialog](../ECTableCustomizerDialog.md#getHelpPageID())
Get the ID of the help page which will be called by the end user.
  Overrides: [getHelpPageID](../ECTableCustomizerDialog.md#getHelpPageID()) in class [ECTableCustomizerDialog](../ECTableCustomizerDialog.md) Returns: the ID of the help page which will be called by the end user or null. See Also:
        * [ECTableCustomizerDialog.getHelpPageID()](../ECTableCustomizerDialog.md#getHelpPageID())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
