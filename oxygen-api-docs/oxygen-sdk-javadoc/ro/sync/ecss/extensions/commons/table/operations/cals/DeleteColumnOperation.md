Package [ro.sync.ecss.extensions.commons.table.operations.cals](package-summary.md)

# Class DeleteColumnOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation](../AbstractTableOperation.md)
        * [ro.sync.ecss.extensions.commons.table.operations.DeleteColumnOperationBase](../DeleteColumnOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.DeleteColumnOperation
   All Implemented Interfaces: [AuthorOperation](../../../../api/AuthorOperation.md), [Extension](../../../../api/Extension.md), [CALSConstants](CALSConstants.md)   Direct Known Subclasses: [DeleteColumnOperation](../../../../dita/topic/table/cals/DeleteColumnOperation.md)   @API(type=INTERNAL, src=PUBLIC) public class DeleteColumnOperation extends [DeleteColumnOperationBase](../DeleteColumnOperationBase.md)implements [CALSConstants](CALSConstants.md)
Operation used to delete a CALS table column.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[DeleteColumnOperationBase](../DeleteColumnOperationBase.md)
 [deletedColumnsIndices](../DeleteColumnOperationBase.md#deletedColumnsIndices), [tableElem](../DeleteColumnOperationBase.md#tableElem)
### Fields inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](../AbstractTableOperation.md#CHANGE_TRACKING_BEHAVIOR_ARGUMENT), [TABLE_INFO_ARGUMENT_DESCRIPTOR](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_DESCRIPTOR), [TABLE_INFO_ARGUMENT_NAME](../AbstractTableOperation.md#TABLE_INFO_ARGUMENT_NAME), [tableHelper](../AbstractTableOperation.md#tableHelper)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
### Fields inherited from interface ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md)
 [ATTRIBUTE_NAME_ALIGN](CALSConstants.md#ATTRIBUTE_NAME_ALIGN), [ATTRIBUTE_NAME_COLNAME](CALSConstants.md#ATTRIBUTE_NAME_COLNAME), [ATTRIBUTE_NAME_COLNUM](CALSConstants.md#ATTRIBUTE_NAME_COLNUM), [ATTRIBUTE_NAME_COLS](CALSConstants.md#ATTRIBUTE_NAME_COLS), [ATTRIBUTE_NAME_COLSEP](CALSConstants.md#ATTRIBUTE_NAME_COLSEP), [ATTRIBUTE_NAME_COLWIDTH](CALSConstants.md#ATTRIBUTE_NAME_COLWIDTH), [ATTRIBUTE_NAME_ID](CALSConstants.md#ATTRIBUTE_NAME_ID), [ATTRIBUTE_NAME_MOREROWS](CALSConstants.md#ATTRIBUTE_NAME_MOREROWS), [ATTRIBUTE_NAME_NAMEEND](CALSConstants.md#ATTRIBUTE_NAME_NAMEEND), [ATTRIBUTE_NAME_NAMEST](CALSConstants.md#ATTRIBUTE_NAME_NAMEST), [ATTRIBUTE_NAME_ROWSEP](CALSConstants.md#ATTRIBUTE_NAME_ROWSEP), [ATTRIBUTE_NAME_SPANNAME](CALSConstants.md#ATTRIBUTE_NAME_SPANNAME), [ATTRIBUTE_NAME_TABLE_WIDTH](CALSConstants.md#ATTRIBUTE_NAME_TABLE_WIDTH), [ATTRIBUTE_NAME_XML_ID](CALSConstants.md#ATTRIBUTE_NAME_XML_ID), [ELEMENT_NAME_COLSPEC](CALSConstants.md#ELEMENT_NAME_COLSPEC), [ELEMENT_NAME_ENTRY](CALSConstants.md#ELEMENT_NAME_ENTRY), [ELEMENT_NAME_INFORMALTABLE](CALSConstants.md#ELEMENT_NAME_INFORMALTABLE), [ELEMENT_NAME_ROW](CALSConstants.md#ELEMENT_NAME_ROW), [ELEMENT_NAME_SPANSPEC](CALSConstants.md#ELEMENT_NAME_SPANSPEC), [ELEMENT_NAME_TABLE](CALSConstants.md#ELEMENT_NAME_TABLE), [ELEMENT_NAME_TGROUP](CALSConstants.md#ELEMENT_NAME_TGROUP)
## Constructor Summary
 Constructors
Constructor

Description
 [DeleteColumnOperation](#%3Cinit%3E())()
Default constructor.
  [DeleteColumnOperation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](../AuthorTableHelper.md) documentTypeHelper)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [updateColspec](#updateColspec(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.Integer))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) deletedColumnIndex)
Update the colspec of a table for a given column.
  protected void [updateTableColSpan](#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) spanProvider, [AuthorElement](../../../../api/node/AuthorElement.md) cell, int colStartIndex, int colEndIndex)
Update the column span for the table cell that is included into the deleted column.

### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[DeleteColumnOperationBase](../DeleteColumnOperationBase.md)
 [canDeleteColumn](../DeleteColumnOperationBase.md#canDeleteColumn()), [doOperationInternal](../DeleteColumnOperationBase.md#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](../DeleteColumnOperationBase.md#getArguments()), [getDescription](../DeleteColumnOperationBase.md#getDescription()), [performDeleteColumn](../DeleteColumnOperationBase.md#performDeleteColumn(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List,boolean)), [updateAppliableColWidthsNumber](../DeleteColumnOperationBase.md#updateAppliableColWidthsNumber(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))
### Methods inherited from class ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md)
 [createEmptyCell](../AbstractTableOperation.md#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D)), [doOperation](../AbstractTableOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [findCellInsertionOffset](../AbstractTableOperation.md#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)), [getElementAncestor](../AbstractTableOperation.md#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int)), [isElement](../AbstractTableOperation.md#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [isTableElement](../AbstractTableOperation.md#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DeleteColumnOperation

public DeleteColumnOperation()

Default constructor.

### DeleteColumnOperation

public DeleteColumnOperation([AuthorTableHelper](../AuthorTableHelper.md) documentTypeHelper)

Constructor.
  Parameters: documentTypeHelper - The document type helper.
## Method Details

### updateColspec

public void updateColspec([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) deletedColumnIndex)
 Description copied from class: [DeleteColumnOperationBase](../DeleteColumnOperationBase.md#updateColspec(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.Integer))
Update the colspec of a table for a given column.
  Overrides: [updateColspec](../DeleteColumnOperationBase.md#updateColspec(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.Integer)) in class [DeleteColumnOperationBase](../DeleteColumnOperationBase.md) Parameters: authorAccess - The Author access. deletedColumnIndex - The index of the deleted column. See Also:
        * [DeleteColumnOperationBase.updateColspec(AuthorAccess, Integer)](../DeleteColumnOperationBase.md#updateColspec(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.Integer))

### updateTableColSpan

protected void updateTableColSpan([AuthorAccess](../../../../api/AuthorAccess.md) authorAccess, [AuthorTableCellSpanProvider](../../../../api/AuthorTableCellSpanProvider.md) spanProvider, [AuthorElement](../../../../api/node/AuthorElement.md) cell, int colStartIndex, int colEndIndex)throws [AuthorOperationException](../../../../api/AuthorOperationException.md)
 Description copied from class: [DeleteColumnOperationBase](../DeleteColumnOperationBase.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))
Update the column span for the table cell that is included into the deleted column.
  Specified by: [updateTableColSpan](../DeleteColumnOperationBase.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int)) in class [DeleteColumnOperationBase](../DeleteColumnOperationBase.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. spanProvider - The table span provider. The object responsible for providing information about the cell spanning. cell - The table cell. colStartIndex - The new column start index, 1 based. colEndIndex - The new column end index, 1 based. Throws: [AuthorOperationException](../../../../api/AuthorOperationException.md) See Also:
        * [DeleteColumnOperationBase.updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider, ro.sync.ecss.extensions.api.node.AuthorElement, int, int)](../DeleteColumnOperationBase.md#updateTableColSpan(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorTableCellSpanProvider,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
