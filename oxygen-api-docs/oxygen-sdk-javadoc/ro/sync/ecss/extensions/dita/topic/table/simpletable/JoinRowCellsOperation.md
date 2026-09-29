Package [ro.sync.ecss.extensions.dita.topic.table.simpletable](package-summary.md)

# Class JoinRowCellsOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.JoinRowCellsOperationBase](../../../../commons/table/operations/JoinRowCellsOperationBase.md)
            * ro.sync.ecss.extensions.dita.topic.table.simpletable.JoinRowCellsOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [SimpleTableConstants](SimpleTableConstants.md)   @API(type=INTERNAL, src=PUBLIC) public class JoinRowCellsOperation extends [JoinRowCellsOperationBase](../../../../commons/table/operations/JoinRowCellsOperationBase.md)implements [SimpleTableConstants](SimpleTableConstants.md)
This is the DITA simple tables implementation of the operation used to join the content of two or more cells from a table row. If there is a selection, the cell at selection start offset determines the destination cell where the content of the next cells will be moved.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../../../../commons/table/operations/AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../../../../commons/table/operations/AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../../../../commons/table/operations/AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.dita.topic.table.simpletable.[SimpleTableConstants](SimpleTableConstants.md)
 [ATTRIBUTE_NAME_ID](SimpleTableConstants.md#ATTRIBUTE_NAME_ID), [ELEMENT_NAME_CHDESC_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHDESC_CHOICETABLE), [ELEMENT_NAME_CHDESCHD_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHDESCHD_CHOICETABLE), [ELEMENT_NAME_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHOICETABLE), [ELEMENT_NAME_CHOPTION_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHOPTION_CHOICETABLE), [ELEMENT_NAME_CHOPTIONHD_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_CHOPTIONHD_CHOICETABLE), [ELEMENT_NAME_ENTRY_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_ENTRY_SIMPLETABLE), [ELEMENT_NAME_HEADER_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_HEADER_CHOICETABLE), [ELEMENT_NAME_HEADER_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_HEADER_PROPERTIES), [ELEMENT_NAME_HEADER_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_HEADER_SIMPLETABLE), [ELEMENT_NAME_PROPDESC_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPDESC_PROPERTIES), [ELEMENT_NAME_PROPDESCHD_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPDESCHD_PROPERTIES), [ELEMENT_NAME_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPERTIES), [ELEMENT_NAME_PROPTYPE_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPTYPE_PROPERTIES), [ELEMENT_NAME_PROPTYPEHD_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPTYPEHD_PROPERTIES), [ELEMENT_NAME_PROPVALUE_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPVALUE_PROPERTIES), [ELEMENT_NAME_PROPVALUEHD_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_PROPVALUEHD_PROPERTIES), [ELEMENT_NAME_ROW_CHOICETABLE](SimpleTableConstants.md#ELEMENT_NAME_ROW_CHOICETABLE), [ELEMENT_NAME_ROW_PROPERTIES](SimpleTableConstants.md#ELEMENT_NAME_ROW_PROPERTIES), [ELEMENT_NAME_ROW_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_ROW_SIMPLETABLE), [ELEMENT_NAME_SIMPLETABLE](SimpleTableConstants.md#ELEMENT_NAME_SIMPLETABLE)
## Constructor Summary
 Constructors
Constructor

Description
 [JoinRowCellsOperation](#%3Cinit%3E())()
Default constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected void [generateColumnSpecifications](#generateColumnSpecifications(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSpanSupport, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement)
Generates column specifications for the given table and inserts them into the document.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[JoinRowCellsOperationBase](../../../../commons/table/operations/JoinRowCellsOperationBase.md)
 [doOperationInternal](../../../../commons/table/operations/JoinRowCellsOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../../../../commons/table/operations/JoinRowCellsOperationBase.md#getArguments()), [getCell](../../../../commons/table/operations/JoinRowCellsOperationBase.md#getCell(ro.sync.ecss.extensions.api.AuthorAccess,int,boolean)), [getDescription](../../../../commons/table/operations/JoinRowCellsOperationBase.md#getDescription())
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../../commons/table/operations/AbstractTableOperation.md)
 [createEmptyCell](../../../../commons/table/operations/AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../../../../commons/table/operations/AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../../../../commons/table/operations/AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../../../../commons/table/operations/AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../../../../commons/table/operations/AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../../../../commons/table/operations/AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### JoinRowCellsOperation

public JoinRowCellsOperation()

Default constructor.

## Method Details

### generateColumnSpecifications

protected void generateColumnSpecifications([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) tableSpanSupport, [AuthorElement](../../../../api/node/AuthorElement.md) tableElement)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from class: [JoinRowCellsOperationBase](../../../../commons/table/operations/JoinRowCellsOperationBase.md#generateColumnSpecifications(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))
Generates column specifications for the given table and inserts them into the document.
  Specified by: [generateColumnSpecifications](../../../../commons/table/operations/JoinRowCellsOperationBase.md#generateColumnSpecifications(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement)) in class [JoinRowCellsOperationBase](../../../../commons/table/operations/JoinRowCellsOperationBase.md) Parameters: authorAccess - Author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. tableSpanSupport - Table cell span provider. tableElement - The table element. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) - Failed to insert the column specifications into the table. See Also:
        * [JoinRowCellsOperationBase.generateColumnSpecifications(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement)](../../../../commons/table/operations/JoinRowCellsOperationBase.md#generateColumnSpecifications(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
