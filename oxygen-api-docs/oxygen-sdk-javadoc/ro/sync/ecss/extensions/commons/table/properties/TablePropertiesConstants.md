Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Interface TablePropertiesConstants
    All Superinterfaces: [TableHelperConstants](TableHelperConstants.md)   All Known Subinterfaces: [TablePropertiesHelper](TablePropertiesHelper.md)   All Known Implementing Classes: [ChoiceTableHelper](../../../dita/topic/table/simpletable/properties/ChoiceTableHelper.md), [DITACALSTableHelper](../../../dita/topic/table/cals/properties/DITACALSTableHelper.md), [Docbook5CALSTableHelper](../../../docbook/table/properties/Docbook5CALSTableHelper.md), [Docbook5HTMLTableHelper](../../../docbook/table/properties/Docbook5HTMLTableHelper.md), [DocbookCALSTableHelper](../../../docbook/table/properties/DocbookCALSTableHelper.md), [DocbookHTMLTableHelper](../../../docbook/table/properties/DocbookHTMLTableHelper.md), [RelTablePropertiesHelper](../../../dita/map/table/RelTablePropertiesHelper.md), [SimpleTableHelper](../../../dita/topic/table/simpletable/properties/SimpleTableHelper.md), [TablePropertiesHelperBase](TablePropertiesHelperBase.md)   @API(type=INTERNAL, src=PUBLIC) public interface TablePropertiesConstantsextends [TableHelperConstants](TableHelperConstants.md)
Interface that contains all constants used in the table properties operation.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ALIGN](#ALIGN)
align attribute name.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTR_NOT_SET](#ATTR_NOT_SET)
Value shown when an attribute is not set.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [BOTTOM](#BOTTOM)
Value for vertical alignment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CENTER](#CENTER)
Value for horizontal alignment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CHAR](#CHAR)
Value for horizontal alignment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [COLSEP](#COLSEP)
Column separator attribute name.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EMPTY_ICON](#EMPTY_ICON)
Empty icon.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME](#FRAME)
Frame attribute name.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_ALIGN_CENTER](#ICON_ALIGN_CENTER)
Icon for horizontal align center.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_ALIGN_JUSTIFY](#ICON_ALIGN_JUSTIFY)
Icon for horizontal align justify.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_ALIGN_LEFT](#ICON_ALIGN_LEFT)
Icon for horizontal align left.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_ALIGN_RIGHT](#ICON_ALIGN_RIGHT)
Icon for horizontal align right.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_COL_ROW_SEP](#ICON_COL_ROW_SEP)
Icon for colsep = 1 and rowsep = 1.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_COLSEP](#ICON_COLSEP)
Icon for colsep = 1.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_FRAME_ALL](#ICON_FRAME_ALL)
Icon for frame all/box/border.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_FRAME_BOTTOM](#ICON_FRAME_BOTTOM)
Icon for frame bottom/bellow.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_FRAME_LHS](#ICON_FRAME_LHS)
Icon for frame lhs.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_FRAME_RHS](#ICON_FRAME_RHS)
Icon for frame rhs.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_FRAME_SIDES](#ICON_FRAME_SIDES)
Icon for frame sides/vsides.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_FRAME_TOP](#ICON_FRAME_TOP)
Icon for frame top/above.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_FRAME_TOPBOT](#ICON_FRAME_TOPBOT)
Icon for frame topbot/hsides.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_ROW_TYPE_BODY](#ICON_ROW_TYPE_BODY)
Icon for row type body.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_ROW_TYPE_FOOTER](#ICON_ROW_TYPE_FOOTER)
Icon for row type footer.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_ROW_TYPE_HEADER](#ICON_ROW_TYPE_HEADER)
Icon for row type header.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_ROWSEP](#ICON_ROWSEP)
Icon for rowsep = 1.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_VALIGN_BOTTOM](#ICON_VALIGN_BOTTOM)
Icon for vertical align bottom.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_VALIGN_MIDDLE](#ICON_VALIGN_MIDDLE)
Icon for vertical align middle.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ICON_VALIGN_TOP](#ICON_VALIGN_TOP)
Icon for vertical align top.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [JUSTIFY](#JUSTIFY)
Value for horizontal alignment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LEFT](#LEFT)
Value for horizontal alignment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MIDDLE](#MIDDLE)
Value for vertical alignment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [NOT_COMPUTED](#NOT_COMPUTED)
Value used to computed the common value of an attribute for multiple elements.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PRESERVE](#PRESERVE)
Used only for values that are not in the possible values list and are set explicitly in the document.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [RIGHT](#RIGHT)
Value for horizontal alignment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ROW_TYPE](#ROW_TYPE)
Name for row type property.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ROW_TYPE_BODY](#ROW_TYPE_BODY)
Value for row type property.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ROW_TYPE_FOOTER](#ROW_TYPE_FOOTER)
Value for row type property.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ROW_TYPE_HEADER](#ROW_TYPE_HEADER)
Value for row type property.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ROW_TYPE_PROPERTY](#ROW_TYPE_PROPERTY)
Row type property name.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ROWSEP](#ROWSEP)
Row separator attribute name.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TITLE_ELEMENT](#TITLE_ELEMENT)
The title element in a rel-table
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TOP](#TOP)
Value for vertical alignment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [VALIGN](#VALIGN)
Vertical alignment attribute name.

### Fields inherited from interface ro.sync.ecss.extensions.commons.table.properties.[TableHelperConstants](TableHelperConstants.md)
 [TYPE_BODY](TableHelperConstants.md#TYPE_BODY), [TYPE_BODY_DESC_CELL](TableHelperConstants.md#TYPE_BODY_DESC_CELL), [TYPE_CELL](TableHelperConstants.md#TYPE_CELL), [TYPE_COLSPEC](TableHelperConstants.md#TYPE_COLSPEC), [TYPE_FOOTER](TableHelperConstants.md#TYPE_FOOTER), [TYPE_GROUP](TableHelperConstants.md#TYPE_GROUP), [TYPE_HEADER](TableHelperConstants.md#TYPE_HEADER), [TYPE_HEADER_CELL](TableHelperConstants.md#TYPE_HEADER_CELL), [TYPE_HEADER_DESC_CELL](TableHelperConstants.md#TYPE_HEADER_DESC_CELL), [TYPE_ROW](TableHelperConstants.md#TYPE_ROW), [TYPE_TABLE](TableHelperConstants.md#TYPE_TABLE)
## Field Details

### ROW_TYPE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ROW_TYPE

Name for row type property.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ROW_TYPE)

### VALIGN

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) VALIGN

Vertical alignment attribute name.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.VALIGN)

### ALIGN

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ALIGN

align attribute name.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ALIGN)

### ROWSEP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ROWSEP

Row separator attribute name.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ROWSEP)

### COLSEP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) COLSEP

Column separator attribute name.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.COLSEP)

### FRAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME

Frame attribute name.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.FRAME)

### ATTR_NOT_SET

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTR_NOT_SET

Value shown when an attribute is not set.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ATTR_NOT_SET)

### NOT_COMPUTED

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) NOT_COMPUTED

Value used to computed the common value of an attribute for multiple elements.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.NOT_COMPUTED)

### EMPTY_ICON

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EMPTY_ICON

Empty icon.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.EMPTY_ICON)

### ICON_ROW_TYPE_HEADER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_ROW_TYPE_HEADER

Icon for row type header.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_ROW_TYPE_HEADER)

### ICON_ROW_TYPE_BODY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_ROW_TYPE_BODY

Icon for row type body.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_ROW_TYPE_BODY)

### ICON_ROW_TYPE_FOOTER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_ROW_TYPE_FOOTER

Icon for row type footer.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_ROW_TYPE_FOOTER)

### ICON_ALIGN_LEFT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_ALIGN_LEFT

Icon for horizontal align left.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_ALIGN_LEFT)

### ICON_ALIGN_RIGHT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_ALIGN_RIGHT

Icon for horizontal align right.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_ALIGN_RIGHT)

### ICON_ALIGN_CENTER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_ALIGN_CENTER

Icon for horizontal align center.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_ALIGN_CENTER)

### ICON_ALIGN_JUSTIFY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_ALIGN_JUSTIFY

Icon for horizontal align justify.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_ALIGN_JUSTIFY)

### ICON_COLSEP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_COLSEP

Icon for colsep = 1.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_COLSEP)

### ICON_ROWSEP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_ROWSEP

Icon for rowsep = 1.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_ROWSEP)

### ICON_COL_ROW_SEP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_COL_ROW_SEP

Icon for colsep = 1 and rowsep = 1.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_COL_ROW_SEP)

### ICON_VALIGN_TOP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_VALIGN_TOP

Icon for vertical align top.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_VALIGN_TOP)

### ICON_VALIGN_BOTTOM

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_VALIGN_BOTTOM

Icon for vertical align bottom.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_VALIGN_BOTTOM)

### ICON_VALIGN_MIDDLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_VALIGN_MIDDLE

Icon for vertical align middle.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_VALIGN_MIDDLE)

### ICON_FRAME_ALL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_FRAME_ALL

Icon for frame all/box/border.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_FRAME_ALL)

### ICON_FRAME_TOP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_FRAME_TOP

Icon for frame top/above.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_FRAME_TOP)

### ICON_FRAME_TOPBOT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_FRAME_TOPBOT

Icon for frame topbot/hsides.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_FRAME_TOPBOT)

### ICON_FRAME_BOTTOM

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_FRAME_BOTTOM

Icon for frame bottom/bellow.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_FRAME_BOTTOM)

### ICON_FRAME_SIDES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_FRAME_SIDES

Icon for frame sides/vsides.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_FRAME_SIDES)

### ICON_FRAME_LHS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_FRAME_LHS

Icon for frame lhs.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_FRAME_LHS)

### ICON_FRAME_RHS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ICON_FRAME_RHS

Icon for frame rhs.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ICON_FRAME_RHS)

### LEFT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LEFT

Value for horizontal alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.LEFT)

### RIGHT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) RIGHT

Value for horizontal alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.RIGHT)

### CENTER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CENTER

Value for horizontal alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.CENTER)

### JUSTIFY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) JUSTIFY

Value for horizontal alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.JUSTIFY)

### CHAR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CHAR

Value for horizontal alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.CHAR)

### TOP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TOP

Value for vertical alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.TOP)

### BOTTOM

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) BOTTOM

Value for vertical alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.BOTTOM)

### MIDDLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MIDDLE

Value for vertical alignment.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.MIDDLE)

### PRESERVE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PRESERVE

Used only for values that are not in the possible values list and are set explicitly in the document.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.PRESERVE)

### TITLE_ELEMENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TITLE_ELEMENT

The title element in a rel-table
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.TITLE_ELEMENT)

### ROW_TYPE_BODY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ROW_TYPE_BODY

Value for row type property.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ROW_TYPE_BODY)

### ROW_TYPE_HEADER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ROW_TYPE_HEADER

Value for row type property.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ROW_TYPE_HEADER)

### ROW_TYPE_FOOTER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ROW_TYPE_FOOTER

Value for row type property.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ROW_TYPE_FOOTER)

### ROW_TYPE_PROPERTY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ROW_TYPE_PROPERTY

Row type property name.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.properties.TablePropertiesConstants.ROW_TYPE_PROPERTY)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
