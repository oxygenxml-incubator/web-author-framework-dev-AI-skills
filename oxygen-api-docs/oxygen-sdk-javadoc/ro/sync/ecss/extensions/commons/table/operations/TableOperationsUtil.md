Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class TableOperationsUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.operations.TableOperationsUtil
   @API(type=INTERNAL, src=PUBLIC) public final class TableOperationsUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Utility class for table operations.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static boolean [areOtherTablesThanChoicetableAllowed](#areOtherTablesThanChoicetableAllowed(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)
Check if a table other than choicetable is allowed here.
  static void [computeElementsList](#computeElementsList(java.util.List,ro.sync.ecss.extensions.api.node.AuthorElement,int,int,int,boolean,ro.sync.ecss.extensions.commons.table.properties.TableHelper))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> elementsList, [AuthorElement](../../../api/node/AuthorElement.md) node, int startOffset, int endOffset, int type, boolean fullySelected, [TableHelper](../properties/TableHelper.md) tableHelper)
Computes all the nodes of the given type starting from the given node, which are in the given selection.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [createCellXMLFragment](#createCellXMLFragment(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,boolean,java.lang.String,int,java.lang.String,ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper,java.lang.String...))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)[] fragments, boolean cellsFragment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cellElementName, int currentFragmentIndex, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorTableHelper](AuthorTableHelper.md) authorTableHelper, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... imposedAttributesFragments)
Create a cell fragment for a specific offset, having the name of the cell and a source fragment from which the attributes and content must be copied.
  static [TableHelper](../properties/TableHelper.md) [createTableHelper](#createTableHelper(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](AuthorTableHelper.md) authorTableHelper)
Create a [TableHelper](../properties/TableHelper.md) starting from an [AuthorTableHelper](AuthorTableHelper.md).
  static [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](../../../api/node/AuthorElement.md),[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)>> [getCellIndexes](#getCellIndexes(java.util.List,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.commons.table.properties.TableHelper,boolean))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> cells, [AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [TableHelper](../properties/TableHelper.md) tableHelper, boolean isCals)
Obtain the indexes for selected cells.
  static void [getChildElements](#getChildElements(ro.sync.ecss.extensions.api.node.AuthorElement,int,java.util.List,ro.sync.ecss.extensions.commons.table.properties.TableHelper))([AuthorElement](../../../api/node/AuthorElement.md) node, int type, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> children, [TableHelper](../properties/TableHelper.md) tableHelper)
\* Obtain a list of children with the given type.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContentFromFragment](#getContentFromFragment(ro.sync.ecss.extensions.api.AuthorAccess,boolean,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, boolean cellsFragment, [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md) fragment)
Get the given fragment content.
  static [AuthorElement](../../../api/node/AuthorElement.md) [getElementAncestor](#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int,ro.sync.ecss.extensions.commons.table.properties.TableHelper))([AuthorNode](../../../api/node/AuthorNode.md) node, int type, [TableHelper](../properties/TableHelper.md) tableHelper)
Search for an ancestor [AuthorNode](../../../api/node/AuthorNode.md) with the specified type.
  static [AuthorElement](../../../api/node/AuthorElement.md) [getTableElementContainingOffset](#getTableElementContainingOffset(int,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String...))(int offset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorAccess](../../../api/AuthorAccess.md) access, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... tableElementNames)
Returns the element representing the table that contains the given offset and has the given properties (name, namespace).
  static [AuthorElement](../../../api/node/AuthorElement.md) [getTableElementContainingOffset](#getTableElementContainingOffset(int,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String...))(int offset, [AuthorAccess](../../../api/AuthorAccess.md) access, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... tableClassValues)
Returns the element representing the table that contains the given offset and has the given properties (name, class attribute).
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> [getTableElementsOfType](#getTableElementsOfType(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,int,ro.sync.ecss.extensions.commons.table.properties.TableHelper))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)[]> selections, int type, [TableHelper](../properties/TableHelper.md) tableHelper)
Collects all the table elements having the given type, determined by the selection intervals.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> [getTableElementsOfTypeFromSelection](#getTableElementsOfTypeFromSelection(ro.sync.ecss.extensions.api.AuthorAccess,int,ro.sync.ecss.extensions.commons.table.properties.TableHelper,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, int type, [TableHelper](../properties/TableHelper.md) tableHelper, [AuthorElement](../../../api/node/AuthorElement.md) tableElement)
Collects all the table elements having the given type, determined by the selection intervals.
  static boolean [handleColumnSpecAttributeChange](#handleColumnSpecAttributeChange(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableHelper](AuthorTableHelper.md) helper, [AuthorElement](../../../api/node/AuthorElement.md) currentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AttrValue](../../../api/node/AttrValue.md) newValue)
Propagate the change of a column name in the entire table.
  static boolean [isChoiceTableAllowed](#isChoiceTableAllowed(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)
Check if a choice table can be inserted in the current context.
  static boolean [isIgnoredAttribute](#isIgnoredAttribute(java.lang.String,ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName, [AuthorTableHelper](AuthorTableHelper.md) tableHelper)
Check if the attribute should be ignored.
  static boolean [isPropertiesTableGlobalElement](#isPropertiesTableGlobalElement(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)
Check if a properties table is allowed as a global element.
  static boolean [nodeHasProperties](#nodeHasProperties(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,java.lang.String))([AuthorNode](../../../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Check if the node has the given namespace and name
  static void [placeCaretInFirstCell](#placeCaretInFirstCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.commons.table.operations.TableInfo,ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.schemaaware.SchemaAwareHandlerResult))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [TableInfo](TableInfo.md) tableInfo, [AuthorDocumentController](../../../api/AuthorDocumentController.md) controller, [SchemaAwareHandlerResult](../../../api/schemaaware/SchemaAwareHandlerResult.md) result)
Place the caret in the first cell of a table that was just inserted (a result of this operation is send as parameter)
  static void [removeInvalidColNamesFromCALSTableCells](#removeInvalidColNamesFromCALSTableCells(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.util.List))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> cells)
Remove invalid column names from CALS table cells.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### createCellXMLFragment

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) createCellXMLFragment([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)[] fragments, boolean cellsFragment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cellElementName, int currentFragmentIndex, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorTableHelper](AuthorTableHelper.md) authorTableHelper, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... imposedAttributesFragments)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Create a cell fragment for a specific offset, having the name of the cell and a source fragment from which the attributes and content must be copied.
  Parameters: authorAccess - The author access. fragments - The list of all content fragments. cellsFragment - true if the fragments represents cells. cellElementName - The cell name. currentFragmentIndex - The index of the fragment that must be used for attributes and content. namespace - The cell namespace. authorTableHelper - Author table helper. imposedAttributesFragments - Imposed attributes for the created cell. Each fragment has the following form: "attribute_name=\"attribute_value\"" Returns: The cell fragment. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md)
### isIgnoredAttribute

public static boolean isIgnoredAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName, [AuthorTableHelper](AuthorTableHelper.md) tableHelper)

Check if the attribute should be ignored.
  Parameters: attrName - The attribute name. tableHelper - Author table helper Returns: true if the attribute should be ignored.
### getContentFromFragment

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContentFromFragment([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, boolean cellsFragment, [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md) fragment)

Get the given fragment content. If the cellsFragment parameter is true, the returned content represent the content of the cell, otherwise the fragment itself.
  Parameters: authorAccess - The author access. cellsFragment - true if the fragment represent a cell fragment fragment - The Author fragment. Returns: The fragment content.
### nodeHasProperties

public static boolean nodeHasProperties([AuthorNode](../../../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)

Check if the node has the given namespace and name
  Parameters: node - The node to check. name - The name to compare the node name with. namespace - The namespace to compare the node namespace with. Returns: true if the node has the given namespace and name.
### getTableElementContainingOffset

public static [AuthorElement](../../../api/node/AuthorElement.md) getTableElementContainingOffset(int offset, [AuthorAccess](../../../api/AuthorAccess.md) access, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... tableClassValues)

Returns the element representing the table that contains the given offset and has the given properties (name, class attribute). Used for DITA and DITA Maps table operations.
  Parameters: offset - The offset to search the parent table element for. access - Access to Author operations. tableClassValues - Possible table class attributes values. Returns: The table element that contains the given offset.
### getTableElementContainingOffset

public static [AuthorElement](../../../api/node/AuthorElement.md) getTableElementContainingOffset(int offset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorAccess](../../../api/AuthorAccess.md) access, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)... tableElementNames)

Returns the element representing the table that contains the given offset and has the given properties (name, namespace).
  Parameters: offset - The offset to search the parent table element for. namespace - The table node namespace. access - Access to Author operations. tableElementNames - Possible table element names. Returns: The table element that contains the given offset.
### isChoiceTableAllowed

public static boolean isChoiceTableAllowed([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)

Check if a choice table can be inserted in the current context.
  Parameters: authorAccess - The author access. Returns: true if a choice table can be inserted in the given context.
### areOtherTablesThanChoicetableAllowed

public static boolean areOtherTablesThanChoicetableAllowed([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)

Check if a table other than choicetable is allowed here.
  Parameters: authorAccess - The author access. Returns: true if a choice table can be inserted in the given context.
### isPropertiesTableGlobalElement

public static boolean isPropertiesTableGlobalElement([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)

Check if a properties table is allowed as a global element.
  Parameters: authorAccess - The author access. Returns: true if the "properties" table element is a global element of the schema.
### getTableElementsOfTypeFromSelection

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> getTableElementsOfTypeFromSelection([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, int type, [TableHelper](../properties/TableHelper.md) tableHelper, [AuthorElement](../../../api/node/AuthorElement.md) tableElement)

Collects all the table elements having the given type, determined by the selection intervals.
  Parameters: authorAccess - The author access type - The type of the elements to be collected. Can be one of TYPE_ prefixed constants from [TableHelperConstants](../properties/TableHelperConstants.md). tableHelper - Utility class to determine information about table nodes. tableElement - The table parent elements. Returns: A list with all the elements used to populate the tabs in "Table Properties" dialog.
### getTableElementsOfType

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> getTableElementsOfType([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)[]> selections, int type, [TableHelper](../properties/TableHelper.md) tableHelper)

Collects all the table elements having the given type, determined by the selection intervals.
  Parameters: authorAccess - The author access selections - The currently selected nodes. They can be mixed. type - The type of the elements to be collected. Can be one of TYPE_ prefixed constants from [TableHelperConstants](../properties/TableHelperConstants.md). tableHelper - Utility class to determine information about table nodes. Returns: A list with all the elements used to populate the tabs in "Table Properties" dialog.
### computeElementsList

public static void computeElementsList([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> elementsList, [AuthorElement](../../../api/node/AuthorElement.md) node, int startOffset, int endOffset, int type, boolean fullySelected, [TableHelper](../properties/TableHelper.md) tableHelper)

Computes all the nodes of the given type starting from the given node, which are in the given selection.
  Parameters: elementsList - The list which will contain the elements. node - The starting node. startOffset - Selection start. endOffset - Selection end. type - The elements type. Can be one of TYPE_ prefixed constants from [TableHelperConstants](../properties/TableHelperConstants.md). fullySelected - true if the nodes should be entire contained by the selection. tableHelper - Utility class to determine information about table nodes.
### getElementAncestor

public static [AuthorElement](../../../api/node/AuthorElement.md) getElementAncestor([AuthorNode](../../../api/node/AuthorNode.md) node, int type, [TableHelper](../properties/TableHelper.md) tableHelper)

Search for an ancestor [AuthorNode](../../../api/node/AuthorNode.md) with the specified type.
  Parameters: node - The starting node. type - The type of the ancestor. tableHelper - Utility class to determine information about table nodes. Returns: The ancestor node of the given node or the node itself if the type matches.
### getChildElements

public static void getChildElements([AuthorElement](../../../api/node/AuthorElement.md) node, int type, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> children, [TableHelper](../properties/TableHelper.md) tableHelper)

\* Obtain a list of children with the given type.
  Parameters: node - The parent node. type - The child elements type. Can be one of TYPE_ prefixed constants from [TableHelperConstants](../properties/TableHelperConstants.md). children - The list with collected children. Empty when the function is called. tableHelper - Utility class to determine information about table nodes.
### getCellIndexes

public static [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](../../../api/node/AuthorElement.md),[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)>> getCellIndexes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> cells, [AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [TableHelper](../properties/TableHelper.md) tableHelper, boolean isCals)

Obtain the indexes for selected cells.
  Parameters: cells - The selected cells. authorAccess - The author access. tableHelper - Utility class to determine information about table nodes. isCals - true if it is a CALS table Returns: A map between the table element and a set of the cell's column indexes.
### createTableHelper

public static [TableHelper](../properties/TableHelper.md) createTableHelper([AuthorTableHelper](AuthorTableHelper.md) authorTableHelper)

Create a [TableHelper](../properties/TableHelper.md) starting from an [AuthorTableHelper](AuthorTableHelper.md).
  Parameters: authorTableHelper - The Author table helper Returns: The [TableHelper](../properties/TableHelper.md)
### placeCaretInFirstCell

public static void placeCaretInFirstCell([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [TableInfo](TableInfo.md) tableInfo, [AuthorDocumentController](../../../api/AuthorDocumentController.md) controller, [SchemaAwareHandlerResult](../../../api/schemaaware/SchemaAwareHandlerResult.md) result)

Place the caret in the first cell of a table that was just inserted (a result of this operation is send as parameter)
  Parameters: authorAccess - Author access. tableInfo - Table information. controller - Controller. result - Insert operation result.
### removeInvalidColNamesFromCALSTableCells

public static void removeInvalidColNamesFromCALSTableCells([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> cells)

Remove invalid column names from CALS table cells. Remove references to column names which are not defined in the table.
  Parameters: authorAccess - Author Access tableElement - The table element cells - The list of cells.
### handleColumnSpecAttributeChange

public static boolean handleColumnSpecAttributeChange([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorTableHelper](AuthorTableHelper.md) helper, [AuthorElement](../../../api/node/AuthorElement.md) currentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AttrValue](../../../api/node/AttrValue.md) newValue)

Propagate the change of a column name in the entire table.
  Parameters: authorAccess - Author access helper - Table helper. currentElement - Current element on which the attribute which should be changed. attributeName - Name of changed attribute newValue - The new attribute value Returns: true if this method handled the change.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
