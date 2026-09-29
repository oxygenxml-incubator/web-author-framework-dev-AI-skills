Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class ECTableCustomizerDialog

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * org.eclipse.jface.window.Window
        * org.eclipse.jface.dialogs.Dialog
            * org.eclipse.jface.dialogs.TrayDialog
                * ro.sync.ecss.extensions.commons.table.operations.ECTableCustomizerDialog
   All Implemented Interfaces: org.eclipse.jface.window.IShellProvider, [TableCustomizerConstants](TableCustomizerConstants.md)   Direct Known Subclasses: [ECDITARelTableCustomizerDialog](../../../dita/map/table/ECDITARelTableCustomizerDialog.md), [ECDITATableCustomizerDialog](../../../dita/topic/table/ECDITATableCustomizerDialog.md), [ECDocbookTableCustomizerDialog](../../../docbook/table/ECDocbookTableCustomizerDialog.md), [ECTEITableCustomizerDialog](../../../tei/table/ECTEITableCustomizerDialog.md), [ECXHTMLTableCustomizerDialog](xhtml/ECXHTMLTableCustomizerDialog.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class ECTableCustomizerDialog extends org.eclipse.jface.dialogs.TrayDialog implements [TableCustomizerConstants](TableCustomizerConstants.md)
Dialog used to customize the insertion of a generic table (number of rows, columns, table caption). It is used on Eclipse platform implementation.

## Nested Class Summary

## Nested classes/interfaces inherited from class org.eclipse.jface.window.Window
 org.eclipse.jface.window.Window.IExceptionHandler
## Nested classes/interfaces inherited from interface ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](TableCustomizerConstants.md)
 [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md)
## Field Summary
 Fields
Modifier and Type

Field

Description
 protected final [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) [authorResourceBundle](#authorResourceBundle)
Author resource bundle.
  protected [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md) [selectedColWidthsType](#selectedColWidthsType)
The selected column widths type

### Fields inherited from class org.eclipse.jface.dialogs.Dialog
 blockedHandler, buttonBar, DIALOG_DEFAULT_BOUNDS, DIALOG_PERSISTLOCATION, DIALOG_PERSISTSIZE, dialogArea, DLG_IMG_ERROR, DLG_IMG_HELP, DLG_IMG_INFO, DLG_IMG_MESSAGE_ERROR, DLG_IMG_MESSAGE_INFO, DLG_IMG_MESSAGE_WARNING, DLG_IMG_QUESTION, DLG_IMG_WARNING, ELLIPSIS
### Fields inherited from class org.eclipse.jface.window.Window
 CANCEL, OK, resizeHasOccurred
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](TableCustomizerConstants.md)
 [CALS_WIDTHS_SPECIFICATIONS](TableCustomizerConstants.md#CALS_WIDTHS_SPECIFICATIONS), [CENTER](TableCustomizerConstants.md#CENTER), [CHAR](TableCustomizerConstants.md#CHAR), [COLS_DYNAMIC](TableCustomizerConstants.md#COLS_DYNAMIC), [COLS_FIXED](TableCustomizerConstants.md#COLS_FIXED), [COLS_PROPORTIONAL](TableCustomizerConstants.md#COLS_PROPORTIONAL), [DITA_CONREF](TableCustomizerConstants.md#DITA_CONREF), [FIXED_COL_WIDTH_DEFAULT_VALUE](TableCustomizerConstants.md#FIXED_COL_WIDTH_DEFAULT_VALUE), [FRAME_ABOVE](TableCustomizerConstants.md#FRAME_ABOVE), [FRAME_ALL](TableCustomizerConstants.md#FRAME_ALL), [FRAME_BELLOW](TableCustomizerConstants.md#FRAME_BELLOW), [FRAME_BORDER](TableCustomizerConstants.md#FRAME_BORDER), [FRAME_BOTTOM](TableCustomizerConstants.md#FRAME_BOTTOM), [FRAME_BOX](TableCustomizerConstants.md#FRAME_BOX), [FRAME_HSIDES](TableCustomizerConstants.md#FRAME_HSIDES), [FRAME_LHS](TableCustomizerConstants.md#FRAME_LHS), [FRAME_NONE](TableCustomizerConstants.md#FRAME_NONE), [FRAME_RHS](TableCustomizerConstants.md#FRAME_RHS), [FRAME_SIDES](TableCustomizerConstants.md#FRAME_SIDES), [FRAME_TOP](TableCustomizerConstants.md#FRAME_TOP), [FRAME_TOPBOT](TableCustomizerConstants.md#FRAME_TOPBOT), [FRAME_VOID](TableCustomizerConstants.md#FRAME_VOID), [FRAME_VSIDES](TableCustomizerConstants.md#FRAME_VSIDES), [HTML_WIDTHS_SPECIFICATIONS](TableCustomizerConstants.md#HTML_WIDTHS_SPECIFICATIONS), [JUSTIFY](TableCustomizerConstants.md#JUSTIFY), [LEFT](TableCustomizerConstants.md#LEFT), [REL_COL_WIDTH_DEFAULT_VALUE](TableCustomizerConstants.md#REL_COL_WIDTH_DEFAULT_VALUE), [RIGHT](TableCustomizerConstants.md#RIGHT), [SIMPLE_WIDTHS_SPECIFICATIONS](TableCustomizerConstants.md#SIMPLE_WIDTHS_SPECIFICATIONS), [UNSPECIFIED](TableCustomizerConstants.md#UNSPECIFIED)
## Constructor Summary
 Constructors
Constructor

Description
 [ECTableCustomizerDialog](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,org.eclipse.swt.widgets.Shell,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,ro.sync.ecss.extensions.api.AuthorResourceBundle,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, boolean hasFooter, boolean hasFrameAttribute, boolean showModelChooser, boolean showSimpleModelRadio, boolean showChoiceTableDialog, boolean isCalsTable, boolean isSimpleOrHtmlTable, boolean innerCalsTable, boolean isPropertiesTableAccepted, boolean isPropertiesTableModel, boolean hasRowsep, boolean hasColsep, boolean hasAlign, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount)
Constructor.
  [ECTableCustomizerDialog](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,org.eclipse.swt.widgets.Shell,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,ro.sync.ecss.extensions.api.AuthorResourceBundle,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, boolean hasFooter, boolean hasFrameAttribute, boolean showModelChooser, boolean showSimpleModelRadio, boolean showChoiceTableDialog, boolean isCalsTable, boolean innerCalsTable, boolean hasRowsep, boolean hasColsep, boolean hasAlign, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount)
Constructor.
  [ECTableCustomizerDialog](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,org.eclipse.swt.widgets.Shell,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,ro.sync.ecss.extensions.api.AuthorResourceBundle,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, boolean hasFooter, boolean hasFrameAttribute, boolean showModelChooser, boolean showSimpleModelRadio, boolean showChoiceTableDialog, boolean innerCalsTable, boolean hasRowsep, boolean hasColsep, boolean hasAlign, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount)
Constructor for TrangDialog.
  [ECTableCustomizerDialog](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,org.eclipse.swt.widgets.Shell,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,ro.sync.ecss.extensions.api.AuthorResourceBundle,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, boolean hasFooter, boolean hasFrameAttribute, boolean showModelChooser, boolean showSimpleModelRadio, boolean innerCalsTable, boolean hasRowsep, boolean hasColsep, boolean hasAlign, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount)
Constructor.
  [ECTableCustomizerDialog](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,org.eclipse.swt.widgets.Shell,boolean,boolean,boolean,ro.sync.ecss.extensions.api.AuthorResourceBundle,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, boolean hasFooter, boolean hasFrameAttribute, boolean showModelChooser, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount)
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [configureShell](#configureShell(org.eclipse.swt.widgets.Shell))(org.eclipse.swt.widgets.Shell newShell)
Configure Shell.
  protected void [createButtonsForButtonBar](#createButtonsForButtonBar(org.eclipse.swt.widgets.Composite))(org.eclipse.swt.widgets.Composite parent)

 protected org.eclipse.swt.widgets.Control [createDialogArea](#createDialogArea(org.eclipse.swt.widgets.Composite))(org.eclipse.swt.widgets.Composite parent)
Create Dialog area.
  protected abstract org.eclipse.swt.widgets.Button [createTitleCheckbox](#createTitleCheckbox(org.eclipse.swt.widgets.Composite))(org.eclipse.swt.widgets.Composite parent)
Create a checkbox with an implementation specific title.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getAlignValues](#getAlignValues(int))(int tableModelType)
Compute the possible values for 'align' attribute.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getColsepValues](#getColsepValues(int))(int tableModelType)
Compute the possible values for 'colsep' attribute.
  protected abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md)> [getColumnWidthsSpecifications](#getColumnWidthsSpecifications(int))(int tableModelType)
Compute the possible values for the column widths specifications.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultAlignValue](#getDefaultAlignValue(int))(int tableModelType)
Get the default align value.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultColsepValue](#getDefaultColsepValue(int))(int tableModelType)
Get the default column separator value.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultFrameValue](#getDefaultFrameValue(int))(int tableModelType)
Get the default frame value.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultRowsepValue](#getDefaultRowsepValue(int))(int tableModelType)
Get the default row separator value.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getFrameValues](#getFrameValues(int))(int tableModelType)
Compute the possible values for 'frame' attribute.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID())()
Get the ID of the help page which will be called by the end user.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getRowsepValues](#getRowsepValues(int))(int tableModelType)
Compute the possible values for 'rowsep' attribute.
  [TableInfo](TableInfo.md) [showDialog](#showDialog(ro.sync.ecss.extensions.commons.table.operations.TableInfo))([TableInfo](TableInfo.md) tableInfo)
Show the dialog to customize the table attributes.

### Methods inherited from class org.eclipse.jface.dialogs.TrayDialog
 closeTray, createButtonBar, createHelpControl, getLayout, getTray, handleShellCloseEvent, isDialogHelpAvailable, isHelpAvailable, openTray, setDialogHelpAvailable, setHelpAvailable
### Methods inherited from class org.eclipse.jface.dialogs.Dialog
 applyDialogFont, buttonPressed, cancelPressed, close, convertHeightInCharsToPixels, convertHeightInCharsToPixels, convertHorizontalDLUsToPixels, convertHorizontalDLUsToPixels, convertVerticalDLUsToPixels, convertVerticalDLUsToPixels, convertWidthInCharsToPixels, convertWidthInCharsToPixels, create, createButton, createContents, dialogFontIsDefault, getBlockedHandler, getButton, getButtonBar, getCancelButton, getDialogArea, getDialogBoundsSettings, getDialogBoundsStrategy, getImage, getInitialLocation, getInitialSize, getOKButton, initializeBounds, initializeDialogUnits, isResizable, okPressed, setBlockedHandler, setButtonLayoutData, setButtonLayoutFormData, shortenText
### Methods inherited from class org.eclipse.jface.window.Window
 canHandleShellCloseEvent, constrainShellSize, createShell, getConstrainedShellBounds, getContents, getDefaultImage, getDefaultImages, getDefaultOrientation, getParentShell, getReturnCode, getShell, getShellListener, getShellStyle, getWindowManager, handleFontChange, open, setBlockOnOpen, setDefaultImage, setDefaultImages, setDefaultModalParent, setDefaultOrientation, setExceptionHandler, setParentShell, setReturnCode, setShellStyle, setWindowManager
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### selectedColWidthsType

protected [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md) selectedColWidthsType

The selected column widths type

### authorResourceBundle

protected final [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle

Author resource bundle.

## Constructor Details

### ECTableCustomizerDialog

public ECTableCustomizerDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, boolean hasFooter, boolean hasFrameAttribute, boolean showModelChooser, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount)

Constructor.
  Parameters: authorAccess - The Author access. parentShell - The parent shell for the dialog. hasFooter - true if this table supports a footer. hasFrameAttribute - true if the table has a frame attribute. showModelChooser - true to show the dialog panel for choosing the table model, one of CALS or HTML. authorResourceBundle - The author resource bundle. predefinedRowsCount - The predefined number of rows. predefinedColumnsCount - The predefined number of columns.
### ECTableCustomizerDialog

public ECTableCustomizerDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, boolean hasFooter, boolean hasFrameAttribute, boolean showModelChooser, boolean showSimpleModelRadio, boolean innerCalsTable, boolean hasRowsep, boolean hasColsep, boolean hasAlign, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount)

Constructor.
  Parameters: authorAccess - The Author access. parentShell - The parent shell for the dialog. hasFooter - true if this table supports a footer. hasFrameAttribute - true if the table has a frame attribute. showModelChooser - true to show the dialog panel for choosing the table model, one of CALS or HTML. showSimpleModelRadio - true to show the simple model radio in the model chooser. innerCalsTable - true if this is an inner calls table. hasRowsep - true if the table has rowsep attribute. Flag used to add a corresponding combo box in the dialog. hasColsep - true if the table has colsep attribute. Flag used to add a corresponding combo box in the dialog. hasAlign - true if the table has align attribute. Flag used to add a corresponding combo box in the dialog. authorResourceBundle - The author resource bundle. predefinedRowsCount - The predefined number of rows. predefinedColumnsCount - The predefined number of columns.
### ECTableCustomizerDialog

public ECTableCustomizerDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, boolean hasFooter, boolean hasFrameAttribute, boolean showModelChooser, boolean showSimpleModelRadio, boolean showChoiceTableDialog, boolean innerCalsTable, boolean hasRowsep, boolean hasColsep, boolean hasAlign, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount)

Constructor for TrangDialog.
  Parameters: authorAccess - The Author access. parentShell - The parent shell for the dialog. hasFooter - true if this table supports a footer. hasFrameAttribute - true if the table has a frame attribute. showModelChooser - true to show the dialog panel for choosing the table model, one of CALS or HTML. showSimpleModelRadio - true to show the simple model radio in the model chooser. showChoiceTableDialog - true to show the dialog for choice table. innerCalsTable - true if this is an inner calls table. hasRowsep - true if the table has rowsep attribute. Flag used to add a corresponding combo box in the dialog. hasColsep - true if the table has colsep attribute. Flag used to add a corresponding combo box in the dialog. hasAlign - true if the table has align attribute. Flag used to add a corresponding combo box in the dialog. authorResourceBundle - The author resource bundle. predefinedRowsCount - The predefined number of rows. predefinedColumnsCount - The predefined number of columns.
### ECTableCustomizerDialog

public ECTableCustomizerDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, boolean hasFooter, boolean hasFrameAttribute, boolean showModelChooser, boolean showSimpleModelRadio, boolean showChoiceTableDialog, boolean isCalsTable, boolean innerCalsTable, boolean hasRowsep, boolean hasColsep, boolean hasAlign, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount)

Constructor.
  Parameters: authorAccess - The Author access. parentShell - The parent shell for the dialog. hasFooter - true if this table supports a footer. hasFrameAttribute - true if the table has a frame attribute. showModelChooser - true to show the dialog panel for choosing the table model, one of CALS or HTML. showSimpleModelRadio - true to show the simple model radio in the model chooser. showChoiceTableDialog - true to show the dialog for choice table. isCalsTable - true if the table model is CALS. innerCalsTable - true if this is an inner calls table. hasRowsep - true if the table has rowsep attribute. Flag used to add a corresponding combo box in the dialog. hasColsep - true if the table has colsep attribute. Flag used to add a corresponding combo box in the dialog. hasAlign - true if the table has align attribute. Flag used to add a corresponding combo box in the dialog. authorResourceBundle - The author resource bundle. predefinedRowsCount - The predefined number of rows. predefinedColumnsCount - The predefined number of columns.
### ECTableCustomizerDialog

public ECTableCustomizerDialog([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, org.eclipse.swt.widgets.Shell parentShell, boolean hasFooter, boolean hasFrameAttribute, boolean showModelChooser, boolean showSimpleModelRadio, boolean showChoiceTableDialog, boolean isCalsTable, boolean isSimpleOrHtmlTable, boolean innerCalsTable, boolean isPropertiesTableAccepted, boolean isPropertiesTableModel, boolean hasRowsep, boolean hasColsep, boolean hasAlign, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, int predefinedRowsCount, int predefinedColumnsCount)

Constructor.
  Parameters: authorAccess - The Author access. parentShell - The parent shell for the dialog. hasFooter - true if this table supports a footer. hasFrameAttribute - true if the table has a frame attribute. showModelChooser - true to show the dialog panel for choosing the table model, one of CALS or HTML. showSimpleModelRadio - true to show the simple model radio in the model chooser. showChoiceTableDialog - true to show the dialog for choice table. isCalsTable - true if the table model is CALS. isSimpleOrHtmlTable - true if the table model is simple or HTML. innerCalsTable - true if this is an inner calls table. isPropertiesTableAccepted - true of a properties table is accepted. isPropertiesTableModel - true if the current table has a properties table model. hasRowsep - true if the table has rowsep attribute. Flag used to add a corresponding combo box in the dialog. hasColsep - true if the table has colsep attribute. Flag used to add a corresponding combo box in the dialog. hasAlign - true if the table has align attribute. Flag used to add a corresponding combo box in the dialog. authorResourceBundle - The author resource bundle. predefinedRowsCount - The predefined number of rows. predefinedColumnsCount - The predefined number of columns.
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
### getFrameValues

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getFrameValues(int tableModelType)

Compute the possible values for 'frame' attribute.
  Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for 'frame' attribute.
### getRowsepValues

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getRowsepValues(int tableModelType)

Compute the possible values for 'rowsep' attribute.
  Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for 'rowsep' attribute.
### getColsepValues

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getColsepValues(int tableModelType)

Compute the possible values for 'colsep' attribute.
  Parameters: tableModelType - The table model. One of the constants: [TableInfo.TABLE_MODEL_CALS](TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for 'colsep' attribute.
### getAlignValues

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getAlignValues(int tableModelType)

Compute the possible values for 'align' attribute.
  Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for 'align' attribute.
### getDefaultFrameValue

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultFrameValue(int tableModelType)

Get the default frame value.
  Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](TableInfo.md#TABLE_MODEL_HTML). Returns: The default frame value
### getDefaultRowsepValue

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultRowsepValue(int tableModelType)

Get the default row separator value.
  Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](TableInfo.md#TABLE_MODEL_HTML). Returns: The default row separator value
### getDefaultColsepValue

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultColsepValue(int tableModelType)

Get the default column separator value.
  Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](TableInfo.md#TABLE_MODEL_HTML). Returns: The default column separator value
### getDefaultAlignValue

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultAlignValue(int tableModelType)

Get the default align value.
  Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](TableInfo.md#TABLE_MODEL_HTML). Returns: The default align value
### getColumnWidthsSpecifications

protected abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md)> getColumnWidthsSpecifications(int tableModelType)

Compute the possible values for the column widths specifications.
  Parameters: tableModelType - The table model type. One of the constants: [TableInfo.TABLE_MODEL_CALS](TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](TableInfo.md#TABLE_MODEL_HTML). Returns: Returns the possible values for the column widths modifications.
### createTitleCheckbox

protected abstract org.eclipse.swt.widgets.Button createTitleCheckbox(org.eclipse.swt.widgets.Composite parent)

Create a checkbox with an implementation specific title.
  Parameters: parent - The parent Composite. Returns: The title checkbox customized according to implementation.
### showDialog

public [TableInfo](TableInfo.md) showDialog([TableInfo](TableInfo.md) tableInfo)

Show the dialog to customize the table attributes.
  Parameters: tableInfo -  Returns: The information about the table to be inserted, or null if the user canceled the table insertion.
### createButtonsForButtonBar

protected void createButtonsForButtonBar(org.eclipse.swt.widgets.Composite parent)
  Overrides: createButtonsForButtonBar in class org.eclipse.jface.dialogs.Dialog See Also:
        * Dialog.createButtonsForButtonBar(org.eclipse.swt.widgets.Composite)

### getHelpPageID

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID()

Get the ID of the help page which will be called by the end user.
  Returns: the ID of the help page which will be called by the end user or null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
