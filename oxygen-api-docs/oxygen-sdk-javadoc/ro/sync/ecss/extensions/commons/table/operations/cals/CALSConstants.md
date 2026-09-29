Package [ro.sync.ecss.extensions.commons.table.operations.cals](package-summary.md)

# Interface CALSConstants
    All Known Implementing Classes: [CALSDocumentTypeHelper](CALSDocumentTypeHelper.md), [CALSTableCellInfoProvider](../../support/CALSTableCellInfoProvider.md), [CALSTableCellSpanProvider](../../spansupport/CALSTableCellSpanProvider.md), [DeleteColumnOperation](DeleteColumnOperation.md), [DeleteColumnOperation](../../../../dita/topic/table/cals/DeleteColumnOperation.md), [DeleteRowOperation](DeleteRowOperation.md), [DeleteRowOperation](../../../../dita/topic/table/cals/DeleteRowOperation.md), [DITACALSTableCellInfoProvider](../../support/DITACALSTableCellInfoProvider.md), [DITATableCellSepInfoProvider](../../support/DITATableCellSepInfoProvider.md), [DITATableDocumentTypeHelper](../../../../dita/topic/table/DITATableDocumentTypeHelper.md), [DocbookTableCellSepInfoProvider](../../../../docbook/table/DocbookTableCellSepInfoProvider.md), [InsertColumnOperation](InsertColumnOperation.md), [InsertColumnOperation](../../../../dita/topic/table/cals/InsertColumnOperation.md), [InsertRowOperation](InsertRowOperation.md), [InsertRowOperation](../../../../dita/topic/table/cals/InsertRowOperation.md), [InsertSingleColumnOperation](InsertSingleColumnOperation.md), [InsertSingleColumnOperation](../../../../dita/topic/table/cals/InsertSingleColumnOperation.md), [InsertSingleRowOperation](InsertSingleRowOperation.md), [InsertSingleRowOperation](../../../../dita/topic/table/cals/InsertSingleRowOperation.md), [JoinRowCellsOperation](JoinRowCellsOperation.md), [JoinRowCellsOperation](../../../../dita/topic/table/cals/JoinRowCellsOperation.md), [SplitCellAboveBelowOperation](SplitCellAboveBelowOperation.md), [SplitCellAboveBelowOperation](../../../../dita/topic/table/cals/SplitCellAboveBelowOperation.md), [SplitLeftRightOperation](SplitLeftRightOperation.md), [SplitLeftRightOperation](../../../../dita/topic/table/cals/SplitLeftRightOperation.md), [SplitOperation](SplitOperation.md), [SplitOperation](../../../../dita/topic/table/cals/SplitOperation.md)   @API(type=INTERNAL, src=PUBLIC) public interface CALSConstants
Contains the names of the elements and attributes used in CALS table model (e.g. DocBook or DITA tables).

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_ALIGN](#ATTRIBUTE_NAME_ALIGN)
The name of the 'colspec' element attribute that specifies the alignament of the column.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_COLNAME](#ATTRIBUTE_NAME_COLNAME)
The name of the attribute that defines the column name.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_COLNUM](#ATTRIBUTE_NAME_COLNUM)
The name of the 'colspec' element attribute that specifies the column number.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_COLS](#ATTRIBUTE_NAME_COLS)
The 'tgroup' element attribute that specifies the number of columns in the table.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_COLSEP](#ATTRIBUTE_NAME_COLSEP)
The name of the attribute that identifies a column separator specification for a table cell.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_COLWIDTH](#ATTRIBUTE_NAME_COLWIDTH)
The name of the 'colspec' element attribute that specifies the width of the column.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_ID](#ATTRIBUTE_NAME_ID)
The name of the id attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_MOREROWS](#ATTRIBUTE_NAME_MOREROWS)
The name of the 'morerows' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_NAMEEND](#ATTRIBUTE_NAME_NAMEEND)
The name of the attribute that specifies the end column name in a column span specification element.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_NAMEST](#ATTRIBUTE_NAME_NAMEST)
The name of the attribute that specifies the start column name in a column span specification element.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_ROWSEP](#ATTRIBUTE_NAME_ROWSEP)
The name of the attribute that identifies a row separator specification for a table cell.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_SPANNAME](#ATTRIBUTE_NAME_SPANNAME)
The name of the attribute that identifies a span specification for a table cell.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_TABLE_WIDTH](#ATTRIBUTE_NAME_TABLE_WIDTH)
The name of the width attribute for the 'table' element.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_XML_ID](#ATTRIBUTE_NAME_XML_ID)
The xml:id attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_COLSPEC](#ELEMENT_NAME_COLSPEC)
The name of the element that defines a column specification.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_ENTRY](#ELEMENT_NAME_ENTRY)
The name of the element that defines a CALS table cell.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_INFORMALTABLE](#ELEMENT_NAME_INFORMALTABLE)
The name of the element that defines an informaltable.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_ROW](#ELEMENT_NAME_ROW)
The name of the element that defines a CALS table row.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_SPANSPEC](#ELEMENT_NAME_SPANSPEC)
The name of the element that defines column span information.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_TABLE](#ELEMENT_NAME_TABLE)
The name of the element that defines a table.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_TGROUP](#ELEMENT_NAME_TGROUP)
The name of the element that defines the main content of a table, or part of a table.

## Field Details

### ELEMENT_NAME_TABLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_TABLE

The name of the element that defines a table. The value is 'table'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ELEMENT_NAME_TABLE)

### ELEMENT_NAME_ENTRY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_ENTRY

The name of the element that defines a CALS table cell. The value is 'entry'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ELEMENT_NAME_ENTRY)

### ELEMENT_NAME_ROW

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_ROW

The name of the element that defines a CALS table row. The value is 'row'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ELEMENT_NAME_ROW)

### ELEMENT_NAME_COLSPEC

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_COLSPEC

The name of the element that defines a column specification. The value is 'colspec'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ELEMENT_NAME_COLSPEC)

### ELEMENT_NAME_INFORMALTABLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_INFORMALTABLE

The name of the element that defines an informaltable. The value is 'informaltable'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ELEMENT_NAME_INFORMALTABLE)

### ELEMENT_NAME_TGROUP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_TGROUP

The name of the element that defines the main content of a table, or part of a table. The value is 'tgroup'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ELEMENT_NAME_TGROUP)

### ELEMENT_NAME_SPANSPEC

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_SPANSPEC

The name of the element that defines column span information. The value is 'spanspec'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ELEMENT_NAME_SPANSPEC)

### ATTRIBUTE_NAME_NAMEST

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_NAMEST

The name of the attribute that specifies the start column name in a column span specification element. The value is 'namest'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_NAMEST)

### ATTRIBUTE_NAME_NAMEEND

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_NAMEEND

The name of the attribute that specifies the end column name in a column span specification element. The value is 'nameend'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_NAMEEND)

### ATTRIBUTE_NAME_COLNAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_COLNAME

The name of the attribute that defines the column name. The value is 'colname'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_COLNAME)

### ATTRIBUTE_NAME_SPANNAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_SPANNAME

The name of the attribute that identifies a span specification for a table cell. The value is 'spanname'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_SPANNAME)

### ATTRIBUTE_NAME_COLSEP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_COLSEP

The name of the attribute that identifies a column separator specification for a table cell. The value is 'colsep'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_COLSEP)

### ATTRIBUTE_NAME_ROWSEP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_ROWSEP

The name of the attribute that identifies a row separator specification for a table cell. The value is 'rowsep'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_ROWSEP)

### ATTRIBUTE_NAME_COLNUM

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_COLNUM

The name of the 'colspec' element attribute that specifies the column number. The value is 'colnum'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_COLNUM)

### ATTRIBUTE_NAME_COLWIDTH

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_COLWIDTH

The name of the 'colspec' element attribute that specifies the width of the column. The value is 'colwidth'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_COLWIDTH)

### ATTRIBUTE_NAME_TABLE_WIDTH

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_TABLE_WIDTH

The name of the width attribute for the 'table' element. The value is 'width'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_TABLE_WIDTH)

### ATTRIBUTE_NAME_MOREROWS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_MOREROWS

The name of the 'morerows' attribute. Specifies on how many additional rows the cell spans. The value is 'morerows'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_MOREROWS)

### ATTRIBUTE_NAME_COLS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_COLS

The 'tgroup' element attribute that specifies the number of columns in the table. The value is 'cols'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_COLS)

### ATTRIBUTE_NAME_ID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_ID

The name of the id attribute. The value is 'id'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_ID)

### ATTRIBUTE_NAME_XML_ID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_XML_ID

The xml:id attribute. The value is 'xml:id'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_XML_ID)

### ATTRIBUTE_NAME_ALIGN

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_ALIGN

The name of the 'colspec' element attribute that specifies the alignament of the column. The value is 'align'.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.cals.CALSConstants.ATTRIBUTE_NAME_ALIGN)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
