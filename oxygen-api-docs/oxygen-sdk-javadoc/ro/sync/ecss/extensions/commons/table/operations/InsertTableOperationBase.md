Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Interface InsertTableOperationBase
    All Known Implementing Classes: [InsertTableOperation](xhtml/InsertTableOperation.md), [InsertTableOperation](../../../dita/map/table/InsertTableOperation.md), [InsertTableOperation](../../../dita/topic/table/InsertTableOperation.md), [InsertTableOperation](../../../docbook/table/InsertTableOperation.md), [InsertTableOperation](../../../tei/table/InsertTableOperation.md)   @API(type=INTERNAL, src=PUBLIC) public interface InsertTableOperationBase
Base for insert Author table operation.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [insertTable](#insertTable(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,boolean,ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper,ro.sync.ecss.extensions.commons.table.operations.TableInfo))([AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)[] fragments, boolean cellsFragments, [AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorTableHelper](AuthorTableHelper.md) tableHelper, [TableInfo](TableInfo.md) tableInfo)
If the fragments array is not null, this method converts the given fragments array into a table.

## Method Details

### insertTable

void insertTable([AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)[] fragments, boolean cellsFragments, [AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace, [AuthorTableHelper](AuthorTableHelper.md) tableHelper, [TableInfo](TableInfo.md) tableInfo)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

If the fragments array is not null, this method converts the given fragments array into a table. Each fragments will correspond to a cell. The resulting table will have one column and as many rows as fragments length. If no fragment is provided an empty table is inserted (a dialog is shown to choose all the table properties)
  Parameters: fragments - An array of AuthorDocumentFragments that are used as content of the inserted cells. cellsFragments - If the value is true then the fragments where originally cells. authorAccess - The author access. namespace - The namespace. tableHelper - The table helper. tableInfo - The details about table creation. If null, a dialog is presented to let the user choose the details. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md)
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
