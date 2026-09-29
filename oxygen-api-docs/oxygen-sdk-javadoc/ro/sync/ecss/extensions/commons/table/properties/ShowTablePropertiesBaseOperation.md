Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Class ShowTablePropertiesBaseOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.properties.ShowTablePropertiesBaseOperation
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   Direct Known Subclasses: [CALSAndHTMLShowTablePropertiesBase](CALSAndHTMLShowTablePropertiesBase.md), [RelTableShowPropertiesOperation](../../../dita/map/table/RelTableShowPropertiesOperation.md), [SimpleTableShowPropertiesOperationBase](../../../dita/topic/table/simpletable/properties/SimpleTableShowPropertiesOperationBase.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class ShowTablePropertiesBaseOperation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorOperation](../../../api/AuthorOperation.md)
Base class for operations that shows a dialog which allows the user to modify some properties for a table.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [AuthorAccess](../../../api/AuthorAccess.md) [authorAccess](#authorAccess)
The current author access.
  protected [TablePropertiesHelper](TablePropertiesHelper.md) [tableHelper](#tableHelper)
The table properties helper.

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [ShowTablePropertiesBaseOperation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.properties.TablePropertiesHelper))([TablePropertiesHelper](TablePropertiesHelper.md) tableHelper)
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [checkRowSpans](#checkRowSpans(java.util.List,int))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> collectedRows, int parentType)
Check if the selected rows can be moved (row spans don't exceed collected rows range).
  protected abstract boolean [computeFragmentMoveInsideHeader](#computeFragmentMoveInsideHeader(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../api/node/AuthorElement.md) currentNode)
Computes the fragment and position, inside header element, for the given node.
  protected abstract boolean [computeFragmentsToMoveInsideBody](#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../api/node/AuthorElement.md) currentNode)
Computes the fragment and position, inside body element, for the given node.
  protected abstract boolean [computeFragmentsToMoveInsideFooter](#computeFragmentsToMoveInsideFooter(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../api/node/AuthorElement.md) currentNode)
Computes the fragment and position, inside footer element, for the given node.
  void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)
Perform the actual operation.
  [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 protected [TableProperty](TableProperty.md) [getAttrProperty](#getAttrProperty(java.util.List,java.lang.String,ro.sync.ecss.extensions.commons.table.properties.TableProperty))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> collectedElements, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) detectedAttributeValue, [TableProperty](TableProperty.md) currentAttribute)
Obtain the table property object for the given attribute.
  protected abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> [getCategoriesAndProperties](#getCategoriesAndProperties(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)[]> selections)
Obtain the categories from the table properties dialog.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCommonValue](#getCommonValue(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String))([AuthorElement](../../../api/node/AuthorElement.md) currentElem, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrQname, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValue)
Obtain the common value for the given attribute set on the given element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> [getElementsWithModifiedAttributes](#getElementsWithModifiedAttributes(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo))([EditedTablePropertiesInfo](EditedTablePropertiesInfo.md) tableInfo)
Obtain all the elements with all the modified attributes.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> [getFragmentsAndOffsetsToInsert](#getFragmentsAndOffsetsToInsert(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo))([EditedTablePropertiesInfo](EditedTablePropertiesInfo.md) tableInfo)
Obtain a map with all the fragments which will be modified and the corresponding offsets (the offsets where the fragments will be inserted).
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHelpPageID](#getHelpPageID())()
Get the ID of the help page which will be called by the end user.
  protected [EditedTablePropertiesInfo.TAB_TYPE](EditedTablePropertiesInfo.TAB_TYPE.md) [getSelectedTab](#getSelectedTab(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)[]> selections)
Obtain the tab that will be selected in the "Table Properties" dialog.
  protected abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> [getTableAttribute](#getTableAttribute())()
Obtain the table attributes.
  protected [TabInfo](TabInfo.md) [getTableInformation](#getTableInformation(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)[]> selections)
Obtain the information for table tab.
  void [showTableProperties](#showTableProperties(ro.sync.ecss.extensions.api.ArgumentsMap))([ArgumentsMap](../../../api/ArgumentsMap.md) args)
Shows the table properties and process all the modifications.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### tableHelper

protected [TablePropertiesHelper](TablePropertiesHelper.md) tableHelper

The table properties helper.

### authorAccess

protected [AuthorAccess](../../../api/AuthorAccess.md) authorAccess

The current author access.

## Constructor Details

### ShowTablePropertiesBaseOperation

public ShowTablePropertiesBaseOperation([TablePropertiesHelper](TablePropertiesHelper.md) tableHelper)

Constructor.
  Parameters: tableHelper - The table properties helper.
## Method Details

### doOperation

public void doOperation([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorOperation](../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation. You can check if the operation was invoked from the oXygen standalone application or from the oXygen plugin for Eclipse by using the method: [ApplicationInformationAccess.getPlatform()](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()). To get to the [Workspace](../../../../../exml/workspace/api/Workspace.md) you may use: [AuthorAccess.getWorkspaceAccess()](../../../api/AuthorAccess.md#getWorkspaceAccess()).
  Specified by: [doOperation](../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in interface [AuthorOperation](../../../api/AuthorOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AuthorOperation.doOperation(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### getArguments

public [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] getArguments()
  Specified by: [getArguments](../../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../../api/AuthorOperation.md) Returns: An array of [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments())

### showTableProperties

public void showTableProperties([ArgumentsMap](../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Shows the table properties and process all the modifications.
  Parameters: args - the arguments the operation was invoked with. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - When the action cannot be performed.
### getElementsWithModifiedAttributes

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> getElementsWithModifiedAttributes([EditedTablePropertiesInfo](EditedTablePropertiesInfo.md) tableInfo)

Obtain all the elements with all the modified attributes.
  Parameters: tableInfo - The obtained table information from the table properties dialog. Returns: A map containing all the elements whose attributes will be modified and the corresponding attributes.
### checkRowSpans

protected boolean checkRowSpans([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> collectedRows, int parentType)

Check if the selected rows can be moved (row spans don't exceed collected rows range).
  Parameters: collectedRows - The rows to be checked. parentType - The type of the parent element. Returns: true if the rows can be moved.
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../../api/Extension.md#getDescription()) in interface [Extension](../../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

### getFragmentsAndOffsetsToInsert

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> getFragmentsAndOffsetsToInsert([EditedTablePropertiesInfo](EditedTablePropertiesInfo.md) tableInfo)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Obtain a map with all the fragments which will be modified and the corresponding offsets (the offsets where the fragments will be inserted).
  Parameters: tableInfo - The obtained table information from the table properties dialog. Returns: a list tab info objects which contains all the fragments which will be modified and the corresponding offsets (the offsets where the fragments will be inserted). Throws: [AuthorOperationException](../../../api/AuthorOperationException.md)
### getTableInformation

protected [TabInfo](TabInfo.md) getTableInformation([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)[]> selections)

Obtain the information for table tab. This information will contain the properties which will be edited, the table elements on which those properties applies and some context information.
  Parameters: selections - The list with the selection intervals. Returns: The tab info object or null is there are no properties to edit for table.
### getAttrProperty

protected [TableProperty](TableProperty.md) getAttrProperty([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> collectedElements, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) detectedAttributeValue, [TableProperty](TableProperty.md) currentAttribute)

Obtain the table property object for the given attribute.
  Parameters: collectedElements - The list of all rows which will be edited. detectedAttributeValue - Current value of the attribute. It is the value set on the element(s). currentAttribute - The current attribute. Returns: a [TableProperty](TableProperty.md) object for the given attribute.
### getCommonValue

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCommonValue([AuthorElement](../../../api/node/AuthorElement.md) currentElem, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrQname, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentValue)

Obtain the common value for the given attribute set on the given element.
  Parameters: currentElem - The element to check for given attribute. attrQname - The attribute qualified name. currentValue - The currently computed common value for the given attribute. Returns: The common value between the given value and the attribute values set on the given element.
### getSelectedTab

protected [EditedTablePropertiesInfo.TAB_TYPE](EditedTablePropertiesInfo.TAB_TYPE.md) getSelectedTab([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)[]> selections)

Obtain the tab that will be selected in the "Table Properties" dialog.
  Parameters: selections - The currently selected nodes or the node at caret position. Returns: the tab that will be selected in the "Table Properties" dialog.
### getCategoriesAndProperties

protected abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> getCategoriesAndProperties([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)[]> selections)

Obtain the categories from the table properties dialog. The categories maps the tab name to the list of properties that will be modified in the corresponding tab panel. Every property will be modified using a combobox/radios which will contain the possible values for that property. The label string for the combobox/radios group will be the provided render string of the property or the property name, if a render string is not provided.
  Parameters: selections - The currently selected nodes or the node at caret position. Returns: A list of tab info objects containing the tab names and the corresponding properties list.
### getTableAttribute

protected abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> getTableAttribute()

Obtain the table attributes.
  Returns: A list with [TableProperty](TableProperty.md) objects containing the table attributes qualified name, render string and possible values.
### computeFragmentsToMoveInsideFooter

protected abstract boolean computeFragmentsToMoveInsideFooter([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../api/node/AuthorElement.md) currentNode)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Computes the fragment and position, inside footer element, for the given node.
  Parameters: fragments - A list with already computed fragments. The new fragment will be added to this list. offsets - A list with positions where the given fragments will be inserted. tabInfo - The current edited tab info. nodesToModify - A list containing all the nodes that will be deleted. currentNode - The node to be checked if it should be moved. Returns: true if the parent of the given node parent should be also deleted. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - If the new parent fragment could not be inserted.
### computeFragmentMoveInsideHeader

protected abstract boolean computeFragmentMoveInsideHeader([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../api/node/AuthorElement.md) currentNode)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Computes the fragment and position, inside header element, for the given node.
  Parameters: fragments - A list with already computed fragments. The new fragment will be added to this list. offsets - A list with positions where the given fragments will be inserted. tabInfo - The current edited tab info. nodesToModify - A list containing all the nodes that will be deleted. currentNode - The node to be checked if it should be moved. Returns: true if the parent of the given node parent should be also deleted. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - If the new parent fragment could not be inserted.
### computeFragmentsToMoveInsideBody

protected abstract boolean computeFragmentsToMoveInsideBody([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../api/node/AuthorElement.md) currentNode)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Computes the fragment and position, inside body element, for the given node.
  Parameters: fragments - A list with already computed fragments. The new fragment will be added to this list. offsets - A list with positions where the given fragments will be inserted. tabInfo - The current edited tab info. nodesToModify - A list containing all the nodes that will be deleted. currentNode - The node to be checked if it should be moved. Returns: true if the parent of the given node parent should be also deleted. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - If the new parent fragment could not be inserted.
### getHelpPageID

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHelpPageID()

Get the ID of the help page which will be called by the end user.
  Returns: the ID of the help page which will be called by the end user or null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
