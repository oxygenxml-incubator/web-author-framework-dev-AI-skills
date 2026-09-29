Package [ro.sync.ecss.extensions.commons.table.support](package-summary.md)

# Class CALSColSpec

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.support.CALSColSpec
   @API(type=INTERNAL, src=PUBLIC) public class CALSColSpec extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The column specification for a CALS table model (e.g. DocBook or DITA tables).

## Constructor Summary
 Constructors
Constructor

Description
 [CALSColSpec](#%3Cinit%3E(int,int,boolean,java.lang.String,java.lang.String,java.lang.Boolean,java.lang.Boolean))(int indexInDocument, int colNumber, boolean colNumberSpecified, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colWidth, [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) colSep, [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) rowSep)
Constructor.
  [CALSColSpec](#%3Cinit%3E(int,int,boolean,java.lang.String,ro.sync.ecss.extensions.api.WidthRepresentation))(int indexInDocument, int colNumber, boolean colNumberSpecified, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colName, [WidthRepresentation](../../../api/WidthRepresentation.md) colWidth)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [createXMLFragment](#createXMLFragment(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ns)
Creates the XML fragment corresponding to the column specification obtained from the colNumber, colName and colWidth fields.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAlign](#getAlign())()
Get the align value specified on the colspec.
  [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) [getColSep](#getColSep())()
Tests the presence of the column separator.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getColumnName](#getColumnName())()

 int [getColumnNumber](#getColumnNumber())()

 [WidthRepresentation](../../../api/WidthRepresentation.md) [getColWidth](#getColWidth())()

 int [getIndexInDocument](#getIndexInDocument())()

 [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) [getRowSep](#getRowSep())()
Tests the presence of the row separator.
  boolean [isColNumberSpecified](#isColNumberSpecified())()

 void [setAlign](#setAlign(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) align)
Set the align value specified on the colspec.
  void [setColWidth](#setColWidth(ro.sync.ecss.extensions.api.WidthRepresentation))([WidthRepresentation](../../../api/WidthRepresentation.md) colWidth)
Set the new [WidthRepresentation](../../../api/WidthRepresentation.md) corresponding to the column specification.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()
Creates a String representation of the column specification.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CALSColSpec

public CALSColSpec(int indexInDocument, int colNumber, boolean colNumberSpecified, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colWidth, [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) colSep, [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) rowSep)

Constructor.
  Parameters: indexInDocument - Index in colspec elements list. colNumber - The number of the column. It is 1 based. colNumberSpecified - true if the column number was specified as an attribute colName - The name of the column. colWidth - The string representation of the column width as described in the [WidthRepresentation](../../../api/WidthRepresentation.md). colSep - true if the column separators are needed for that column, false if not, null if the framework default should apply. For instance Docbook has the colsep on true by default, while DITA on false. rowSep - true if the row separators are needed for that column, false if not, null if the framework default should apply. For instance Docbook has the rowsep on true by default, while DITA on false.
### CALSColSpec

public CALSColSpec(int indexInDocument, int colNumber, boolean colNumberSpecified, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) colName, [WidthRepresentation](../../../api/WidthRepresentation.md) colWidth)

Constructor. The rowsep and colsep are set to null, i.e. the document type default.
  Parameters: indexInDocument - Index in colspec elements list. colNumber - The number of this column. It is 1 based. colNumberSpecified - true if the column number was specified as an attribute colName - The name of this column. colWidth - The column width representation.
## Method Details

### getColSep

public [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) getColSep()

Tests the presence of the column separator.
  Returns: true if the separator should be painted at the right of the cell, false if no separator is needed, or null if the default specified by the document type should be applied. For instance in Docbook, the default value is true while in DITA is false. If the cell is the last in the row, this value is disregarded.
### getRowSep

public [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) getRowSep()

Tests the presence of the row separator.
  Returns: true if the separator should be painted below the cell, false if no separator is needed, or null if the default specified by the document type should be applied. For instance in Docbook, the default value is true while in DITA is false. If the cell is the in the last row, this value is disregarded.
### isColNumberSpecified

public boolean isColNumberSpecified()
  Returns: Returns the colNumberSpecified.
### getIndexInDocument

public int getIndexInDocument()
  Returns: Returns the indexInDocument.
### getColumnNumber

public int getColumnNumber()
  Returns: The column number. It is 1 based.
### getColumnName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getColumnName()
  Returns: The name of the column.
### getColWidth

public [WidthRepresentation](../../../api/WidthRepresentation.md) getColWidth()
  Returns: Returns the column width representation.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()

Creates a String representation of the column specification.
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### createXMLFragment

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) createXMLFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ns)

Creates the XML fragment corresponding to the column specification obtained from the colNumber, colName and colWidth fields. The general format of the generated fragment is:  <colspec colnum="integer_value" colname="string_value" colwidth="string_value" xmlns="URI"/>
  Parameters: ns - The namespace URI of the table element. It can be null. Returns: The XML fragment corresponding to the column specification.
### setColWidth

public void setColWidth([WidthRepresentation](../../../api/WidthRepresentation.md) colWidth)

Set the new [WidthRepresentation](../../../api/WidthRepresentation.md) corresponding to the column specification.
  Parameters: colWidth - The column width to be set.
### getAlign

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAlign()

Get the align value specified on the colspec.
  Returns: Returns the align value.
### setAlign

public void setAlign([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) align)

Set the align value specified on the colspec.
  Parameters: align - The textAlign to set.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
