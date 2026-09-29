Package [ro.sync.ecss.extensions.tei.table](package-summary.md)

# Interface TEIConstants
    All Known Implementing Classes: [DeleteColumnOperation](DeleteColumnOperation.md), [DeleteRowOperation](DeleteRowOperation.md), [InsertColumnOperation](InsertColumnOperation.md), [InsertRowOperation](InsertRowOperation.md), [InsertSingleColumnOperation](InsertSingleColumnOperation.md), [InsertSingleRowOperation](InsertSingleRowOperation.md), [SplitCellAboveBelowOperation](SplitCellAboveBelowOperation.md), [SplitLeftRightOperation](SplitLeftRightOperation.md), [SplitOperation](SplitOperation.md), [TEIDocumentTypeHelper](../TEIDocumentTypeHelper.md)   @API(type=INTERNAL, src=PUBLIC) public interface TEIConstants
Interface containing the names of the elements and attributes used in TEI.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_COLS](#ATTRIBUTE_NAME_COLS)
The name of the 'cols' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_ID](#ATTRIBUTE_NAME_ID)
The name of the 'id' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_ROWS](#ATTRIBUTE_NAME_ROWS)
The name of the 'rows' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_XML_ID](#ATTRIBUTE_NAME_XML_ID)
The 'xml:id' attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_CELL](#ELEMENT_NAME_CELL)
The name of the element that defines a table cell.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_ROW](#ELEMENT_NAME_ROW)
The name of the element that defines a table row.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_TABLE](#ELEMENT_NAME_TABLE)
The name of the element that defines the main content of a table.

## Field Details

### ELEMENT_NAME_CELL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_CELL

The name of the element that defines a table cell. The value is cell.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.tei.table.TEIConstants.ELEMENT_NAME_CELL)

### ELEMENT_NAME_ROW

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_ROW

The name of the element that defines a table row. The value is row.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.tei.table.TEIConstants.ELEMENT_NAME_ROW)

### ELEMENT_NAME_TABLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_TABLE

The name of the element that defines the main content of a table. The value is table.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.tei.table.TEIConstants.ELEMENT_NAME_TABLE)

### ATTRIBUTE_NAME_ID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_ID

The name of the 'id' attribute.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.tei.table.TEIConstants.ATTRIBUTE_NAME_ID)

### ATTRIBUTE_NAME_XML_ID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_XML_ID

The 'xml:id' attribute.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.tei.table.TEIConstants.ATTRIBUTE_NAME_XML_ID)

### ATTRIBUTE_NAME_COLS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_COLS

The name of the 'cols' attribute. For the 'cell' element the attribute specifies the number of occupied columns in the table.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.tei.table.TEIConstants.ATTRIBUTE_NAME_COLS)

### ATTRIBUTE_NAME_ROWS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_ROWS

The name of the 'rows' attribute. For the 'cell' element the attribute specifies the number of occupied rows in the table.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.tei.table.TEIConstants.ATTRIBUTE_NAME_ROWS)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
