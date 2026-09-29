Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Class CALSAndHTMLShowTablePropertiesBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.properties.ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md)
        * ro.sync.ecss.extensions.commons.table.properties.CALSAndHTMLShowTablePropertiesBase
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   Direct Known Subclasses: [CALSShowTableProperties](CALSShowTableProperties.md), [DocbookHTMLShowTablePropertiesOperationBase](../../../docbook/table/properties/DocbookHTMLShowTablePropertiesOperationBase.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class CALSAndHTMLShowTablePropertiesBase extends [ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md)
Base class for edit properties on CALS and HTML tables.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [HORIZONTAL_ALIGN_VALUES](#HORIZONTAL_ALIGN_VALUES)
Array with common possible values for horizontal alignment
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [VERTICAL_ALIGN_VALUES](#VERTICAL_ALIGN_VALUES)
Array with common possible values for vertical alignment

### Fields inherited from class ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md)
 [authorAccess](ShowTablePropertiesBaseOperation.md#authorAccess), [tableHelper](ShowTablePropertiesBaseOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [CALSAndHTMLShowTablePropertiesBase](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.properties.TablePropertiesHelper))([TablePropertiesHelper](TablePropertiesHelper.md) helper)
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [computeFragmentMoveInsideHeader](#computeFragmentMoveInsideHeader(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../api/node/AuthorElement.md) currentNode)
Computes the fragment and position, inside header element, for the given node.
  protected boolean [computeFragmentsToMoveInsideBody](#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../api/node/AuthorElement.md) currentNode)
Computes the fragment and position, inside body element, for the given node.
  protected boolean [computeFragmentsToMoveInsideFooter](#computeFragmentsToMoveInsideFooter(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../api/node/AuthorElement.md) currentNode)
Computes the fragment and position, inside footer element, for the given node.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> [getCategoriesAndProperties](#getCategoriesAndProperties(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)[]> selections)
Obtain the categories from the table properties dialog.
  protected abstract [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](../../../api/node/AuthorElement.md),[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)>> [getCellIndexes](#getCellIndexes(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> cells)
Obtain the indexes for selected cells.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> [getCellsAttributes](#getCellsAttributes())()
Obtain the value for the given attribute set on the given element.
  protected abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> [getColSpecs](#getColSpecs(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](../../../api/node/AuthorElement.md),[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)>> map)
Obtain the colspecs elements for the given cells indexes.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> [getColumnsAttributes](#getColumnsAttributes())()
Obtain the value for the given attribute set on the given element.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> [getRowsAttributesToEdit](#getRowsAttributesToEdit())()
Obtain the attributes qualified name and render string (for rows).
  protected void [processFragment](#processFragment(ro.sync.ecss.extensions.api.node.AuthorElement,java.util.List,boolean))([AuthorElement](../../../api/node/AuthorElement.md) currentNode, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, boolean moveToHeader)
Process the fragments and add them to the fragments to insert.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md)
 [checkRowSpans](ShowTablePropertiesBaseOperation.md#checkRowSpans(java.util.List,int)), [doOperation](ShowTablePropertiesBaseOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](ShowTablePropertiesBaseOperation.md#getArguments()), [getAttrProperty](ShowTablePropertiesBaseOperation.md#getAttrProperty(java.util.List,java.lang.String,ro.sync.ecss.extensions.commons.table.properties.TableProperty)), [getCommonValue](ShowTablePropertiesBaseOperation.md#getCommonValue(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String)), [getDescription](ShowTablePropertiesBaseOperation.md#getDescription()), [getElementsWithModifiedAttributes](ShowTablePropertiesBaseOperation.md#getElementsWithModifiedAttributes(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo)), [getFragmentsAndOffsetsToInsert](ShowTablePropertiesBaseOperation.md#getFragmentsAndOffsetsToInsert(ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo)), [getHelpPageID](ShowTablePropertiesBaseOperation.md#getHelpPageID()), [getSelectedTab](ShowTablePropertiesBaseOperation.md#getSelectedTab(java.util.List)), [getTableAttribute](ShowTablePropertiesBaseOperation.md#getTableAttribute()), [getTableInformation](ShowTablePropertiesBaseOperation.md#getTableInformation(java.util.List)), [showTableProperties](ShowTablePropertiesBaseOperation.md#showTableProperties(ro.sync.ecss.extensions.api.ArgumentsMap))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### HORIZONTAL_ALIGN_VALUES

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] HORIZONTAL_ALIGN_VALUES

Array with common possible values for horizontal alignment

### VERTICAL_ALIGN_VALUES

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] VERTICAL_ALIGN_VALUES

Array with common possible values for vertical alignment

## Constructor Details

### CALSAndHTMLShowTablePropertiesBase

public CALSAndHTMLShowTablePropertiesBase([TablePropertiesHelper](TablePropertiesHelper.md) helper)

Constructor.
  Parameters: helper - The table helper.
## Method Details

### getCategoriesAndProperties

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> getCategoriesAndProperties([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)[]> selections)
 Description copied from class: [ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md#getCategoriesAndProperties(java.util.List))
Obtain the categories from the table properties dialog. The categories maps the tab name to the list of properties that will be modified in the corresponding tab panel. Every property will be modified using a combobox/radios which will contain the possible values for that property. The label string for the combobox/radios group will be the provided render string of the property or the property name, if a render string is not provided.
  Specified by: [getCategoriesAndProperties](ShowTablePropertiesBaseOperation.md#getCategoriesAndProperties(java.util.List)) in class [ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md) Parameters: selections - The currently selected nodes or the node at caret position. Returns: A list of tab info objects containing the tab names and the corresponding properties list. See Also:
        * [ShowTablePropertiesBaseOperation.getCategoriesAndProperties(java.util.List)](ShowTablePropertiesBaseOperation.md#getCategoriesAndProperties(java.util.List))

### getCellsAttributes

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> getCellsAttributes()

Obtain the value for the given attribute set on the given element.
  Returns: A list with allowed attributes.
### computeFragmentsToMoveInsideFooter

protected boolean computeFragmentsToMoveInsideFooter([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../api/node/AuthorElement.md) currentNode)throws [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from class: [ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md#computeFragmentsToMoveInsideFooter(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))
Computes the fragment and position, inside footer element, for the given node.
  Specified by: [computeFragmentsToMoveInsideFooter](ShowTablePropertiesBaseOperation.md#computeFragmentsToMoveInsideFooter(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)) in class [ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md) Parameters: fragments - A list with already computed fragments. The new fragment will be added to this list. offsets - A list with positions where the given fragments will be inserted. tabInfo - The current edited tab info. nodesToModify - A list containing all the nodes that will be deleted. currentNode - The node to be checked if it should be moved. Returns: true if the parent of the given node parent should be also deleted. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - If the new parent fragment could not be inserted. See Also:
        * [ShowTablePropertiesBaseOperation.computeFragmentsToMoveInsideFooter(java.util.List, java.util.List, ro.sync.ecss.extensions.commons.table.properties.TabInfo, java.util.List, ro.sync.ecss.extensions.api.node.AuthorElement)](ShowTablePropertiesBaseOperation.md#computeFragmentsToMoveInsideFooter(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))

### computeFragmentMoveInsideHeader

protected boolean computeFragmentMoveInsideHeader([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../api/node/AuthorElement.md) currentNode)throws [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from class: [ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md#computeFragmentMoveInsideHeader(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))
Computes the fragment and position, inside header element, for the given node.
  Specified by: [computeFragmentMoveInsideHeader](ShowTablePropertiesBaseOperation.md#computeFragmentMoveInsideHeader(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)) in class [ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md) Parameters: fragments - A list with already computed fragments. The new fragment will be added to this list. offsets - A list with positions where the given fragments will be inserted. tabInfo - The current edited tab info. nodesToModify - A list containing all the nodes that will be deleted. currentNode - The node to be checked if it should be moved. Returns: true if the parent of the given node parent should be also deleted. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - If the new parent fragment could not be inserted.
### computeFragmentsToMoveInsideBody

protected boolean computeFragmentsToMoveInsideBody([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> offsets, [TabInfo](TabInfo.md) tabInfo, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodesToModify, [AuthorElement](../../../api/node/AuthorElement.md) currentNode)throws [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from class: [ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))
Computes the fragment and position, inside body element, for the given node.
  Specified by: [computeFragmentsToMoveInsideBody](ShowTablePropertiesBaseOperation.md#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement)) in class [ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md) Parameters: fragments - A list with already computed fragments. The new fragment will be added to this list. offsets - A list with positions where the given fragments will be inserted. tabInfo - The current edited tab info. nodesToModify - A list containing all the nodes that will be deleted. currentNode - The node to be checked if it should be moved. Returns: true if the parent of the given node parent should be also deleted. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - If the new parent fragment could not be inserted. See Also:
        * [ShowTablePropertiesBaseOperation.computeFragmentsToMoveInsideBody(java.util.List, java.util.List, ro.sync.ecss.extensions.commons.table.properties.TabInfo, java.util.List, ro.sync.ecss.extensions.api.node.AuthorElement)](ShowTablePropertiesBaseOperation.md#computeFragmentsToMoveInsideBody(java.util.List,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TabInfo,java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement))

### processFragment

protected void processFragment([AuthorElement](../../../api/node/AuthorElement.md) currentNode, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragments, boolean moveToHeader)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Process the fragments and add them to the fragments to insert.
  Parameters: currentNode - The current row node. fragments - The list with fragment which will be inserted. moveToHeader - true if the current node is moved from body/footer to header. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### getRowsAttributesToEdit

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> getRowsAttributesToEdit()

Obtain the attributes qualified name and render string (for rows).
  Returns: A list with attributes to edit.
### getColumnsAttributes

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> getColumnsAttributes()

Obtain the value for the given attribute set on the given element.
  Returns: A list with allowed attributes.
### getColSpecs

protected abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> getColSpecs([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](../../../api/node/AuthorElement.md),[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)>> map)

Obtain the colspecs elements for the given cells indexes.
  Parameters: map - A map containing the table elements and cells indexes. Returns: A list with the colspecs elements for the given cells indexes.
### getCellIndexes

protected abstract [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](../../../api/node/AuthorElement.md),[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)>> getCellIndexes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> cells)

Obtain the indexes for selected cells.
  Parameters: cells - The selected cells. Returns: A map containing the cell indexes based on the parent tgroup.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
