Package [ro.sync.ecss.extensions.dita.topic.table.simpletable.properties](package-summary.md)

# Class ChoiceTableShowPropertiesOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.properties.ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md)
        * [ro.sync.ecss.extensions.dita.topic.table.simpletable.properties.SimpleTableShowPropertiesOperationBase](SimpleTableShowPropertiesOperationBase.md)
            * ro.sync.ecss.extensions.dita.topic.table.simpletable.properties.ChoiceTableShowPropertiesOperation
   All Implemented Interfaces: [AuthorOperation](../../../../../api/AuthorOperation.md), [Extension](../../../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class ChoiceTableShowPropertiesOperation extends [SimpleTableShowPropertiesOperationBase](SimpleTableShowPropertiesOperationBase.md)
Class for edit properties on DITA choice tables.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md)
 [authorAccess](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#authorAccess), [tableHelper](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [ChoiceTableShowPropertiesOperation](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [computeFragmentMoveInsideHeader](#computeFragmentMoveInsideHeader(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](../../../../../commons/table/properties/TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../../../api/node/AuthorElement.md) currentNode)
Computes the fragment and position, inside header element, for the given node.
  protected boolean [computeFragmentsToMoveInsideBody](#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](../../../../../commons/table/properties/TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../../../api/node/AuthorElement.md) currentNode)
Computes the fragment and position, inside body element, for the given node.

### Methods inherited from class ro.sync.ecss.extensions.dita.topic.table.simpletable.properties.[SimpleTableShowPropertiesOperationBase](SimpleTableShowPropertiesOperationBase.md)
 [computeFragmentsToMoveInsideFooter](SimpleTableShowPropertiesOperationBase.md#computeFragmentsToMoveInsideFooter(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)), [getCategoriesAndProperties](SimpleTableShowPropertiesOperationBase.md#getCategoriesAndProperties(java.util.List)), [getHelpPageID](SimpleTableShowPropertiesOperationBase.md#getHelpPageID()), [getTableAttribute](SimpleTableShowPropertiesOperationBase.md#getTableAttribute())
### Methods inherited from class ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md)
 [checkRowSpans](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#checkRowSpans(java.util.List,int)), [doOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getArguments()), [getAttrProperty](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getAttrProperty(java.util.List,java.lang.String,ro.sync.ecss.extensions.commons.table.properties.TableProperty)), [getCommonValue](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getCommonValue(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String)), [getDescription](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getDescription()), [getElementsWithModifiedAttributes](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getElementsWithModifiedAttributes(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo)), [getFragmentsAndOffsetsToInsert](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getFragmentsAndOffsetsToInsert(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo)), [getSelectedTab](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getSelectedTab(java.util.List)), [getTableInformation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#getTableInformation(java.util.List)), [showTableProperties](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#showTableProperties(ro.sync.ecss.extensions.api.ArgumentsMap))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ChoiceTableShowPropertiesOperation

public ChoiceTableShowPropertiesOperation()

Constructor.

## Method Details

### computeFragmentMoveInsideHeader

protected boolean computeFragmentMoveInsideHeader([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](../../../../../commons/table/properties/TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../../../api/node/AuthorElement.md) currentNode)throws [AuthorOperationException](../../../../../api/AuthorOperationException.md)
 Description copied from class: [ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#computeFragmentMoveInsideHeader(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))
Computes the fragment and position, inside header element, for the given node.
  Overrides: [computeFragmentMoveInsideHeader](SimpleTableShowPropertiesOperationBase.md#computeFragmentMoveInsideHeader(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)) in class [SimpleTableShowPropertiesOperationBase](SimpleTableShowPropertiesOperationBase.md) Parameters: fragments - A list with already computed fragments. The new fragment will be added to this list. offsets - A list with positions where the given fragments will be inserted. tabInfo - The current edited tab info. nodesToModify - A list containing all the nodes that will be deleted. currentNode - The node to be checked if it should be moved. Returns: true if the parent of the given node parent should be also deleted. Throws: [AuthorOperationException](../../../../../api/AuthorOperationException.md) - If the new parent fragment could not be inserted. See Also:
        * [ShowTablePropertiesBaseOperation.computeFragmentMoveInsideHeader(java.util.List, java.util.List, ro.sync.ecss.extensions.commons.table.properties.TabInfo, java.util.List, ro.sync.ecss.extensions.api.node.AuthorElement)](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#computeFragmentMoveInsideHeader(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))

### computeFragmentsToMoveInsideBody

protected boolean computeFragmentsToMoveInsideBody([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](../../../../../commons/table/properties/TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../../../api/node/AuthorElement.md) currentNode)throws [AuthorOperationException](../../../../../api/AuthorOperationException.md)
 Description copied from class: [ShowTablePropertiesBaseOperation](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))
Computes the fragment and position, inside body element, for the given node.
  Overrides: [computeFragmentsToMoveInsideBody](SimpleTableShowPropertiesOperationBase.md#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)) in class [SimpleTableShowPropertiesOperationBase](SimpleTableShowPropertiesOperationBase.md) Parameters: fragments - A list with already computed fragments. The new fragment will be added to this list. offsets - A list with positions where the given fragments will be inserted. tabInfo - The current edited tab info. nodesToModify - A list containing all the nodes that will be deleted. currentNode - The node to be checked if it should be moved. Returns: true if the parent of the given node parent should be also deleted. Throws: [AuthorOperationException](../../../../../api/AuthorOperationException.md) - If the new parent fragment could not be inserted. See Also:
        * [ShowTablePropertiesBaseOperation.computeFragmentsToMoveInsideBody(java.util.List, java.util.List, ro.sync.ecss.extensions.commons.table.properties.TabInfo, java.util.List, ro.sync.ecss.extensions.api.node.AuthorElement)](../../../../../commons/table/properties/ShowTablePropertiesBaseOperation.md#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
