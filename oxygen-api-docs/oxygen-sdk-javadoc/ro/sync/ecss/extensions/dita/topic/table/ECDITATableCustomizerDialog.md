Package [ro.sync.ecss.extensions.dita.topic.table](package-summary.md)

# Class ECDITATableCustomizerDialog

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * org.eclipse.jface.window.Window
        * org.eclipse.jface.dialogs.Dialog
            * org.eclipse.jface.dialogs.TrayDialog
                * [ro.sync.ecss.extensions.commons.table.operations.ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md)
                    * ro.sync.ecss.extensions.dita.topic.table.ECDITATableCustomizerDialog
   All Implemented Interfaces: org.eclipse.jface.window.IShellProvider, [TableCustomizerConstants](../../../commons/table/operations/TableCustomizerConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class ECDITATableCustomizerDialog extends [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md)
Dialog used to customize DITA table creation. It is used for Eclipse platform implementation.

## Nested Class Summary

## Nested classes/interfaces inherited from class org.eclipse.jface.window.Window
 org.eclipse.jface.window.Window.IExceptionHandler
## Nested classes/interfaces inherited from interface ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](../../../commons/table/operations/TableCustomizerConstants.md)
 [TableCustomizerConstants.ColumnWidthsType](../../../commons/table/operations/TableCustomizerConstants.ColumnWidthsType.md)
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [ALIGN_VALUES](#ALIGN_VALUES)
Array with common possible values for alignment.

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md)
 [authorResourceBundle](../../../commons/table/operations/ECTableCustomizerDialog.md#authorResourceBundle), [selectedColWidthsType](../../../commons/table/operations/ECTableCustomizerDialog.md#selectedColWidthsType)
### Fields inherited from class org.eclipse.jface.dialogs.Dialog
 blockedHandler, buttonBar, DIALOG_DEFAULT_BOUNDS, DIALOG_PERSISTLOCATION, DIALOG_PERSISTSIZE, dialogArea, DLG_IMG_ERROR, DLG_IMG_HELP, DLG_IMG_INFO, DLG_IMG_MESSAGE_ERROR, DLG_IMG_MESSAGE_INFO, DLG_IMG_MESSAGE_WARNING, DLG_IMG_QUESTION, DLG_IMG_WARNING, ELLIPSIS
### Fields inherited from class org.eclipse.jface.window.Window
 CANCEL, OK, resizeHasOccurred
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](../../../commons/table/operations/TableCustomizerConstants.md)
 [CALS_WIDTHS_SPECIFICATIONS](../../../commons/table/operations/TableCustomizerConstants.md#CALS_WIDTHS_SPECIFICATIONS), [CENTER](../../../commons/table/operations/TableCustomizerConstants.md#CENTER), [CHAR](../../../commons/table/operations/TableCustomizerConstants.md#CHAR), [COLS_DYNAMIC](../../../commons/table/operations/TableCustomizerConstants.md#COLS_DYNAMIC), [COLS_FIXED](../../../commons/table/operations/TableCustomizerConstants.md#COLS_FIXED), [COLS_PROPORTIONAL](../../../commons/table/operations/TableCustomizerConstants.md#COLS_PROPORTIONAL), [FIXED_COL_WIDTH_DEFAULT_VALUE](../../../commons/table/operations/TableCustomizerConstants.md#FIXED_COL_WIDTH_DEFAULT_VALUE), [FRAME_ABOVE](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_ABOVE), [FRAME_ALL](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_ALL), [FRAME_BELLOW](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_BELLOW), [FRAME_BORDER](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_BORDER), [FRAME_BOTTOM](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_BOTTOM), [FRAME_BOX](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_BOX), [FRAME_HSIDES](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_HSIDES), [FRAME_LHS](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_LHS), [FRAME_NONE](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_NONE), [FRAME_RHS](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_RHS), [FRAME_SIDES](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_SIDES), [FRAME_TOP](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_TOP), [FRAME_TOPBOT](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_TOPBOT), [FRAME_VOID](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_VOID), [FRAME_VSIDES](../../../commons/table/operations/TableCustomizerConstants.md#FRAME_VSIDES), [HTML_WIDTHS_SPECIFICATIONS](../../../commons/table/operations/TableCustomizerConstants.md#HTML_WIDTHS_SPECIFICATIONS), [JUSTIFY](../../../commons/table/operations/TableCustomizerConstants.md#JUSTIFY), [LEFT](../../../commons/table/operations/TableCustomizerConstants.md#LEFT), [REL_COL_WIDTH_DEFAULT_VALUE](../../../commons/table/operations/TableCustomizerConstants.md#REL_COL_WIDTH_DEFAULT_VALUE), [RIGHT](../../../commons/table/operations/TableCustomizerConstants.md#RIGHT), [SIMPLE_WIDTHS_SPECIFICATIONS](../../../commons/table/operations/TableCustomizerConstants.md#SIMPLE_WIDTHS_SPECIFICATIONS), [UNSPECIFIED](../../../commons/table/operations/TableCustomizerConstants.md#UNSPECIFIED)
## Constructor Summary
 Constructors
Constructor

Description
 [ECDITATableCustomizerDialog](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,org.eclipse.swt.widgets.Shell,ro.sync.ecss.extensions.api.AuthorResourceBundle,int,int,boolean))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount, boolean insertChoiceTable)
Constructor.
  [ECDITATableCustomizerDialog](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,org.eclipse.swt.widgets.Shell,ro.sync.ecss.extensions.api.AuthorResourceBundle,int,int,boolean,boolean,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount, boolean insertChoiceTable, boolean isPropertiesTableAccepted, int defaultTableModel)
Constructor.
  [ECDITATableCustomizerDialog](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,org.eclipse.swt.widgets.Shell,ro.sync.ecss.extensions.api.AuthorResourceBundle,int,int,boolean,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount, boolean insertChoiceTable, int defaultTableModel)
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
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableCustomizerConstants.ColumnWidthsType](../../../commons/table/operations/TableCustomizerConstants.ColumnWidthsType.md)> [getColumnWidthsSpecifications](#getColumnWidthsSpecifications(int))(int tableModelType)
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

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md)
 [configureShell](../../../commons/table/operations/ECTableCustomizerDialog.md#configureShell(org.eclipse.swt.widgets.Shell)), [createButtonsForButtonBar](../../../commons/table/operations/ECTableCustomizerDialog.md#createButtonsForButtonBar(org.eclipse.swt.widgets.Composite)), [createDialogArea](../../../commons/table/operations/ECTableCustomizerDialog.md#createDialogArea(org.eclipse.swt.widgets.Composite)), [showDialog](../../../commons/table/operations/ECTableCustomizerDialog.md#showDialog(ro.sync.ecss.extensions.commons.table.operations.TableInfo))
### Methods inherited from class org.eclipse.jface.dialogs.TrayDialog
 closeTray, createButtonBar, createHelpControl, getLayout, getTray, handleShellCloseEvent, isDialogHelpAvailable, isHelpAvailable, openTray, setDialogHelpAvailable, setHelpAvailable
### Methods inherited from class org.eclipse.jface.dialogs.Dialog
 applyDialogFont, buttonPressed, cancelPressed, close, convertHeightInCharsToPixels, convertHeightInCharsToPixels, convertHorizontalDLUsToPixels, convertHorizontalDLUsToPixels, convertVerticalDLUsToPixels, convertVerticalDLUsToPixels, convertWidthInCharsToPixels, convertWidthInCharsToPixels, create, createButton, createContents, dialogFontIsDefault, getBlockedHandler, getButton, getButtonBar, getCancelButton, getDialogArea, getDialogBoundsSettings, getDialogBoundsStrategy, getImage, getInitialLocation, getInitialSize, getOKButton, initializeBounds, initializeDialogUnits, isResizable, okPressed, setBlockedHandler, setButtonLayoutData, setButtonLayoutFormData, shortenText
### Methods inherited from class org.eclipse.jface.window.Window
 canHandleShellCloseEvent, constrainShellSize, createShell, getConstrainedShellBounds, getContents, getDefaultImage, getDefaultImages, getDefaultOrientation, getParentShell, getReturnCode, getShell, getShellListener, getShellStyle, getWindowManager, handleFontChange, open, setBlockOnOpen, setDefaultImage, setDefaultImages, setDefaultModalParent, setDefaultOrientation, setExceptionHandler, setParentShell, setReturnCode, setShellStyle, setWindowManager
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### ALIGN_VALUES

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] ALIGN_VALUES

Array with common possible values for alignment.

## Constructor Details

### ECDITATableCustomizerDialog

public ECDITATableCustomizerDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount, boolean insertChoiceTable)

Constructor.
  Parameters: authorAccess - The Author access. parentShell - The parent Shell. authorResourceBundle - The author resource bundle. predefinedRowsCount - The predefined number of rows. predefinedColumnsCount - The predefined number of columns. insertChoiceTable - true if should insert a DITA choice table.
### ECDITATableCustomizerDialog

public ECDITATableCustomizerDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount, boolean insertChoiceTable, int defaultTableModel)

Constructor.
  Parameters: authorAccess - The Author access. parentShell - The parent Shell. authorResourceBundle - The author resource bundle. predefinedRowsCount - The predefined number of rows. predefinedColumnsCount - The predefined number of columns. insertChoiceTable - true if should insert a DITA choice table. defaultTableModel - The default model of the table that will be inserted.
### ECDITATableCustomizerDialog

public ECDITATableCustomizerDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount, boolean insertChoiceTable, boolean isPropertiesTableAccepted, int defaultTableModel)

Constructor.
  Parameters: authorAccess - The Author access. parentShell - The parent Shell. authorResourceBundle - The author resource bundle. predefinedRowsCount - The predefined number of rows. predefinedColumnsCount - The predefined number of columns. insertChoiceTable - true if should insert a DITA choice table. isPropertiesTableAccepted - true if a properties table is accepted by the schema (i.e. if it is a global element). defaultTableModel - The default model of the table that will be inserted.
## Method Details

### getColumnWidthsSpecifications

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableCustomizerConstants.ColumnWidthsType](../../../commons/table/operations/TableCustomizerConstants.ColumnWidthsType.md)> getColumnWidthsSpecifications(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md#getColumnWidthsSpecifications(int))
Compute the possible values for the column widths specifications.
  Specified by: [getColumnWidthsSpecifications](../../../commons/table/operations/ECTableCustomizerDialog.md#getColumnWidthsSpecifications(int)) in class [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for the column widths modifications. See Also:
        * [ECTableCustomizerDialog.getColumnWidthsSpecifications(int)](../../../commons/table/operations/ECTableCustomizerDialog.md#getColumnWidthsSpecifications(int))

### getFrameValues

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getFrameValues(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md#getFrameValues(int))
Compute the possible values for 'frame' attribute.
  Specified by: [getFrameValues](../../../commons/table/operations/ECTableCustomizerDialog.md#getFrameValues(int)) in class [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for 'frame' attribute. See Also:
        * [ECTableCustomizerDialog.getFrameValues(int)](../../../commons/table/operations/ECTableCustomizerDialog.md#getFrameValues(int))

### createTitleCheckbox

protected org.eclipse.swt.widgets.Button createTitleCheckbox(org.eclipse.swt.widgets.Composite parent)
 Description copied from class: [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md#createTitleCheckbox(org.eclipse.swt.widgets.Composite))
Create a checkbox with an implementation specific title.
  Specified by: [createTitleCheckbox](../../../commons/table/operations/ECTableCustomizerDialog.md#createTitleCheckbox(org.eclipse.swt.widgets.Composite)) in class [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md) Parameters: parent - The parent Composite. Returns: The title checkbox customized according to implementation. See Also:
        * [ECTableCustomizerDialog.createTitleCheckbox(org.eclipse.swt.widgets.Composite)](../../../commons/table/operations/ECTableCustomizerDialog.md#createTitleCheckbox(org.eclipse.swt.widgets.Composite))

### getDefaultFrameValue

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultFrameValue(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md#getDefaultFrameValue(int))
Get the default frame value.
  Specified by: [getDefaultFrameValue](../../../commons/table/operations/ECTableCustomizerDialog.md#getDefaultFrameValue(int)) in class [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_HTML). Returns: The default frame value See Also:
        * [ECTableCustomizerDialog.getDefaultFrameValue(int)](../../../commons/table/operations/ECTableCustomizerDialog.md#getDefaultFrameValue(int))

### getRowsepValues

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getRowsepValues(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md#getRowsepValues(int))
Compute the possible values for 'rowsep' attribute.
  Specified by: [getRowsepValues](../../../commons/table/operations/ECTableCustomizerDialog.md#getRowsepValues(int)) in class [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for 'rowsep' attribute. See Also:
        * [ECTableCustomizerDialog.getRowsepValues(int)](../../../commons/table/operations/ECTableCustomizerDialog.md#getRowsepValues(int))

### getColsepValues

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getColsepValues(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md#getColsepValues(int))
Compute the possible values for 'colsep' attribute.
  Specified by: [getColsepValues](../../../commons/table/operations/ECTableCustomizerDialog.md#getColsepValues(int)) in class [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md) Parameters: tableModelType - The table model. One of the constants: [TableInfo.TABLE_MODEL_CALS](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for 'colsep' attribute. See Also:
        * [ECTableCustomizerDialog.getColsepValues(int)](../../../commons/table/operations/ECTableCustomizerDialog.md#getColsepValues(int))

### getDefaultRowsepValue

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultRowsepValue(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md#getDefaultRowsepValue(int))
Get the default row separator value.
  Specified by: [getDefaultRowsepValue](../../../commons/table/operations/ECTableCustomizerDialog.md#getDefaultRowsepValue(int)) in class [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_HTML). Returns: The default row separator value See Also:
        * [ECTableCustomizerDialog.getDefaultRowsepValue(int)](../../../commons/table/operations/ECTableCustomizerDialog.md#getDefaultRowsepValue(int))

### getDefaultColsepValue

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultColsepValue(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md#getDefaultColsepValue(int))
Get the default column separator value.
  Specified by: [getDefaultColsepValue](../../../commons/table/operations/ECTableCustomizerDialog.md#getDefaultColsepValue(int)) in class [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_HTML). Returns: The default column separator value See Also:
        * [ECTableCustomizerDialog.getDefaultColsepValue(int)](../../../commons/table/operations/ECTableCustomizerDialog.md#getDefaultColsepValue(int))

### getAlignValues

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getAlignValues(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md#getAlignValues(int))
Compute the possible values for 'align' attribute.
  Specified by: [getAlignValues](../../../commons/table/operations/ECTableCustomizerDialog.md#getAlignValues(int)) in class [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for 'align' attribute. See Also:
        * [ECTableCustomizerDialog.getAlignValues(int)](../../../commons/table/operations/ECTableCustomizerDialog.md#getAlignValues(int))

### getDefaultAlignValue

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultAlignValue(int tableModelType)
 Description copied from class: [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md#getDefaultAlignValue(int))
Get the default align value.
  Specified by: [getDefaultAlignValue](../../../commons/table/operations/ECTableCustomizerDialog.md#getDefaultAlignValue(int)) in class [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md) Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](../../../commons/table/operations/TableInfo.md#TABLE_MODEL_HTML). Returns: The default align value See Also:
        * [ECTableCustomizerDialog.getDefaultAlignValue(int)](../../../commons/table/operations/ECTableCustomizerDialog.md#getDefaultAlignValue(int))

### getHelpPageID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID()
 Description copied from class: [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md#getHelpPageID())
Get the ID of the help page which will be called by the end user.
  Overrides: [getHelpPageID](../../../commons/table/operations/ECTableCustomizerDialog.md#getHelpPageID()) in class [ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md) Returns: the ID of the help page which will be called by the end user or null. See Also:
        * [ECTableCustomizerDialog.getHelpPageID()](../../../commons/table/operations/ECTableCustomizerDialog.md#getHelpPageID())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
