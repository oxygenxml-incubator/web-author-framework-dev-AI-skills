Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Class TablePropertiesHelperBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.properties.TablePropertiesHelperBase
   All Implemented Interfaces: [TableHelper](TableHelper.md), [TableHelperConstants](TableHelperConstants.md), [TablePropertiesConstants](TablePropertiesConstants.md), [TablePropertiesHelper](TablePropertiesHelper.md)   Direct Known Subclasses: [DITACALSTableHelper](../../../dita/topic/table/cals/properties/DITACALSTableHelper.md), [DocbookCALSTableHelper](../../../docbook/table/properties/DocbookCALSTableHelper.md), [RelTablePropertiesHelper](../../../dita/map/table/RelTablePropertiesHelper.md), [SimpleTableHelper](../../../dita/topic/table/simpletable/properties/SimpleTableHelper.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class TablePropertiesHelperBase extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [TablePropertiesHelper](TablePropertiesHelper.md)
Abstract class for table properties helper.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.commons.table.properties.[TableHelperConstants](TableHelperConstants.md)
 [TYPE_BODY](TableHelperConstants.md#TYPE_BODY), [TYPE_BODY_DESC_CELL](TableHelperConstants.md#TYPE_BODY_DESC_CELL), [TYPE_CELL](TableHelperConstants.md#TYPE_CELL), [TYPE_COLSPEC](TableHelperConstants.md#TYPE_COLSPEC), [TYPE_FOOTER](TableHelperConstants.md#TYPE_FOOTER), [TYPE_GROUP](TableHelperConstants.md#TYPE_GROUP), [TYPE_HEADER](TableHelperConstants.md#TYPE_HEADER), [TYPE_HEADER_CELL](TableHelperConstants.md#TYPE_HEADER_CELL), [TYPE_HEADER_DESC_CELL](TableHelperConstants.md#TYPE_HEADER_DESC_CELL), [TYPE_ROW](TableHelperConstants.md#TYPE_ROW), [TYPE_TABLE](TableHelperConstants.md#TYPE_TABLE)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesConstants](TablePropertiesConstants.md)
 [ALIGN](TablePropertiesConstants.md#ALIGN), [ATTR_NOT_SET](TablePropertiesConstants.md#ATTR_NOT_SET), [BOTTOM](TablePropertiesConstants.md#BOTTOM), [CENTER](TablePropertiesConstants.md#CENTER), [CHAR](TablePropertiesConstants.md#CHAR), [COLSEP](TablePropertiesConstants.md#COLSEP), [EMPTY_ICON](TablePropertiesConstants.md#EMPTY_ICON), [FRAME](TablePropertiesConstants.md#FRAME), [ICON_ALIGN_CENTER](TablePropertiesConstants.md#ICON_ALIGN_CENTER), [ICON_ALIGN_JUSTIFY](TablePropertiesConstants.md#ICON_ALIGN_JUSTIFY), [ICON_ALIGN_LEFT](TablePropertiesConstants.md#ICON_ALIGN_LEFT), [ICON_ALIGN_RIGHT](TablePropertiesConstants.md#ICON_ALIGN_RIGHT), [ICON_COL_ROW_SEP](TablePropertiesConstants.md#ICON_COL_ROW_SEP), [ICON_COLSEP](TablePropertiesConstants.md#ICON_COLSEP), [ICON_FRAME_ALL](TablePropertiesConstants.md#ICON_FRAME_ALL), [ICON_FRAME_BOTTOM](TablePropertiesConstants.md#ICON_FRAME_BOTTOM), [ICON_FRAME_LHS](TablePropertiesConstants.md#ICON_FRAME_LHS), [ICON_FRAME_RHS](TablePropertiesConstants.md#ICON_FRAME_RHS), [ICON_FRAME_SIDES](TablePropertiesConstants.md#ICON_FRAME_SIDES), [ICON_FRAME_TOP](TablePropertiesConstants.md#ICON_FRAME_TOP), [ICON_FRAME_TOPBOT](TablePropertiesConstants.md#ICON_FRAME_TOPBOT), [ICON_ROW_TYPE_BODY](TablePropertiesConstants.md#ICON_ROW_TYPE_BODY), [ICON_ROW_TYPE_FOOTER](TablePropertiesConstants.md#ICON_ROW_TYPE_FOOTER), [ICON_ROW_TYPE_HEADER](TablePropertiesConstants.md#ICON_ROW_TYPE_HEADER), [ICON_ROWSEP](TablePropertiesConstants.md#ICON_ROWSEP), [ICON_VALIGN_BOTTOM](TablePropertiesConstants.md#ICON_VALIGN_BOTTOM), [ICON_VALIGN_MIDDLE](TablePropertiesConstants.md#ICON_VALIGN_MIDDLE), [ICON_VALIGN_TOP](TablePropertiesConstants.md#ICON_VALIGN_TOP), [JUSTIFY](TablePropertiesConstants.md#JUSTIFY), [LEFT](TablePropertiesConstants.md#LEFT), [MIDDLE](TablePropertiesConstants.md#MIDDLE), [NOT_COMPUTED](TablePropertiesConstants.md#NOT_COMPUTED), [PRESERVE](TablePropertiesConstants.md#PRESERVE), [RIGHT](TablePropertiesConstants.md#RIGHT), [ROW_TYPE](TablePropertiesConstants.md#ROW_TYPE), [ROW_TYPE_BODY](TablePropertiesConstants.md#ROW_TYPE_BODY), [ROW_TYPE_FOOTER](TablePropertiesConstants.md#ROW_TYPE_FOOTER), [ROW_TYPE_HEADER](TablePropertiesConstants.md#ROW_TYPE_HEADER), [ROW_TYPE_PROPERTY](TablePropertiesConstants.md#ROW_TYPE_PROPERTY), [ROWSEP](TablePropertiesConstants.md#ROWSEP), [TITLE_ELEMENT](TablePropertiesConstants.md#TITLE_ELEMENT), [TOP](TablePropertiesConstants.md#TOP), [VALIGN](TablePropertiesConstants.md#VALIGN)
## Constructor Summary
 Constructors
Constructor

Description
 [TablePropertiesHelperBase](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [allowsFooter](#allowsFooter())()
true if the current table allows footer element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getElementName](#getElementName(int))(int elementType)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getElementTag](#getElementTag(int))(int elementType)
Obtain the element name.
  int [getElementType](#getElementType(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Obtain the type of the given node.
  [AuthorElement](../../../api/node/AuthorElement.md) [getFirstChildOfTypeFromParentWithType](#getFirstChildOfTypeFromParentWithType(ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorElement](../../../api/node/AuthorElement.md) currentRow, int childType, int parentType)
Obtain the first row child of the parent which has the given type.
  boolean [isNodeOfType](#isNodeOfType(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../api/node/AuthorElement.md) node, int type)
Test if an [AuthorNode](../../../api/node/AuthorNode.md) is an element and it has one of the following types: [AuthorTableHelper.TYPE_CELL](../operations/AuthorTableHelper.md#TYPE_CELL), [AuthorTableHelper.TYPE_ROW](../operations/AuthorTableHelper.md#TYPE_ROW) or [AuthorTableHelper.TYPE_TABLE](../operations/AuthorTableHelper.md#TYPE_TABLE).
  boolean [isTable](#isTable(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents the table element.
  boolean [isTableBody](#isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table body element.
  boolean [isTableCell](#isTableCell(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table cell element.
  boolean [isTableColspec](#isTableColspec(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table colspec element.
  boolean [isTableFoot](#isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table foot element.
  boolean [isTableGroup](#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table group element.
  boolean [isTableHead](#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table head element.
  boolean [isTableRow](#isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table row element.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TablePropertiesHelperBase

public TablePropertiesHelperBase()

## Method Details

### isTable

public boolean isTable([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from interface: [TableHelper](TableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorElement))
Checks if the given node represents the table element.
  Specified by: [isTable](TableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [TableHelper](TableHelper.md) Parameters: node - The node to be checked. Returns: true if the given node is the table element. See Also:
        * [TableHelper.isTable(ro.sync.ecss.extensions.api.node.AuthorElement)](TableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTableGroup

public boolean isTableGroup([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from interface: [TableHelper](TableHelper.md#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement))
Checks if the given node represents a table group element.
  Specified by: [isTableGroup](TableHelper.md#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [TableHelper](TableHelper.md) Parameters: node - The node to be checked. Returns: true if the given node is the table group element. See Also:
        * [TableHelper.isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement)](TableHelper.md#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTableBody

public boolean isTableBody([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from interface: [TablePropertiesHelper](TablePropertiesHelper.md#isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement))
Checks if the given node represents a table body element.
  Specified by: [isTableBody](TablePropertiesHelper.md#isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [TablePropertiesHelper](TablePropertiesHelper.md) Parameters: node - The node to be checked. Returns: true if the given node is a table body element. See Also:
        * [TablePropertiesHelper.isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement)](TablePropertiesHelper.md#isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTableHead

public boolean isTableHead([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from interface: [TablePropertiesHelper](TablePropertiesHelper.md#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement))
Checks if the given node represents a table head element.
  Specified by: [isTableHead](TablePropertiesHelper.md#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [TablePropertiesHelper](TablePropertiesHelper.md) Parameters: node - The node to be checked. Returns: true if the given node is a table head element. See Also:
        * [TablePropertiesHelper.isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement)](TablePropertiesHelper.md#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTableFoot

public boolean isTableFoot([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from interface: [TablePropertiesHelper](TablePropertiesHelper.md#isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement))
Checks if the given node represents a table foot element.
  Specified by: [isTableFoot](TablePropertiesHelper.md#isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [TablePropertiesHelper](TablePropertiesHelper.md) Parameters: node - The node to be checked. Returns: true if the given node is a table foot element. See Also:
        * [TablePropertiesHelper.isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement)](TablePropertiesHelper.md#isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTableRow

public boolean isTableRow([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from interface: [TablePropertiesHelper](TablePropertiesHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement))
Checks if the given node represents a table row element.
  Specified by: [isTableRow](TablePropertiesHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [TablePropertiesHelper](TablePropertiesHelper.md) Parameters: node - The node to be checked. Returns: true if the given node is a table row element. See Also:
        * [TablePropertiesHelper.isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement)](TablePropertiesHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTableCell

public boolean isTableCell([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from interface: [TablePropertiesHelper](TablePropertiesHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorElement))
Checks if the given node represents a table cell element.
  Specified by: [isTableCell](TablePropertiesHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [TablePropertiesHelper](TablePropertiesHelper.md) Parameters: node - The node to be checked. Returns: true if the given node is a table cell element. See Also:
        * [TablePropertiesHelper.isTableCell(ro.sync.ecss.extensions.api.node.AuthorElement)](TablePropertiesHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorElement))

### isTableColspec

public boolean isTableColspec([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from interface: [TablePropertiesHelper](TablePropertiesHelper.md#isTableColspec(ro.sync.ecss.extensions.api.node.AuthorElement))
Checks if the given node represents a table colspec element.
  Specified by: [isTableColspec](TablePropertiesHelper.md#isTableColspec(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [TablePropertiesHelper](TablePropertiesHelper.md) Parameters: node - The node to be checked. Returns: true if the given node is a table colspec element. See Also:
        * [TablePropertiesHelper.isTableColspec(ro.sync.ecss.extensions.api.node.AuthorElement)](TablePropertiesHelper.md#isTableColspec(ro.sync.ecss.extensions.api.node.AuthorElement))

### isNodeOfType

public boolean isNodeOfType([AuthorElement](../../../api/node/AuthorElement.md) node, int type)
 Description copied from interface: [TableHelper](TableHelper.md#isNodeOfType(ro.sync.ecss.extensions.api.node.AuthorElement,int))
Test if an [AuthorNode](../../../api/node/AuthorNode.md) is an element and it has one of the following types: [AuthorTableHelper.TYPE_CELL](../operations/AuthorTableHelper.md#TYPE_CELL), [AuthorTableHelper.TYPE_ROW](../operations/AuthorTableHelper.md#TYPE_ROW) or [AuthorTableHelper.TYPE_TABLE](../operations/AuthorTableHelper.md#TYPE_TABLE).
  Specified by: [isNodeOfType](TableHelper.md#isNodeOfType(ro.sync.ecss.extensions.api.node.AuthorElement,int)) in interface [TableHelper](TableHelper.md) Parameters: node - The node to be checked. type - The type to search for. Returns: true if the node is an element with the specified type. See Also:
        * [TableHelper.isNodeOfType(ro.sync.ecss.extensions.api.node.AuthorElement, int)](TableHelper.md#isNodeOfType(ro.sync.ecss.extensions.api.node.AuthorElement,int))

### allowsFooter

public boolean allowsFooter()
 Description copied from interface: [TablePropertiesHelper](TablePropertiesHelper.md#allowsFooter())
true if the current table allows footer element.
  Specified by: [allowsFooter](TablePropertiesHelper.md#allowsFooter()) in interface [TablePropertiesHelper](TablePropertiesHelper.md) Returns: true if the table allows footer. See Also:
        * [TablePropertiesHelper.allowsFooter()](TablePropertiesHelper.md#allowsFooter())

### getFirstChildOfTypeFromParentWithType

public [AuthorElement](../../../api/node/AuthorElement.md) getFirstChildOfTypeFromParentWithType([AuthorElement](../../../api/node/AuthorElement.md) currentRow, int childType, int parentType)
 Description copied from interface: [TablePropertiesHelper](TablePropertiesHelper.md#getFirstChildOfTypeFromParentWithType(ro.sync.ecss.extensions.api.node.AuthorElement,int,int))
Obtain the first row child of the parent which has the given type. The type could be one of TYPE_HEADED, TYPE_BODY, TYPE_FOOTER.
  Specified by: [getFirstChildOfTypeFromParentWithType](TablePropertiesHelper.md#getFirstChildOfTypeFromParentWithType(ro.sync.ecss.extensions.api.node.AuthorElement,int,int)) in interface [TablePropertiesHelper](TablePropertiesHelper.md) Parameters: currentRow - The current row element. childType - The type of the child that is needed. parentType - The type for the parent which will contain the returned row element. Returns: The first row from the parent or null if a parent with the given type is not found or if it does not contain any rows. See Also:
        * [TablePropertiesHelper.isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement)](TablePropertiesHelper.md#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement))

### getElementType

public int getElementType([AuthorElement](../../../api/node/AuthorElement.md) node)
 Description copied from interface: [TablePropertiesHelper](TablePropertiesHelper.md#getElementType(ro.sync.ecss.extensions.api.node.AuthorElement))
Obtain the type of the given node. Type can be one of [TableHelperConstants.TYPE_TABLE](TableHelperConstants.md#TYPE_TABLE), [TableHelperConstants.TYPE_GROUP](TableHelperConstants.md#TYPE_GROUP), [TableHelperConstants.TYPE_HEADER](TableHelperConstants.md#TYPE_HEADER), [TableHelperConstants.TYPE_BODY](TableHelperConstants.md#TYPE_BODY), [TableHelperConstants.TYPE_FOOTER](TableHelperConstants.md#TYPE_FOOTER), [TableHelperConstants.TYPE_ROW](TableHelperConstants.md#TYPE_ROW), [TableHelperConstants.TYPE_CELL](TableHelperConstants.md#TYPE_CELL), [TableHelperConstants.TYPE_COLSPEC](TableHelperConstants.md#TYPE_COLSPEC).
  Specified by: [getElementType](TablePropertiesHelper.md#getElementType(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [TablePropertiesHelper](TablePropertiesHelper.md) Parameters: node - The node to compute type for. Returns: The type of the given node or -1 if the node is not a table node. See Also:
        * [TablePropertiesHelper.getElementType(ro.sync.ecss.extensions.api.node.AuthorElement)](TablePropertiesHelper.md#getElementType(ro.sync.ecss.extensions.api.node.AuthorElement))

### getElementTag

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getElementTag(int elementType)
 Description copied from interface: [TablePropertiesHelper](TablePropertiesHelper.md#getElementTag(int))
Obtain the element name.
  Specified by: [getElementTag](TablePropertiesHelper.md#getElementTag(int)) in interface [TablePropertiesHelper](TablePropertiesHelper.md) Parameters: elementType - The type of the element. Returns: the element tag. See Also:
        * [TablePropertiesHelper.getElementTag(int)](TablePropertiesHelper.md#getElementTag(int))

### getElementName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getElementName(int elementType)
  Specified by: [getElementName](TablePropertiesHelper.md#getElementName(int)) in interface [TablePropertiesHelper](TablePropertiesHelper.md) Parameters: elementType - The element type. Returns: The element name. See Also:
        * [TablePropertiesHelper.getElementName(int)](TablePropertiesHelper.md#getElementName(int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
