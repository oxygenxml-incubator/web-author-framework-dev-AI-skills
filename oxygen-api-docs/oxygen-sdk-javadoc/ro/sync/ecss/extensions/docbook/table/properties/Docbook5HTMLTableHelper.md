Package [ro.sync.ecss.extensions.docbook.table.properties](package-summary.md)

# Class Docbook5HTMLTableHelper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.properties.TablePropertiesHelperBase](../../../commons/table/properties/TablePropertiesHelperBase.md)
        * [ro.sync.ecss.extensions.docbook.table.properties.DocbookCALSTableHelper](DocbookCALSTableHelper.md)
            * [ro.sync.ecss.extensions.docbook.table.properties.DocbookHTMLTableHelper](DocbookHTMLTableHelper.md)
                * ro.sync.ecss.extensions.docbook.table.properties.Docbook5HTMLTableHelper
   All Implemented Interfaces: [TableHelper](../../../commons/table/properties/TableHelper.md), [TableHelperConstants](../../../commons/table/properties/TableHelperConstants.md), [TablePropertiesConstants](../../../commons/table/properties/TablePropertiesConstants.md), [TablePropertiesHelper](../../../commons/table/properties/TablePropertiesHelper.md)   @API(type=INTERNAL, src=PUBLIC) public class Docbook5HTMLTableHelper extends [DocbookHTMLTableHelper](DocbookHTMLTableHelper.md)
Docbook CALS table helper.

## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.commons.table.properties.[TableHelperConstants](../../../commons/table/properties/TableHelperConstants.md)
 [TYPE_BODY](../../../commons/table/properties/TableHelperConstants.md#TYPE_BODY), [TYPE_BODY_DESC_CELL](../../../commons/table/properties/TableHelperConstants.md#TYPE_BODY_DESC_CELL), [TYPE_CELL](../../../commons/table/properties/TableHelperConstants.md#TYPE_CELL), [TYPE_COLSPEC](../../../commons/table/properties/TableHelperConstants.md#TYPE_COLSPEC), [TYPE_FOOTER](../../../commons/table/properties/TableHelperConstants.md#TYPE_FOOTER), [TYPE_GROUP](../../../commons/table/properties/TableHelperConstants.md#TYPE_GROUP), [TYPE_HEADER](../../../commons/table/properties/TableHelperConstants.md#TYPE_HEADER), [TYPE_HEADER_CELL](../../../commons/table/properties/TableHelperConstants.md#TYPE_HEADER_CELL), [TYPE_HEADER_DESC_CELL](../../../commons/table/properties/TableHelperConstants.md#TYPE_HEADER_DESC_CELL), [TYPE_ROW](../../../commons/table/properties/TableHelperConstants.md#TYPE_ROW), [TYPE_TABLE](../../../commons/table/properties/TableHelperConstants.md#TYPE_TABLE)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesConstants](../../../commons/table/properties/TablePropertiesConstants.md)
 [ALIGN](../../../commons/table/properties/TablePropertiesConstants.md#ALIGN), [ATTR_NOT_SET](../../../commons/table/properties/TablePropertiesConstants.md#ATTR_NOT_SET), [BOTTOM](../../../commons/table/properties/TablePropertiesConstants.md#BOTTOM), [CENTER](../../../commons/table/properties/TablePropertiesConstants.md#CENTER), [CHAR](../../../commons/table/properties/TablePropertiesConstants.md#CHAR), [COLSEP](../../../commons/table/properties/TablePropertiesConstants.md#COLSEP), [EMPTY_ICON](../../../commons/table/properties/TablePropertiesConstants.md#EMPTY_ICON), [FRAME](../../../commons/table/properties/TablePropertiesConstants.md#FRAME), [ICON_ALIGN_CENTER](../../../commons/table/properties/TablePropertiesConstants.md#ICON_ALIGN_CENTER), [ICON_ALIGN_JUSTIFY](../../../commons/table/properties/TablePropertiesConstants.md#ICON_ALIGN_JUSTIFY), [ICON_ALIGN_LEFT](../../../commons/table/properties/TablePropertiesConstants.md#ICON_ALIGN_LEFT), [ICON_ALIGN_RIGHT](../../../commons/table/properties/TablePropertiesConstants.md#ICON_ALIGN_RIGHT), [ICON_COL_ROW_SEP](../../../commons/table/properties/TablePropertiesConstants.md#ICON_COL_ROW_SEP), [ICON_COLSEP](../../../commons/table/properties/TablePropertiesConstants.md#ICON_COLSEP), [ICON_FRAME_ALL](../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_ALL), [ICON_FRAME_BOTTOM](../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_BOTTOM), [ICON_FRAME_LHS](../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_LHS), [ICON_FRAME_RHS](../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_RHS), [ICON_FRAME_SIDES](../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_SIDES), [ICON_FRAME_TOP](../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_TOP), [ICON_FRAME_TOPBOT](../../../commons/table/properties/TablePropertiesConstants.md#ICON_FRAME_TOPBOT), [ICON_ROW_TYPE_BODY](../../../commons/table/properties/TablePropertiesConstants.md#ICON_ROW_TYPE_BODY), [ICON_ROW_TYPE_FOOTER](../../../commons/table/properties/TablePropertiesConstants.md#ICON_ROW_TYPE_FOOTER), [ICON_ROW_TYPE_HEADER](../../../commons/table/properties/TablePropertiesConstants.md#ICON_ROW_TYPE_HEADER), [ICON_ROWSEP](../../../commons/table/properties/TablePropertiesConstants.md#ICON_ROWSEP), [ICON_VALIGN_BOTTOM](../../../commons/table/properties/TablePropertiesConstants.md#ICON_VALIGN_BOTTOM), [ICON_VALIGN_MIDDLE](../../../commons/table/properties/TablePropertiesConstants.md#ICON_VALIGN_MIDDLE), [ICON_VALIGN_TOP](../../../commons/table/properties/TablePropertiesConstants.md#ICON_VALIGN_TOP), [JUSTIFY](../../../commons/table/properties/TablePropertiesConstants.md#JUSTIFY), [LEFT](../../../commons/table/properties/TablePropertiesConstants.md#LEFT), [MIDDLE](../../../commons/table/properties/TablePropertiesConstants.md#MIDDLE), [NOT_COMPUTED](../../../commons/table/properties/TablePropertiesConstants.md#NOT_COMPUTED), [PRESERVE](../../../commons/table/properties/TablePropertiesConstants.md#PRESERVE), [RIGHT](../../../commons/table/properties/TablePropertiesConstants.md#RIGHT), [ROW_TYPE](../../../commons/table/properties/TablePropertiesConstants.md#ROW_TYPE), [ROW_TYPE_BODY](../../../commons/table/properties/TablePropertiesConstants.md#ROW_TYPE_BODY), [ROW_TYPE_FOOTER](../../../commons/table/properties/TablePropertiesConstants.md#ROW_TYPE_FOOTER), [ROW_TYPE_HEADER](../../../commons/table/properties/TablePropertiesConstants.md#ROW_TYPE_HEADER), [ROW_TYPE_PROPERTY](../../../commons/table/properties/TablePropertiesConstants.md#ROW_TYPE_PROPERTY), [ROWSEP](../../../commons/table/properties/TablePropertiesConstants.md#ROWSEP), [TITLE_ELEMENT](../../../commons/table/properties/TablePropertiesConstants.md#TITLE_ELEMENT), [TOP](../../../commons/table/properties/TablePropertiesConstants.md#TOP), [VALIGN](../../../commons/table/properties/TablePropertiesConstants.md#VALIGN)
## Constructor Summary
 Constructors
Constructor

Description
 [Docbook5HTMLTableHelper](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getElementTag](#getElementTag(int))(int elementType)
Obtain the element name.

### Methods inherited from class ro.sync.ecss.extensions.docbook.table.properties.[DocbookHTMLTableHelper](DocbookHTMLTableHelper.md)
 [getElementName](DocbookHTMLTableHelper.md#getElementName(int)), [isTable](DocbookHTMLTableHelper.md#isTable(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableCell](DocbookHTMLTableHelper.md#isTableCell(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableColspec](DocbookHTMLTableHelper.md#isTableColspec(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableFoot](DocbookHTMLTableHelper.md#isTableFoot(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableGroup](DocbookHTMLTableHelper.md#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableRow](DocbookHTMLTableHelper.md#isTableRow(ro.sync.ecss.extensions.api.node.AuthorElement))
### Methods inherited from class ro.sync.ecss.extensions.docbook.table.properties.[DocbookCALSTableHelper](DocbookCALSTableHelper.md)
 [allowsFooter](DocbookCALSTableHelper.md#allowsFooter()), [isTableBody](DocbookCALSTableHelper.md#isTableBody(ro.sync.ecss.extensions.api.node.AuthorElement)), [isTableHead](DocbookCALSTableHelper.md#isTableHead(ro.sync.ecss.extensions.api.node.AuthorElement))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesHelperBase](../../../commons/table/properties/TablePropertiesHelperBase.md)
 [getElementType](../../../commons/table/properties/TablePropertiesHelperBase.md#getElementType(ro.sync.ecss.extensions.api.node.AuthorElement)), [getFirstChildOfTypeFromParentWithType](../../../commons/table/properties/TablePropertiesHelperBase.md#getFirstChildOfTypeFromParentWithType(ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [isNodeOfType](../../../commons/table/properties/TablePropertiesHelperBase.md#isNodeOfType(ro.sync.ecss.extensions.api.node.AuthorElement,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### Docbook5HTMLTableHelper

public Docbook5HTMLTableHelper()

## Method Details

### getElementTag

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getElementTag(int elementType)
 Description copied from interface: [TablePropertiesHelper](../../../commons/table/properties/TablePropertiesHelper.md#getElementTag(int))
Obtain the element name.
  Specified by: [getElementTag](../../../commons/table/properties/TablePropertiesHelper.md#getElementTag(int)) in interface [TablePropertiesHelper](../../../commons/table/properties/TablePropertiesHelper.md) Overrides: [getElementTag](DocbookHTMLTableHelper.md#getElementTag(int)) in class [DocbookHTMLTableHelper](DocbookHTMLTableHelper.md) Parameters: elementType - The type of the element. Returns: the element tag. See Also:
        * [TablePropertiesHelperBase.getElementTag(int)](../../../commons/table/properties/TablePropertiesHelperBase.md#getElementTag(int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
