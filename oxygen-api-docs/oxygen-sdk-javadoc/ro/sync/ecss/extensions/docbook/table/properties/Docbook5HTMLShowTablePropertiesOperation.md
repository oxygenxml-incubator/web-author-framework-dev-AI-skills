Package [ro.sync.ecss.extensions.docbook.table.properties](package-summary.md)

# Class Docbook5HTMLShowTablePropertiesOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.properties.ShowTablePropertiesBaseOperation](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md)
        * [ro.sync.ecss.extensions.commons.table.properties.CALSAndHTMLShowTablePropertiesBase](../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md)
            * [ro.sync.ecss.extensions.docbook.table.properties.DocbookHTMLShowTablePropertiesOperationBase](DocbookHTMLShowTablePropertiesOperationBase.md)
                * ro.sync.ecss.extensions.docbook.table.properties.Docbook5HTMLShowTablePropertiesOperation
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class Docbook5HTMLShowTablePropertiesOperation extends [DocbookHTMLShowTablePropertiesOperationBase](DocbookHTMLShowTablePropertiesOperationBase.md)
Class for edit properties on DB4 CALS tables.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.docbook.table.properties.[DocbookHTMLShowTablePropertiesOperationBase](DocbookHTMLShowTablePropertiesOperationBase.md)
 [BASELINE](DocbookHTMLShowTablePropertiesOperationBase.md#BASELINE), [TABLE_FRAME_VALUES](DocbookHTMLShowTablePropertiesOperationBase.md#TABLE_FRAME_VALUES)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.properties.[CALSAndHTMLShowTablePropertiesBase](../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md)
 [HORIZONTAL_ALIGN_VALUES](../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#HORIZONTAL_ALIGN_VALUES), [VERTICAL_ALIGN_VALUES](../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#VERTICAL_ALIGN_VALUES)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md)
 [authorAccess](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#authorAccess), [tableHelper](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [Docbook5HTMLShowTablePropertiesOperation](#%3Cinit%3E())()
Constructor.

## Method Summary

### Methods inherited from class ro.sync.ecss.extensions.docbook.table.properties.[DocbookHTMLShowTablePropertiesOperationBase](DocbookHTMLShowTablePropertiesOperationBase.md)
 [getCellIndexes](DocbookHTMLShowTablePropertiesOperationBase.md#getCellIndexes(java.util.List)), [getCellsAttributes](DocbookHTMLShowTablePropertiesOperationBase.md#getCellsAttributes()), [getColSpecs](DocbookHTMLShowTablePropertiesOperationBase.md#getColSpecs(java.util.Map)), [getColumnsAttributes](DocbookHTMLShowTablePropertiesOperationBase.md#getColumnsAttributes()), [getHelpPageID](DocbookHTMLShowTablePropertiesOperationBase.md#getHelpPageID()), [getRowsAttributesToEdit](DocbookHTMLShowTablePropertiesOperationBase.md#getRowsAttributesToEdit()), [getTableAttribute](DocbookHTMLShowTablePropertiesOperationBase.md#getTableAttribute()), [processFragment](DocbookHTMLShowTablePropertiesOperationBase.md#processFragment(ro.sync.ecss.extensions.api.node.AuthorElement,java.util.List,boolean))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.properties.[CALSAndHTMLShowTablePropertiesBase](../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md)
 [computeFragmentMoveInsideHeader](../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#computeFragmentMoveInsideHeader(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [computeFragmentsToMoveInsideBody](../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [computeFragmentsToMoveInsideFooter](../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#computeFragmentsToMoveInsideFooter(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [getCategoriesAndProperties](../../../commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md#getCategoriesAndProperties(java.util.List))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md)
 [checkRowSpans](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#checkRowSpans(java.util.List,int)), [doOperation](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getArguments()), [getAttrProperty](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getAttrProperty(java.util.List,java.lang.String,ro.sync.ecss.extensions.commons.table.properties.TableProperty)), [getCommonValue](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getCommonValue(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String)), [getDescription](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getDescription()), [getElementsWithModifiedAttributes](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getElementsWithModifiedAttributes(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo)), [getFragmentsAndOffsetsToInsert](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getFragmentsAndOffsetsToInsert(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo)), [getSelectedTab](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getSelectedTab(java.util.List)), [getTableInformation](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getTableInformation(java.util.List)), [showTableProperties](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#showTableProperties(ro.sync.ecss.extensions.api.ArgumentsMap))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### Docbook5HTMLShowTablePropertiesOperation

public Docbook5HTMLShowTablePropertiesOperation()

Constructor.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
