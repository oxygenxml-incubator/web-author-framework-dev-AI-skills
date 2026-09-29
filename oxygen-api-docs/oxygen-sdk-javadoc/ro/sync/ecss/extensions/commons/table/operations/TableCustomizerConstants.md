Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Interface TableCustomizerConstants
    All Known Subinterfaces: [DocbookTableCustomizerConstants](../../../docbook/table/DocbookTableCustomizerConstants.md), [XHTMLTableCustomizerConstants](xhtml/XHTMLTableCustomizerConstants.md)   All Known Implementing Classes: [ECDITARelTableCustomizerDialog](../../../dita/map/table/ECDITARelTableCustomizerDialog.md), [ECDITATableCustomizerDialog](../../../dita/topic/table/ECDITATableCustomizerDialog.md), [ECDocbookTableCustomizerDialog](../../../docbook/table/ECDocbookTableCustomizerDialog.md), [ECTableCustomizerDialog](ECTableCustomizerDialog.md), [ECTEITableCustomizerDialog](../../../tei/table/ECTEITableCustomizerDialog.md), [ECXHTMLTableCustomizerDialog](xhtml/ECXHTMLTableCustomizerDialog.md), [SADITARelTableCustomizerDialog](../../../dita/map/table/SADITARelTableCustomizerDialog.md), [SADITATableCustomizerDialog](../../../dita/topic/table/SADITATableCustomizerDialog.md), [SADocbook4TableCustomizerDialog](../../../docbook/table/SADocbook4TableCustomizerDialog.md), [SADocbook5TableCustomizerDialog](../../../docbook/table/SADocbook5TableCustomizerDialog.md), [SADocbookTableCustomizerDialog](../../../docbook/table/SADocbookTableCustomizerDialog.md), [SATableCustomizerDialog](SATableCustomizerDialog.md), [SATEITableCustomizerDialog](../../../tei/table/SATEITableCustomizerDialog.md), [SAXHTMLTableCustomizerDialog](xhtml/SAXHTMLTableCustomizerDialog.md)   @API(type=INTERNAL, src=PUBLIC) public interface TableCustomizerConstants
Constants used to choose certain table attributes.

## Nested Class Summary
 Nested Classes
Modifier and Type

Interface

Description
 static enum  [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md)
Column widths specifications

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md)[] [CALS_WIDTHS_SPECIFICATIONS](#CALS_WIDTHS_SPECIFICATIONS)
The column widths type for CALS tables.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CENTER](#CENTER)
Value for horizontal alignment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CHAR](#CHAR)
Value for horizontal alignment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [COLS_DYNAMIC](#COLS_DYNAMIC)
Dynamic column widths.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [COLS_FIXED](#COLS_FIXED)
Fixed column widths.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [COLS_PROPORTIONAL](#COLS_PROPORTIONAL)
Proportional column widths.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_CONREF](#DITA_CONREF)
DITA specific frame value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FIXED_COL_WIDTH_DEFAULT_VALUE](#FIXED_COL_WIDTH_DEFAULT_VALUE)
Fixed col width default value
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_ABOVE](#FRAME_ABOVE)
Possible value for 'frame' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_ALL](#FRAME_ALL)
Frame all four sides of the table.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_BELLOW](#FRAME_BELLOW)
Possible value for 'frame' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_BORDER](#FRAME_BORDER)
Possible value for 'frame' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_BOTTOM](#FRAME_BOTTOM)
Frame only the bottom of the table.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_BOX](#FRAME_BOX)
Possible value for 'frame' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_HSIDES](#FRAME_HSIDES)
Possible value for 'frame' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_LHS](#FRAME_LHS)
Possible value for 'frame' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_NONE](#FRAME_NONE)
Place no border on the table.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_RHS](#FRAME_RHS)
Possible value for 'frame' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_SIDES](#FRAME_SIDES)
Frame the left and right sides of the table.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_TOP](#FRAME_TOP)
Frame the top of the table.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_TOPBOT](#FRAME_TOPBOT)
Frame the top and bottom of the table.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_VOID](#FRAME_VOID)
Possible value for 'frame' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_VSIDES](#FRAME_VSIDES)
Possible value for 'frame' attribute.
  static final [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md)[] [HTML_WIDTHS_SPECIFICATIONS](#HTML_WIDTHS_SPECIFICATIONS)
The column widths type for HTML tables.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [JUSTIFY](#JUSTIFY)
Value for horizontal alignment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LEFT](#LEFT)
Value for horizontal alignment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [REL_COL_WIDTH_DEFAULT_VALUE](#REL_COL_WIDTH_DEFAULT_VALUE)
Default value for relative col widths.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [RIGHT](#RIGHT)
Value for horizontal alignment.
  static final [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md)[] [SIMPLE_WIDTHS_SPECIFICATIONS](#SIMPLE_WIDTHS_SPECIFICATIONS)
The column widths type for Simple tables.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UNSPECIFIED](#UNSPECIFIED)
Do not insert frame attribute.

## Field Details

### FRAME_ALL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_ALL

Frame all four sides of the table. The value is all.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_ALL)

### FRAME_BOTTOM

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_BOTTOM

Frame only the bottom of the table. The value is bottom.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_BOTTOM)

### FRAME_NONE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_NONE

Place no border on the table. The value is none.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_NONE)

### UNSPECIFIED

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UNSPECIFIED

Do not insert frame attribute. The value is .
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.UNSPECIFIED)

### FRAME_SIDES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_SIDES

Frame the left and right sides of the table. The value is sides.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_SIDES)

### FRAME_TOP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_TOP

Frame the top of the table. The value is top.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_TOP)

### FRAME_TOPBOT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_TOPBOT

Frame the top and bottom of the table. The value is topbot.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_TOPBOT)

### FRAME_ABOVE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_ABOVE

Possible value for 'frame' attribute. The value is above.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_ABOVE)

### FRAME_BELLOW

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_BELLOW

Possible value for 'frame' attribute. The value is below.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_BELLOW)

### FRAME_BORDER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_BORDER

Possible value for 'frame' attribute. The value is border.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_BORDER)

### FRAME_BOX

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_BOX

Possible value for 'frame' attribute. The value is box.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_BOX)

### FRAME_HSIDES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_HSIDES

Possible value for 'frame' attribute. The value is hsides.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_HSIDES)

### FRAME_VSIDES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_VSIDES

Possible value for 'frame' attribute. The value is vsides.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_VSIDES)

### FRAME_LHS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_LHS

Possible value for 'frame' attribute. The value is lhs.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_LHS)

### FRAME_RHS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_RHS

Possible value for 'frame' attribute. The value is rhs.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_RHS)

### FRAME_VOID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_VOID

Possible value for 'frame' attribute. The value is void.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FRAME_VOID)

### LEFT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LEFT

Value for horizontal alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.LEFT)

### RIGHT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) RIGHT

Value for horizontal alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.RIGHT)

### CENTER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CENTER

Value for horizontal alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.CENTER)

### JUSTIFY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) JUSTIFY

Value for horizontal alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.JUSTIFY)

### CHAR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CHAR

Value for horizontal alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.CHAR)

### DITA_CONREF

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_CONREF

DITA specific frame value.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.DITA_CONREF)

### COLS_DYNAMIC

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) COLS_DYNAMIC

Dynamic column widths.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.COLS_DYNAMIC)

### COLS_PROPORTIONAL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) COLS_PROPORTIONAL

Proportional column widths.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.COLS_PROPORTIONAL)

### COLS_FIXED

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) COLS_FIXED

Fixed column widths.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.COLS_FIXED)

### SIMPLE_WIDTHS_SPECIFICATIONS

static final [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md)[] SIMPLE_WIDTHS_SPECIFICATIONS

The column widths type for Simple tables.

### CALS_WIDTHS_SPECIFICATIONS

static final [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md)[] CALS_WIDTHS_SPECIFICATIONS

The column widths type for CALS tables.

### HTML_WIDTHS_SPECIFICATIONS

static final [TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md)[] HTML_WIDTHS_SPECIFICATIONS

The column widths type for HTML tables.

### REL_COL_WIDTH_DEFAULT_VALUE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) REL_COL_WIDTH_DEFAULT_VALUE

Default value for relative col widths.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.REL_COL_WIDTH_DEFAULT_VALUE)

### FIXED_COL_WIDTH_DEFAULT_VALUE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FIXED_COL_WIDTH_DEFAULT_VALUE

Fixed col width default value
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.TableCustomizerConstants.FIXED_COL_WIDTH_DEFAULT_VALUE)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
