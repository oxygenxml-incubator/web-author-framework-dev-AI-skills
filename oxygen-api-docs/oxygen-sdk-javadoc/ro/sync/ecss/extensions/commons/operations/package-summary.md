# Package ro.sync.ecss.extensions.commons.operations

package ro.sync.ecss.extensions.commons.operations
    Related Packages
Package

Description
 [ro.sync.ecss.extensions.commons](../package-summary.md)
Common implementations for Docbook, DITA, TEI and XHTML (Java source also available in the Author SDK).
  [ro.sync.ecss.extensions.commons.operations.text](text/package-summary.md)

 [ro.sync.ecss.extensions.commons.editor](../editor/package-summary.md)

 [ro.sync.ecss.extensions.commons.id](../id/package-summary.md)

 [ro.sync.ecss.extensions.commons.imagemap](../imagemap/package-summary.md)

 [ro.sync.ecss.extensions.commons.sort](../sort/package-summary.md)

 [ro.sync.ecss.extensions.commons.ui](../ui/package-summary.md)

     All Classes and InterfacesInterfacesClasses
Class

Description
 [ChangeAttributeOperation](ChangeAttributeOperation.md)
An implementation of an operation to change the value of an attribute.
  [ChangeAttributesOperation](ChangeAttributesOperation.md)
Operation that can change/insert/remove one or more attributes of one or more elements.
  [ChangePseudoClassesOperation](ChangePseudoClassesOperation.md)
An implementation of an operation to set a list of pseudo class values to nodes identified by an XPath expression and to remove a list of values from nodes identified by an XPath expression.
  [CommonsOperationsUtil](CommonsOperationsUtil.md)
Util methods for common Author operations.
  [CommonsOperationsUtil.ConversionElementHelper](CommonsOperationsUtil.ConversionElementHelper.md)
Interface used to check the elements that will be converted in other elements (table cells or list entries)
  [CommonsOperationsUtil.SelectedFragmentInfo](CommonsOperationsUtil.SelectedFragmentInfo.md)
Class containing the new fragment and info about it.
  [DefaultExtensions](DefaultExtensions.md)
Interface containing all the default operation distributed with Oxygen.
  [DeleteElementOperation](DeleteElementOperation.md)
An implementation of a delete operation that deletes the node at caret.
  [DeleteElementsOperation](DeleteElementsOperation.md)
An implementation of a delete operation that deletes all the nodes identified by a XPath expression.
  [EditImageMapOperation](EditImageMapOperation.md)
Operation used to edit an ImageMap in some documents.
  [ExecuteCommandLineOperation](ExecuteCommandLineOperation.md)
Author operation allowing the execution of command lines.
  [ExecuteCustomizableTransformationScenarioOperation](ExecuteCustomizableTransformationScenarioOperation.md)
An implementation of an operation which runs a single transformation scenario.
  [ExecuteMultipleActionsOperation](ExecuteMultipleActionsOperation.md)
An implementation of an operation which runs a sequence of actions, defined as a list of IDs.
  [ExecuteMultipleWebappCompatibleActionsOperation](ExecuteMultipleWebappCompatibleActionsOperation.md)
An implementation of an operation which runs a sequence of webapp-compatible ([WebappCompatible](../../api/WebappCompatible.md)) actions, defined as a list of IDs.
  [ExecuteTransformationScenariosOperation](ExecuteTransformationScenariosOperation.md)
An implementation of an operation which runs a certain transformation scenario.
  [ExecuteValidationScenariosOperation](ExecuteValidationScenariosOperation.md)
An implementation of an operation which runs validation scenarios.
  [GetCurrentElementSaxonExtension](GetCurrentElementSaxonExtension.md)
Returns the current element for an XSLT operation.
  [InsertEquationOperation](InsertEquationOperation.md)
Operation used to insert an MathML Equation in any documents.
  [InsertFragmentOperation](InsertFragmentOperation.md)
An implementation of an insert operation for an argument of type fragment.
  [InsertListOperation](InsertListOperation.md)
Operation used to convert a selection to an ordered/unordered list.
  [InsertOrReplaceFragmentOperation](InsertOrReplaceFragmentOperation.md)
Identical with [InsertFragmentOperation](InsertFragmentOperation.md) with the difference that the selection will be removed.
  [InsertOrReplaceTextOperation](InsertOrReplaceTextOperation.md)
An implementation of an insert/replace operation for an argument of type [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html).
  [InsertXIncludeOperation](InsertXIncludeOperation.md)
Insert an XInclude.
  [InvokeAIActionOperation](InvokeAIActionOperation.md)
Author operation which invokes an AI action by ID.
  [JSOperation](JSOperation.md)
An implementation of an operation that allows you to call the Java API from custom JavaScript content.
  [MoveBlockAuthorOperation](MoveBlockAuthorOperation.md)
Operation capable of moving the block element from the caret or the selected block elements by one position up or down.
  [MoveCaretOperation](MoveCaretOperation.md)
Author operation capable of moving the caret relative to an XML node identified by an XPath expression.
  [MoveCaretUtil](MoveCaretUtil.md)
Utility to detect an editor variable in the Author page and move the caret to that place.
  [MoveElementOperation](MoveElementOperation.md)
Flexible operation for moving an element to another location.
  [OpenInSystemAppOperation](OpenInSystemAppOperation.md)
Detects the application that is associated with the given file in the OS and uses it to open the file.
  [PromoteDemoteItemOperation](PromoteDemoteItemOperation.md)
Operation that promotes or demotes a list item.
  [PseudoClassOperation](PseudoClassOperation.md)
A base class for the operations that changes a pseudo-class from an element.
  [ReloadContentOperation](ReloadContentOperation.md)
Reloads the content of the editor by reading again from the URL used to open it.
  [RemovePseudoClassOperation](RemovePseudoClassOperation.md)
An operation that removes a pseudo-class from an element.
  [RenameElementOperation](RenameElementOperation.md)
An implementation of an operation that renames one or more elements identified by the given XPath expression.
  [ReplaceContentOperation](ReplaceContentOperation.md)
An implementation of an operation to replace the content of the document.
  [ReplaceElementContentOperation](ReplaceElementContentOperation.md)
Replaces the content of the: - specified element (indicated by an XPath expression) or - fully selected element or - element at caret (if the selection is empty or a node is not entirely selected).
  [SetPseudoClassOperation](SetPseudoClassOperation.md)
An operation that sets a pseudo-class to an element.
  [SetReadOnlyStatusOperation](SetReadOnlyStatusOperation.md)
Operation that sets the read-only status of a document.
  [ShowElementDocumentationOperation](ShowElementDocumentationOperation.md)
Operation that opens the associated specification html page for the current element.
  [StopCurrentTransformationScenarioOperation](StopCurrentTransformationScenarioOperation.md)
An implementation of an operation which stops the currently running transformation scenario.
  [SurroundWithFragmentOperation](SurroundWithFragmentOperation.md)
Surround with fragment operation.
  [SurroundWithTextOperation](SurroundWithTextOperation.md)
Surround with text operation.
  [ToggleCommentOperation](ToggleCommentOperation.md)
Provides an operation to toggle comment.
  [TogglePseudoClassOperation](TogglePseudoClassOperation.md)
An implementation of an operation to toggle on/off the pseudo-class of an element.
  [ToggleSurroundWithElementOperation](ToggleSurroundWithElementOperation.md)
Toggle "surround with element" operation.
  [TransformOperation](TransformOperation.md)
An implementation of an operation to apply a script (XSLT or XQuery) on a element and replacing it with the result of the transformation or inserting the result in the document.
  [UnwrapTagsOperation](UnwrapTagsOperation.md)
Unwrap tags operation.
  [WebappMarkAsSavedOperation](WebappMarkAsSavedOperation.md)
Operation that marks a webapp document as saved.
  [XQueryOperation](XQueryOperation.md)
An implementation of an operation to apply an XQuery script on a element and replacing it with the result of the XQuery transformation, or inserting the result in the document.
  [XQueryUpdateOperation](XQueryUpdateOperation.md)
An implementation of an operation that applies an XQuery Update script.
  [XSLTOperation](XSLTOperation.md)
An implementation of an operation to apply an XSLT stylesheet on a element and replacing it with the result of the XSLT transformation or inserting the result in the document.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
