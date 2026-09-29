Package [ro.sync.ecss.extensions.api.webapp.cc](package-summary.md)

# Interface ContentCompletionManager
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ContentCompletionManager
This class offers support for actions with content completion such as: insert element, surround with tags and rename element. For every action we have two methods: one that returns a list of proposals to be presented to the user and another one that performs the action based on the user choice. Users of the API will typically show a dialog with the proposals and after the user selects one of the call the second method to finish the action.
  Since: 15.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [executeAction](#executeAction(ro.sync.ecss.extensions.api.webapp.cc.CCItemProxy,ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel))([CCItemProxy](CCItemProxy.md) ccItem, [AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)
Inserts an element from content completion which is provided from a custom content completion action.
  void [executeInsert](#executeInsert(ro.sync.ecss.extensions.api.webapp.cc.CCItemProxy,ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel))([CCItemProxy](CCItemProxy.md) ccItem, [AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)
Executes the insert element action.
  void [executeInsertInvalid](#executeInsertInvalid(ro.sync.ecss.extensions.api.webapp.cc.CCItemProxy,ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel))([CCItemProxy](CCItemProxy.md) ccItem, [AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)
Inserts an element from content completion which is invalid at the caret position.
  void [executeNewLine](#executeNewLine(ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel))([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)
Executes a new line insertion.
  void [executeRename](#executeRename(ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel,ro.sync.ecss.extensions.api.webapp.cc.CCItemProxy))([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel, [CCItemProxy](CCItemProxy.md) ccItem)
Executes the rename operation.
  void [executeSplit](#executeSplit(ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel))([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)
Splits the element at current caret offset.
  void [executeSplit](#executeSplit(ro.sync.ecss.extensions.api.webapp.cc.CCItemProxy,ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel))([CCItemProxy](CCItemProxy.md) ccItem, [AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)
Splits the element chosen by the user.
  void [executeSurround](#executeSurround(ro.sync.ecss.extensions.api.webapp.cc.CCItemProxy,ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel))([CCItemProxy](CCItemProxy.md) ccItem, [AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)
Surrounds the current selection with an element that has the specified render string and type as chosen by the user/
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CCItemProxy](CCItemProxy.md)> [getAllPossibleElementsForInsert](#getAllPossibleElementsForInsert())()
Returns all possible elements defined by the schema, including those that are not valid to be inserted at the caret position.
  [CCItemProxy](CCItemProxy.md) [getNewLineProposal](#getNewLineProposal(ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel))([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)
If the selection/caret is inside a space preserve content it will return a proposal for inserting a new line.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CCItemProxy](CCItemProxy.md)> [getProposedElementsForInsert](#getProposedElementsForInsert(ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel))([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)
Returns the proposals for element insertions at the current offset.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CCItemProxy](CCItemProxy.md)> [getProposedElementsForRename](#getProposedElementsForRename(ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel))([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)
Returns the proposals for renaming.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CCItemProxy](CCItemProxy.md)> [getProposedElementsForSurround](#getProposedElementsForSurround(ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel))([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)
Returns the proposals for a tag to surround the current selection with.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CCItemProxy](CCItemProxy.md)> [getProposedElementsToSplit](#getProposedElementsToSplit(ro.sync.ecss.extensions.api.AuthorSelectionAndCaretModel))([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)
Returns the block elements around the caret position that can be split.

## Method Details

### getProposedElementsForInsert

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CCItemProxy](CCItemProxy.md)> getProposedElementsForInsert([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Returns the proposals for element insertions at the current offset.
  Parameters: selectionModel - The selection and caret model of the document. Returns: The proposals for element insertions at the current offset. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### getAllPossibleElementsForInsert

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CCItemProxy](CCItemProxy.md)> getAllPossibleElementsForInsert()

Returns all possible elements defined by the schema, including those that are not valid to be inserted at the caret position.
  Returns: The list of all possible elements.
### executeInsert

void executeInsert([CCItemProxy](CCItemProxy.md) ccItem, [AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [ItemNotFoundException](ItemNotFoundException.md)

Executes the insert element action.
  Parameters: ccItem - The content completion item chosen by the user. selectionModel - The selection and caret model of the document. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [ItemNotFoundException](ItemNotFoundException.md)
### getProposedElementsForRename

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CCItemProxy](CCItemProxy.md)> getProposedElementsForRename([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Returns the proposals for renaming.
  Parameters: selectionModel - The selection and caret model of the document. The selection should be either collapsed, or an entire element should be selected. Returns: The proposed elements for rename. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If the selection does not comply with the restrictions above.
### executeRename

void executeRename([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel, [CCItemProxy](CCItemProxy.md) ccItem)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Executes the rename operation.
  Parameters: selectionModel - The selection and caret model of the document. ccItem - The content completion item chosen for rename. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### executeNewLine

void executeNewLine([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Executes a new line insertion.
  Parameters: selectionModel - The selection and caret model of the document. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### getProposedElementsForSurround

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CCItemProxy](CCItemProxy.md)> getProposedElementsForSurround([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Returns the proposals for a tag to surround the current selection with.
  Parameters: selectionModel - The selection and caret model of the document. Returns: The list of proposals. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### executeSurround

void executeSurround([CCItemProxy](CCItemProxy.md) ccItem, [AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [ItemNotFoundException](ItemNotFoundException.md)

Surrounds the current selection with an element that has the specified render string and type as chosen by the user/
  Parameters: ccItem - The content completion item chosen by the user. selectionModel - The selection and caret model of the document. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [ItemNotFoundException](ItemNotFoundException.md)
### getProposedElementsToSplit

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CCItemProxy](CCItemProxy.md)> getProposedElementsToSplit([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Returns the block elements around the caret position that can be split.
  Parameters: selectionModel - The selection and caret model of the document. Returns: The list of block elements that can be split. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### executeSplit

void executeSplit([CCItemProxy](CCItemProxy.md) ccItem, [AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [ItemNotFoundException](ItemNotFoundException.md)

Splits the element chosen by the user.
  Parameters: ccItem - The element chosen by the user. selectionModel - The selection model of the document. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [ItemNotFoundException](ItemNotFoundException.md)
### executeSplit

void executeSplit([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)

Splits the element at current caret offset.
  Parameters: selectionModel - The selection and caret model of the document. Since: 19
### getNewLineProposal

[CCItemProxy](CCItemProxy.md) getNewLineProposal([AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

If the selection/caret is inside a space preserve content it will return a proposal for inserting a new line.
  Parameters: selectionModel - Selection and caret model. Returns: A new line insertion proposal or null if the caret is not in a space preserve context. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - Bad offsets.
### executeInsertInvalid

void executeInsertInvalid([CCItemProxy](CCItemProxy.md) ccItem, [AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [ItemNotFoundException](ItemNotFoundException.md)

Inserts an element from content completion which is invalid at the caret position. Some schema aware strategies will be employed to find a good position to insert the element.
  Parameters: ccItem - The selected element. selectionModel - The selection. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [ItemNotFoundException](ItemNotFoundException.md)
### executeAction

void executeAction([CCItemProxy](CCItemProxy.md) ccItem, [AuthorSelectionAndCaretModel](../../AuthorSelectionAndCaretModel.md) selectionModel)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [ItemNotFoundException](ItemNotFoundException.md)

Inserts an element from content completion which is provided from a custom content completion action.
  Parameters: ccItem - The selected element. selectionModel - The selection. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [ItemNotFoundException](ItemNotFoundException.md) Since: 19
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
