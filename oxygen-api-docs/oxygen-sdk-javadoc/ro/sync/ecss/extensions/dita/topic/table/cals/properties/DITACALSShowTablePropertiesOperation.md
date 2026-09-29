Package [ro.sync.ecss.extensions.dita.topic.table.cals.properties](package-summary.md)

# Class DITACALSShowTablePropertiesOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.properties.ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md)
        * [ro.sync.ecss.extensions.commons.table.properties.CALSAndHTMLShowTablePropertiesBase](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md)
            * [ro.sync.ecss.extensions.commons.table.properties.CALSShowTableProperties](../../../../../commons/table/properties/CALSShowTableProperties.md)
                * ro.sync.ecss.extensions.dita.topic.table.cals.properties.DITACALSShowTablePropertiesOperation
   All Implemented Interfaces: [AuthorOperation](../../../../../api/AuthorOperation.md), [Extension](../../../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DITACALSShowTablePropertiesOperation extends [CALSShowTableProperties](../../../../../commons/table/properties/CALSShowTableProperties.md)
Class for dita CALS table properties action.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAME_DITA_CONREF](#FRAME_DITA_CONREF)
DITA specific frame value.

### Fields inherited from class ro.sync.ecss.extensions.commons.table.properties.[CALSAndHTMLShowTablePropertiesBase](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md)
 [HORIZONTAL_ALIGN_VALUES](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#HORIZONTAL_ALIGN_VALUES), [VERTICAL_ALIGN_VALUES](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#VERTICAL_ALIGN_VALUES)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md)
 [authorAccess](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#authorAccess), [tableHelper](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [DITACALSShowTablePropertiesOperation](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](../../../../../commons/table/properties/TableProperty.md)> [getCellsAttributes](#getCellsAttributes())()
Obtain the value for the given attribute set on the given element.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](../../../../../commons/table/properties/TableProperty.md)> [getColumnsAttributes](#getColumnsAttributes())()
Obtain the value for the given attribute set on the given element.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID())()
Get the ID of the help page which will be called by the end user.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](../../../../../commons/table/properties/TableProperty.md)> [getRowsAttributesToEdit](#getRowsAttributesToEdit())()
Obtain the attributes qualified name and render string (for rows).
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](../../../../../commons/table/properties/TableProperty.md)> [getTableAttribute](#getTableAttribute())()
Obtain the table attributes.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.properties.[CALSShowTableProperties](../../../../../commons/table/properties/CALSShowTableProperties.md)
 [getCellIndexes](../../../../../commons/table/properties/CALSShowTableProperties.md#getCellIndexes(java.util.List)), [getColSpecs](../../../../../commons/table/properties/CALSShowTableProperties.md#getColSpecs(java.util.Map)), [getElementsWithModifiedAttributes](../../../../../commons/table/properties/CALSShowTableProperties.md#getElementsWithModifiedAttributes(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.properties.[CALSAndHTMLShowTablePropertiesBase](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md)
 [computeFragmentMoveInsideHeader](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#computeFragmentMoveInsideHeader(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [computeFragmentsToMoveInsideBody](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [computeFragmentsToMoveInsideFooter](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#computeFragmentsToMoveInsideFooter(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [getCategoriesAndProperties](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#getCategoriesAndProperties(java.util.List)), [processFragment](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#processFragment(ro.sync.ecss.extensions.api.node.AuthorElement,java.util.List,boolean))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md)
 [checkRowSpans](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#checkRowSpans(java.util.List,int)), [doOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getArguments()), [getAttrProperty](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getAttrProperty(java.util.List,java.lang.String,ro.sync.ecss.extensions.commons.table.properties.TableProperty)), [getCommonValue](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getCommonValue(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String)), [getDescription](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getDescription()), [getFragmentsAndOffsetsToInsert](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getFragmentsAndOffsetsToInsert(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo)), [getSelectedTab](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getSelectedTab(java.util.List)), [getTableInformation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getTableInformation(java.util.List)), [showTableProperties](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#showTableProperties(ro.sync.ecss.extensions.api.ArgumentsMap))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### FRAME_DITA_CONREF

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAME_DITA_CONREF

DITA specific frame value.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.ecss.extensions.dita.topic.table.cals.properties.DITACALSShowTablePropertiesOperation.FRAME_DITA_CONREF)

## Constructor Details

### DITACALSShowTablePropertiesOperation

public DITACALSShowTablePropertiesOperation()

Constructor.

## Method Details

### getTableAttribute

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](../../../../../commons/table/properties/TableProperty.md)> getTableAttribute()
 Description copied from class: [ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getTableAttribute())
Obtain the table attributes.
  Specified by: [getTableAttribute](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getTableAttribute()) in class [ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md) Returns: A list with [TableProperty](../../../../../commons/table/properties/TableProperty.md) objects containing the table attributes qualified name, render string and possible values. See Also:
        * [ShowTablePropertiesBaseOperation.getTableAttribute()](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getTableAttribute())

### getRowsAttributesToEdit

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](../../../../../commons/table/properties/TableProperty.md)> getRowsAttributesToEdit()
 Description copied from class: [CALSAndHTMLShowTablePropertiesBase](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#getRowsAttributesToEdit())
Obtain the attributes qualified name and render string (for rows).
  Overrides: [getRowsAttributesToEdit](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#getRowsAttributesToEdit()) in class [CALSAndHTMLShowTablePropertiesBase](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md) Returns: A list with attributes to edit. See Also:
        * [CALSAndHTMLShowTablePropertiesBase.getRowsAttributesToEdit()](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#getRowsAttributesToEdit())

### getCellsAttributes

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](../../../../../commons/table/properties/TableProperty.md)> getCellsAttributes()
 Description copied from class: [CALSAndHTMLShowTablePropertiesBase](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#getCellsAttributes())
Obtain the value for the given attribute set on the given element.
  Overrides: [getCellsAttributes](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#getCellsAttributes()) in class [CALSAndHTMLShowTablePropertiesBase](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md) Returns: A list with allowed attributes. See Also:
        * [CALSAndHTMLShowTablePropertiesBase.getCellsAttributes()](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#getCellsAttributes())

### getColumnsAttributes

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](../../../../../commons/table/properties/TableProperty.md)> getColumnsAttributes()
 Description copied from class: [CALSAndHTMLShowTablePropertiesBase](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#getColumnsAttributes())
Obtain the value for the given attribute set on the given element.
  Overrides: [getColumnsAttributes](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#getColumnsAttributes()) in class [CALSAndHTMLShowTablePropertiesBase](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md) Returns: A list with allowed attributes. See Also:
        * [CALSAndHTMLShowTablePropertiesBase.getColumnsAttributes()](../../../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#getColumnsAttributes())

### getHelpPageID

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID()
 Description copied from class: [ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getHelpPageID())
Get the ID of the help page which will be called by the end user.
  Overrides: [getHelpPageID](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getHelpPageID()) in class [ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md) Returns: the ID of the help page which will be called by the end user or null. See Also:
        * [ShowTablePropertiesBaseOperation.getHelpPageID()](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getHelpPageID())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
