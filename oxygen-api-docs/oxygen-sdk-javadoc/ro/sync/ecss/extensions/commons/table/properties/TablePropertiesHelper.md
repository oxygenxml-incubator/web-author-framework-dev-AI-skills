Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Interface TablePropertiesHelper
    All Superinterfaces: [TableHelper](TableHelper.md), [TableHelperConstants](TableHelperConstants.md), [TablePropertiesConstants](TablePropertiesConstants.md)   All Known Implementing Classes: [ChoiceTableHelper](../../../dita/topic/table/simpletable/properties/ChoiceTableHelper.md), [DITACALSTableHelper](../../../dita/topic/table/cals/properties/DITACALSTableHelper.md), [Docbook5CALSTableHelper](../../../docbook/table/properties/Docbook5CALSTableHelper.md), [Docbook5HTMLTableHelper](../../../docbook/table/properties/Docbook5HTMLTableHelper.md), [DocbookCALSTableHelper](../../../docbook/table/properties/DocbookCALSTableHelper.md), [DocbookHTMLTableHelper](../../../docbook/table/properties/DocbookHTMLTableHelper.md), [RelTablePropertiesHelper](../../../dita/map/table/RelTablePropertiesHelper.md), [SimpleTableHelper](../../../dita/topic/table/simpletable/properties/SimpleTableHelper.md), [TablePropertiesHelperBase](TablePropertiesHelperBase.md)   @API(type=INTERNAL, src=PUBLIC) public interface TablePropertiesHelperextends [TableHelper](TableHelper.md), [TablePropertiesConstants](TablePropertiesConstants.md)
Table helper for 'Table Properties' dialog.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.commons.table.properties.[TableHelperConstants](TableHelperConstants.md)
 [TYPE_BODY](TableHelperConstants.md#TYPE_BODY), [TYPE_BODY_DESC_CELL](TableHelperConstants.md#TYPE_BODY_DESC_CELL), [TYPE_CELL](TableHelperConstants.md#TYPE_CELL), [TYPE_COLSPEC](TableHelperConstants.md#TYPE_COLSPEC), [TYPE_FOOTER](TableHelperConstants.md#TYPE_FOOTER), [TYPE_GROUP](TableHelperConstants.md#TYPE_GROUP), [TYPE_HEADER](TableHelperConstants.md#TYPE_HEADER), [TYPE_HEADER_CELL](TableHelperConstants.md#TYPE_HEADER_CELL), [TYPE_HEADER_DESC_CELL](TableHelperConstants.md#TYPE_HEADER_DESC_CELL), [TYPE_ROW](TableHelperConstants.md#TYPE_ROW), [TYPE_TABLE](TableHelperConstants.md#TYPE_TABLE)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesConstants](TablePropertiesConstants.md)
 [ALIGN](TablePropertiesConstants.md#ALIGN), [ATTR_NOT_SET](TablePropertiesConstants.md#ATTR_NOT_SET), [BOTTOM](TablePropertiesConstants.md#BOTTOM), [CENTER](TablePropertiesConstants.md#CENTER), [CHAR](TablePropertiesConstants.md#CHAR), [COLSEP](TablePropertiesConstants.md#COLSEP), [EMPTY_ICON](TablePropertiesConstants.md#EMPTY_ICON), [FRAME](TablePropertiesConstants.md#FRAME), [ICON_ALIGN_CENTER](TablePropertiesConstants.md#ICON_ALIGN_CENTER), [ICON_ALIGN_JUSTIFY](TablePropertiesConstants.md#ICON_ALIGN_JUSTIFY), [ICON_ALIGN_LEFT](TablePropertiesConstants.md#ICON_ALIGN_LEFT), [ICON_ALIGN_RIGHT](TablePropertiesConstants.md#ICON_ALIGN_RIGHT), [ICON_COL_ROW_SEP](TablePropertiesConstants.md#ICON_COL_ROW_SEP), [ICON_COLSEP](TablePropertiesConstants.md#ICON_COLSEP), [ICON_FRAME_ALL](TablePropertiesConstants.md#ICON_FRAME_ALL), [ICON_FRAME_BOTTOM](TablePropertiesConstants.md#ICON_FRAME_BOTTOM), [ICON_FRAME_LHS](TablePropertiesConstants.md#ICON_FRAME_LHS), [ICON_FRAME_RHS](TablePropertiesConstants.md#ICON_FRAME_RHS), [ICON_FRAME_SIDES](TablePropertiesConstants.md#ICON_FRAME_SIDES), [ICON_FRAME_TOP](TablePropertiesConstants.md#ICON_FRAME_TOP), [ICON_FRAME_TOPBOT](TablePropertiesConstants.md#ICON_FRAME_TOPBOT), [ICON_ROW_TYPE_BODY](TablePropertiesConstants.md#ICON_ROW_TYPE_BODY), [ICON_ROW_TYPE_FOOTER](TablePropertiesConstants.md#ICON_ROW_TYPE_FOOTER), [ICON_ROW_TYPE_HEADER](TablePropertiesConstants.md#ICON_ROW_TYPE_HEADER), [ICON_ROWSEP](TablePropertiesConstants.md#ICON_ROWSEP), [ICON_VALIGN_BOTTOM](TablePropertiesConstants.md#ICON_VALIGN_BOTTOM), [ICON_VALIGN_MIDDLE](TablePropertiesConstants.md#ICON_VALIGN_MIDDLE), [ICON_VALIGN_TOP](TablePropertiesConstants.md#ICON_VALIGN_TOP), [JUSTIFY](TablePropertiesConstants.md#JUSTIFY), [LEFT](TablePropertiesConstants.md#LEFT), [MIDDLE](TablePropertiesConstants.md#MIDDLE), [NOT_COMPUTED](TablePropertiesConstants.md#NOT_COMPUTED), [PRESERVE](TablePropertiesConstants.md#PRESERVE), [RIGHT](TablePropertiesConstants.md#RIGHT), [ROW_TYPE](TablePropertiesConstants.md#ROW_TYPE), [ROW_TYPE_BODY](TablePropertiesConstants.md#ROW_TYPE_BODY), [ROW_TYPE_FOOTER](TablePropertiesConstants.md#ROW_TYPE_FOOTER), [ROW_TYPE_HEADER](TablePropertiesConstants.md#ROW_TYPE_HEADER), [ROW_TYPE_PROPERTY](TablePropertiesConstants.md#ROW_TYPE_PROPERTY), [ROWSEP](TablePropertiesConstants.md#ROWSEP), [TITLE_ELEMENT](TablePropertiesConstants.md#TITLE_ELEMENT), [TOP](TablePropertiesConstants.md#TOP), [VALIGN](TablePropertiesConstants.md#VALIGN)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
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
  boolean [isTableBody](#isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table body element.
  boolean [isTableCell](#isTableCell(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table cell element.
  boolean [isTableColspec](#isTableColspec(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table colspec element.
  boolean [isTableFoot](#isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table foot element.
  boolean [isTableHead](#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table head element.
  boolean [isTableRow](#isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table row element.

### Methods inherited from interface ro.sync.ecss.extensions.commons.table.properties.[TableHelper](TableHelper.md)
 [isNodeOfType](TableHelper.md#isNodeOfType(ro.sync.ecss.extensions.api.node.AuthorElement,int)), [isTable](TableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableGroup](TableHelper.md#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement))
## Method Details

### isTableBody

boolean isTableBody([AuthorElement](../../../api/node/AuthorElement.md) node)

Checks if the given node represents a table body element.
  Parameters: node - The node to be checked. Returns: true if the given node is a table body element.
### isTableHead

boolean isTableHead([AuthorElement](../../../api/node/AuthorElement.md) node)

Checks if the given node represents a table head element.
  Parameters: node - The node to be checked. Returns: true if the given node is a table head element.
### isTableFoot

boolean isTableFoot([AuthorElement](../../../api/node/AuthorElement.md) node)

Checks if the given node represents a table foot element.
  Parameters: node - The node to be checked. Returns: true if the given node is a table foot element.
### isTableRow

boolean isTableRow([AuthorElement](../../../api/node/AuthorElement.md) node)

Checks if the given node represents a table row element.
  Parameters: node - The node to be checked. Returns: true if the given node is a table row element.
### isTableCell

boolean isTableCell([AuthorElement](../../../api/node/AuthorElement.md) node)

Checks if the given node represents a table cell element.
  Parameters: node - The node to be checked. Returns: true if the given node is a table cell element.
### isTableColspec

boolean isTableColspec([AuthorElement](../../../api/node/AuthorElement.md) node)

Checks if the given node represents a table colspec element.
  Parameters: node - The node to be checked. Returns: true if the given node is a table colspec element.
### allowsFooter

boolean allowsFooter()

true if the current table allows footer element.
  Returns: true if the table allows footer.
### getFirstChildOfTypeFromParentWithType

[AuthorElement](../../../api/node/AuthorElement.md) getFirstChildOfTypeFromParentWithType([AuthorElement](../../../api/node/AuthorElement.md) currentRow, int childType, int parentType)

Obtain the first row child of the parent which has the given type. The type could be one of TYPE_HEADED, TYPE_BODY, TYPE_FOOTER.
  Parameters: currentRow - The current row element. childType - The type of the child that is needed. parentType - The type for the parent which will contain the returned row element. Returns: The first row from the parent or null if a parent with the given type is not found or if it does not contain any rows.
### getElementType

int getElementType([AuthorElement](../../../api/node/AuthorElement.md) node)

Obtain the type of the given node. Type can be one of [TableHelperConstants.TYPE_TABLE](TableHelperConstants.md#TYPE_TABLE), [TableHelperConstants.TYPE_GROUP](TableHelperConstants.md#TYPE_GROUP), [TableHelperConstants.TYPE_HEADER](TableHelperConstants.md#TYPE_HEADER), [TableHelperConstants.TYPE_BODY](TableHelperConstants.md#TYPE_BODY), [TableHelperConstants.TYPE_FOOTER](TableHelperConstants.md#TYPE_FOOTER), [TableHelperConstants.TYPE_ROW](TableHelperConstants.md#TYPE_ROW), [TableHelperConstants.TYPE_CELL](TableHelperConstants.md#TYPE_CELL), [TableHelperConstants.TYPE_COLSPEC](TableHelperConstants.md#TYPE_COLSPEC).
  Parameters: node - The node to compute type for. Returns: The type of the given node or -1 if the node is not a table node.
### getElementTag

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getElementTag(int elementType)

Obtain the element name.
  Parameters: elementType - The type of the element. Returns: the element tag.
### getElementName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getElementName(int elementType)
  Parameters: elementType - The element type. Returns: The element name.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
