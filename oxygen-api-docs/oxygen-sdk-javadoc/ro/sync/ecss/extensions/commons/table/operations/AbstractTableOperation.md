Package [ro.sync.ecss.extensions.commons.table.operations](package-summary.md)

# Class AbstractTableOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   Direct Known Subclasses: [DeleteColumnOperationBase](DeleteColumnOperationBase.md), [DeleteRowOperationBase](DeleteRowOperationBase.md), [InsertColumnOperationBase](InsertColumnOperationBase.md), [InsertRowOperationBase](InsertRowOperationBase.md), [InsertTableOperation](../../../docbook/table/InsertTableOperation.md), [JoinCellAboveBelowOperationBase](JoinCellAboveBelowOperationBase.md), [JoinOperationBase](JoinOperationBase.md), [JoinRowCellsOperationBase](JoinRowCellsOperationBase.md), [SplitCellAboveBelowOperationBase](SplitCellAboveBelowOperationBase.md), [SplitLeftRightOperationBase](SplitLeftRightOperationBase.md), [SplitOperationBase](SplitOperationBase.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class AbstractTableOperation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorOperation](../../../api/AuthorOperation.md)
Base class for table operations.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) [CHANGE_TRACKING_BEHAVIOR_ARGUMENT](#CHANGE_TRACKING_BEHAVIOR_ARGUMENT)
Argument descriptor for change tracking behavior.
  static final [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) [TABLE_INFO_ARGUMENT_DESCRIPTOR](#TABLE_INFO_ARGUMENT_DESCRIPTOR)
Argument descriptor for a table info argument.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TABLE_INFO_ARGUMENT_NAME](#TABLE_INFO_ARGUMENT_NAME)
The name of the table info argument.
  protected [AuthorTableHelper](AuthorTableHelper.md) [tableHelper](#tableHelper)
Table helper, has methods specific to each document type.

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [AbstractTableOperation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper))([AuthorTableHelper](AuthorTableHelper.md) authorTableHelper)
Constructor.
  [AbstractTableOperation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.table.operations.AuthorTableHelper,boolean))([AuthorTableHelper](AuthorTableHelper.md) authorTableHelper, boolean markAsChange)
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md) [createEmptyCell](#createEmptyCell(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) cell, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] skippedAttributes)
Create an [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md) representing an empty cell by duplicating the given cell without its content and skipping the specified attributes.
  final void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)
Perform the actual operation.
  protected abstract void [doOperationInternal](#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)
Perform the actual operation.
  protected int [findCellInsertionOffset](#findCellInsertionOffset(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorElement,int,int))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, int row, int column)
Find the offset in the document where a new entry (table cell) should be inserted for the given table row and column.
  protected [AuthorElement](../../../api/node/AuthorElement.md) [getElementAncestor](#getElementAncestor(ro.sync.ecss.extensions.api.node.AuthorNode,int))([AuthorNode](../../../api/node/AuthorNode.md) node, int type)
Search for an ancestor [AuthorNode](../../../api/node/AuthorNode.md) with the specified type.
  protected boolean [isElement](#isElement(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([AuthorNode](../../../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elemLocalName)
Test if a given [AuthorNode](../../../api/node/AuthorNode.md) is an element and has the a specific local name.
  protected boolean [isTableElement](#isTableElement(ro.sync.ecss.extensions.api.node.AuthorNode,int))([AuthorNode](../../../api/node/AuthorNode.md) node, int type)
Test if an [AuthorNode](../../../api/node/AuthorNode.md) is an element and it has one of the following types: [AuthorTableHelper.TYPE_CELL](AuthorTableHelper.md#TYPE_CELL), [AuthorTableHelper.TYPE_ROW](AuthorTableHelper.md#TYPE_ROW) or [AuthorTableHelper.TYPE_TABLE](AuthorTableHelper.md#TYPE_TABLE).

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [getArguments](../../../api/AuthorOperation.md#getArguments())
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../../api/Extension.md)
 [getDescription](../../../api/Extension.md#getDescription())
## Field Details

### CHANGE_TRACKING_BEHAVIOR_ARGUMENT

public static final [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) CHANGE_TRACKING_BEHAVIOR_ARGUMENT

Argument descriptor for change tracking behavior.

### TABLE_INFO_ARGUMENT_NAME

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TABLE_INFO_ARGUMENT_NAME

The name of the table info argument.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.table.operations.AbstractTableOperation.TABLE_INFO_ARGUMENT_NAME)

### TABLE_INFO_ARGUMENT_DESCRIPTOR

public static final [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) TABLE_INFO_ARGUMENT_DESCRIPTOR

Argument descriptor for a table info argument.

### tableHelper

protected [AuthorTableHelper](AuthorTableHelper.md) tableHelper

Table helper, has methods specific to each document type.

## Constructor Details

### AbstractTableOperation

public AbstractTableOperation([AuthorTableHelper](AuthorTableHelper.md) authorTableHelper)

Constructor.
  Parameters: authorTableHelper - Table helper, has methods specific to each document type.
### AbstractTableOperation

public AbstractTableOperation([AuthorTableHelper](AuthorTableHelper.md) authorTableHelper, boolean markAsChange)

Constructor.
  Parameters: authorTableHelper - Table helper, has methods specific to each document type. markAsChange - true if the operation result is marked as a change.
## Method Details

### getElementAncestor

protected [AuthorElement](../../../api/node/AuthorElement.md) getElementAncestor([AuthorNode](../../../api/node/AuthorNode.md) node, int type)

Search for an ancestor [AuthorNode](../../../api/node/AuthorNode.md) with the specified type.
  Parameters: node - The starting node. type - The type of the ancestor. Returns: The ancestor node of the given node or the node itself if the type matches.
### isElement

protected boolean isElement([AuthorNode](../../../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elemLocalName)

Test if a given [AuthorNode](../../../api/node/AuthorNode.md) is an element and has the a specific local name.
  Parameters: node - The [AuthorNode](../../../api/node/AuthorNode.md) to be checked. elemLocalName - The local name of the element. Returns: true if the given [AuthorNode](../../../api/node/AuthorNode.md) is an element and its local name matches the given string.
### isTableElement

protected boolean isTableElement([AuthorNode](../../../api/node/AuthorNode.md) node, int type)

Test if an [AuthorNode](../../../api/node/AuthorNode.md) is an element and it has one of the following types: [AuthorTableHelper.TYPE_CELL](AuthorTableHelper.md#TYPE_CELL), [AuthorTableHelper.TYPE_ROW](AuthorTableHelper.md#TYPE_ROW) or [AuthorTableHelper.TYPE_TABLE](AuthorTableHelper.md#TYPE_TABLE).
  Parameters: node - The node to be checked. type - The type to search for. Returns: true if the node is an element with the specified type.
### findCellInsertionOffset

protected int findCellInsertionOffset([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) tableElement, int row, int column)

Find the offset in the document where a new entry (table cell) should be inserted for the given table row and column.
  Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility tableElement - The element rendered as a table. Its 'display' CSS property is set to 'table'. row - The table row where the insertion will occur, 0 based. column - The column where the insertion will occur, 0 based. Returns: The offset where the new entry should be inserted.
### createEmptyCell

protected [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md) createEmptyCell([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorElement](../../../api/node/AuthorElement.md) cell, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] skippedAttributes)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create an [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md) representing an empty cell by duplicating the given cell without its content and skipping the specified attributes.
  Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility cell - The reference cell. skippedAttributes - The attributes which should not be copied. Returns: The document fragment representing the empty cell created starting from the original cell. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the fragment cannot be created.
### doOperation

public final void doOperation([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorOperation](../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation. You can check if the operation was invoked from the oXygen standalone application or from the oXygen plugin for Eclipse by using the method: [ApplicationInformationAccess.getPlatform()](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()). To get to the [Workspace](../../../../../exml/workspace/api/Workspace.md) you may use: [AuthorAccess.getWorkspaceAccess()](../../../api/AuthorAccess.md#getWorkspaceAccess()).
  Specified by: [doOperation](../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in interface [AuthorOperation](../../../api/AuthorOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AuthorOperation.doOperation(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### doOperationInternal

protected abstract void doOperationInternal([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Perform the actual operation.
  Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - Thrown when one or more arguments are illegal. [AuthorOperationException](../../../api/AuthorOperationException.md) - Thrown when the operation fails.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
