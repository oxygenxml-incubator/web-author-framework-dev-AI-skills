Package [ro.sync.ecss.extensions.dita.topic.table.simpletable.properties](package-summary.md)

# Class ChoiceTableHelper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.properties.TablePropertiesHelperBase](../../../../../commons/table/properties/TablePropertiesHelperBase.md)
        * [ro.sync.ecss.extensions.dita.topic.table.simpletable.properties.SimpleTableHelper](SimpleTableHelper.md)
            * ro.sync.ecss.extensions.dita.topic.table.simpletable.properties.ChoiceTableHelper
   All Implemented Interfaces: [TableHelper](../../../../../commons/table/properties/TableHelper.md), [TableHelperConstants](../../../../../commons/table/properties/TableHelperConstants.md), [TablePropertiesConstants](../../../../../commons/table/properties/TablePropertiesConstants.md), [TablePropertiesHelper](../../../../../commons/table/properties/TablePropertiesHelper.md)   @API(type=INTERNAL, src=PUBLIC) public class ChoiceTableHelper extends [SimpleTableHelper](SimpleTableHelper.md)
Helper class for edit properties on DITA Simple tables.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.commons.table.properties.[TableHelperConstants](../../../../../commons/table/properties/TableHelperConstants.md)
 [TYPE_BODY](../../../../../commons/table/properties/TableHelperConstants.md#TYPE_BODY), [TYPE_BODY_DESC_CELL](../../../../../commons/table/properties/TableHelperConstants.md#TYPE_BODY_DESC_CELL), [TYPE_CELL](../../../../../commons/table/properties/TableHelperConstants.md#TYPE_CELL), [TYPE_COLSPEC](../../../../../commons/table/properties/TableHelperConstants.md#TYPE_COLSPEC), [TYPE_FOOTER](../../../../../commons/table/properties/TableHelperConstants.md#TYPE_FOOTER), [TYPE_GROUP](../../../../../commons/table/properties/TableHelperConstants.md#TYPE_GROUP), [TYPE_HEADER](../../../../../commons/table/properties/TableHelperConstants.md#TYPE_HEADER), [TYPE_HEADER_CELL](../../../../../commons/table/properties/TableHelperConstants.md#TYPE_HEADER_CELL), [TYPE_HEADER_DESC_CELL](../../../../../commons/table/properties/TableHelperConstants.md#TYPE_HEADER_DESC_CELL), [TYPE_ROW](../../../../../commons/table/properties/TableHelperConstants.md#TYPE_ROW), [TYPE_TABLE](../../../../../commons/table/properties/TableHelperConstants.md#TYPE_TABLE)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesConstants](../../../../../commons/table/properties/TablePropertiesConstants.md)
 [ALIGN](../../../../../commons/table/properties/TablePropertiesConstants.md#ALIGN), [ATTR_NOT_SET](../../../../../commons/table/properties/TablePropertiesConstants.md#ATTR_NOT_SET), [BOTTOM](../../../../../commons/table/properties/TablePropertiesConstants.md#BOTTOM), [CENTER](../../../../../commons/table/properties/TablePropertiesConstants.md#CENTER), [CHAR](../../../../../commons/table/properties/TablePropertiesConstants.md#CHAR), [COLSEP](../../../../../commons/table/properties/TablePropertiesConstants.md#COLSEP), [EMPTY_ICON](../../../../../commons/table/properties/TablePropertiesConstants.md#EMPTY_ICON), [FRAME](../../../../../commons/table/properties/TablePropertiesConstants.md#FRAME), [ICON_ALIGN_CENTER](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_ALIGN_CENTER), [ICON_ALIGN_JUSTIFY](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_ALIGN_JUSTIFY), [ICON_ALIGN_LEFT](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_ALIGN_LEFT), [ICON_ALIGN_RIGHT](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_ALIGN_RIGHT), [ICON_COL_ROW_SEP](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_COL_ROW_SEP), [ICON_COLSEP](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_COLSEP), [ICON_FRAME_ALL](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_ALL), [ICON_FRAME_BOTTOM](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_BOTTOM), [ICON_FRAME_LHS](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_LHS), [ICON_FRAME_RHS](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_RHS), [ICON_FRAME_SIDES](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_SIDES), [ICON_FRAME_TOP](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_TOP), [ICON_FRAME_TOPBOT](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_TOPBOT), [ICON_ROW_TYPE_BODY](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_ROW_TYPE_BODY), [ICON_ROW_TYPE_FOOTER](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_ROW_TYPE_FOOTER), [ICON_ROW_TYPE_HEADER](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_ROW_TYPE_HEADER), [ICON_ROWSEP](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_ROWSEP), [ICON_VALIGN_BOTTOM](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_VALIGN_BOTTOM), [ICON_VALIGN_MIDDLE](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_VALIGN_MIDDLE), [ICON_VALIGN_TOP](../../../../../commons/table/properties/TablePropertiesConstants.md#ICON_VALIGN_TOP), [JUSTIFY](../../../../../commons/table/properties/TablePropertiesConstants.md#JUSTIFY), [LEFT](../../../../../commons/table/properties/TablePropertiesConstants.md#LEFT), [MIDDLE](../../../../../commons/table/properties/TablePropertiesConstants.md#MIDDLE), [NOT_COMPUTED](../../../../../commons/table/properties/TablePropertiesConstants.md#NOT_COMPUTED), [PRESERVE](../../../../../commons/table/properties/TablePropertiesConstants.md#PRESERVE), [RIGHT](../../../../../commons/table/properties/TablePropertiesConstants.md#RIGHT), [ROW_TYPE](../../../../../commons/table/properties/TablePropertiesConstants.md#ROW_TYPE), [ROW_TYPE_BODY](../../../../../commons/table/properties/TablePropertiesConstants.md#ROW_TYPE_BODY), [ROW_TYPE_FOOTER](../../../../../commons/table/properties/TablePropertiesConstants.md#ROW_TYPE_FOOTER), [ROW_TYPE_HEADER](../../../../../commons/table/properties/TablePropertiesConstants.md#ROW_TYPE_HEADER), [ROW_TYPE_PROPERTY](../../../../../commons/table/properties/TablePropertiesConstants.md#ROW_TYPE_PROPERTY), [ROWSEP](../../../../../commons/table/properties/TablePropertiesConstants.md#ROWSEP), [TITLE_ELEMENT](../../../../../commons/table/properties/TablePropertiesConstants.md#TITLE_ELEMENT), [TOP](../../../../../commons/table/properties/TablePropertiesConstants.md#TOP), [VALIGN](../../../../../commons/table/properties/TablePropertiesConstants.md#VALIGN)
## Constructor Summary
 Constructors
Constructor

Description
 [ChoiceTableHelper](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getElementName](#getElementName(int))(int elementType)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getElementTag](#getElementTag(int))(int elementType)
Obtain the element name.
  boolean [isTable](#isTable(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../../api/node/AuthorElement.md) node)
Checks if the given node represents the table element.

### Methods inherited from class ro.sync.ecss.extensions.dita.topic.table.simpletable.properties.[SimpleTableHelper](SimpleTableHelper.md)
 [isBodyRow](SimpleTableHelper.md#isBodyRow(ro.sync.ecss.extensions.api.node.AuthorElement)), [isHeaderRow](SimpleTableHelper.md#isHeaderRow(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableBody](SimpleTableHelper.md#isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableCell](SimpleTableHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableHead](SimpleTableHelper.md#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableRow](SimpleTableHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesHelperBase](../../../../../commons/table/properties/TablePropertiesHelperBase.md)
 [allowsFooter](../../../../../commons/table/properties/TablePropertiesHelperBase.md#allowsFooter()), [getElementType](../../../../../commons/table/properties/TablePropertiesHelperBase.md#getElementType(ro.sync.ecss.extensions.api.node.AuthorElement)), [getFirstChildOfTypeFromParentWithType](../../../../../commons/table/properties/TablePropertiesHelperBase.md#getFirstChildOfTypeFromParentWithType(ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [isNodeOfType](../../../../../commons/table/properties/TablePropertiesHelperBase.md#isNodeOfType(ro.sync.ecss.extensions.api.node.AuthorElement,int)), [isTableColspec](../../../../../commons/table/properties/TablePropertiesHelperBase.md#isTableColspec(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableFoot](../../../../../commons/table/properties/TablePropertiesHelperBase.md#isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableGroup](../../../../../commons/table/properties/TablePropertiesHelperBase.md#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ChoiceTableHelper

public ChoiceTableHelper()

## Method Details

### getElementTag

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getElementTag(int elementType)
 Description copied from interface: [TablePropertiesHelper](../../../../../commons/table/properties/TablePropertiesHelper.md#getElementTag(int))
Obtain the element name.
  Specified by: [getElementTag](../../../../../commons/table/properties/TablePropertiesHelper.md#getElementTag(int)) in interface [TablePropertiesHelper](../../../../../commons/table/properties/TablePropertiesHelper.md) Overrides: [getElementTag](SimpleTableHelper.md#getElementTag(int)) in class [SimpleTableHelper](SimpleTableHelper.md) Parameters: elementType - The type of the element. Returns: the element tag. See Also:
        * [TablePropertiesHelperBase.getElementTag(int)](../../../../../commons/table/properties/TablePropertiesHelperBase.md#getElementTag(int))

### getElementName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getElementName(int elementType)
  Specified by: [getElementName](../../../../../commons/table/properties/TablePropertiesHelper.md#getElementName(int)) in interface [TablePropertiesHelper](../../../../../commons/table/properties/TablePropertiesHelper.md) Overrides: [getElementName](../../../../../commons/table/properties/TablePropertiesHelperBase.md#getElementName(int)) in class [TablePropertiesHelperBase](../../../../../commons/table/properties/TablePropertiesHelperBase.md) Parameters: elementType - The element type. Returns: The element name. See Also:
        * [TablePropertiesHelperBase.getElementName(int)](../../../../../commons/table/properties/TablePropertiesHelperBase.md#getElementName(int))

### isTable

public boolean isTable([AuthorElement](../../../../../api/node/AuthorElement.md) node)
 Description copied from interface: [TableHelper](../../../../../commons/table/properties/TableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorElement))
Checks if the given node represents the table element.
  Specified by: [isTable](../../../../../commons/table/properties/TableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [TableHelper](../../../../../commons/table/properties/TableHelper.md) Overrides: [isTable](SimpleTableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [SimpleTableHelper](SimpleTableHelper.md) Parameters: node - The node to be checked. Returns: true if the given node is the table element. See Also:
        * [SimpleTableHelper.isTable(ro.sync.ecss.extensions.api.node.AuthorElement)](SimpleTableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorElement))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
