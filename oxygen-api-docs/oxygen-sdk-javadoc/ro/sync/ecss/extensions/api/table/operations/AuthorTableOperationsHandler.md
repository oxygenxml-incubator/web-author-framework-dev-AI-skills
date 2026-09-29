Package [ro.sync.ecss.extensions.api.table.operations](package-summary.md)

# Class AuthorTableOperationsHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.table.operations.AuthorTableOperationsHandler
   Direct Known Subclasses: [DITAAuthorTableOperationsHandler](../../../dita/DITAAuthorTableOperationsHandler.md), [DITAMapAuthorTableOperationsHandler](../../../dita/map/DITAMapAuthorTableOperationsHandler.md), [DocbookAuthorTableOperationsHandler](../../../docbook/DocbookAuthorTableOperationsHandler.md), [TEIAuthorTableOperationsHandler](../../../tei/TEIAuthorTableOperationsHandler.md), [XHTMLAuthorTableOperationsHandler](../../../xhtml/XHTMLAuthorTableOperationsHandler.md)   @API(type=EXTENDABLE, src=PUBLIC) public class AuthorTableOperationsHandler extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Handler for Author table operations. It should be implemented when the author extension being developed offers support for editing data in tabular form.
  Since: 14
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorTableOperationsHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 [TableColumnSpecificationInformation](TableColumnSpecificationInformation.md) [getColumnSpecification](#getColumnSpecification(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int))([AuthorAccess](../../AuthorAccess.md) access, [AuthorElement](../../node/AuthorElement.md) tableElement, int columnIndex)
Returns the column specification information of a table column.
  [AuthorElement](../../node/AuthorElement.md) [getTableElementContainingOffset](#getTableElementContainingOffset(ro.sync.ecss.extensions.api.AuthorAccess,int))([AuthorAccess](../../AuthorAccess.md) access, int offset)
Returns the element representing the table that contains the given offset.
  boolean [handleAttributeChange](#handleAttributeChange(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue))([AuthorAccess](../../AuthorAccess.md) authorAccess, [AuthorElement](../../node/AuthorElement.md) currentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AttrValue](../../node/AttrValue.md) newValue)
Handle an attribute change.
  boolean [handleCreateTable](#handleCreateTable(ro.sync.ecss.extensions.api.table.operations.AuthorTableArguments))([AuthorTableArguments](AuthorTableArguments.md) arguments)
Handles how a new table is created from cells selected from other table.
  boolean [handleDeleteColumn](#handleDeleteColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteColumnArguments))([AuthorTableDeleteColumnArguments](AuthorTableDeleteColumnArguments.md) arguments)
Handles delete column operation.
  boolean [handleDeleteRow](#handleDeleteRow(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowArguments))([AuthorTableDeleteRowArguments](AuthorTableDeleteRowArguments.md) arguments)  Deprecated.
Use [handleDeleteRows(AuthorTableDeleteRowsArguments)](#handleDeleteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowsArguments)) method instead.
   boolean [handleDeleteRows](#handleDeleteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowsArguments))([AuthorTableDeleteRowsArguments](AuthorTableDeleteRowsArguments.md) arguments)
Handles delete rows operation.
  boolean [handleInsertColumn](#handleInsertColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertColumnArguments))([AuthorTableInsertColumnArguments](AuthorTableInsertColumnArguments.md) arguments)
Handles insert column operation.
  boolean [handlePasteRows](#handlePasteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertRowArguments))([AuthorTableInsertRowArguments](AuthorTableInsertRowArguments.md) arguments)
Handles paste rows operation.
  void [handleRemoveInvalidColNamesFromTableCells](#handleRemoveInvalidColNamesFromTableCells(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.util.List))([AuthorAccess](../../AuthorAccess.md) authorAccess, [AuthorElement](../../node/AuthorElement.md) tableElement, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../node/AuthorElement.md)> cells)
Remove from each cell attributes pointing to missing column names (usually namest, nameend, colname).

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorTableOperationsHandler

public AuthorTableOperationsHandler()

## Method Details

### handleInsertColumn

public boolean handleInsertColumn([AuthorTableInsertColumnArguments](AuthorTableInsertColumnArguments.md) arguments)throws [AuthorOperationException](../../AuthorOperationException.md)

Handles insert column operation. This method is called when pasting or dropping content for which the [SelectionInterpretationMode.TABLE_COLUMN](../../SelectionInterpretationMode.md#TABLE_COLUMN) interpretation mode was imposed.  The [SelectionInterpretationMode.TABLE_COLUMN](../../SelectionInterpretationMode.md#TABLE_COLUMN) interpretation mode is already set by default by the application when a table column is selected. It can be also imposed from the [AuthorSelectionModel.setSelectionInterpretationMode(SelectionInterpretationMode)](../../AuthorSelectionModel.md#setSelectionInterpretationMode(ro.sync.ecss.extensions.api.SelectionInterpretationMode))method, for any selection content. For instance, when two paragraphs are copied, the clipboard object contains a list with two Author document fragments (one for each paragraph). If the selection interpretation mode is imposed to [SelectionInterpretationMode.TABLE_COLUMN](../../SelectionInterpretationMode.md#TABLE_COLUMN), when pasting the fragments this method is called. The fragments array are included in the argument object.
  Parameters: arguments - The arguments for insert column operation like: the offset where the column is inserted, the array containing the cells fragments that compose an Author table column, information about column width specification, the Author access. Returns: true if the insert column operation succeeds. Throws: [AuthorOperationException](../../AuthorOperationException.md) - An insert column operation exception. If the [AuthorOperationException.isOperationRejectedOnPurpose()](../../AuthorOperationException.md#isOperationRejectedOnPurpose()) method of this exception returns true, the exception is presented to the user.
### handleDeleteColumn

public boolean handleDeleteColumn([AuthorTableDeleteColumnArguments](AuthorTableDeleteColumnArguments.md) arguments)throws [AuthorOperationException](../../AuthorOperationException.md)

Handles delete column operation. This method is called when deleting content (by drag and drop or cut operations) for which the [SelectionInterpretationMode.TABLE_COLUMN](../../SelectionInterpretationMode.md#TABLE_COLUMN) interpretation mode was imposed.  The [SelectionInterpretationMode.TABLE_COLUMN](../../SelectionInterpretationMode.md#TABLE_COLUMN) interpretation mode is already set by default by the application when a table column is selected. It can be also imposed from the [AuthorSelectionModel.setSelectionInterpretationMode(SelectionInterpretationMode)](../../AuthorSelectionModel.md#setSelectionInterpretationMode(ro.sync.ecss.extensions.api.SelectionInterpretationMode))method, for any selection content. For instance, when two paragraphs are copied, the clipboard object contains a list with two Author document fragments (one for each paragraph). If the selection interpretation mode is imposed to [SelectionInterpretationMode.TABLE_COLUMN](../../SelectionInterpretationMode.md#TABLE_COLUMN), when deleting the fragments this method is called. The fragments array are included in the argument object.
  Parameters: arguments - The arguments for delete column operation (like the Author access and the column cells start and end offsets). Returns: true if the delete column operation succeeds. Throws: [AuthorOperationException](../../AuthorOperationException.md) - A delete column operation exception. If the [AuthorOperationException.isOperationRejectedOnPurpose()](../../AuthorOperationException.md#isOperationRejectedOnPurpose()) method of this exception returns true, the exception is presented to the user.
### handleDeleteRow

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public boolean handleDeleteRow([AuthorTableDeleteRowArguments](AuthorTableDeleteRowArguments.md) arguments)throws [AuthorOperationException](../../AuthorOperationException.md)
 Deprecated.
Use [handleDeleteRows(AuthorTableDeleteRowsArguments)](#handleDeleteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowsArguments)) method instead.

Handles delete row operation. This method is called when deleting content (by drag and drop or cut operations) for which the [SelectionInterpretationMode.TABLE_ROW](../../SelectionInterpretationMode.md#TABLE_ROW) interpretation mode was imposed.  The [SelectionInterpretationMode.TABLE_ROW](../../SelectionInterpretationMode.md#TABLE_ROW) interpretation mode is already set by default by the application when a table row is selected. It can be also imposed from the [AuthorSelectionModel.setSelectionInterpretationMode(SelectionInterpretationMode)](../../AuthorSelectionModel.md#setSelectionInterpretationMode(ro.sync.ecss.extensions.api.SelectionInterpretationMode))method, for any selection content. For instance, when two paragraphs are copied, the clipboard object contains a list with two Author document fragments (one for each paragraph). If the selection interpretation mode is imposed to [SelectionInterpretationMode.TABLE_ROW](../../SelectionInterpretationMode.md#TABLE_ROW), when deleting the fragments this method is called. The fragments array are included in the argument object.
  Parameters: arguments - The arguments for delete row operation (like the Author access and the content interval of the row element that must be deleted). Returns: true if the delete row operation succeeds. Throws: [AuthorOperationException](../../AuthorOperationException.md) - A delete row operation exception. If the [AuthorOperationException.isOperationRejectedOnPurpose()](../../AuthorOperationException.md#isOperationRejectedOnPurpose()) method of this exception returns true, the exception is presented to the user.
### handleDeleteRows

public boolean handleDeleteRows([AuthorTableDeleteRowsArguments](AuthorTableDeleteRowsArguments.md) arguments)throws [AuthorOperationException](../../AuthorOperationException.md)

Handles delete rows operation. All the rows that intersects the given content intervals will be deleted. This method is called when deleting content (by drag and drop or cut operations) for which the [SelectionInterpretationMode.TABLE_ROW](../../SelectionInterpretationMode.md#TABLE_ROW) interpretation mode was imposed.  The [SelectionInterpretationMode.TABLE_ROW](../../SelectionInterpretationMode.md#TABLE_ROW) interpretation mode is already set by default by the application when a table row is selected. It can be also imposed from the [AuthorSelectionModel.setSelectionInterpretationMode(SelectionInterpretationMode)](../../AuthorSelectionModel.md#setSelectionInterpretationMode(ro.sync.ecss.extensions.api.SelectionInterpretationMode))method, for any selection content. For instance, when two paragraphs are copied, the clipboard object contains a list with two Author document fragments (one for each paragraph). If the selection interpretation mode is imposed to [SelectionInterpretationMode.TABLE_ROW](../../SelectionInterpretationMode.md#TABLE_ROW), when deleting the fragments this method is called.
  Parameters: arguments - The arguments for delete rows operation (like the Author access and the content intervals that determine the rows element that must be deleted). Returns: true if the delete rows operation succeeds. Throws: [AuthorOperationException](../../AuthorOperationException.md) - A delete row operation exception. If the [AuthorOperationException.isOperationRejectedOnPurpose()](../../AuthorOperationException.md#isOperationRejectedOnPurpose()) method of this exception returns true, the exception is presented to the user. [UnsupportedOperationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/UnsupportedOperationException.html) - if this method is not implemented. In this case, the [handleDeleteRow(AuthorTableDeleteRowArguments)](#handleDeleteRow(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowArguments)) operation is called for each content interval. Since: 18
### getTableElementContainingOffset

public [AuthorElement](../../node/AuthorElement.md) getTableElementContainingOffset([AuthorAccess](../../AuthorAccess.md) access, int offset)

Returns the element representing the table that contains the given offset. This method can be used to obtain the closest table that contains the given offset.
  Parameters: access - Access to Author operations. offset - The offset to search the parent table element for. Returns: The table node that contains the given offset.
### getColumnSpecification

public [TableColumnSpecificationInformation](TableColumnSpecificationInformation.md) getColumnSpecification([AuthorAccess](../../AuthorAccess.md) access, [AuthorElement](../../node/AuthorElement.md) tableElement, int columnIndex)

Returns the column specification information of a table column.  This information is requested when a column is copied or dragged and it can be used when the column must be inserted in the document (on paste or drop). The column specification is send as an argument to the [handleInsertColumn(AuthorTableInsertColumnArguments)](#handleInsertColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertColumnArguments)) method.
  Parameters: access - Access to Author operations. tableElement - The table that contains the column. columnIndex - The column index, 0 based. Returns: The column specification element. It can be null if there is no specification for this column.
### handleRemoveInvalidColNamesFromTableCells

public void handleRemoveInvalidColNamesFromTableCells([AuthorAccess](../../AuthorAccess.md) authorAccess, [AuthorElement](../../node/AuthorElement.md) tableElement, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../node/AuthorElement.md)> cells)throws [AuthorOperationException](../../AuthorOperationException.md)

Remove from each cell attributes pointing to missing column names (usually namest, nameend, colname).
  Parameters: authorAccess - The author access. tableElement - The table element. cells - The list of table cells. Throws: [AuthorOperationException](../../AuthorOperationException.md) Since: 19.1
### handleAttributeChange

public boolean handleAttributeChange([AuthorAccess](../../AuthorAccess.md) authorAccess, [AuthorElement](../../node/AuthorElement.md) currentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AttrValue](../../node/AttrValue.md) newValue)

Handle an attribute change.
  Parameters: authorAccess - The Author Access. currentElement - The current element. attributeName - The attribute name. newValue - The new value. Returns: true if the changed was handled, false to perform the default bahavior. Since: 19.1
### handlePasteRows

public boolean handlePasteRows([AuthorTableInsertRowArguments](AuthorTableInsertRowArguments.md) arguments)throws [AuthorOperationException](../../AuthorOperationException.md)

Handles paste rows operation. This method is called when pasting or dropping content for which the [SelectionInterpretationMode.TABLE_ROW](../../SelectionInterpretationMode.md#TABLE_ROW) interpretation mode was imposed.  The [SelectionInterpretationMode.TABLE_ROW](../../SelectionInterpretationMode.md#TABLE_ROW) interpretation mode is already set by default by the application when a table row is selected. It can be also imposed from the [AuthorSelectionModel.setSelectionInterpretationMode(SelectionInterpretationMode)](../../AuthorSelectionModel.md#setSelectionInterpretationMode(ro.sync.ecss.extensions.api.SelectionInterpretationMode))method, for any selection content. For instance, when two paragraphs are copied, the clipboard object contains a list with two Author document fragments (one for each paragraph). If the selection interpretation mode is imposed to [SelectionInterpretationMode.TABLE_ROW](../../SelectionInterpretationMode.md#TABLE_ROW), when pasting the fragments this method is called. The fragments array are included in the argument object.
  Parameters: arguments - The arguments for insert column operation like: the offset where the rows are inserted, the array containing the rows fragments, information about column width specification, the Author access. Returns: true if the paste rows operation succeeds. Throws: [AuthorOperationException](../../AuthorOperationException.md) - An insert rows operation exception. If the [AuthorOperationException.isOperationRejectedOnPurpose()](../../AuthorOperationException.md#isOperationRejectedOnPurpose()) method of this exception returns true, the exception is presented to the user.
### handleCreateTable

public boolean handleCreateTable([AuthorTableArguments](AuthorTableArguments.md) arguments)throws [AuthorOperationException](../../AuthorOperationException.md)

Handles how a new table is created from cells selected from other table.
  Parameters: arguments - The arguments for copied cells like: the offset where the rows are inserted, the array containing the rows fragments, how many rows and columns the new table should have, the Author access. Returns: true of the table was successfully created. Throws: [AuthorOperationException](../../AuthorOperationException.md) - A table creation exception. If the [AuthorOperationException.isOperationRejectedOnPurpose()](../../AuthorOperationException.md#isOperationRejectedOnPurpose()) method of this exception returns true, the exception is presented to the user. Since: 21.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
