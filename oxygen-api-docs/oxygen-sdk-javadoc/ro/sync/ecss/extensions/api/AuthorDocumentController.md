Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorDocumentController
    All Superinterfaces: [AuthorAttributesController](AuthorAttributesController.md), [AuthorPseudoClassController](AuthorPseudoClassController.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorDocumentControllerextends [AuthorAttributesController](AuthorAttributesController.md), [AuthorPseudoClassController](AuthorPseudoClassController.md)
Provides methods for modifying the Author document.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 void [addAuthorListener](#addAuthorListener(ro.sync.ecss.extensions.api.AuthorListener))([AuthorListener](AuthorListener.md) listener)
Add an Author listener to be notified about changes regarding the document and the document structure.
  void [addAuthorPersistentHighlightListener](#addAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener))([AuthorPersistentHighlightsListener](highlights/AuthorPersistentHighlightsListener.md) listener)  Deprecated.
Use [AuthorReviewController.addAuthorPersistentHighlightListener(AuthorPersistentHighlightsListener)](AuthorReviewController.md#addAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener)) instead
   void [addClipboardFragmentProcessor](#addClipboardFragmentProcessor(ro.sync.ecss.extensions.api.content.ClipboardFragmentProcessor))([ClipboardFragmentProcessor](content/ClipboardFragmentProcessor.md) clipboardFragmentProcessor)
Add a processor which can analyze and modify [AuthorDocumentFragment](node/AuthorDocumentFragment.md) objects before they are inserted in the Author.
  void [addPersistentHighlightsFilter](#addPersistentHighlightsFilter(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsFilter))([AuthorPersistentHighlightsFilter](highlights/AuthorPersistentHighlightsFilter.md) persistentHighlightsFilter)  Deprecated.
Use [AuthorReviewController.addPersistentHighlightsFilter(AuthorPersistentHighlightsFilter)](AuthorReviewController.md#addPersistentHighlightsFilter(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsFilter)) instead
   void [addUniqueAttributesProcessor](#addUniqueAttributesProcessor(ro.sync.ecss.extensions.api.UniqueAttributesProcessor))([UniqueAttributesProcessor](UniqueAttributesProcessor.md) uniqueAttributesProcessor)
Add a processor which is asked to automatically generate unique IDs after content has been inserted in the Author.
  void [beginCompoundEdit](#beginCompoundEdit())()
Begin a compound edit.
  void [cancelCompoundEdit](#cancelCompoundEdit())()
Cancel the current compound edit.
  [AuthorDocumentFragment](node/AuthorDocumentFragment.md) [createDocumentFragment](#createDocumentFragment(int,int))(int startOffset, int endOffset)
Create an Author content fragment containing a clone of the document content for the given range of offsets.
  [AuthorDocumentFragment](node/AuthorDocumentFragment.md) [createDocumentFragment](#createDocumentFragment(int,int,boolean))(int startOffset, int endOffset, boolean preserveTrackChange)
Create an Author content fragment containing a clone of the document content for the given range of offsets.
  [AuthorDocumentFragment](node/AuthorDocumentFragment.md) [createDocumentFragment](#createDocumentFragment(ro.sync.ecss.extensions.api.node.AuthorNode,boolean))([AuthorNode](node/AuthorNode.md) node, boolean copyContent)
Create a document fragment containing a copy of the node.
  [AuthorElement](node/AuthorElement.md) [createElement](#createElement(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName)
Creates an element.
  [AuthorDocumentFragment](node/AuthorDocumentFragment.md) [createNewDocumentFragmentInContext](#createNewDocumentFragmentInContext(java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int contentOffset)
Create a new [AuthorDocumentFragment](node/AuthorDocumentFragment.md) from an XML string in a specified context.
  [AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] [createNewDocumentFragmentsInContext](#createNewDocumentFragmentsInContext(java.lang.String%5B%5D,int%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] xmlFragments, int[] contentOffsets)
Create an array of [AuthorDocumentFragment](node/AuthorDocumentFragment.md) from an array of XML strings in specified contexts.
  [AuthorDocumentFragment](node/AuthorDocumentFragment.md) [createNewDocumentTextFragment](#createNewDocumentTextFragment(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textFragment)
Create a new [AuthorDocumentFragment](node/AuthorDocumentFragment.md) from an string.
  [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html) [createPositionInContent](#createPositionInContent(int))(int offset)
Create a flexible position in the Author Content.
  boolean [delete](#delete(int,int))(int startOffset, int endOffset)
Deletes a document fragment between the start and end offset.
  boolean [delete](#delete(int,int,boolean))(int startOffset, int endOffset, boolean backspace)
Deletes a document fragment between the start and end offset.
  boolean [deleteNode](#deleteNode(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node)
Delete a node.
  void [disableLayoutUpdate](#disableLayoutUpdate())()
INTERNAL USE ONLY.
  void [enableLayoutUpdate](#enableLayoutUpdate(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) ancestorOfChanges)
INTERNAL USE ONLY.
  void [endCompoundEdit](#endCompoundEdit())()
End a compound edit.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] [evaluateXPath](#evaluateXPath(java.lang.String,boolean,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments)
Evaluates an XPath 2.0 expression.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] [evaluateXPath](#evaluateXPath(java.lang.String,boolean,boolean,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers)
Evaluates an XPath 2.0 expression.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] [evaluateXPath](#evaluateXPath(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode,boolean,boolean,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, [AuthorNode](node/AuthorNode.md) contextNode, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers)
Evaluates an XPath 2.0 expression.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] [evaluateXPath](#evaluateXPath(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode,boolean,boolean,boolean,boolean,ro.sync.ecss.extensions.api.XPathVersion))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, [AuthorNode](node/AuthorNode.md) contextNode, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers, [XPathVersion](XPathVersion.md) xpathVersion)
Evaluates an XPath expression.
  [AuthorNode](node/AuthorNode.md)[] [findNodesByXPath](#findNodesByXPath(java.lang.String,boolean,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments)
Finds the author nodes selected by the given XPath 2.0 expression.
  [AuthorNode](node/AuthorNode.md)[] [findNodesByXPath](#findNodesByXPath(java.lang.String,boolean,boolean,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers)
Finds the author nodes selected by the given XPath 2.0 expression.
  [AuthorNode](node/AuthorNode.md)[] [findNodesByXPath](#findNodesByXPath(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode,boolean,boolean,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, [AuthorNode](node/AuthorNode.md) contextNode, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers)
Finds the author nodes selected by the given XPath 2.0 expression.
  [AuthorNode](node/AuthorNode.md)[] [findNodesByXPath](#findNodesByXPath(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode,boolean,boolean,boolean,boolean,ro.sync.ecss.extensions.api.XPathVersion))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, [AuthorNode](node/AuthorNode.md) contextNode, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers, [XPathVersion](XPathVersion.md) xpathVersion)
Finds the author nodes selected by the given XPath expression.
  [AuthorNode](node/AuthorNode.md)[] [findNodesByXPath](#findNodesByXPath(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode,boolean,boolean,boolean,boolean,ro.sync.ecss.extensions.api.XPathVersion,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, [AuthorNode](node/AuthorNode.md) contextNode, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers, [XPathVersion](XPathVersion.md) xpathVersion, boolean transparentReferences)
Finds the author nodes selected by the given XPath expression.
  [AuthorDocument](node/AuthorDocument.md) [getAuthorDocumentNode](#getAuthorDocumentNode())()
Returns the edited author document.
  [AuthorSchemaManager](AuthorSchemaManager.md) [getAuthorSchemaManager](#getAuthorSchemaManager())()

 void [getChars](#getChars(int,int,javax.swing.text.Segment))(int where, int len, [Segment](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Segment.html) chars)
The content represents the entire text content of the Author page + additional markers/sentinels at offsets which are pointed to by the AuthorNodes.
  [AuthorNode](node/AuthorNode.md) [getCommonAncestor](#getCommonAncestor(ro.sync.ecss.extensions.api.node.AuthorNode%5B%5D))([AuthorNode](node/AuthorNode.md)[] nodes)
Get the common parent for the nodes.
  [AuthorNode](node/AuthorNode.md) [getCommonParentNode](#getCommonParentNode(ro.sync.ecss.extensions.api.node.AuthorDocument,int,int))([AuthorDocument](node/AuthorDocument.md) doc, int startOffset, int endOffset)
Find the common ancestor node of the two offsets.
  [CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html) [getContentCharSequence](#getContentCharSequence())()
Retrieves a char sequence over the entire content of the document containing the text nodes and node markers. The content represents the entire text content of the Author page + additional markers/sentinels at offsets which are pointed to by the AuthorNodes.
  [OffsetInformation](content/OffsetInformation.md) [getContentInformationAtOffset](#getContentInformationAtOffset(int))(int offset)
Returns content information for the offset.
  [AuthorDocumentType](AuthorDocumentType.md) [getDoctype](#getDoctype())()
Returns information about the internal associated document type.
  [AuthorDocumentFilter](AuthorDocumentFilter.md) [getDocumentFilter](#getDocumentFilter())()
Gets the [AuthorDocumentFilter](AuthorDocumentFilter.md) which is currently set for altering the document edits.
  [AuthorFilteredContent](filter/AuthorFilteredContent.md) [getFilteredContent](#getFilteredContent(int,int,ro.sync.ecss.extensions.api.filter.AuthorNodesFilter))(int start, int end, [AuthorNodesFilter](filter/AuthorNodesFilter.md) nodesFilter)
Retrieves the content between the given start and end offset, excluding the content of the invisible nodes (that have display none style property), the content deleted with track changes, the sentinels of inline elements and the The filtered nodes are the nodes for which [AuthorNodesFilter.shouldFilterNode(AuthorNode)](filter/AuthorNodesFilter.md#shouldFilterNode(ro.sync.ecss.extensions.api.node.AuthorNode)) returns true.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFilteredText](#getFilteredText(int,int))(int offset, int length)
Gets a sequence of text from the document content.
  [AuthorNode](node/AuthorNode.md) [getNodeAtOffset](#getNodeAtOffset(int))(int offset)
Returns the node at the given offset.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](node/AuthorNode.md)> [getNodesToSelect](#getNodesToSelect(int,int))(int selectionStart, int selectionEnd)
Compute the list with nodes to select when a selection is present in editor.
  [AuthorNode](node/AuthorNode.md) [getStrictCommonAncestor](#getStrictCommonAncestor(ro.sync.ecss.extensions.api.node.AuthorNode%5B%5D))([AuthorNode](node/AuthorNode.md)[] nodes)
Get a node that is a strict ancestor for all the nodes in the given array.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getText](#getText(int,int))(int offset, int length)  Deprecated.
Please use the API [getContentCharSequence()](#getContentCharSequence()).
   [TextContentIterator](content/TextContentIterator.md) [getTextContentIterator](#getTextContentIterator(int,int))(int startOffset, int endOffset)
Get an iterator over the text content between two offsets.
  int [getTextContentLength](#getTextContentLength())()  Deprecated.
Use the API based on the [AuthorNode](node/AuthorNode.md) to get the length of the displayed text only, without mark-up markers.
   [UndoManager](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html) [getUndoManager](#getUndoManager())()
Get access to the Author undo manager.
  [UniqueAttributesProcessor](UniqueAttributesProcessor.md) [getUniqueAttributesProcessor](#getUniqueAttributesProcessor())()
Get the compound unique attributes processor which can be asked if a certain attribute should get copied on a split.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getUnparsedEntityUri](#getUnparsedEntityUri(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([AuthorNode](node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) entityName)
Returns the URI of the unparsed entity with the specified name, in the same document as the context node.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXPathExpression](#getXPathExpression(int))(int offset)
Returns the XPath expression of the node identified by the given offset.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXPathExpression](#getXPathExpression(int,boolean))(int offset, boolean processChanges)
Returns the XPath expression of the node identified by the given offset.
  [AuthorXPathExpressionBuilder](AuthorXPathExpressionBuilder.md) [getXPathExpressionBuilder](#getXPathExpressionBuilder(int))(int offset)
Returns a builder to generate an XPath expression of the node identified by the given offset.
  int [getXPathLocationOffset](#getXPathLocationOffset(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)
Compute the document offset defined by the XPath location and relative position.
  int [getXPathLocationOffset](#getXPathLocationOffset(java.lang.String,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition, boolean processChangeMarkers)
Compute the document offset defined by the XPath location and relative position.
  boolean [inInlineContext](#inInlineContext(int))(int offset)
Test if the context at the given offset is **inline**(as defined in the CSS specs) or not.
  boolean [insertElement](#insertElement(int,ro.sync.ecss.extensions.api.node.AuthorNode))(int caretOffset, [AuthorNode](node/AuthorNode.md) element)
Insert a simple element, at the specified offset in the document.
  void [insertFragment](#insertFragment(int,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment))(int insertOffset, [AuthorDocumentFragment](node/AuthorDocumentFragment.md) frag)
Insert an [AuthorDocumentFragment](node/AuthorDocumentFragment.md) at the given offset.
  [SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) [insertFragmentSchemaAware](#insertFragmentSchemaAware(int,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment))(int insertOffset, [AuthorDocumentFragment](node/AuthorDocumentFragment.md) frag)
Insert an [AuthorDocumentFragment](node/AuthorDocumentFragment.md) at the given offset in schema aware mode.
  void [insertMultipleElements](#insertMultipleElements(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,int%5B%5D,java.lang.String))([AuthorElement](node/AuthorElement.md) parentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementNames, int[] offsets, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Insert multiple elements at the given offsets.
  boolean [insertMultipleFragments](#insertMultipleFragments(ro.sync.ecss.extensions.api.node.AuthorElement,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,int%5B%5D))([AuthorElement](node/AuthorElement.md) parentElement, [AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragments, int[] offsets)
Insert multiple fragments at the given offsets.
  void [insertText](#insertText(int,java.lang.String))(int offset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text)
Inserts a text at the given offset.
  void [insertXMLFragment](#insertXMLFragment(java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int offset)
Insert an XML fragment at the given offset.
  void [insertXMLFragment](#insertXMLFragment(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)
Insert an XML fragment relative to the node identified by the xpathLocation and according with the relativePosition.
  void [insertXMLFragment](#insertXMLFragment(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, [AuthorNode](node/AuthorNode.md) relativeTo, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)
Insert an XML fragment relative to the given node and according with the relativePosition.
  [SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) [insertXMLFragmentSchemaAware](#insertXMLFragmentSchemaAware(java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int offset)
Insert an XML fragment at the given offset in schema aware mode.
  [SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) [insertXMLFragmentSchemaAware](#insertXMLFragmentSchemaAware(java.lang.String,int,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int offset, boolean replaceSelection)
Insert an XML fragment at the given offset in schema aware mode.
  [SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) [insertXMLFragmentSchemaAware](#insertXMLFragmentSchemaAware(java.lang.String,int,int,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int offset, int actionID, boolean replaceSelection)
Insert an XML fragment at the given offset in schema aware mode.
  [SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) [insertXMLFragmentSchemaAware](#insertXMLFragmentSchemaAware(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)
Insert an XML fragment relative to the node identified by the xpathLocation and according with the relativePosition.
  [SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) [insertXMLFragmentSchemaAware](#insertXMLFragmentSchemaAware(java.lang.String,java.lang.String,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition, boolean insertEvenIfInvalid)
Insert an XML fragment relative to the node identified by the xpathLocation and according with the relativePosition.
  boolean [isEditable](#isEditable(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node)
Test if a node is editable or not.
  void [markSelection](#markSelection(java.util.List,int,ro.sync.ecss.extensions.api.SelectionInterpretationMode,java.util.List,int,ro.sync.ecss.extensions.api.SelectionInterpretationMode))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<int[]> newSelection, int newCaretOffset, [SelectionInterpretationMode](SelectionInterpretationMode.md) newSelectionType, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<int[]> oldSelection, int oldCaretOffset, [SelectionInterpretationMode](SelectionInterpretationMode.md) oldSelectionType)
Add Author editor page selection intervals and marks the caret offset.
  void [multipleDelete](#multipleDelete(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D,int%5B%5D))([AuthorElement](node/AuthorElement.md) parentElement, int[] startOffsets, int[] endOffsets)
Deletes the given intervals.
  boolean [processContentRange](#processContentRange(int,int,ro.sync.ecss.extensions.api.content.RangeProcessor))(int startOffset, int endOffset, [RangeProcessor](content/RangeProcessor.md) rangeProcessor)
This method is useful if you want to make text processing on a given Author selection.
  void [refreshNodeReferences](#refreshNodeReferences(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node)
Refresh node references recursively.
  void [removeAttribute](#removeAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AuthorElement](node/AuthorElement.md) element)
Removes an attribute from the given element.
  void [removeAuthorListener](#removeAuthorListener(ro.sync.ecss.extensions.api.AuthorListener))([AuthorListener](AuthorListener.md) listener)
Remove an Author listener.
  void [removeAuthorPersistentHighlightListener](#removeAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener))([AuthorPersistentHighlightsListener](highlights/AuthorPersistentHighlightsListener.md) listener)  Deprecated.
Use [AuthorReviewController.removeAuthorPersistentHighlightListener(AuthorPersistentHighlightsListener)](AuthorReviewController.md#removeAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener)) instead
   void [removeClipboardFragmentProcessor](#removeClipboardFragmentProcessor(ro.sync.ecss.extensions.api.content.ClipboardFragmentProcessor))([ClipboardFragmentProcessor](content/ClipboardFragmentProcessor.md) clipboardFragmentProcessor)
Remove a processor which can analyze and modify [AuthorDocumentFragment](node/AuthorDocumentFragment.md) objects before they are inserted in the Author.
  void [removePseudoClassUndoable](#removePseudoClassUndoable(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pseudoClass, [AuthorElement](node/AuthorElement.md) element)
Removes a pseudo class from the given element.
  void [removeUniqueAttributesProcessor](#removeUniqueAttributesProcessor(ro.sync.ecss.extensions.api.UniqueAttributesProcessor))([UniqueAttributesProcessor](UniqueAttributesProcessor.md) uniqueAttributesProcessor)
Remove a processor which is asked to automatically generate unique IDs after content has been inserted in the Author.
  void [renameElement](#renameElement(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String))([AuthorElement](node/AuthorElement.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newName)
Rename an Author Element, set another qualified name to it.
  void [replaceRoot](#replaceRoot(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment))([AuthorDocumentFragment](node/AuthorDocumentFragment.md) fragment)
Replace the current root element with the new given one.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [serializeFragmentToXML](#serializeFragmentToXML(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment))([AuthorDocumentFragment](node/AuthorDocumentFragment.md) fragment)
Takes the given fragment and serializes it to XML text in the context of the current document.
  void [setAttribute](#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AttrValue](node/AttrValue.md) value, [AuthorElement](node/AuthorElement.md) element)
Sets the value of an attribute in the specified element.
  void [setDoctype](#setDoctype(ro.sync.ecss.extensions.api.AuthorDocumentType))([AuthorDocumentType](AuthorDocumentType.md) docType)
Set a new internal document type to the Author content.
  void [setDocumentFilter](#setDocumentFilter(ro.sync.ecss.extensions.api.AuthorDocumentFilter))([AuthorDocumentFilter](AuthorDocumentFilter.md) authorDocumentFilter)
Sets the [AuthorDocumentFilter](AuthorDocumentFilter.md) to be used for altering the document edits.WARNING: If filters are set by two or more plugins or customizations, only the last set filter will be taken into account.
  void [setMultipleAttributes](#setMultipleAttributes(int,int%5B%5D,java.util.Map))(int parentElementStartOffset, int[] elementOffsets, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](node/AttrValue.md)> attributes)
Sets the value of the given attribute in the specified elements.
  void [setMultipleDistinctAttributes](#setMultipleDistinctAttributes(int,int%5B%5D,java.util.List))(int parentElementStartOffset, int[] elementOffsets, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](node/AttrValue.md)>> attributes)
For each element look at the corresponding map of attributes from the list and set it on the element.
  void [setPseudoClassUndoable](#setPseudoClassUndoable(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pseudoClass, [AuthorElement](node/AuthorElement.md) element)
Sets a pseudo class in the specified element.
  void [setRenderingInfoChangedListener](#setRenderingInfoChangedListener(ro.sync.ecss.component.RenderingInfoChangedListener))([RenderingInfoChangedListener](../../component/RenderingInfoChangedListener.md) listener)
Sets the listener to be notified when the rendering info of a node has changed.
  boolean [split](#split(ro.sync.ecss.extensions.api.node.AuthorNode,int))([AuthorNode](node/AuthorNode.md) toSplit, int splitOffset)
Split the node at the given offset.
  void [surroundInFragment](#surroundInFragment(java.lang.String,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int startOffset, int endOffset)
Surround the content between the given offsets with the xmlFragment.
  void [surroundInFragment](#surroundInFragment(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment,int,int))([AuthorDocumentFragment](node/AuthorDocumentFragment.md) xmlFragment, int startOffset, int endOffset)
Surround the content between the given offsets with the xmlFragment.
  void [surroundInText](#surroundInText(java.lang.String,java.lang.String,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) header, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) footer, int startOffset, int endOffset)
Surround the content between the given offsets with plain text fragments(without XML parsing).
  [AuthorDocumentFragment](node/AuthorDocumentFragment.md) [unwrapDocumentFragment](#unwrapDocumentFragment(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment))([AuthorDocumentFragment](node/AuthorDocumentFragment.md) fragmentToUnwrap)
Unwrap a given Author document fragment.

### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorPseudoClassController](AuthorPseudoClassController.md)
 [removePseudoClass](AuthorPseudoClassController.md#removePseudoClass(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement)), [setPseudoClass](AuthorPseudoClassController.md#setPseudoClass(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))
## Method Details

### delete

boolean delete(int startOffset, int endOffset)

Deletes a document fragment between the start and end offset. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: startOffset - Start offset, 0 based, inclusive. endOffset - End offset, 0 based, inclusive. Returns: true if the delete operation was successful.
### delete

boolean delete(int startOffset, int endOffset, boolean backspace)

Deletes a document fragment between the start and end offset. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: startOffset - Start offset, 0 based, inclusive. endOffset - End offset, 0 based, inclusive. backspace - true if delete operation was triggered by the user pressing the backspace key. Returns: true if the delete operation was successful.
### deleteNode

boolean deleteNode([AuthorNode](node/AuthorNode.md) node)

Delete a node.
  Parameters: node - The [AuthorNode](node/AuthorNode.md) to delete. Returns: true if the delete node operation was successful.
### replaceRoot

void replaceRoot([AuthorDocumentFragment](node/AuthorDocumentFragment.md) fragment)

Replace the current root element with the new given one. The fragment must contain only one element, otherwise the replacement will not be performed.
  Parameters: fragment - The document fragment containing the new root element.
### createDocumentFragment

[AuthorDocumentFragment](node/AuthorDocumentFragment.md) createDocumentFragment(int startOffset, int endOffset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create an Author content fragment containing a clone of the document content for the given range of offsets. The offset ranges must be from the current AuthorDocument. The change tracking markers are automatically accepted in the fragment if change tracking is enabled in the document.  The Author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: startOffset - The start offset, 0 based, inclusive. endOffset - The end offset, 0 based, inclusive. Returns: A new [AuthorDocumentFragment](node/AuthorDocumentFragment.md). It does not return a null fragment. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offsets are not between 0 and the content length, or the startOffset is greater than the endOffset.
### createDocumentFragment

[AuthorDocumentFragment](node/AuthorDocumentFragment.md) createDocumentFragment(int startOffset, int endOffset, boolean preserveTrackChange)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create an Author content fragment containing a clone of the document content for the given range of offsets.  The offset ranges must be from the current AuthorDocument.  The Author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: startOffset - The start offset, 0 based, inclusive. endOffset - The end offset, 0 based, inclusive. preserveTrackChange - true to preserve track changes exactly as they are, no matter if change tracking is enabled or disabled. false to preserve the changes if change tracking is disabled or to automatically accept them if change tracking is enabled. Returns: A new [AuthorDocumentFragment](node/AuthorDocumentFragment.md). It does not return a null fragment. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offsets are not between 0 and the content length, or the startOffset is greater than the endOffset. Since: 23
### createNewDocumentFragmentInContext

[AuthorDocumentFragment](node/AuthorDocumentFragment.md) createNewDocumentFragmentInContext([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int contentOffset)throws [AuthorOperationException](AuthorOperationException.md)

Create a new [AuthorDocumentFragment](node/AuthorDocumentFragment.md) from an XML string in a specified context. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: xmlFragment - The XML Fragment. contentOffset - The offset where the XML fragment should be inserted. This method doesn't perform any insertion. This parameter is used to resolve entities and default attribute values from the DTD in the specified XML fragment. Returns: The newly created [AuthorDocumentFragment](node/AuthorDocumentFragment.md). It does not return a null fragment. Throws: [AuthorOperationException](AuthorOperationException.md) - If the new fragment creation fails.
### createNewDocumentFragmentsInContext

[AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] createNewDocumentFragmentsInContext([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] xmlFragments, int[] contentOffsets)throws [AuthorOperationException](AuthorOperationException.md)

Create an array of [AuthorDocumentFragment](node/AuthorDocumentFragment.md) from an array of XML strings in specified contexts. This method should be used when multiple Author document fragments must be created. In this situation the fragments are created faster than creating each of them by calling [createNewDocumentFragmentInContext(String, int)](#createNewDocumentFragmentInContext(java.lang.String,int)) method.  The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: xmlFragments - The array of XML fragments. contentOffsets - The offsets where the XML fragments should be inserted. The xml fragments and context offsets arrays must have the same size. The nth offset corresponds to the nth xml fragment. Returns: The newly created [AuthorDocumentFragment](node/AuthorDocumentFragment.md). It does not return a null fragment. Throws: [AuthorOperationException](AuthorOperationException.md) - If the xml fragments and context offsets sizes are different or a fragment creation fails. Since: 14
### createNewDocumentTextFragment

[AuthorDocumentFragment](node/AuthorDocumentFragment.md) createNewDocumentTextFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textFragment)throws [AuthorOperationException](AuthorOperationException.md)

Create a new [AuthorDocumentFragment](node/AuthorDocumentFragment.md) from an string. The returned fragment will contain **only a text node** and if the text fragment contains mark-up, it will be escaped. If the text has mark-up and you actually want to create author nodes from it then you should use [createNewDocumentFragmentInContext(String, int)](#createNewDocumentFragmentInContext(java.lang.String,int)).
  Parameters: textFragment - The text fragment. Returns: The newly created [AuthorDocumentFragment](node/AuthorDocumentFragment.md) holding the text node. If the text fragment contains mark-up, it will be escaped. It does not return a null fragment. Throws: [AuthorOperationException](AuthorOperationException.md) - If the new fragment creation fails.
### serializeFragmentToXML

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) serializeFragmentToXML([AuthorDocumentFragment](node/AuthorDocumentFragment.md) fragment)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Takes the given fragment and serializes it to XML text in the context of the current document. The following code example extracts the selection as an XML fragment, processes and then reinserts it:

```

 if(authorAccess.getEditorAccess().hasSelection()) {
    AuthorDocumentController documentController = authorAccess.getDocumentController();
    AuthorDocumentFragment selectionAsAFragment = documentController.createDocumentFragment(
         authorAccess.getEditorAccess().getSelectionStart(), authorAccess.getEditorAccess().getSelectionEnd());
    String selectionAsXML = documentController.serializeFragmentToXML(selectionAsAFragment);

    //Deletes the selection
    authorAccess.getEditorAccess().deleteSelection();

    //Process the selectionAsXML fragment, modify it.
    //................

    //Insert the XML fragment back at caret position.
    documentController.insertXMLFragment(selectionAsXML, authorAccess.getEditorAccess().getCaretOffset());
 }

```
If the fragment contains change tracking highlights, they will be serialized as processing instructions.
  Parameters: fragment - The [AuthorDocumentFragment](node/AuthorDocumentFragment.md) to serialize. Returns: An equivalent [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) representation of the given fragment. It does not return a null String. If the fragment cannot be serialized it will return an empty String. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If the serialization could not be accomplished, usually because the fragment was not properly built.
### setAttribute

void setAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AttrValue](node/AttrValue.md) value, [AuthorElement](node/AuthorElement.md) element)

Sets the value of an attribute in the specified element. If the element does not have the attribute specified by name, then an attribute with the specified value will be automatically created.  Attributes set in this manner (as opposed to calling [AuthorElement.setAttribute(String, AttrValue)](node/AuthorElement.md#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue)) directly) will be subject to undo/redo.
  Specified by: [setAttribute](AuthorAttributesController.md#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue,ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorAttributesController](AuthorAttributesController.md) Parameters: attributeName - Name of the attribute being changed. value - New [AttrValue](node/AttrValue.md) for the attribute. If null, the attribute is removed from the element. element - The [AuthorElement](node/AuthorElement.md) whose attribute is changing.
### setMultipleAttributes

void setMultipleAttributes(int parentElementStartOffset, int[] elementOffsets, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](node/AttrValue.md)> attributes)

Sets the value of the given attribute in the specified elements. Attributes set in this manner will be subject to undo/redo.
  Parameters: parentElementStartOffset - The start offset of the parent element. elementOffsets - The start offset for each element. attributes - The list with attributes. Every attribute name is mapped to an [AttrValue](node/AttrValue.md) object. If the value is null, the attribute will be removed. Since: 16
### setMultipleDistinctAttributes

void setMultipleDistinctAttributes(int parentElementStartOffset, int[] elementOffsets, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](node/AttrValue.md)>> attributes)

For each element look at the corresponding map of attributes from the list and set it on the element.
  Parameters: parentElementStartOffset - The start offset of an ancestor node which contains all other elements. elementOffsets - The start offset for each element. attributes - The list with attribute sets. Every attribute name is mapped to an [AttrValue](node/AttrValue.md) object. If the value is null, the attribute will be removed. Since: 17
### removeAttribute

void removeAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AuthorElement](node/AuthorElement.md) element)

Removes an attribute from the given element. Attributes removed in this manner (as opposed to calling [AuthorElement.setAttribute(String, AttrValue)](node/AuthorElement.md#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue)) directly) will be subject to undo/redo.
  Parameters: attributeName - Name of the attribute to remove. element - The [AuthorElement](node/AuthorElement.md) whose attribute will be removed.
### setPseudoClassUndoable

void setPseudoClassUndoable([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pseudoClass, [AuthorElement](node/AuthorElement.md) element)

Sets a pseudo class in the specified element.

This change \*IS\* subject to undo/redo.
  Parameters: pseudoClass - Name of the pseudo class being set. element - The [AuthorElement](node/AuthorElement.md) whose attribute is changing. Since: 21 See Also:
        * [AuthorPseudoClassController.setPseudoClass(String, AuthorElement)](AuthorPseudoClassController.md#setPseudoClass(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))

### removePseudoClassUndoable

void removePseudoClassUndoable([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pseudoClass, [AuthorElement](node/AuthorElement.md) element)

Removes a pseudo class from the given element. This change \*IS\* subject to undo/redo.
  Parameters: pseudoClass - Name of the pseudo class being set. element - The [AuthorElement](node/AuthorElement.md) whose attribute will be removed. Since: 21
### getNodeAtOffset

[AuthorNode](node/AuthorNode.md) getNodeAtOffset(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Returns the node at the given offset. The given offset must be greater or equal to 0 and less than the current document length. Note: *If the caret has the offset of an element's start offset marker character, it is considered to be before the element.*  *If the caret has the offset of an element's end offset marker character, it is considered to be inside the element.* The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: offset - The offset in the content, zero based. Returns: The [AuthorNode](node/AuthorNode.md) containing the offset, or null when the actual document is null. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offset is negative or greater than the content length.
### getContentInformationAtOffset

[OffsetInformation](content/OffsetInformation.md) getContentInformationAtOffset(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Returns content information for the offset. If the offset is on a marker character the returned result will also contain the node which contains the range indicated by the marker.
  Parameters: offset - The offset in the content, zero based. Returns: content information for the offset.    The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset() The image represents part of the document content and red markers represent special control characters which represent the node ranges. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) Since: 12.2
### createDocumentFragment

[AuthorDocumentFragment](node/AuthorDocumentFragment.md) createDocumentFragment([AuthorNode](node/AuthorNode.md) node, boolean copyContent)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create a document fragment containing a copy of the node. The node must be from the current AuthorDocument. The attributes of the elements will be copied. If copyContent is true the node content will be copied also.
  Parameters: node - The [AuthorNode](node/AuthorNode.md) to be duplicated. copyContent - If true the content of the node will also be duplicated. Returns: The [AuthorDocumentFragment](node/AuthorDocumentFragment.md) containing the duplicated node. It does not return a null fragment. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the operation fails.
### getText

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getText(int offset, int length)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
 Deprecated.
Please use the API [getContentCharSequence()](#getContentCharSequence()).

Gets a sequence of text from the document text content. The document text content can be obtained by adding all the text nodes content. The offset is considered to be relative to the text content start offset. So the 0 offset corresponds to the offset of the first valid char in the document. The length represents also a number of valid chars encountered after the real start offset was determined.  For the document:  [?PI?][article][!COMMENT][para]PARAGRAPH[/para][/article]    getText(0, 18) returns "PICOMMENTPARAGRAPH"  getText(5, 8) returns "MENTPARA"
  Parameters: offset - The starting offset >= 0. length - The number of characters to retrieve >= 0 Returns: The text Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - The range given includes a position that is not a valid position within the document text content.
### getTextContentLength

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) int getTextContentLength() throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
 Deprecated.
Use the API based on the [AuthorNode](node/AuthorNode.md) to get the length of the displayed text only, without mark-up markers.

Returns the length of the text content of the document. This is the number of valid characters in the document text. The length can be determined by the adding all text nodes content length.   For the document:  [?PI?][article][!COMMENT][para]PARAGRAPH[/para][/article]  The text content length will be:  "PI".length() + "COMMENT".length() + "PARAGRAPH".length() 2 + 7 + 9 = 18
  Returns: The text content length >= 0 Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### getUndoManager

[UndoManager](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html) getUndoManager()

Get access to the Author undo manager.
  Returns: The Author undo manager. The returned undo manager cannot be null.
### beginCompoundEdit

void beginCompoundEdit()

Begin a compound edit. This method should be called to signal to the editing support that a complex editing operation begins. The editing operations that occur between beginCompoundEdit()and endCompoundEdit() methods calls are regarded by the UndoManager as a single operation which can be undone/redone in one step.

### endCompoundEdit

void endCompoundEdit()

End a compound edit. This method should be called to signal to the editing support that a complex editing operation ends.
  See Also:
        * [beginCompoundEdit()](#beginCompoundEdit())

### cancelCompoundEdit

void cancelCompoundEdit()

Cancel the current compound edit. This method should be called to signal to the editing support that all edits performed so far inside a current compound edit must be undone. The editing operations that occurred after the previous call to beginCompoundEdit()will be undo by the UndoManager. Note that the compound edit does not end after a call to this method, so an explicit call to [endCompoundEdit()](#endCompoundEdit()) is required.
  See Also:
        * [beginCompoundEdit()](#beginCompoundEdit())
        * [endCompoundEdit()](#endCompoundEdit())

### insertText

void insertText(int offset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text)

Inserts a text at the given offset. After the operation the caret will be positioned at the end of the inserted text. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: offset - The insert position, 0 based. text - The text to be inserted.
### insertXMLFragment

void insertXMLFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int offset)throws [AuthorOperationException](AuthorOperationException.md)

Insert an XML fragment at the given offset. After the operation the caret will be positioned in the first leaf of the fragment. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: xmlFragment - The XML fragment to insert. offset - The insert position, 0 based. Throws: [AuthorOperationException](AuthorOperationException.md) - If the fragment could not be inserted.
### insertXMLFragment

void insertXMLFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)throws [AuthorOperationException](AuthorOperationException.md)

Insert an XML fragment relative to the node identified by the xpathLocation and according with the relativePosition. Note: if the xpathLocation is not specified then the XML fragment will be inserted at caret position and the relativePosition will be ignored.
After the operation the caret will be positioned in the first leaf of the fragment.

  Parameters: xmlFragment - The XML fragment. xpathLocation - The XPath location. relativePosition - The position relative to the node identified by the XPath location. Can be one of the constants: [AuthorConstants.POSITION_BEFORE](AuthorConstants.md#POSITION_BEFORE), [AuthorConstants.POSITION_AFTER](AuthorConstants.md#POSITION_AFTER), [AuthorConstants.POSITION_INSIDE_FIRST](AuthorConstants.md#POSITION_INSIDE_FIRST) or [AuthorConstants.POSITION_INSIDE_LAST](AuthorConstants.md#POSITION_INSIDE_LAST). Throws: [AuthorOperationException](AuthorOperationException.md) - If the fragment could not be inserted.
### insertXMLFragment

void insertXMLFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, [AuthorNode](node/AuthorNode.md) relativeTo, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)throws [AuthorOperationException](AuthorOperationException.md)

Insert an XML fragment relative to the given node and according with the relativePosition.
After the operation the caret will be positioned at the end of the inserted XML fragment.

  Parameters: xmlFragment - The XML fragment. relativeTo - The node to insert fragment relative to. relativePosition - The position relative to the node. Can be one of the constants: [AuthorConstants.POSITION_BEFORE](AuthorConstants.md#POSITION_BEFORE), [AuthorConstants.POSITION_AFTER](AuthorConstants.md#POSITION_AFTER), [AuthorConstants.POSITION_INSIDE_FIRST](AuthorConstants.md#POSITION_INSIDE_FIRST) or [AuthorConstants.POSITION_INSIDE_LAST](AuthorConstants.md#POSITION_INSIDE_LAST). Throws: [AuthorOperationException](AuthorOperationException.md) - If the fragment could not be inserted.
### insertXMLFragmentSchemaAware

[SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) insertXMLFragmentSchemaAware([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int offset)throws [AuthorOperationException](AuthorOperationException.md)

Insert an XML fragment at the given offset in schema aware mode. A normal insertion is executed when no schema is specified or schema aware feature is disable by the user (see Preferences / Editor / Pages / Author / Schema aware). If the fragments insertion is not allowed, a dialog will be shown proposing one of following solutions if they apply:
        * insert the fragments inside a new element. The name of the element to wrap the fragments in is computed by analyzing the left or right siblings.  By example, for the next Docbook situation:
```
<sect1>
  <title>Section title</title>
  {caret}
  <para>para content</para>
</sect1>

```
 if insert a fragment like: <emphasis>text</emphasis> the proposal is to create a new para element and insert the fragment inside it. The proposal result will be:
```
<sect1>
  <title>Section title</title>
  <para><emphasis>text</emphasis></para>
  <para>para content</para>
</sect1>

```

        * split an ancestor of the node at insertion offset and insert the fragments between the resulted elements.  By example, for the next Docbook situation:
```
<sect1>
  <title>Section title</title>
  {caret}
  <para>para content</para>
</sect1>

```
 if insert a fragment like: <sect1>...section content...</sect1> the proposal is to split the parent sect1 element and insert the fragment between the resulted sections. The proposal result will be:
```
<sect1>
  <title>Section title</title>
</sect1>
<sect1>...section content...</sect1>
<sect1>
  <para>para content</para>
</sect1>
```

        * insert the fragments somewhere in the proximity of the insertion offset(left or right without skipping content).  By example, for the next Docbook situation:
```
<sect1>
  <title>Section title</title>
  {caret}
  <para>para content</para>
</sect1>

```
 if insert a fragment like: <emphasis>text</emphasis> the proposals are to insert the fragment at the end of title or at beginning of para element.
        * insert at offset the plain text resulted after removing the mark-up.  By example, for the next Docbook situation:
```
<sect1>
  <title>Section title {caret}</title>
</sect1>

```
 if insert a fragment like: <para>fragment <emphasis>content</emphasis></para> the proposal is to remove the fragment mark-up and insert the text 'fragment content' at caret position. The proposal result will be:
```
<sect1>
  <title>Section title fragment content</title>
</sect1>

```

        * insert the fragments at insertion offset, even they are not allowed.

If the developer specifies an [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) then this handler has priority for executing the insert operation.

  Parameters: xmlFragment - The XML fragment to insert. offset - The insert position, 0 based. Returns: The result of the schema aware insertion. Can be used to get the insertion offset for the given fragments. Throws: [AuthorOperationException](AuthorOperationException.md) - If the fragment could not be inserted.
### insertXMLFragmentSchemaAware

[SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) insertXMLFragmentSchemaAware([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int offset, boolean replaceSelection)throws [AuthorOperationException](AuthorOperationException.md)

Insert an XML fragment at the given offset in schema aware mode. A normal insertion is executed when no schema is specified or schema aware feature is disable by the user (see Preferences / Editor / Pages / Author / Schema aware). If the fragments insertion is not allowed, a dialog will be shown proposing one of following solutions if they apply:
        * insert the fragments inside a new element. The name of the element to wrap the fragments in is computed by analyzing the left or right siblings.  By example, for the next Docbook situation:
```
<sect1>
  <title>Section title</title>
  {caret}
  <para>para content</para>
</sect1>

```
 if insert a fragment like: <emphasis>text</emphasis> the proposal is to create a new para element and insert the fragment inside it. The proposal result will be:
```
<sect1>
  <title>Section title</title>
  <para><emphasis>text</emphasis></para>
  <para>para content</para>
</sect1>

```

        * split an ancestor of the node at insertion offset and insert the fragments between the resulted elements.  By example, for the next Docbook situation:
```
<sect1>
  <title>Section title</title>
  {caret}
  <para>para content</para>
</sect1>

```
 if insert a fragment like: <sect1>...section content...</sect1> the proposal is to split the parent sect1 element and insert the fragment between the resulted sections. The proposal result will be:
```
<sect1>
  <title>Section title</title>
</sect1>
<sect1>...section content...</sect1>
<sect1>
  <para>para content</para>
</sect1>
```

        * insert the fragments somewhere in the proximity of the insertion offset(left or right without skipping content).  By example, for the next Docbook situation:
```
<sect1>
  <title>Section title</title>
  {caret}
  <para>para content</para>
</sect1>

```
 if insert a fragment like: <emphasis>text</emphasis> the proposals are to insert the fragment at the end of title or at beginning of para element.
        * insert at offset the plain text resulted after removing the mark-up.  By example, for the next Docbook situation:
```
<sect1>
  <title>Section title {caret}</title>
</sect1>

```
 if insert a fragment like: <para>fragment <emphasis>content</emphasis></para> the proposal is to remove the fragment mark-up and insert the text 'fragment content' at caret position. The proposal result will be:
```
<sect1>
  <title>Section title fragment content</title>
</sect1>

```

        * insert the fragments at insertion offset, even they are not allowed.

If the developer specifies an [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) then this handler has priority for executing the insert operation.

  Parameters: xmlFragment - The XML fragment to insert. offset - The insert position, 0 based. replaceSelection - true to replace the selected Author content with the fragment, false to leave the selected content and paste at caret position. Returns: The result of the schema aware insertion. Can be used to get the insertion offset for the given fragments. Throws: [AuthorOperationException](AuthorOperationException.md) - If the fragment could not be inserted.
### insertXMLFragmentSchemaAware

[SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) insertXMLFragmentSchemaAware([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int offset, int actionID, boolean replaceSelection)throws [AuthorOperationException](AuthorOperationException.md)

Insert an XML fragment at the given offset in schema aware mode.

The insertion behavior depends on the action type (specified by the actionID parameter) that triggered it. For more details see the description of [insertXMLFragmentSchemaAware(String, int, boolean)](#insertXMLFragmentSchemaAware(java.lang.String,int,boolean)).
  Parameters: xmlFragment - The XML fragment to insert. offset - The insert position, 0 based. actionID - The action that caused the insertion. One of the constants in [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md). replaceSelection - true to replace the selected Author content with the fragment, false to leave the selected content and paste at caret position. Returns: The result of the schema aware insertion. Can be used to get the insertion offset for the given fragments. Throws: [AuthorOperationException](AuthorOperationException.md) - If the fragment could not be inserted. Since: 17
### insertFragment

void insertFragment(int insertOffset, [AuthorDocumentFragment](node/AuthorDocumentFragment.md) frag)

Insert an [AuthorDocumentFragment](node/AuthorDocumentFragment.md) at the given offset. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: insertOffset - The offset where the fragment will be inserted, 0 based. frag - The [AuthorDocumentFragment](node/AuthorDocumentFragment.md) to be inserted. Never null.
### processContentRange

boolean processContentRange(int startOffset, int endOffset, [RangeProcessor](content/RangeProcessor.md) rangeProcessor)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [AuthorOperationException](AuthorOperationException.md)

This method is useful if you want to make text processing on a given Author selection. You will receive a call back which will give you the AuthorDocumentFragment to process. When finished, the range will be replaced with the processed fragment.
The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range.

The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset().

The image represents part of the document content and red markers represent special control characters which represent the node ranges.

  Parameters: startOffset - Start offset of the processed range (inclusive). endOffset - End offset of the processed range (inclusive). rangeProcessor - The range processor which gets notified to process the [AuthorDocumentFragment](node/AuthorDocumentFragment.md). Returns: true if the modifications were merged back in the Author content. For example when the selection cannot be replaced (inside a not-editable element) this method can return false. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [AuthorOperationException](AuthorOperationException.md) Since: 12.2
### insertFragmentSchemaAware

[SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) insertFragmentSchemaAware(int insertOffset, [AuthorDocumentFragment](node/AuthorDocumentFragment.md) frag)throws [AuthorOperationException](AuthorOperationException.md)

Insert an [AuthorDocumentFragment](node/AuthorDocumentFragment.md) at the given offset in schema aware mode. A normal insertion is executed when no schema is specified or schema aware feature is disable by the user (see Preferences / Editor / Pages / Author / Schema aware).
For more details about schema aware solutions see comments from [insertXMLFragmentSchemaAware(String, int)](#insertXMLFragmentSchemaAware(java.lang.String,int)) method.
 The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: insertOffset - The offset where the fragment will be inserted, 0 based. frag - The [AuthorDocumentFragment](node/AuthorDocumentFragment.md) to be inserted. Returns: The result of the schema aware insertion. Throws: [AuthorOperationException](AuthorOperationException.md) - If the fragment could not be inserted.
### surroundInFragment

void surroundInFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int startOffset, int endOffset)throws [AuthorOperationException](AuthorOperationException.md)

Surround the content between the given offsets with the xmlFragment. If endOffset < startOffset the xmlFragment will be inserted at startOffset. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: xmlFragment - The XML fragment which will surround the given interval. The first leaf node of the XML fragment will be the parent of the surrounded content. startOffset - The start offset of the content to be surrounded, 0 based and inclusive. endOffset - The end offset of the content to be surrounded, 0 based and inclusive. Throws: [AuthorOperationException](AuthorOperationException.md) - If the content between start and end offset could not be surrounded.
### surroundInFragment

void surroundInFragment([AuthorDocumentFragment](node/AuthorDocumentFragment.md) xmlFragment, int startOffset, int endOffset)throws [AuthorOperationException](AuthorOperationException.md)

Surround the content between the given offsets with the xmlFragment. If endOffset < startOffset the xmlFragment will be inserted at startOffset. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: xmlFragment - The XML fragment which will surround the given interval. The first leaf node of the XML fragment will be the parent of the surrounded content. startOffset - The start offset of the content to be surrounded, 0 based and inclusive. endOffset - The end offset of the content to be surrounded, 0 based and inclusive. Throws: [AuthorOperationException](AuthorOperationException.md) - If the content between start and end offset could not be surrounded. Since: 12.1
### surroundInText

void surroundInText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) header, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) footer, int startOffset, int endOffset)throws [AuthorOperationException](AuthorOperationException.md)

Surround the content between the given offsets with plain text fragments(without XML parsing). The method inserts the header at startOffset and the footer at endOffset. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: header - The header to be inserted before the surrounded text. footer - The footer to be inserted after the surrounded text. startOffset - The start offset of the text to be surrounded, 0 based. endOffset - The end offset of the text to be surrounded, 0 based. Throws: [AuthorOperationException](AuthorOperationException.md) - If the operation failed.
### inInlineContext

boolean inInlineContext(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [AuthorOperationException](AuthorOperationException.md)

Test if the context at the given offset is **inline**(as defined in the CSS specs) or not.
The CSS **display** property is taken into account when determining this state.
For example a text paragraph determines an **inline** context, and for an offset inside this paragraph the method will return true. For an offset between two paragraphs (considered to be **block** level) the method will return false.
  Parameters: offset - The offset in the document, zero based. Returns: Returns true if the given offset is inside an inline context. false otherwise. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offset does not exists in the document content. [AuthorOperationException](AuthorOperationException.md) - If the operation failed.
### addAuthorListener

void addAuthorListener([AuthorListener](AuthorListener.md) listener)

Add an Author listener to be notified about changes regarding the document and the document structure.
  Parameters: listener - The [AuthorListener](AuthorListener.md) to be added.
### addAuthorPersistentHighlightListener

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void addAuthorPersistentHighlightListener([AuthorPersistentHighlightsListener](highlights/AuthorPersistentHighlightsListener.md) listener)
 Deprecated.
Use [AuthorReviewController.addAuthorPersistentHighlightListener(AuthorPersistentHighlightsListener)](AuthorReviewController.md#addAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener)) instead

Adds a listener to be notified about changes regarding the persistent highlights. In the persistent highlights are included:
        *  Change tracking markers and comments
        *  Additional persistent highlights added using [AuthorPersistentHighlighter.addHighlight(int, int, java.util.LinkedHashMap)](highlights/AuthorPersistentHighlighter.md#addHighlight(int,int,java.util.LinkedHashMap))

  Parameters: listener - The listener Since: 14 See Also:
        * [AuthorPersistentHighlight.PersistentHighlightType](highlights/AuthorPersistentHighlight.PersistentHighlightType.md)
        * [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md)

### removeAuthorPersistentHighlightListener

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void removeAuthorPersistentHighlightListener([AuthorPersistentHighlightsListener](highlights/AuthorPersistentHighlightsListener.md) listener)
 Deprecated.
Use [AuthorReviewController.removeAuthorPersistentHighlightListener(AuthorPersistentHighlightsListener)](AuthorReviewController.md#removeAuthorPersistentHighlightListener(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsListener)) instead

Removes a persistent highlights listener.
  Parameters: listener - The listener to remove. Since: 14
### addPersistentHighlightsFilter

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void addPersistentHighlightsFilter([AuthorPersistentHighlightsFilter](highlights/AuthorPersistentHighlightsFilter.md) persistentHighlightsFilter)
 Deprecated.
Use [AuthorReviewController.addPersistentHighlightsFilter(AuthorPersistentHighlightsFilter)](AuthorReviewController.md#addPersistentHighlightsFilter(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightsFilter)) instead

Add a persistent highlights filter. A filter capable of filtering the highlights by author is present by default.
  Parameters: persistentHighlightsFilter - The filter to be added. Since: 15
### removeAuthorListener

void removeAuthorListener([AuthorListener](AuthorListener.md) listener)

Remove an Author listener.
  Parameters: listener - The [AuthorListener](AuthorListener.md) to be removed.
### evaluateXPath

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] evaluateXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers)throws [AuthorOperationException](AuthorOperationException.md)

Evaluates an XPath 2.0 expression. This function returns the result of the given XPath expression as an array of [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html). Author DOM text nodes, DOM CDATA sections and DOM comment wrappers can be ignored for performance reasons. For example, executing the expression:  //node() will return an array with all the Author DOM Node wrappers in the document. while evaluating the expression:  count(//node()) will return an array having a single component representing the number of nodes in the document. Evaluating the expression:  //node(), count(//node()) will return an array containing all the Author DOM Node wrappers in the document and having as last component the total number of nodes.
You can also use the XPath extension functions *oxy:current-selected-element()* and *oxy:allows-child-element()*.

  Parameters: xpathExpression - The XPath expression. If the XPath expression is relative, it will be computed in the context of the current caret position. ignoreTexts - If true DOM text nodes will not be returned. ignoreCData - If true DOM CDATA sections will not be returned. ignoreComments - If true DOM comments will not be returned. processChangeMarkers - If false the change markers (inserts/deletes/comments) will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored. If true the XPath will be applied over the document as if the change markers are applied. (All changes processed to processing instructions like when the XML document gets saved on disk). Returns: An array of objects representing the XPath result. It does not return a null array. If the XPath evaluation fails it will return an empty array. Throws: [AuthorOperationException](AuthorOperationException.md) - If the XPath expression failed to be evaluated.
### evaluateXPath

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] evaluateXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, [AuthorNode](node/AuthorNode.md) contextNode, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers, [XPathVersion](XPathVersion.md) xpathVersion)throws [AuthorOperationException](AuthorOperationException.md)

Evaluates an XPath expression. This function returns the result of the given XPath expression as an array of [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html). Author DOM text nodes, DOM CDATA sections and DOM comment wrappers can be ignored for performance reasons. For example, executing the expression:  //node() will return an array with all the Author DOM Node wrappers in the document. while evaluating the expression:  count(//node()) will return an array having a single component representing the number of nodes in the document. Evaluating the expression:  //node(), count(//node()) will return an array containing all the Author DOM Node wrappers in the document and having as last component the total number of nodes.
You can also use the XPath extension functions *oxy:current-selected-element()* and *oxy:allows-child-element()*.

  Parameters: xpathExpression - The XPath expression. If the XPath expression is relative, it will be computed in the context of the current caret position. contextNode - The node in the context of which the relative XPath Expressions will computed. If null the context node will be the node at the current caret position. ignoreTexts - If true DOM text nodes will not be returned. ignoreCData - If true DOM CDATA sections will not be returned. ignoreComments - If true DOM comments will not be returned. processChangeMarkers - If false the change markers (inserts/deletes/comments) will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored. If true the XPath will be applied over the document as if the change markers are applied. (All changes processed to processing instructions like when the XML document gets saved on disk). xpathVersion - Used version of XPath. Returns: An array of objects representing the XPath result. It does not return a null array. If the XPath evaluation fails it will return an empty array. Throws: [AuthorOperationException](AuthorOperationException.md) - If the XPath expression failed to be evaluated. Since: 15
### evaluateXPath

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] evaluateXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments)throws [AuthorOperationException](AuthorOperationException.md)

Evaluates an XPath 2.0 expression. This function returns the result of the given XPath expression as an array of [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html). Author DOM text nodes, DOM CDATA sections and DOM comment wrappers can be ignored for performance reasons. For example, executing the expression:  //node() will return an array with all the Author DOM Node wrappers in the document. while evaluating the expression:  count(//node()) will return an array having a single component representing the number of nodes in the document. Evaluating the expression:  //node(), count(//node()) will return an array containing all the Author DOM Node wrappers in the document and having as last component the total number of nodes. If change tracking (insert/remove/comment) markers exist in the document they will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored.
You can also use the XPath extension functions *oxy:current-selected-element()* and *oxy:allows-child-element()*.

  Parameters: xpathExpression - The XPath expression. If the XPath expression is relative, it will be computed in the context of the current caret position. ignoreTexts - If true DOM text nodes will not be returned. ignoreCData - If true DOM CDATA sections will not be returned. ignoreComments - If true DOM comments will not be returned. Returns: An array of objects representing the XPath result. It does not return a null array. If the XPath evaluation fails it will return an empty array. Throws: [AuthorOperationException](AuthorOperationException.md) - If the XPath expression failed to be evaluated.
### findNodesByXPath

[AuthorNode](node/AuthorNode.md)[] findNodesByXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers)throws [AuthorOperationException](AuthorOperationException.md)

Finds the author nodes selected by the given XPath 2.0 expression. The result of this function is an array of [AuthorNode](node/AuthorNode.md) selected by the given XPath expression. Author text nodes, Author CDATA section nodes and Author comment nodes can be ignored for performance reasons. For example executing the expression:  //node() will return an array with all the AuthorNode's in the document. But the result of calling the function with the expression:  count(//node()) will return an empty array. If change tracking (insert/remove/comment) markers exist in the document they will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored.
  Parameters: xpathExpression - The XPath expression. ignoreTexts - If true Author text nodes will not be returned. ignoreCData - If true Author CDATA sections will not be returned. ignoreComments - If true Author comments will not be returned. processChangeMarkers - If false the change markers (inserts/deletes/comments) will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored. If true the XPath will be applied over the document as if the change markers are applied. (All changes processed to processing instructions like when the XML document gets saved on disk). Returns: The Author nodes selected by the XPath expression. It does not return a null array of nodes. If the evaluation of the XPath expression fails it will return an empty array. Throws: [AuthorOperationException](AuthorOperationException.md) - If the XPath expression failed to be evaluated.
### findNodesByXPath

[AuthorNode](node/AuthorNode.md)[] findNodesByXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments)throws [AuthorOperationException](AuthorOperationException.md)

Finds the author nodes selected by the given XPath 2.0 expression. The result of this function is an array of [AuthorNode](node/AuthorNode.md) selected by the given XPath expression. Author text nodes, Author CDATA section nodes and Author comment nodes can be ignored for performance reasons. For example executing the expression:  //node() will return an array with all the AuthorNode's in the document. But the result of calling the function with the expression:  count(//node()) will return an empty array. If change tracking (insert/remove/comment) markers exist in the document the XPath will be applied over the document as if the change tracking is applied (All changes processed to processing instructions like when the XML document gets saved on disk).
  Parameters: xpathExpression - The XPath expression. If the XPath expression is relative, it will be computed in the context of the current caret position. ignoreTexts - If true Author text nodes will not be returned. ignoreCData - If true Author CDATA sections will not be returned. ignoreComments - If true Author comments will not be returned. Returns: The Author nodes selected by the XPath expression. It does not return a null array of nodes. If the evaluation of the XPath expression fails it will return an empty array. Throws: [AuthorOperationException](AuthorOperationException.md) - If the XPath expression failed to be evaluated.
### getXPathLocationOffset

int getXPathLocationOffset([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition, boolean processChangeMarkers)throws [AuthorOperationException](AuthorOperationException.md)

Compute the document offset defined by the XPath location and relative position.
  Parameters: xpathLocation - The XPath defining a node in document. relativePosition - The relative position to the node. One of the following: [AuthorConstants.POSITION_BEFORE](AuthorConstants.md#POSITION_BEFORE), [AuthorConstants.POSITION_INSIDE_FIRST](AuthorConstants.md#POSITION_INSIDE_FIRST), [AuthorConstants.POSITION_INSIDE_LAST](AuthorConstants.md#POSITION_INSIDE_LAST) or [AuthorConstants.POSITION_AFTER](AuthorConstants.md#POSITION_AFTER) processChangeMarkers - If false the change markers (inserts/deletes/comments) will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored. If true the XPath will be applied over the document as if the change markers are applied. (All changes processed to processing instructions like when the XML document gets saved on disk). Returns: The offset in document. Throws: [AuthorOperationException](AuthorOperationException.md) - If it fails. Since: 18
### getXPathLocationOffset

int getXPathLocationOffset([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)throws [AuthorOperationException](AuthorOperationException.md)

Compute the document offset defined by the XPath location and relative position. If change tracking (insert/remove/comment) markers exist in the document they will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored.
  Parameters: xpathLocation - The XPath defining a node in document. relativePosition - The relative position to the node. One of the following: [AuthorConstants.POSITION_BEFORE](AuthorConstants.md#POSITION_BEFORE), [AuthorConstants.POSITION_INSIDE_FIRST](AuthorConstants.md#POSITION_INSIDE_FIRST), [AuthorConstants.POSITION_INSIDE_LAST](AuthorConstants.md#POSITION_INSIDE_LAST) or [AuthorConstants.POSITION_AFTER](AuthorConstants.md#POSITION_AFTER) Returns: The offset in document. Throws: [AuthorOperationException](AuthorOperationException.md) - If it fails.
### insertMultipleElements

void insertMultipleElements([AuthorElement](node/AuthorElement.md) parentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementNames, int[] offsets, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)

Insert multiple elements at the given offsets. Note: *The offsets and fragments must be in document order. The offset must be given in the original document, before any insertion occurs.*
 To insert two elements one after another:

```

          String[] fragments = new String[] {"elem1", "elem2"};
          insertMultipleElements(parentElement, fragments, new int[] {offset, offset}, null);

```

The result of running the above code will be:

```

   parent
     elem1
     elem2

```

 The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.

  Parameters: parentElement - The parent element that contains all the new inserted elements. elementNames - The element names to be inserted. offsets - The absolute offsets where the elements will be inserted. namespace - The namespace of the new inserted elements.
### insertMultipleFragments

boolean insertMultipleFragments([AuthorElement](node/AuthorElement.md) parentElement, [AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragments, int[] offsets)

Insert multiple fragments at the given offsets. Note: *The offsets and fragments must be in document order. The offset must be given in the original document, before any insertion occurs.*
 To insert two fragment one after another:

```

          AuthorDocumentFragment[] fragments = new AuthorDocumentFragment[] {frag1, frag2};
          insertMultipleFragments(parentElement, fragments, new int[] {offset, offset});

```

The result of running the above code will be:

```

   parent
     frag1
     frag2

```

 The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.

  Parameters: parentElement - The parent element that contains all the new inserted elements. fragments - The fragments to be inserted. offsets - The absolute offsets where the fragments will be inserted. The offset must be given in the original document. Returns: true if the operation succeed. Since: 14
### multipleDelete

void multipleDelete([AuthorElement](node/AuthorElement.md) parentElement, int[] startOffsets, int[] endOffsets)

Deletes the given intervals. Note: *The offsets must be in document order and the intervals must not intersect with each other.* The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: parentElement - The element that contains all the deleted intervals. startOffsets - The start offset for each interval. Must be in document order. endOffsets - The end offset for each interval. Must be in document order. 0 based and inclusive.
### setDoctype

void setDoctype([AuthorDocumentType](AuthorDocumentType.md) docType)

Set a new internal document type to the Author content. This is a good method to add new entities (regular or unparsed) to the internal document type of the document. WARNING: if these modifications affect regular entities already inserted and expanded, they will not be re-parsed and their old content will remain rendered as such.
  Parameters: docType - The document type information.
### getDoctype

[AuthorDocumentType](AuthorDocumentType.md) getDoctype()

Returns information about the internal associated document type.
  Returns: The internal associated document type information. If the document does not have an internal Doctype section the method will return null.
### getCommonParentNode

[AuthorNode](node/AuthorNode.md) getCommonParentNode([AuthorDocument](node/AuthorDocument.md) doc, int startOffset, int endOffset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Find the common ancestor node of the two offsets. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Parameters: doc - The author document. startOffset - The start offset. endOffset - The end offset. Returns: The common ancestor. Can be the document but it cannot be null. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### getNodesToSelect

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](node/AuthorNode.md)> getNodesToSelect(int selectionStart, int selectionEnd)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Compute the list with nodes to select when a selection is present in editor. Balanced selection and select all nodes between first and last selected nodes.
  Parameters: selectionStart - The selection start. selectionEnd - The selection end exclusive. Returns: The list with nodes that have to be selected. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### getCommonAncestor

[AuthorNode](node/AuthorNode.md) getCommonAncestor([AuthorNode](node/AuthorNode.md)[] nodes)

Get the common parent for the nodes.
  Parameters: nodes - The array which contains the nodes. Returns: The common node. This is either a node from the array which is equal with or contains all other nodes or the closest ancestor which contains all the nodes. null if the nodes are not from the same document or do not belong to a document.
### getStrictCommonAncestor

[AuthorNode](node/AuthorNode.md) getStrictCommonAncestor([AuthorNode](node/AuthorNode.md)[] nodes)

Get a node that is a strict ancestor for all the nodes in the given array.
  Parameters: nodes - The array which contains the nodes. Returns: The common ancestor node. This is the closest ancestor which contains all the nodes. null if the nodes array is null, empty, or if the nodes are not from the same document or do not belong to a document. Since: 21
### getAuthorDocumentNode

[AuthorDocument](node/AuthorDocument.md) getAuthorDocumentNode()

Returns the edited author document.
  Returns: The author document. The document cannot be null.
### setDocumentFilter

void setDocumentFilter([AuthorDocumentFilter](AuthorDocumentFilter.md) authorDocumentFilter)

Sets the [AuthorDocumentFilter](AuthorDocumentFilter.md) to be used for altering the document edits.WARNING: If filters are set by two or more plugins or customizations, only the last set filter will be taken into account.
  Parameters: authorDocumentFilter - The [AuthorDocumentFilter](AuthorDocumentFilter.md) to be used.
### getDocumentFilter

[AuthorDocumentFilter](AuthorDocumentFilter.md) getDocumentFilter()

Gets the [AuthorDocumentFilter](AuthorDocumentFilter.md) which is currently set for altering the document edits.
  Returns: the [AuthorDocumentFilter](AuthorDocumentFilter.md) which is currently set for altering the document edits or null if no filter was set. Since: 15.2
### getChars

void getChars(int where, int len, [Segment](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Segment.html) chars)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

The content represents the entire text content of the Author page + additional markers/sentinels at offsets which are pointed to by the AuthorNodes. Each AuthorNode points to specific start and end character markers in the content. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   Retrieves a portion of the content into the specified [Segment](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Segment.html).
  Parameters: where - The starting position >= 0, where + len <= length() len - The number of characters to be retrieved >= 0 chars - The [Segment](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Segment.html) object to return the characters int.o Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If the specified position or length are invalid.
### getContentCharSequence

[CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html) getContentCharSequence()

Retrieves a char sequence over the entire content of the document containing the text nodes and node markers. The content represents the entire text content of the Author page + additional markers/sentinels at offsets which are pointed to by the AuthorNodes. Each AuthorNode points to specific start and end character markers in the content. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()
  Returns: a char sequence over the entire content of the document containing the text nodes and node markers. Since: 25.0
### getFilteredContent

[AuthorFilteredContent](filter/AuthorFilteredContent.md) getFilteredContent(int start, int end, [AuthorNodesFilter](filter/AuthorNodesFilter.md) nodesFilter)

Retrieves the content between the given start and end offset, excluding the content of the invisible nodes (that have display none style property), the content deleted with track changes, the sentinels of inline elements and the The filtered nodes are the nodes for which [AuthorNodesFilter.shouldFilterNode(AuthorNode)](filter/AuthorNodesFilter.md#shouldFilterNode(ro.sync.ecss.extensions.api.node.AuthorNode)) returns true. The content represents the entire text content of the Author page + additional markers/sentinels at offsets which are pointed to by the AuthorNodes. Each AuthorNode points to specific start and end character markers in the content. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()   Retrieves the content from start to end offsets,
  Parameters: start - The starting position >= 0. end - The end position >= 0, inclusive nodesFilter - Provides information about the Author nodes that should be filtered. Returns: The char sequence representing the filtered Author content. Since: 12.1
### getAuthorSchemaManager

[AuthorSchemaManager](AuthorSchemaManager.md) getAuthorSchemaManager()
  Returns: The schema manager associated with this document. Null value is returned if there is no schema associated.
### insertXMLFragmentSchemaAware

[SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) insertXMLFragmentSchemaAware([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)throws [AuthorOperationException](AuthorOperationException.md)

Insert an XML fragment relative to the node identified by the xpathLocation and according with the relativePosition. Note: if the xpathLocation is not specified then the XML fragment will be inserted at caret position and the relativePosition will be ignored.

For more details about schema aware solutions see comments from [insertXMLFragmentSchemaAware(String, int)](#insertXMLFragmentSchemaAware(java.lang.String,int)) method.

  Parameters: xmlFragment - The XML fragment. xpathLocation - The XPath location. relativePosition - The position relative to the node identified by the XPath location. Can be one of the constants: [AuthorConstants.POSITION_BEFORE](AuthorConstants.md#POSITION_BEFORE), [AuthorConstants.POSITION_AFTER](AuthorConstants.md#POSITION_AFTER), [AuthorConstants.POSITION_INSIDE_FIRST](AuthorConstants.md#POSITION_INSIDE_FIRST) or [AuthorConstants.POSITION_INSIDE_LAST](AuthorConstants.md#POSITION_INSIDE_LAST). Returns: The result of the schema aware insertion. Throws: [AuthorOperationException](AuthorOperationException.md) - If the fragment could not be inserted. See Also:
        * [insertXMLFragmentSchemaAware(String, int)](#insertXMLFragmentSchemaAware(java.lang.String,int))

### insertXMLFragmentSchemaAware

[SchemaAwareHandlerResult](schemaaware/SchemaAwareHandlerResult.md) insertXMLFragmentSchemaAware([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition, boolean insertEvenIfInvalid)throws [AuthorOperationException](AuthorOperationException.md)

Insert an XML fragment relative to the node identified by the xpathLocation and according with the relativePosition. Note: if the xpathLocation is not specified then the XML fragment will be inserted at caret position and the relativePosition will be ignored.

For more details about schema aware solutions see comments from [insertXMLFragmentSchemaAware(String, int)](#insertXMLFragmentSchemaAware(java.lang.String,int)) method.

  Parameters: xmlFragment - The XML fragment. xpathLocation - The XPath location. relativePosition - The position relative to the node identified by the XPath location. Can be one of the constants: [AuthorConstants.POSITION_BEFORE](AuthorConstants.md#POSITION_BEFORE), [AuthorConstants.POSITION_AFTER](AuthorConstants.md#POSITION_AFTER), [AuthorConstants.POSITION_INSIDE_FIRST](AuthorConstants.md#POSITION_INSIDE_FIRST) or [AuthorConstants.POSITION_INSIDE_LAST](AuthorConstants.md#POSITION_INSIDE_LAST). insertEvenIfInvalid - true to insert the fragment even if the document becomes invalid. This is used as a last attempt after all the schema aware insertion strategies have failed. Returns: The result of the schema aware insertion. Throws: [AuthorOperationException](AuthorOperationException.md) - If the fragment could not be inserted. Since: 23 See Also:
        * [insertXMLFragmentSchemaAware(String, int)](#insertXMLFragmentSchemaAware(java.lang.String,int))

### insertElement

boolean insertElement(int caretOffset, [AuthorNode](node/AuthorNode.md) element)

Insert a simple element, at the specified offset in the document.
  Parameters: caretOffset - The offset in the document. element - The element to insert. Returns: true if success. See Also:
        * [createElement(String)](#createElement(java.lang.String))

### createElement

[AuthorElement](node/AuthorElement.md) createElement([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName)

Creates an element. Please note that this method does not insert the default attributes from the schema so it is recommended to use [createNewDocumentFragmentInContext(String, int)](#createNewDocumentFragmentInContext(java.lang.String,int))instead, if it is possible.
  Parameters: qName - The qualified name of the element. Returns: an new [AuthorElement](node/AuthorElement.md) instance. See Also:
        * [insertElement(int, AuthorNode)](#insertElement(int,ro.sync.ecss.extensions.api.node.AuthorNode))

### isEditable

boolean isEditable([AuthorNode](node/AuthorNode.md) node)

Test if a node is editable or not. A node is not editable for one of the following cases:
        * the CSS property 'editable' is to 'false';
        * the node is entirely included into a DELETED change marker.
  Parameters: node - The node to test if is editable. Returns: True if the node is editable, false otherwise.
### renameElement

void renameElement([AuthorElement](node/AuthorElement.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newName)

Rename an Author Element, set another qualified name to it.
  Parameters: contextNode - The element to rename. newName - The new qualified name to set to it. Since: 12.1
### getTextContentIterator

[TextContentIterator](content/TextContentIterator.md) getTextContentIterator(int startOffset, int endOffset)

Get an iterator over the text content between two offsets.
  Parameters: startOffset - Start offset, 0 based, inclusive. endOffset - End offset, 0 based, inclusive. Returns: The text content iterator Since: 13
### createPositionInContent

[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html) createPositionInContent(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create a flexible position in the Author Content. The position is updated automatically when modifications occur before it. It behaves exactly like a [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html) added to a swing [Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html).
  Parameters: offset - The offset where to create the position Returns: The created position. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) Since: 13
### addClipboardFragmentProcessor

void addClipboardFragmentProcessor([ClipboardFragmentProcessor](content/ClipboardFragmentProcessor.md) clipboardFragmentProcessor)

Add a processor which can analyze and modify [AuthorDocumentFragment](node/AuthorDocumentFragment.md) objects before they are inserted in the Author. The processor specified in the [ExtensionsBundle](ExtensionsBundle.md) will have maximum priority.
  Parameters: clipboardFragmentProcessor - a processor which can analyze and modify [AuthorDocumentFragment](node/AuthorDocumentFragment.md) objects before they are inserted in the Author. Since: 13
### removeClipboardFragmentProcessor

void removeClipboardFragmentProcessor([ClipboardFragmentProcessor](content/ClipboardFragmentProcessor.md) clipboardFragmentProcessor)

Remove a processor which can analyze and modify [AuthorDocumentFragment](node/AuthorDocumentFragment.md) objects before they are inserted in the Author.
  Parameters: clipboardFragmentProcessor - a processor which can analyze and modify [AuthorDocumentFragment](node/AuthorDocumentFragment.md) objects before they are inserted in the Author. Since: 13
### addUniqueAttributesProcessor

void addUniqueAttributesProcessor([UniqueAttributesProcessor](UniqueAttributesProcessor.md) uniqueAttributesProcessor)

Add a processor which is asked to automatically generate unique IDs after content has been inserted in the Author. The processor can also specify which attributes can be copied on split. The [UniqueAttributesRecognizer](UniqueAttributesRecognizer.md) specified in the [ExtensionsBundle](ExtensionsBundle.md) will have maximum priority.
  Parameters: uniqueAttributesProcessor - a processor which is asked to automatically generate unique IDs after content has been inserted in the Author. The processor can also specify which attributes can be copied on split. Since: 13
### getUniqueAttributesProcessor

[UniqueAttributesProcessor](UniqueAttributesProcessor.md) getUniqueAttributesProcessor()

Get the compound unique attributes processor which can be asked if a certain attribute should get copied on a split.
  Returns: The compound unique attributes processor which can be asked if a certain attribute should get copied on a split. Since: 15.2
### removeUniqueAttributesProcessor

void removeUniqueAttributesProcessor([UniqueAttributesProcessor](UniqueAttributesProcessor.md) uniqueAttributesProcessor)

Remove a processor which is asked to automatically generate unique IDs after content has been inserted in the Author. The processor can also specify which attributes can be copied on split. The [UniqueAttributesRecognizer](UniqueAttributesRecognizer.md) specified in the [ExtensionsBundle](ExtensionsBundle.md) will have maximum priority.
  Parameters: uniqueAttributesProcessor - a processor which is asked to automatically generate unique IDs after content has been inserted in the Author. The processor can also specify which attributes can be copied on split. Since: 13
### findNodesByXPath

[AuthorNode](node/AuthorNode.md)[] findNodesByXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, [AuthorNode](node/AuthorNode.md) contextNode, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers)throws [AuthorOperationException](AuthorOperationException.md)

Finds the author nodes selected by the given XPath 2.0 expression. The result of this function is an array of [AuthorNode](node/AuthorNode.md) selected by the given XPath expression. Author text nodes, Author CDATA section nodes and Author comment nodes can be ignored for performance reasons. For example executing the expression:  //node() will return an array with all the AuthorNode's in the document. But the result of calling the function with the expression:  count(//node()) will return an empty array. If change tracking (insert/remove/comment) markers exist in the document they will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored. **Note:** References (like XInclude) will be transparent for the Xpath execution. The Xpath will see the referenced nodes as though they belong to the document.
  Parameters: xpathExpression - The XPath expression. If the XPath expression is relative, it will be computed in the context of the current caret position. contextNode - The node in the context of which the relative XPath Expressions will computed. The context node should be an [AuthorElement](node/AuthorElement.md). If null, the context node will be the element at the current caret position. ignoreTexts - If true Author text nodes will not be returned. ignoreCData - If true Author CDATA sections will not be returned. ignoreComments - If true Author comments will not be returned. processChangeMarkers - If false the change markers (inserts/deletes/comments) will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored. If true the XPath will be applied over the document as if the change markers are applied. (All changes processed to processing instructions like when the XML document gets saved on disk). Returns: The Author nodes selected by the XPath expression. It does not return a null array of nodes. If the evaluation of the XPath expression fails it will return an empty array. Throws: [AuthorOperationException](AuthorOperationException.md) - If the XPath expression failed to be evaluated. Since: 13
### findNodesByXPath

[AuthorNode](node/AuthorNode.md)[] findNodesByXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, [AuthorNode](node/AuthorNode.md) contextNode, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers, [XPathVersion](XPathVersion.md) xpathVersion)throws [AuthorOperationException](AuthorOperationException.md)

Finds the author nodes selected by the given XPath expression. The result of this function is an array of [AuthorNode](node/AuthorNode.md) selected by the given XPath expression. Author text nodes, Author CDATA section nodes and Author comment nodes can be ignored for performance reasons. For example executing the expression:  //node() will return an array with all the AuthorNode's in the document. But the result of calling the function with the expression:  count(//node()) will return an empty array. If change tracking (insert/remove/comment) markers exist in the document they will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored.
  Parameters: xpathExpression - The XPath expression. If the XPath expression is relative, it will be computed in the context of the current caret position. contextNode - The node in the context of which the relative XPath Expressions will computed. The context node should be an [AuthorElement](node/AuthorElement.md). If null, the context node will be the element at the current caret position. ignoreTexts - If true Author text nodes will not be returned. ignoreCData - If true Author CDATA sections will not be returned. ignoreComments - If true Author comments will not be returned. processChangeMarkers - If false the change markers (inserts/deletes/comments) will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored. If true the XPath will be applied over the document as if the change markers are applied. (All changes processed to processing instructions like when the XML document gets saved on disk). xpathVersion - Used version of XPath. Returns: The Author nodes selected by the XPath expression. It does not return a null array of nodes. If the evaluation of the XPath expression fails it will return an empty array. Throws: [AuthorOperationException](AuthorOperationException.md) - If the XPath expression failed to be evaluated. Since: 15
### findNodesByXPath

[AuthorNode](node/AuthorNode.md)[] findNodesByXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, [AuthorNode](node/AuthorNode.md) contextNode, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers, [XPathVersion](XPathVersion.md) xpathVersion, boolean transparentReferences)throws [AuthorOperationException](AuthorOperationException.md)

Finds the author nodes selected by the given XPath expression. The result of this function is an array of [AuthorNode](node/AuthorNode.md) selected by the given XPath expression. Author text nodes, Author CDATA section nodes and Author comment nodes can be ignored for performance reasons. For example executing the expression:  //node() will return an array with all the AuthorNode's in the document. But the result of calling the function with the expression:  count(//node()) will return an empty array. If change tracking (insert/remove/comment) markers exist in the document they will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored.
  Parameters: xpathExpression - The XPath expression. If the XPath expression is relative, it will be computed in the context of the current caret position. contextNode - The node in the context of which the relative XPath Expressions will computed. The context node should be an [AuthorElement](node/AuthorElement.md). If null, the context node will be the element at the current caret position. ignoreTexts - If true Author text nodes will not be returned. ignoreCData - If true Author CDATA sections will not be returned. ignoreComments - If true Author comments will not be returned. processChangeMarkers - If false the change markers (inserts/deletes/comments) will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored. If true the XPath will be applied over the document as if the change markers are applied. (All changes processed to processing instructions like when the XML document gets saved on disk). xpathVersion - Used version of XPath. transparentReferences - If true the references (like XInclude, or entities) will be transparent for the Xpath execution. The Xpath will see the referenced nodes as though they belong to the document. Returns: The Author nodes selected by the XPath expression. It does not return a null array of nodes. If the evaluation of the XPath expression fails it will return an empty array. Throws: [AuthorOperationException](AuthorOperationException.md) - If the XPath expression failed to be evaluated. Since: 17.1
### evaluateXPath

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] evaluateXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, [AuthorNode](node/AuthorNode.md) contextNode, boolean ignoreTexts, boolean ignoreCData, boolean ignoreComments, boolean processChangeMarkers)throws [AuthorOperationException](AuthorOperationException.md)

Evaluates an XPath 2.0 expression. This function returns the result of the given XPath expression as an array of [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html). Author DOM text nodes, DOM CDATA sections and DOM comment wrappers can be ignored for performance reasons. For example, executing the expression:  //node() will return an array with all the Author DOM Node wrappers in the document. while evaluating the expression:  count(//node()) will return an array having a single component representing the number of nodes in the document. Evaluating the expression:  //node(), count(//node()) will return an array containing all the Author DOM Node wrappers in the document and having as last component the total number of nodes.
You can also use the XPath extension functions *oxy:current-selected-element()* and *oxy:allows-child-element()*.
 **Note:** References (like XInclude) will be transparent for the Xpath execution. The Xpath will see the referenced nodes as though they belong to the document.
  Parameters: xpathExpression - The XPath expression. If the XPath expression is relative, it will be computed in the context of the context node. contextNode - The node in the context of which the relative XPath Expressions will computed. If null the context node will be the node at the current caret position. ignoreTexts - If true DOM text nodes will not be returned. ignoreCData - If true DOM CDATA sections will not be returned. ignoreComments - If true DOM comments will not be returned. processChangeMarkers - If false the change markers (inserts/deletes/comments) will be ignored and the XPath will return results as if the insert changes are accepted, the delete changes are rejected and the comment changes are ignored. If true the XPath will be applied over the document as if the change markers are applied. (All changes processed to processing instructions like when the XML document gets saved on disk). Returns: An array of objects representing the XPath result. It does not return a null array. If the XPath evaluation fails it will return an empty array. Throws: [AuthorOperationException](AuthorOperationException.md) - If the XPath expression failed to be evaluated. Since: 13
### unwrapDocumentFragment

[AuthorDocumentFragment](node/AuthorDocumentFragment.md) unwrapDocumentFragment([AuthorDocumentFragment](node/AuthorDocumentFragment.md) fragmentToUnwrap)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Unwrap a given Author document fragment. If the given fragment has a root element, this method returns a fragment containing the content of the root (or null if the root is empty), else the given fragment is returned.  The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset() The following image represents the architecture of an Author document fragment that is a part of the document content. The red markers represent special control characters which represent the node ranges:
  Parameters: fragmentToUnwrap - The Author document fragment to be unwrapped. Returns: The content of the fragment root (null if the root is empty) or the given fragment. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offsets are not between 0 and the content length, or the startOffset is greater than the endOffset. Since: 14
### getUnparsedEntityUri

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getUnparsedEntityUri([AuthorNode](node/AuthorNode.md) contextNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) entityName)

Returns the URI of the unparsed entity with the specified name, in the same document as the context node.
  Parameters: contextNode - Context node. entityName - Unparsed entity name. Returns: The URI of the entity or null if the entity is undefined. Since: 14.2
### refreshNodeReferences

void refreshNodeReferences([AuthorNode](node/AuthorNode.md) node)

Refresh node references recursively. If a node has expanded references on it created using the "ro.sync.ecss.extensions.api.AuthorReferenceResolver" API this method will call again the API to provide a fresh reference content for the node.
  Parameters: node - The node on which to refresh the references. Since: 15.2
### setRenderingInfoChangedListener

void setRenderingInfoChangedListener([RenderingInfoChangedListener](../../component/RenderingInfoChangedListener.md) listener)

Sets the listener to be notified when the rendering info of a node has changed.

The rendering info is represented by the node's styles computed from the associated CSS stylesheet and its content.
  Parameters: listener - The listener. Since: 15.2
### getXPathExpression

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXPathExpression(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Returns the XPath expression of the node identified by the given offset. The offset must be a valid document offset. Nodes deleted with change tracking are also considered when creating the context for the XPath expression. **Note:** If the offset is inside an expanded reference (for example an XIncluded content) the reference is transparent. The result will be just as the reference was replaced with the refered content.
  Parameters: offset - The offset of the node to get the XPath expression for. Returns: The XPath expression of the element from the given offset or an empty string if no XPath could be found. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offset is outside the valid interval (0 and the content length). Since: 16.1
### getXPathExpression

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXPathExpression(int offset, boolean processChanges)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Returns the XPath expression of the node identified by the given offset. The offset must be a valid document offset.  **Note:** If the offset is inside an expanded reference (for example an XIncluded content) the reference is transparent. The result will be just as the reference was replaced with the refered content.
  Parameters: offset - The offset of the node to get the XPath expression for. processChanges - if true nodes which have been marked as deletion changes are ignored when building the expession. Returns: The XPath expression of the element from the given offset or an empty string if no XPath could be found. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offset is outside the valid interval (0 and the content length). Since: 17
### getXPathExpressionBuilder

[AuthorXPathExpressionBuilder](AuthorXPathExpressionBuilder.md) getXPathExpressionBuilder(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Returns a builder to generate an XPath expression of the node identified by the given offset. The offset must be a valid document offset.  **Note:** If the offset is inside an expanded reference (for example an XIncluded content) the reference is transparent. The result will be just as the reference was replaced with the refered content.
  Parameters: offset - The offset of the node to get the XPath expression for. Returns: The XPath expression expression builder on which more options can be set. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offset is outside the valid interval (0 and the content length). Since: 24.0
### disableLayoutUpdate

void disableLayoutUpdate()

INTERNAL USE ONLY. On every model change event the view model is updated accordingly. This call will disable this support. When is this desirable: - when processing a large number or nodes. It might be best to disable the notifications generated by node and just generate a notification for the parent node. Possible side effects to be aware of: - if these notifications are disabled the view model will become unsynchronized with the nodes model. If the views model will be interogated at this point it will give eronous results. **Important**  [enableLayoutUpdate(AuthorNode)](#enableLayoutUpdate(ro.sync.ecss.extensions.api.node.AuthorNode)) should allways be called at the end.
  Since: 17
### enableLayoutUpdate

void enableLayoutUpdate([AuthorNode](node/AuthorNode.md) ancestorOfChanges)

INTERNAL USE ONLY. Enables the layout update on model changes that was previously disabled using [disableLayoutUpdate()](#disableLayoutUpdate()) and fires the required notifications to update the views and styles.
  Parameters: ancestorOfChanges - The node that contains all the structural changes. If null the root element will be used instead. Since: 17
### split

boolean split([AuthorNode](node/AuthorNode.md) toSplit, int splitOffset)

Split the node at the given offset.
  Parameters: toSplit - The node to split splitOffset - The split offset Returns: True if the nodes were split. Since: 18
### getFilteredText

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFilteredText(int offset, int length)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Gets a sequence of text from the document content. The content marked as deleted (using change tracking) will be filtered out. Also the special sentinel characters are removed.
  Parameters: offset - The starting offset >= 0. length - The number of characters to retrieve >= 0 Returns: The text Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - The range given includes a position that is not a valid position within the document text content. Since: 18
### markSelection

void markSelection([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<int[]> newSelection, int newCaretOffset, [SelectionInterpretationMode](SelectionInterpretationMode.md) newSelectionType, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<int[]> oldSelection, int oldCaretOffset, [SelectionInterpretationMode](SelectionInterpretationMode.md) oldSelectionType)

Add Author editor page selection intervals and marks the caret offset. It also keeps and restores the selection when undo and redo actions are performed.
  Parameters: newSelection - New selection intervals. An interval is an array with start and end offsets or null if not interested. Each [ContentInterval](ContentInterval.md) contains the **inclusive** start selection offset and the **exclusive** end selection offset. newCaretOffset - New caret offset. newSelectionType - New selection type. oldSelection - Old selection intervals. An interval is an array with start and end offsets or null if not interested. Each [ContentInterval](ContentInterval.md) contains the **inclusive** start selection offset and the **exclusive** end selection offset. oldCaretOffset - Old caret offset. oldSelectionType - Old selection type. Since: 19.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
