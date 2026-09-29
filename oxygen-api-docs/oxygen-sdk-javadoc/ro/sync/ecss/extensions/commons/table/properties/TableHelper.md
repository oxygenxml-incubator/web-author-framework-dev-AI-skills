Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Interface TableHelper
    All Known Subinterfaces: [TablePropertiesHelper](TablePropertiesHelper.md)   All Known Implementing Classes: [ChoiceTableHelper](../../../dita/topic/table/simpletable/properties/ChoiceTableHelper.md), [DITACALSTableHelper](../../../dita/topic/table/cals/properties/DITACALSTableHelper.md), [Docbook5CALSTableHelper](../../../docbook/table/properties/Docbook5CALSTableHelper.md), [Docbook5HTMLTableHelper](../../../docbook/table/properties/Docbook5HTMLTableHelper.md), [DocbookCALSTableHelper](../../../docbook/table/properties/DocbookCALSTableHelper.md), [DocbookHTMLTableHelper](../../../docbook/table/properties/DocbookHTMLTableHelper.md), [RelTablePropertiesHelper](../../../dita/map/table/RelTablePropertiesHelper.md), [SimpleTableHelper](../../../dita/topic/table/simpletable/properties/SimpleTableHelper.md), [TablePropertiesHelperBase](TablePropertiesHelperBase.md)   @API(type=INTERNAL, src=PUBLIC) public interface TableHelper
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [isNodeOfType](#isNodeOfType(ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorElement](../../../api/node/AuthorElement.md) node, int type)
Test if an [AuthorNode](../../../api/node/AuthorNode.md) is an element and it has one of the following types: [AuthorTableHelper.TYPE_CELL](../operations/AuthorTableHelper.md#TYPE_CELL), [AuthorTableHelper.TYPE_ROW](../operations/AuthorTableHelper.md#TYPE_ROW) or [AuthorTableHelper.TYPE_TABLE](../operations/AuthorTableHelper.md#TYPE_TABLE).
  boolean [isTable](#isTable(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents the table element.
  boolean [isTableGroup](#isTableGroup(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) node)
Checks if the given node represents a table group element.

## Method Details

### isNodeOfType

boolean isNodeOfType([AuthorElement](../../../api/node/AuthorElement.md) node, int type)

Test if an [AuthorNode](../../../api/node/AuthorNode.md) is an element and it has one of the following types: [AuthorTableHelper.TYPE_CELL](../operations/AuthorTableHelper.md#TYPE_CELL), [AuthorTableHelper.TYPE_ROW](../operations/AuthorTableHelper.md#TYPE_ROW) or [AuthorTableHelper.TYPE_TABLE](../operations/AuthorTableHelper.md#TYPE_TABLE).
  Parameters: node - The node to be checked. type - The type to search for. Returns: true if the node is an element with the specified type.
### isTable

boolean isTable([AuthorElement](../../../api/node/AuthorElement.md) node)

Checks if the given node represents the table element.
  Parameters: node - The node to be checked. Returns: true if the given node is the table element.
### isTableGroup

boolean isTableGroup([AuthorElement](../../../api/node/AuthorElement.md) node)

Checks if the given node represents a table group element.
  Parameters: node - The node to be checked. Returns: true if the given node is the table group element.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
