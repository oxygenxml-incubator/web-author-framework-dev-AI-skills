Package [ro.sync.ecss.extensions.dita.topic.table.simpletable](package-summary.md)

# Class InsertSingleColumnOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md)
            * [ro.sync.ecss.extensions.dita.topic.table.simpletable.InsertColumnOperation](InsertColumnOperation.md)
                * ro.sync.ecss.extensions.dita.topic.table.simpletable.InsertSingleColumnOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [InsertTableCellsContentConstants](../../../../commons/table/operations/InsertTableCellsContentConstants.md), [SimpleTableConstants](SimpleTableConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertSingleColumnOperation extends [InsertColumnOperation](InsertColumnOperation.md)
Operation used to insert one or more DITA simple table columns. It does not allow custom insertion of multiple columns, and thus is webapp-compatible.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.dita.topic.table.simpletable.[InsertColumnOperation](InsertColumnOperation.md)
 [cellContent](InsertColumnOperation.md#cellContent)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md)
 [INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR](../../../../commons/table/operations/InsertColumnOperationBase.md#INSERT_MULTIPLE_COLUMNS_ARGUMENT_DESCRIPTOR), [POSITION_ARGUMENT](../../../../commons/table/operations/InsertColumnOperationBase.md#POSITION_ARGUMENT), [POSITION_ARGUMENT_DESCRIPTOR](../../../../commons/table/operations/InsertColumnOperationBase.md#POSITION_ARGUMENT_DESCRIPTOR)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../../../../commons/table/operations/AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../../../../commons/table/operations/AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.[InsertTableCellsContentConstants](../../../../commons/table/operations/InsertTableCellsContentConstants.md)
 [CELL_FRAGMENT_ARGUMENT](../../../../commons/table/operations/InsertTableCellsContentConstants.md#CELL_FRAGMENT_ARGUMENT), [CELL_FRAGMENT_ARGUMENT_IN_ARRAY](../../../../commons/table/operations/InsertTableCellsContentConstants.md#CELL_FRAGMENT_ARGUMENT_IN_ARRAY), [CELL_FRAGMENT_ARGUMENT_NAME](../../../../commons/table/operations/InsertTableCellsContentConstants.md#CELL_FRAGMENT_ARGUMENT_NAME)
### Fields inherited from interface ro.sync.ecss.extensions.dita.topic.table.simpletable.[SimpleTableConstants](SimpleTableConstants.md)
 [ATTRIBUTE_NAME_ID](SimpleTableConstants.md#ATTRIBUTE_NAME_ID), [ELEMENT_NAME_CHDESC_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHDESC_CHOICETABLE), [ELEMENT_NAME_CHDESCHD_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHDESCHD_CHOICETABLE), [ELEMENT_NAME_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHOICETABLE), [ELEMENT_NAME_CHOPTION_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHOPTION_CHOICETABLE), [ELEMENT_NAME_CHOPTIONHD_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHOPTIONHD_CHOICETABLE), [ELEMENT_NAME_ENTRY_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_ENTRY_SIMPLETABLE), [ELEMENT_NAME_HEADER_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_HEADER_CHOICETABLE), [ELEMENT_NAME_HEADER_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_HEADER_PROPERTIES), [ELEMENT_NAME_HEADER_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_HEADER_SIMPLETABLE), [ELEMENT_NAME_PROPDESC_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPDESC_PROPERTIES), [ELEMENT_NAME_PROPDESCHD_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPDESCHD_PROPERTIES), [ELEMENT_NAME_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPERTIES), [ELEMENT_NAME_PROPTYPE_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPTYPE_PROPERTIES), [ELEMENT_NAME_PROPTYPEHD_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPTYPEHD_PROPERTIES), [ELEMENT_NAME_PROPVALUE_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPVALUE_PROPERTIES), [ELEMENT_NAME_PROPVALUEHD_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPVALUEHD_PROPERTIES), [ELEMENT_NAME_ROW_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_ROW_CHOICETABLE), [ELEMENT_NAME_ROW_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_ROW_PROPERTIES), [ELEMENT_NAME_ROW_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_ROW_SIMPLETABLE), [ELEMENT_NAME_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_SIMPLETABLE)
## Constructor Summary
 Constructors
Constructor

Description
 [InsertSingleColumnOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

### Methods inherited from class ro.sync.ecss.extensions.dita.topic.table.simpletable.[InsertColumnOperation](InsertColumnOperation.md)
 [doOperationInternal](InsertColumnOperation.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getCellElementName](InsertColumnOperation.md#getCellElementName(ro.sync.ecss.extensions.api.node.AuthorElement,int)), [getDefaultContentForEmptyCells](InsertColumnOperation.md#getDefaultContentForEmptyCells()), [updateColumnCellsSpan](InsertColumnOperation.md#updateColumnCellsSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,java.lang.String,int))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](../../../../commons/table/operations/InsertColumnOperationBase.md)
 [getDescription](../../../../commons/table/operations/InsertColumnOperationBase.md#getDescription()), [insertColumns](../../../../commons/table/operations/InsertColumnOperationBase.md#insertColumns(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,boolean,ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase,int,int,ro.sync.ecss.extensions.api.node.AuthorElement)), [insertColumns](../../../../commons/table/operations/InsertColumnOperationBase.md#insertColumns(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String,int,int)), [performInsertColumn](../../../../commons/table/operations/InsertColumnOperationBase.md#performInsertColumn(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation,boolean,ro.sync.ecss.extensions.commons.table.operations.InsertRowOperationBase,ro.sync.ecss.extensions.commons.table.operations.InsertTableOperationBase)), [removeMultipleInsertionDescriptor](../../../../commons/table/operations/InsertColumnOperationBase.md#removeMultipleInsertionDescriptor(ro.sync.ecss.extensions.api.ArgumentDescriptor%5B%5D))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
 [createEmptyCell](../../../../commons/table/operations/AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../../../../commons/table/operations/AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../../../../commons/table/operations/AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../../../../commons/table/operations/AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../../../../commons/table/operations/AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../../../../commons/table/operations/AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### InsertSingleColumnOperation

public InsertSingleColumnOperation()

## Method Details

### getArguments

public [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md)[] getArguments()
  Specified by: [getArguments](../../../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../../../api/AuthorOperation.md) Overrides: [getArguments](InsertColumnOperation.md#getArguments()) in class [InsertColumnOperation](InsertColumnOperation.md) Returns: An array of [ArgumentDescriptor](../../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [InsertColumnOperation.getArguments()](InsertColumnOperation.md#getArguments())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
