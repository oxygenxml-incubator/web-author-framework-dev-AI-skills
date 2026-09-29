Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorDocumentFilterBypass
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorDocumentFilterBypass
Used as a way to circumvent calling back into the AuthorDocumentController to change the AuthorDocument.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) [addCommentMarker](#addCommentMarker(int,int,java.lang.String,java.lang.String))(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) comment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentID)
Add a comment marker for the given interval.
  [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) [addPersistentMarker](#addPersistentMarker(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight.PersistentHighlightType,int,int,java.util.Map))([AuthorPersistentHighlight.PersistentHighlightType](highlights/AuthorPersistentHighlight.PersistentHighlightType.md) type, int startOffset, int endOffset, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties)
Add a comment marker for the given interval.
  boolean [delete](#delete(int,int,boolean))(int startOffset, int endOffset, boolean withBackspace)
Deletes a document fragment between the start and end offset.
  boolean [deleteNode](#deleteNode(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node)
Deletes the specified node from the document.
  void [insertFragment](#insertFragment(int,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment))(int offset, [AuthorDocumentFragment](node/AuthorDocumentFragment.md) frag)
Insert an [AuthorDocumentFragment](node/AuthorDocumentFragment.md) at the given offset.
  void [insertMultipleElements](#insertMultipleElements(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,int%5B%5D,java.lang.String))([AuthorElement](node/AuthorElement.md) parentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementNames, int[] offsets, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Insert multiple elements at the given offsets.
  boolean [insertMultipleFragments](#insertMultipleFragments(ro.sync.ecss.extensions.api.node.AuthorElement,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,int%5B%5D))([AuthorElement](node/AuthorElement.md) parentElement, [AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragments, int[] offsets)
Insert multiple fragments at the given offsets.
  boolean [insertNode](#insertNode(int,ro.sync.ecss.extensions.api.node.AuthorNode))(int offset, [AuthorNode](node/AuthorNode.md) node)
Insert the specified node at the given offset.
  void [insertText](#insertText(int,java.lang.String))(int offset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text)
Inserts a text at the given offset.
  void [multipleDelete](#multipleDelete(ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D,int%5B%5D))([AuthorElement](node/AuthorElement.md) parentElement, int[] startOffsets, int[] endOffsets)
Deletes the given intervals.
  void [removeAttribute](#removeAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AuthorElement](node/AuthorElement.md) element)
Removes an attribute from the given element.
  boolean [removeMarker](#removeMarker(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) marker)
Remove a persistent marker
  void [renameElement](#renameElement(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.Object))([AuthorElement](node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newName, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) infoProvider)
Rename the given element.
  void [setAttribute](#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AttrValue](node/AttrValue.md) value, [AuthorElement](node/AuthorElement.md) element)
Sets the value of an attribute in the specified element.
  void [setDoctype](#setDoctype(ro.sync.ecss.extensions.api.AuthorDocumentType))([AuthorDocumentType](AuthorDocumentType.md) docType)
Set a new internal document type to the Author content.
  void [setMultipleAttributes](#setMultipleAttributes(int,int%5B%5D,java.util.Map))(int parentElementStartOffset, int[] elementOffsets, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](node/AttrValue.md)> attributes)
Sets the value of the given attribute in the specified elements.
  void [setMultipleDistinctAttributes](#setMultipleDistinctAttributes(int,int%5B%5D,java.util.List))(int parentElementStartOffset, int[] elementOffsets, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](node/AttrValue.md)>> attributes)
Sets the value of the given attribute in the specified elements.
  boolean [split](#split(ro.sync.ecss.extensions.api.node.AuthorNode,int))([AuthorNode](node/AuthorNode.md) toSplit, int splitOffset)
Splits the specified node at the given offset.
  void [surroundInFragment](#surroundInFragment(java.lang.String,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int startOffset, int endOffset)
Surround the content between the given offsets with the xmlFragment.
  void [surroundInFragment](#surroundInFragment(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment,int,int))([AuthorDocumentFragment](node/AuthorDocumentFragment.md) xmlFragment, int startOffset, int endOffset)
Surround the content between the given offsets with the xmlFragment.
  void [surroundInText](#surroundInText(java.lang.String,java.lang.String,int,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) header, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) footer, int startOffset, int endOffset)
Surround the content between the given offsets with plain text fragments(without XML parsing).
  void [surroundWithNode](#surroundWithNode(ro.sync.ecss.extensions.api.node.AuthorNode,int,int,boolean))([AuthorNode](node/AuthorNode.md) node, int startOffset, int endOffset, boolean leftToRight)
Surrounds the fragment between the specified offset with the specified node.

## Method Details

### insertText

void insertText(int offset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text)

Inserts a text at the given offset. After the operation the caret will be positioned at the end of the inserted text.
  Parameters: offset - The insert position, 0 based. text - The text to be inserted.
### insertFragment

void insertFragment(int offset, [AuthorDocumentFragment](node/AuthorDocumentFragment.md) frag)

Insert an [AuthorDocumentFragment](node/AuthorDocumentFragment.md) at the given offset.
  Parameters: offset - The offset where the fragment will be inserted, 0 based. frag - The [AuthorDocumentFragment](node/AuthorDocumentFragment.md) to be inserted.
### insertNode

boolean insertNode(int offset, [AuthorNode](node/AuthorNode.md) node)

Insert the specified node at the given offset.
  Parameters: offset - The offset where the node will be inserted. 0 based. node - The [AuthorNode](node/AuthorNode.md) to insert. Returns: true if the operation was successful.
### insertMultipleElements

void insertMultipleElements([AuthorElement](node/AuthorElement.md) parentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementNames, int[] offsets, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)

Insert multiple elements at the given offsets. Note: *The offsets and elements must be in document order.*
  Parameters: parentElement - The parent element that contains all the new inserted elements. elementNames - The element names to be inserted. offsets - The absolute offsets where the elements will be inserted. 0 based. namespace - The namespace of the new inserted elements.
### insertMultipleFragments

boolean insertMultipleFragments([AuthorElement](node/AuthorElement.md) parentElement, [AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragments, int[] offsets)

Insert multiple fragments at the given offsets. Note: *The offsets and fragments must be in document order.*
  Parameters: parentElement - The parent element that contains all the new inserted elements. fragments - The fragments to be inserted. offsets - The absolute offsets where the elements will be inserted. 0 based. Returns: true if the operation succeed. Since: 14
### delete

boolean delete(int startOffset, int endOffset, boolean withBackspace)

Deletes a document fragment between the start and end offset.
  Parameters: startOffset - Start offset, 0 based and inclusive. endOffset - End offset, 0 based and inclusive. withBackspace - true if BACKSPACE key was used when deleting the fragment. Returns: true if the delete operation was successful.
### deleteNode

boolean deleteNode([AuthorNode](node/AuthorNode.md) node)

Deletes the specified node from the document.
  Parameters: node - The [AuthorNode](node/AuthorNode.md) to delete. Returns: true if the delete node operation was successful.
### multipleDelete

void multipleDelete([AuthorElement](node/AuthorElement.md) parentElement, int[] startOffsets, int[] endOffsets)

Deletes the given intervals. Note: *The offsets must be in document order and the intervals must not intersect with each other.*
  Parameters: parentElement - The element that contains all the deleted intervals. startOffsets - The start offset for each interval. Must be in document order. 0 based and inclusive. endOffsets - The end offset for each interval. Must be in document order. 0 based and inclusive.
### renameElement

void renameElement([AuthorElement](node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newName, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) infoProvider)

Rename the given element. Any compound must be handled externally.
  Parameters: element - The [AuthorElement](node/AuthorElement.md) that is renamed. newName - The new name for the element. infoProvider - Information provider used for internal processing.
### setAttribute

void setAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AttrValue](node/AttrValue.md) value, [AuthorElement](node/AuthorElement.md) element)

Sets the value of an attribute in the specified element. Attributes set in this manner (as opposed to calling [AuthorElement.setAttribute(String, AttrValue)](node/AuthorElement.md#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue)) directly) will be subject to undo/redo.
  Parameters: attributeName - Name of the attribute being changed. value - New [AttrValue](node/AttrValue.md) for the attribute. If null, the attribute is removed from the element. element - The [AuthorElement](node/AuthorElement.md) whose attribute is changing.
### removeAttribute

void removeAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AuthorElement](node/AuthorElement.md) element)

Removes an attribute from the given element. Attributes removed in this manner (as opposed to calling [AuthorElement.setAttribute(String, AttrValue)](node/AuthorElement.md#setAttribute(java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue)) directly) will be subject to undo/redo.
  Parameters: attributeName - Name of the attribute to remove. element - The [AuthorElement](node/AuthorElement.md) whose attribute will be removed.
### split

boolean split([AuthorNode](node/AuthorNode.md) toSplit, int splitOffset)

Splits the specified node at the given offset. The attributes of the splitted node will also be copied excepting the unique ones. The unique attributes are identified by the [UniqueAttributesRecognizer](UniqueAttributesRecognizer.md).
  Parameters: toSplit - The [AuthorNode](node/AuthorNode.md) to split. splitOffset - The split offset. The offset must be greater or equal to 1 and less than the current document length. Returns: true if the node was split.
### surroundWithNode

void surroundWithNode([AuthorNode](node/AuthorNode.md) node, int startOffset, int endOffset, boolean leftToRight)

Surrounds the fragment between the specified offset with the specified node. The fragment between the start and end offsets will become the node actual content.
  Parameters: node - The [AuthorNode](node/AuthorNode.md) that will surround the fragment. startOffset - Start offset of the surrounded fragment. 0 based and inclusive. endOffset - End offset of the surrounded fragment. 0 based and inclusive. leftToRight - true if after the operation the selection in the author page is done from the left to the right.
### surroundInFragment

void surroundInFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int startOffset, int endOffset)throws [AuthorOperationException](AuthorOperationException.md)

Surround the content between the given offsets with the xmlFragment. If endOffset < startOffset the xmlFragment will be inserted at startOffset.
  Parameters: xmlFragment - The XML fragment which will surround the given interval. The first leaf node of the XML fragment will be the parent of the surrounded content. startOffset - The start offset of the content to be surrounded, 0 based and inclusive. endOffset - The end offset of the content to be surrounded, 0 based and inclusive. Throws: [AuthorOperationException](AuthorOperationException.md) - If the content between start and end offset could not be surrounded.
### surroundInText

void surroundInText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) header, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) footer, int startOffset, int endOffset)throws [AuthorOperationException](AuthorOperationException.md)

Surround the content between the given offsets with plain text fragments(without XML parsing). The method inserts the header at startOffset and the footer at endOffset.
  Parameters: header - The header to be inserted before the surrounded text. footer - The footer to be inserted after the surrounded text. startOffset - The start offset of the text to be surrounded, 0 based and inclusive. endOffset - The end offset of the text to be surrounded, 0 based and inclusive. Throws: [AuthorOperationException](AuthorOperationException.md) - If the operation failed.
### setDoctype

void setDoctype([AuthorDocumentType](AuthorDocumentType.md) docType)

Set a new internal document type to the Author content. This is a good method to add new entities (regular or unparsed) to the internal document type of the document. WARNING: if these modifications affect regular entities already inserted and expanded, they will not be re-parsed and their old content will remain rendered as such.
  Parameters: docType - The document type information.
### surroundInFragment

void surroundInFragment([AuthorDocumentFragment](node/AuthorDocumentFragment.md) xmlFragment, int startOffset, int endOffset)throws [AuthorOperationException](AuthorOperationException.md)

Surround the content between the given offsets with the xmlFragment. If endOffset < startOffset the xmlFragment will be inserted at startOffset.
  Parameters: xmlFragment - The XML fragment which will surround the given interval. The first leaf node of the XML fragment will be the parent of the surrounded content. startOffset - The start offset of the content to be surrounded, 0 based and inclusive. endOffset - The end offset of the content to be surrounded, 0 based and inclusive. Throws: [AuthorOperationException](AuthorOperationException.md) Since: 12.1
### setMultipleDistinctAttributes

void setMultipleDistinctAttributes(int parentElementStartOffset, int[] elementOffsets, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](node/AttrValue.md)>> attributes)

Sets the value of the given attribute in the specified elements. Attributes set in this manner will be subject to undo/redo.
  Parameters: parentElementStartOffset - The start offset of the parent element. elementOffsets - The start offset for each element. attributes - The list with attributes. Every attribute name is mapped to an [AttrValue](node/AttrValue.md) object. If the value is null, the attribute will be removed.
### setMultipleAttributes

void setMultipleAttributes(int parentElementStartOffset, int[] elementOffsets, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](node/AttrValue.md)> attributes)

Sets the value of the given attribute in the specified elements. Attributes set in this manner will be subject to undo/redo.
  Parameters: parentElementStartOffset - The start offset of the parent element. elementOffsets - The start offset for each element. attributes - The list with attributes. Every attribute name is mapped to an [AttrValue](node/AttrValue.md) object. If the value is null, the attribute will be removed.
### addCommentMarker

[AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) addCommentMarker(int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) comment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentID)

Add a comment marker for the given interval.
  Parameters: startOffset - Start offset of marker endOffset - End offset of marker comment - The comment to be added. parentID - The comment parent id (not null for replies). Returns: The added comment highlight if the comment was added or null. Since: 22
### addPersistentMarker

[AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) addPersistentMarker([AuthorPersistentHighlight.PersistentHighlightType](highlights/AuthorPersistentHighlight.PersistentHighlightType.md) type, int startOffset, int endOffset, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties)

Add a comment marker for the given interval.
  Parameters: type - The persistent marker type (comment or custom) startOffset - Start offset of marker endOffset - End offset of marker properties - not null comment properties. Returns: The added comment highlight if the comment was added or null. Since: 23
### removeMarker

boolean removeMarker([AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) marker)

Remove a persistent marker
  Parameters: marker - The marker Returns: True if the marker was removed Since: 22
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
