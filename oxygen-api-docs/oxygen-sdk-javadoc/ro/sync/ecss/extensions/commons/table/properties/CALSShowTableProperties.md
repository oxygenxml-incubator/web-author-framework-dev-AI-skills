Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Class CALSShowTableProperties

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.properties.ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md)
        * [ro.sync.ecss.extensions.commons.table.properties.CALSAndHTMLShowTablePropertiesBase](CALSAndHTMLShowTablePropertiesBase.md)
            * ro.sync.ecss.extensions.commons.table.properties.CALSShowTableProperties
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   Direct Known Subclasses: [DITACALSShowTablePropertiesOperation](../../../dita/topic/table/cals/properties/DITACALSShowTablePropertiesOperation.md), [Docbook4CALSShowTablePropertiesOperation](../../../docbook/table/properties/Docbook4CALSShowTablePropertiesOperation.md), [Docbook5CALSShowTablePropertiesOperation](../../../docbook/table/properties/Docbook5CALSShowTablePropertiesOperation.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class CALSShowTableProperties extends [CALSAndHTMLShowTablePropertiesBase](CALSAndHTMLShowTablePropertiesBase.md)
## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.properties.[CALSAndHTMLShowTablePropertiesBase](CALSAndHTMLShowTablePropertiesBase.md)
 [HORIZONTAL_ALIGN_VALUES](CALSAndHTMLShowTablePropertiesBase.md#HORIZONTAL_ALIGN_VALUES), [VERTICAL_ALIGN_VALUES](CALSAndHTMLShowTablePropertiesBase.md#VERTICAL_ALIGN_VALUES)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md)
 [authorAccess](ShowTablePropertiesBaseOperation.md#authorAccess), [tableHelper](ShowTablePropertiesBaseOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [CALSShowTableProperties](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.properties.TablePropertiesHelper))([TablePropertiesHelper](TablePropertiesHelper.md) helper)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](../../../api/node/AuthorElement.md),[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)>> [getCellIndexes](#getCellIndexes(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> cells)
Obtain the indexes for selected cells.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> [getColSpecs](#getColSpecs(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](../../../api/node/AuthorElement.md),[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)>> map)
Obtain the colspecs elements for the given cells indexes.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> [getElementsWithModifiedAttributes](#getElementsWithModifiedAttributes(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo))([EditedTablePropertiesInfo](EditedTablePropertiesInfo.md) tableInfo)
Obtain all the elements with all the modified attributes.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.properties.[CALSAndHTMLShowTablePropertiesBase](CALSAndHTMLShowTablePropertiesBase.md)
 [computeFragmentMoveInsideHeader](CALSAndHTMLShowTablePropertiesBase.md#computeFragmentMoveInsideHeader(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [computeFragmentsToMoveInsideBody](CALSAndHTMLShowTablePropertiesBase.md#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [computeFragmentsToMoveInsideFooter](CALSAndHTMLShowTablePropertiesBase.md#computeFragmentsToMoveInsideFooter(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [getCategoriesAndProperties](CALSAndHTMLShowTablePropertiesBase.md#getCategoriesAndProperties(java.util.List)), [getCellsAttributes](CALSAndHTMLShowTablePropertiesBase.md#getCellsAttributes()), [getColumnsAttributes](CALSAndHTMLShowTablePropertiesBase.md#getColumnsAttributes()), [getRowsAttributesToEdit](CALSAndHTMLShowTablePropertiesBase.md#getRowsAttributesToEdit()), [processFragment](CALSAndHTMLShowTablePropertiesBase.md#processFragment(ro.sync.ecss.extensions.api.node.AuthorElement,java.util.List,boolean))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md)
 [checkRowSpans](ShowTablePropertiesBaseOperation.md#checkRowSpans(java.util.List,int)), [doOperation](ShowTablePropertiesBaseOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](ShowTablePropertiesBaseOperation.md#getArguments()), [getAttrProperty](ShowTablePropertiesBaseOperation.md#getAttrProperty(java.util.List,java.lang.String,ro.sync.ecss.extensions.commons.table.properties.TableProperty)), [getCommonValue](ShowTablePropertiesBaseOperation.md#getCommonValue(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String)), [getDescription](ShowTablePropertiesBaseOperation.md#getDescription()), [getFragmentsAndOffsetsToInsert](ShowTablePropertiesBaseOperation.md#getFragmentsAndOffsetsToInsert(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo)), [getHelpPageID](ShowTablePropertiesBaseOperation.md#getHelpPageID()), [getSelectedTab](ShowTablePropertiesBaseOperation.md#getSelectedTab(java.util.List)), [getTableAttribute](ShowTablePropertiesBaseOperation.md#getTableAttribute()), [getTableInformation](ShowTablePropertiesBaseOperation.md#getTableInformation(java.util.List)), [showTableProperties](ShowTablePropertiesBaseOperation.md#showTableProperties(ro.sync.ecss.extensions.api.ArgumentsMap))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CALSShowTableProperties

public CALSShowTableProperties([TablePropertiesHelper](TablePropertiesHelper.md) helper)

Constructor.
  Parameters: helper - The table properties.
## Method Details

### getElementsWithModifiedAttributes

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> getElementsWithModifiedAttributes([EditedTablePropertiesInfo](EditedTablePropertiesInfo.md) tableInfo)
 Description copied from class: [ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md#getElementsWithModifiedAttributes(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo))
Obtain all the elements with all the modified attributes.
  Overrides: [getElementsWithModifiedAttributes](ShowTablePropertiesBaseOperation.md#getElementsWithModifiedAttributes(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo)) in class [ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md) Parameters: tableInfo - The obtained table information from the table properties dialog. Returns: A map containing all the elements whose attributes will be modified and the corresponding attributes. See Also:
        * [ShowTablePropertiesBaseOperation.getElementsWithModifiedAttributes(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo)](ShowTablePropertiesBaseOperation.md#getElementsWithModifiedAttributes(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo))

### getColSpecs

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> getColSpecs([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](../../../api/node/AuthorElement.md),[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)>> map)
 Description copied from class: [CALSAndHTMLShowTablePropertiesBase](CALSAndHTMLShowTablePropertiesBase.md#getColSpecs(java.util.Map))
Obtain the colspecs elements for the given cells indexes.
  Specified by: [getColSpecs](CALSAndHTMLShowTablePropertiesBase.md#getColSpecs(java.util.Map)) in class [CALSAndHTMLShowTablePropertiesBase](CALSAndHTMLShowTablePropertiesBase.md) Parameters: map - A map containing the table elements and cells indexes. Returns: A list with the colspecs elements for the given cells indexes. See Also:
        * [CALSAndHTMLShowTablePropertiesBase.getColSpecs(Map)](CALSAndHTMLShowTablePropertiesBase.md#getColSpecs(java.util.Map))

### getCellIndexes

protected [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](../../../api/node/AuthorElement.md),[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)>> getCellIndexes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> cells)
 Description copied from class: [CALSAndHTMLShowTablePropertiesBase](CALSAndHTMLShowTablePropertiesBase.md#getCellIndexes(java.util.List))
Obtain the indexes for selected cells.
  Specified by: [getCellIndexes](CALSAndHTMLShowTablePropertiesBase.md#getCellIndexes(java.util.List)) in class [CALSAndHTMLShowTablePropertiesBase](CALSAndHTMLShowTablePropertiesBase.md) Parameters: cells - The selected cells. Returns: A map containing the cell indexes based on the parent tgroup. See Also:
        * [CALSAndHTMLShowTablePropertiesBase.getCellIndexes(java.util.List)](CALSAndHTMLShowTablePropertiesBase.md#getCellIndexes(java.util.List))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
