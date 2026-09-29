Package [ro.sync.ecss.extensions.commons.table.operations.xhtml](package-summary.md)

# Interface XHTMLConstants
    All Known Implementing Classes: [DeleteColumnOperation](DeleteColumnOperation.md), [DeleteRowOperation](DeleteRowOperation.md), [InsertColumnOperation](InsertColumnOperation.md), [InsertRowOperation](InsertRowOperation.md), [InsertSingleColumnOperation](InsertSingleColumnOperation.md), [InsertSingleRowOperation](InsertSingleRowOperation.md), [SplitCellAboveBelowOperation](SplitCellAboveBelowOperation.md), [SplitLeftRightOperation](SplitLeftRightOperation.md), [SplitOperation](SplitOperation.md), [XHTMLDocumentTypeHelper](XHTMLDocumentTypeHelper.md)   @API(type=INTERNAL, src=PUBLIC) public interface XHTMLConstants
This interface contains the name of the elements and attributes used in XHTML.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_COLSPAN](#ATTRIBUTE_NAME_COLSPAN)
The name of the attribute that specifies the column span of a table cell.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_ID](#ATTRIBUTE_NAME_ID)
The name of the ID attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_ROWSPAN](#ATTRIBUTE_NAME_ROWSPAN)
The name of the attribute that specifies the row span of a table cell.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTRIBUTE_NAME_XML_ID](#ATTRIBUTE_NAME_XML_ID)
The xml:id attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_INFORMALTABLE](#ELEMENT_NAME_INFORMALTABLE)
The name of element that defines an XHTML table for DocBook model.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_TABLE](#ELEMENT_NAME_TABLE)
The name of element that defines an XHTML table.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_TD](#ELEMENT_NAME_TD)
The name of element that defines a table cell.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_TH](#ELEMENT_NAME_TH)
The name of element that defines a table header row.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_THEAD](#ELEMENT_NAME_THEAD)
The name of the table header element.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ELEMENT_NAME_TR](#ELEMENT_NAME_TR)
The name of element that defines a table row.

## Field Details

### ELEMENT_NAME_TD

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_TD

The name of element that defines a table cell. The value is td.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.xhtml.XHTMLConstants.ELEMENT_NAME_TD)

### ELEMENT_NAME_TR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_TR

The name of element that defines a table row. The value is tr.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.xhtml.XHTMLConstants.ELEMENT_NAME_TR)

### ELEMENT_NAME_TH

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_TH

The name of element that defines a table header row. The value is th.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.xhtml.XHTMLConstants.ELEMENT_NAME_TH)

### ELEMENT_NAME_TABLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_TABLE

The name of element that defines an XHTML table. The value is table.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.xhtml.XHTMLConstants.ELEMENT_NAME_TABLE)

### ELEMENT_NAME_INFORMALTABLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_INFORMALTABLE

The name of element that defines an XHTML table for DocBook model. The value is informaltable.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.xhtml.XHTMLConstants.ELEMENT_NAME_INFORMALTABLE)

### ATTRIBUTE_NAME_COLSPAN

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_COLSPAN

The name of the attribute that specifies the column span of a table cell. The value is colspan.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.xhtml.XHTMLConstants.ATTRIBUTE_NAME_COLSPAN)

### ATTRIBUTE_NAME_ID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_ID

The name of the ID attribute. The value is id.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.xhtml.XHTMLConstants.ATTRIBUTE_NAME_ID)

### ATTRIBUTE_NAME_XML_ID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_XML_ID

The xml:id attribute. The value is xml:id.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.xhtml.XHTMLConstants.ATTRIBUTE_NAME_XML_ID)

### ATTRIBUTE_NAME_ROWSPAN

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTRIBUTE_NAME_ROWSPAN

The name of the attribute that specifies the row span of a table cell. The value is rowspan.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.xhtml.XHTMLConstants.ATTRIBUTE_NAME_ROWSPAN)

### ELEMENT_NAME_THEAD

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ELEMENT_NAME_THEAD

The name of the table header element. The value is thead.
  See Also:
        * [Constant Field Values](../../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.xhtml.XHTMLConstants.ELEMENT_NAME_THEAD)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
