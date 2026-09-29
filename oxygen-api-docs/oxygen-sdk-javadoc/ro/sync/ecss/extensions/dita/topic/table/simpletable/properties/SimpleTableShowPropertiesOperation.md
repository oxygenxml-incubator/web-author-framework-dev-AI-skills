Package [ro.sync.ecss.extensions.dita.topic.table.simpletable.properties](package-summary.md)

# Class SimpleTableShowPropertiesOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.properties.ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md)
        * [ro.sync.ecss.extensions.dita.topic.table.simpletable.properties.SimpleTableShowPropertiesOperationBase](SimpleTableShowPropertiesOperationBase.md)
            * ro.sync.ecss.extensions.dita.topic.table.simpletable.properties.SimpleTableShowPropertiesOperation
   All Implemented Interfaces: [AuthorOperation](../../../../../api/AuthorOperation.md), [Extension](../../../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class SimpleTableShowPropertiesOperation extends [SimpleTableShowPropertiesOperationBase](SimpleTableShowPropertiesOperationBase.md)
Class for edit properties on DITA CALS tables.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md)
 [authorAccess](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#authorAccess), [tableHelper](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [SimpleTableShowPropertiesOperation](#%3Cinit%3E())()
Constructor.

## Method Summary

### Methods inherited from class ro.sync.ecss.extensions.dita.topic.table.simpletable.properties.[SimpleTableShowPropertiesOperationBase](SimpleTableShowPropertiesOperationBase.md)
 [computeFragmentMoveInsideHeader](SimpleTableShowPropertiesOperationBase.md#computeFragmentMoveInsideHeader(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [computeFragmentsToMoveInsideBody](SimpleTableShowPropertiesOperationBase.md#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [computeFragmentsToMoveInsideFooter](SimpleTableShowPropertiesOperationBase.md#computeFragmentsToMoveInsideFooter(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [getCategoriesAndProperties](SimpleTableShowPropertiesOperationBase.md#getCategoriesAndProperties(java.util.List)), [getHelpPageID](SimpleTableShowPropertiesOperationBase.md#getHelpPageID()), [getTableAttribute](SimpleTableShowPropertiesOperationBase.md#getTableAttribute())
### Methods inherited from class ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md)
 [checkRowSpans](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#checkRowSpans(java.util.List,int)), [doOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getArguments()), [getAttrProperty](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getAttrProperty(java.util.List,java.lang.String,ro.sync.ecss.extensions.commons.table.properties.TableProperty)), [getCommonValue](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getCommonValue(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String)), [getDescription](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getDescription()), [getElementsWithModifiedAttributes](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getElementsWithModifiedAttributes(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo)), [getFragmentsAndOffsetsToInsert](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getFragmentsAndOffsetsToInsert(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo)), [getSelectedTab](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getSelectedTab(java.util.List)), [getTableInformation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getTableInformation(java.util.List)), [showTableProperties](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#showTableProperties(ro.sync.ecss.extensions.api.ArgumentsMap))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SimpleTableShowPropertiesOperation

public SimpleTableShowPropertiesOperation()

Constructor.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
