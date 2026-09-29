Package [ro.sync.ecss.extensions.tei](package-summary.md)

# Class TEIAuthorTableOperationsHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.table.operations.AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md)
        * ro.sync.ecss.extensions.tei.TEIAuthorTableOperationsHandler
   @API(type=INTERNAL, src=PUBLIC) public class TEIAuthorTableOperationsHandler extends [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md)
Author table operations handler for TEIP4 framework.

## Constructor Summary
 Constructors
Constructor

Description
 [TEIAuthorTableOperationsHandler](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorElement](../api/node/AuthorElement.md) [getTableElementContainingOffset](#getTableElementContainingOffset(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](../api/AuthorAccess.md) access, int offset)
Returns the element representing the table that contains the given offset.
  boolean [handleDeleteColumn](#handleDeleteColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteColumnArguments))([AuthorTableDeleteColumnArguments](../api/table/operations/AuthorTableDeleteColumnArguments.md) arguments)
Handles delete column operation.
  boolean [handleDeleteRow](#handleDeleteRow(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowArguments))([AuthorTableDeleteRowArguments](../api/table/operations/AuthorTableDeleteRowArguments.md) arguments)
Handles delete row operation.
  boolean [handleDeleteRows](#handleDeleteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowsArguments))([AuthorTableDeleteRowsArguments](../api/table/operations/AuthorTableDeleteRowsArguments.md) arguments)
Handles delete rows operation.
  boolean [handleInsertColumn](#handleInsertColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertColumnArguments))([AuthorTableInsertColumnArguments](../api/table/operations/AuthorTableInsertColumnArguments.md) tablePasteColumnsArgs)
Handles insert column operation.

### Methods inherited from class ro.sync.ecss.extensions.api.table.operations.[AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md)
 [getColumnSpecification](../api/table/operations/AuthorTableOperationsHandler.md#getColumnSpecification(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int)), [handleAttributeChange](../api/table/operations/AuthorTableOperationsHandler.md#handleAttributeChange(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue)), [handleCreateTable](../api/table/operations/AuthorTableOperationsHandler.md#handleCreateTable(ro.sync.ecss.extensions.api.table.operations.AuthorTableArguments)), [handlePasteRows](../api/table/operations/AuthorTableOperationsHandler.md#handlePasteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertRowArguments)), [handleRemoveInvalidColNamesFromTableCells](../api/table/operations/AuthorTableOperationsHandler.md#handleRemoveInvalidColNamesFromTableCells(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.util.List))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TEIAuthorTableOperationsHandler

public TEIAuthorTableOperationsHandler([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)

Constructor.
  Parameters: namespace - The namespace.
## Method Details

### handleInsertColumn

public boolean handleInsertColumn([AuthorTableInsertColumnArguments](../api/table/operations/AuthorTableInsertColumnArguments.md) tablePasteColumnsArgs)throws [AuthorOperationException](../api/AuthorOperationException.md)
 Description copied from class: [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md#handleInsertColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertColumnArguments))
Handles insert column operation. This method is called when pasting or dropping content for which the [SelectionInterpretationMode.TABLE_COLUMN](../api/SelectionInterpretationMode.md#TABLE_COLUMN) interpretation mode was imposed.  The [SelectionInterpretationMode.TABLE_COLUMN](../api/SelectionInterpretationMode.md#TABLE_COLUMN) interpretation mode is already set by default by the application when a table column is selected. It can be also imposed from the [AuthorSelectionModel.setSelectionInterpretationMode(SelectionInterpretationMode)](../api/AuthorSelectionModel.md#setSelectionInterpretationMode(ro.sync.ecss.extensions.api.SelectionInterpretationMode))method, for any selection content. For instance, when two paragraphs are copied, the clipboard object contains a list with two Author document fragments (one for each paragraph). If the selection interpretation mode is imposed to [SelectionInterpretationMode.TABLE_COLUMN](../api/SelectionInterpretationMode.md#TABLE_COLUMN), when pasting the fragments this method is called. The fragments array are included in the argument object.
  Overrides: [handleInsertColumn](../api/table/operations/AuthorTableOperationsHandler.md#handleInsertColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertColumnArguments)) in class [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) Parameters: tablePasteColumnsArgs - The arguments for insert column operation like: the offset where the column is inserted, the array containing the cells fragments that compose an Author table column, information about column width specification, the Author access. Returns: true if the insert column operation succeeds. Throws: [AuthorOperationException](../api/AuthorOperationException.md) - An insert column operation exception. If the [AuthorOperationException.isOperationRejectedOnPurpose()](../api/AuthorOperationException.md#isOperationRejectedOnPurpose()) method of this exception returns true, the exception is presented to the user. See Also:
        * [AuthorTableOperationsHandler.handleInsertColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertColumnArguments)](../api/table/operations/AuthorTableOperationsHandler.md#handleInsertColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertColumnArguments))

### handleDeleteColumn

public boolean handleDeleteColumn([AuthorTableDeleteColumnArguments](../api/table/operations/AuthorTableDeleteColumnArguments.md) arguments)throws [AuthorOperationException](../api/AuthorOperationException.md)
 Description copied from class: [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md#handleDeleteColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteColumnArguments))
Handles delete column operation. This method is called when deleting content (by drag and drop or cut operations) for which the [SelectionInterpretationMode.TABLE_COLUMN](../api/SelectionInterpretationMode.md#TABLE_COLUMN) interpretation mode was imposed.  The [SelectionInterpretationMode.TABLE_COLUMN](../api/SelectionInterpretationMode.md#TABLE_COLUMN) interpretation mode is already set by default by the application when a table column is selected. It can be also imposed from the [AuthorSelectionModel.setSelectionInterpretationMode(SelectionInterpretationMode)](../api/AuthorSelectionModel.md#setSelectionInterpretationMode(ro.sync.ecss.extensions.api.SelectionInterpretationMode))method, for any selection content. For instance, when two paragraphs are copied, the clipboard object contains a list with two Author document fragments (one for each paragraph). If the selection interpretation mode is imposed to [SelectionInterpretationMode.TABLE_COLUMN](../api/SelectionInterpretationMode.md#TABLE_COLUMN), when deleting the fragments this method is called. The fragments array are included in the argument object.
  Overrides: [handleDeleteColumn](../api/table/operations/AuthorTableOperationsHandler.md#handleDeleteColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteColumnArguments)) in class [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) Parameters: arguments - The arguments for delete column operation (like the Author access and the column cells start and end offsets). Returns: true if the delete column operation succeeds. Throws: [AuthorOperationException](../api/AuthorOperationException.md) - A delete column operation exception. If the [AuthorOperationException.isOperationRejectedOnPurpose()](../api/AuthorOperationException.md#isOperationRejectedOnPurpose()) method of this exception returns true, the exception is presented to the user. See Also:
        * [AuthorTableOperationsHandler.handleDeleteColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteColumnArguments)](../api/table/operations/AuthorTableOperationsHandler.md#handleDeleteColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteColumnArguments))

### handleDeleteRow

public boolean handleDeleteRow([AuthorTableDeleteRowArguments](../api/table/operations/AuthorTableDeleteRowArguments.md) arguments)throws [AuthorOperationException](../api/AuthorOperationException.md)
 Description copied from class: [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md#handleDeleteRow(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowArguments))
Handles delete row operation. This method is called when deleting content (by drag and drop or cut operations) for which the [SelectionInterpretationMode.TABLE_ROW](../api/SelectionInterpretationMode.md#TABLE_ROW) interpretation mode was imposed.  The [SelectionInterpretationMode.TABLE_ROW](../api/SelectionInterpretationMode.md#TABLE_ROW) interpretation mode is already set by default by the application when a table row is selected. It can be also imposed from the [AuthorSelectionModel.setSelectionInterpretationMode(SelectionInterpretationMode)](../api/AuthorSelectionModel.md#setSelectionInterpretationMode(ro.sync.ecss.extensions.api.SelectionInterpretationMode))method, for any selection content. For instance, when two paragraphs are copied, the clipboard object contains a list with two Author document fragments (one for each paragraph). If the selection interpretation mode is imposed to [SelectionInterpretationMode.TABLE_ROW](../api/SelectionInterpretationMode.md#TABLE_ROW), when deleting the fragments this method is called. The fragments array are included in the argument object.
  Overrides: [handleDeleteRow](../api/table/operations/AuthorTableOperationsHandler.md#handleDeleteRow(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowArguments)) in class [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) Parameters: arguments - The arguments for delete row operation (like the Author access and the content interval of the row element that must be deleted). Returns: true if the delete row operation succeeds. Throws: [AuthorOperationException](../api/AuthorOperationException.md) - A delete row operation exception. If the [AuthorOperationException.isOperationRejectedOnPurpose()](../api/AuthorOperationException.md#isOperationRejectedOnPurpose()) method of this exception returns true, the exception is presented to the user. See Also:
        * [AuthorTableOperationsHandler.handleDeleteRow(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowArguments)](../api/table/operations/AuthorTableOperationsHandler.md#handleDeleteRow(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowArguments))

### handleDeleteRows

public boolean handleDeleteRows([AuthorTableDeleteRowsArguments](../api/table/operations/AuthorTableDeleteRowsArguments.md) arguments)throws [AuthorOperationException](../api/AuthorOperationException.md)
 Description copied from class: [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md#handleDeleteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowsArguments))
Handles delete rows operation. All the rows that intersects the given content intervals will be deleted. This method is called when deleting content (by drag and drop or cut operations) for which the [SelectionInterpretationMode.TABLE_ROW](../api/SelectionInterpretationMode.md#TABLE_ROW) interpretation mode was imposed.  The [SelectionInterpretationMode.TABLE_ROW](../api/SelectionInterpretationMode.md#TABLE_ROW) interpretation mode is already set by default by the application when a table row is selected. It can be also imposed from the [AuthorSelectionModel.setSelectionInterpretationMode(SelectionInterpretationMode)](../api/AuthorSelectionModel.md#setSelectionInterpretationMode(ro.sync.ecss.extensions.api.SelectionInterpretationMode))method, for any selection content. For instance, when two paragraphs are copied, the clipboard object contains a list with two Author document fragments (one for each paragraph). If the selection interpretation mode is imposed to [SelectionInterpretationMode.TABLE_ROW](../api/SelectionInterpretationMode.md#TABLE_ROW), when deleting the fragments this method is called.
  Overrides: [handleDeleteRows](../api/table/operations/AuthorTableOperationsHandler.md#handleDeleteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowsArguments)) in class [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) Parameters: arguments - The arguments for delete rows operation (like the Author access and the content intervals that determine the rows element that must be deleted). Returns: true if the delete rows operation succeeds. Throws: [AuthorOperationException](../api/AuthorOperationException.md) - A delete row operation exception. If the [AuthorOperationException.isOperationRejectedOnPurpose()](../api/AuthorOperationException.md#isOperationRejectedOnPurpose()) method of this exception returns true, the exception is presented to the user. See Also:
        * [AuthorTableOperationsHandler.handleDeleteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowsArguments)](../api/table/operations/AuthorTableOperationsHandler.md#handleDeleteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowsArguments))

### getTableElementContainingOffset

public [AuthorElement](../api/node/AuthorElement.md) getTableElementContainingOffset([AuthorAccess](../api/AuthorAccess.md) access, int offset)
 Description copied from class: [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md#getTableElementContainingOffset(ro.sync.ecss.extensions.api.AuthorAccess,int))
Returns the element representing the table that contains the given offset. This method can be used to obtain the closest table that contains the given offset.
  Overrides: [getTableElementContainingOffset](../api/table/operations/AuthorTableOperationsHandler.md#getTableElementContainingOffset(ro.sync.ecss.extensions.api.AuthorAccess,int)) in class [AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md) Parameters: access - Access to Author operations. offset - The offset to search the parent table element for. Returns: The table node that contains the given offset. See Also:
        * [AuthorTableOperationsHandler.getTableElementContainingOffset(ro.sync.ecss.extensions.api.AuthorAccess, int)](../api/table/operations/AuthorTableOperationsHandler.md#getTableElementContainingOffset(ro.sync.ecss.extensions.api.AuthorAccess,int))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
