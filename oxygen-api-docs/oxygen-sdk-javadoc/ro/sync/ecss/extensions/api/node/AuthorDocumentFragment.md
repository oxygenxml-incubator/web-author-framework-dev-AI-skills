Package [ro.sync.ecss.extensions.api.node](package-summary.md)

# Class AuthorDocumentFragment

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.node.AuthorDocumentFragment
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorDocumentFragment extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Represents a fragment of an XML document. It holds a copy of the content of a document fragment. A change in the fragment does not change the edited document. For changing the edited document use insert methods of [AuthorDocumentController](../AuthorDocumentController.md).  For the following XML code fragment:  accounting<person><name>John W.</name><email>john@gmail.com</email></person><person><name>Mary B.</name><email>mary@msn.com</email></person>  the corresponding document fragment structure can be represented as:    The image represents the content of the fragment and the red markers represent special control characters which are used to point to the start and the end offsets of the fragment containing nodes.

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorDocumentFragment](#%3Cinit%3E(ro.sync.ecss.extensions.api.Content,java.util.List,int,int))([Content](../Content.md) content, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> elements, int leftSplits, int righSplits)
Constructor.
  [AuthorDocumentFragment](#%3Cinit%3E(ro.sync.ecss.extensions.api.Content,java.util.List,int,int,java.util.List,java.util.List))([Content](../Content.md) content, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> elements, int leftSplits, int righSplits, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> changeMarkers, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> commentMarkers)
Constructor.
  [AuthorDocumentFragment](#%3Cinit%3E(ro.sync.ecss.extensions.api.Content,java.util.List,int,int,java.util.List,java.util.List,java.util.Map))([Content](../Content.md) content, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> elements, int leftSplits, int righSplits, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> changeMarkers, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> commentMarkers, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](AuthorElement.md),[LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)>> attributesChanges)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorDocumentFragment](AuthorDocumentFragment.md) [clone](#clone())()
Clone a fragment.
  boolean [containsSimpleText](#containsSimpleText())()
Check if an author document fragment content contains simple text.
  int [getAcceptedLength](#getAcceptedLength())()

 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](AuthorElement.md),[LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)>> [getAttributesChangeHighlights](#getAttributesChangeHighlights())()
Get the map of attribute changes in the fragment.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> [getChangeHighlights](#getChangeHighlights())()
Returns the list with the fragment change tracking highlights.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> [getCommentsAndCustomHighlights](#getCommentsAndCustomHighlights())()
Returns the list with the fragment comment highlights or custom highlights.
  [Content](../Content.md) [getContent](#getContent())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> [getContentNodes](#getContentNodes())()
Get the list of the first-level nodes contained in this Author document fragment.
  int [getLeftSplits](#getLeftSplits())()  **This method is intended for internal use only.**  int [getLength](#getLength())()

 int [getRightSplits](#getRightSplits())()  **This method is intended for internal use only.**  int [getSuggestedRelativeCaretOffset](#getSuggestedRelativeCaretOffset())()
Get the offset were the caret should be placed, relative to the beginning of the fragment.
  boolean [isEmpty](#isEmpty())()

 void [setAttributesChanges](#setAttributesChanges(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](AuthorElement.md),[LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)>> attributesChanges)
Set the map of element to attribute changes.
  void [setChangeHighlights](#setChangeHighlights(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> markers)
**This class is intended for internal use only.** Set the list with the change tracking highlights.
  void [setCommentAndCustomHighlights](#setCommentAndCustomHighlights(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> highlights)
**This class is intended for internal use only.** Set the list with the fragment comment highlights or custom highlights.
  void [setContentNodes](#setContentNodes(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> nodes)
Set the content nodes.
  void [setLeftSplits](#setLeftSplits(int))(int leftSplits)
**This method is intended for internal use only.** Set the number of the elements the fragment splits to the left.
  void [setRighSplits](#setRighSplits(int))(int righSplits)
**This method is intended for internal use only.** Set the number of the elements the fragment splits to the right.
  void [setSuggestedRelativeCaretOffset](#setSuggestedRelativeCaretOffset(int))(int suggestedRelativeCaretOffset)
Set the offset were the caret should be placed, relative to the beginning of the fragment.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorDocumentFragment

public AuthorDocumentFragment([Content](../Content.md) content, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> elements, int leftSplits, int righSplits)

Constructor.
  Parameters: content - The [Content](../Content.md) holding the fragment's content. elements - Elements that make up this fragment. leftSplits - Number of elements it splits to the left. righSplits - Number of elements it splits to the right.
### AuthorDocumentFragment

public AuthorDocumentFragment([Content](../Content.md) content, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> elements, int leftSplits, int righSplits, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> changeMarkers, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> commentMarkers)

Constructor.
  Parameters: content - The [Content](../Content.md) holding the fragment's content. elements - Elements that make up this fragment. leftSplits - Number of elements it splits to the left. righSplits - Number of elements it splits to the right. changeMarkers - The list of change markers commentMarkers - Comment markers
### AuthorDocumentFragment

public AuthorDocumentFragment([Content](../Content.md) content, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> elements, int leftSplits, int righSplits, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> changeMarkers, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> commentMarkers, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](AuthorElement.md),[LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)>> attributesChanges)

Constructor.
  Parameters: content - The [Content](../Content.md) holding the fragment's content. elements - Elements that make up this fragment. leftSplits - Number of elements it splits to the left. righSplits - Number of elements it splits to the right. changeMarkers - The list of change markers commentMarkers - Comment markers attributesChanges - The map of attribute changes.
## Method Details

### getContent

public [Content](../Content.md) getContent()
  Returns: the [Content](../Content.md) object holding this fragment's content.
### getAcceptedLength

public int getAcceptedLength()
  Returns: The number of characters, including sentinels (element start and end markers), present in the fragment. If there are delete change markers, they are treated as accepted
### getLength

public int getLength()
  Returns: The number of characters, including sentinels (element start and end markers), present in the fragment.
### getContentNodes

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> getContentNodes()

Get the list of the first-level nodes contained in this Author document fragment. Each of this [AuthorNode](AuthorNode.md) can contain another nodes (the Author nodes model is similar with the DOM model).
  Returns: The nodes that make up this fragment.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### getLeftSplits

public int getLeftSplits()
 **This method is intended for internal use only.**  Returns: Number of nodes the fragment splits to the left.
### getRightSplits

public int getRightSplits()
 **This method is intended for internal use only.**  Returns: Number of nodes the fragment splits to the right.
### setLeftSplits

public void setLeftSplits(int leftSplits)

**This method is intended for internal use only.** Set the number of the elements the fragment splits to the left.
  Parameters: leftSplits - The left splits count.
### setRighSplits

public void setRighSplits(int righSplits)

**This method is intended for internal use only.** Set the number of the elements the fragment splits to the right.
  Parameters: righSplits - The right splits count.
### getChangeHighlights

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> getChangeHighlights()

Returns the list with the fragment change tracking highlights. If the fragment is created when change tracking is turned **OFF** and the fragment contains Track Changes, then the returned list will contain the changes which intersected the fragment region, made relative to the fragment content. If the fragment is created when change tracking in turned **ON** then the fragment will contain the selection with all changes accepted (so the list will be always NULL). To get the list with all change tracking highlights from the document use the [ChangeTrackingController.getChangeHighlights()](../ChangeTrackingController.md#getChangeHighlights()) method.
  Returns: Returns list with the fragment change tracking highlights. The start and end offset of the returned change tracking highlights are relative to the start offset of this document fragment.  The type of the highlights can be one of [AuthorPersistentHighlight.PersistentHighlightType.CHANGE_INSERT](../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#CHANGE_INSERT) or [AuthorPersistentHighlight.PersistentHighlightType.CHANGE_DELETE](../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#CHANGE_DELETE) Since: 12
### getAttributesChangeHighlights

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](AuthorElement.md),[LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)>> getAttributesChangeHighlights()

Get the map of attribute changes in the fragment. Can be null. Each element can have one or more attribute changes.
  Returns: Returns the attributesChangeTracking. Since: 15.1
### getCommentsAndCustomHighlights

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> getCommentsAndCustomHighlights()

Returns the list with the fragment comment highlights or custom highlights. If the fragment contains comments or custom highlights then the returned list will contain the comments which intersected the fragment, made relative to the fragment content. To get the list with all the comments or persistent highlights from the document see the [AuthorReviewController.getCommentHighlights()](../AuthorReviewController.md#getCommentHighlights()) and [AuthorPersistentHighlighter.getHighlights()](../highlights/AuthorPersistentHighlighter.md#getHighlights()) methods.
  Returns: Returns the fragment comment highlights or custom highlights list. The type for a returned [AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md) can be [AuthorPersistentHighlight.PersistentHighlightType.COMMENT](../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#COMMENT) or [AuthorPersistentHighlight.PersistentHighlightType.CUSTOM_HIGHLIGHT](../highlights/AuthorPersistentHighlight.PersistentHighlightType.md#CUSTOM_HIGHLIGHT). The custom highlights can be inserted and managed by using the [AuthorPersistentHighlighter](../highlights/AuthorPersistentHighlighter.md). Since: 12
### setCommentAndCustomHighlights

public void setCommentAndCustomHighlights([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> highlights)

**This class is intended for internal use only.** Set the list with the fragment comment highlights or custom highlights.
  Parameters: highlights - The comment highlights or custom highlights list. Since: 12
### setChangeHighlights

public void setChangeHighlights([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> markers)

**This class is intended for internal use only.** Set the list with the change tracking highlights.
  Parameters: markers - The change tracking highlights list. Since: 12
### setAttributesChanges

public void setAttributesChanges([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[AuthorElement](AuthorElement.md),[LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)>> attributesChanges)

Set the map of element to attribute changes.
  Parameters: attributesChanges - The map between element and attribute changes Since: 15.1
### isEmpty

public boolean isEmpty()
  Returns: true If the fragment is empty.
### containsSimpleText

public boolean containsSimpleText()

Check if an author document fragment content contains simple text.
  Returns: True if the content of the given author document fragment contains simple text (the whitespaces are ignored).
### clone

public [AuthorDocumentFragment](AuthorDocumentFragment.md) clone() throws [CloneNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CloneNotSupportedException.html)

Clone a fragment.
  Overrides: [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Throws: [CloneNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CloneNotSupportedException.html) Since: 21.1 See Also:
        * [Object.clone()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone())

### setSuggestedRelativeCaretOffset

public void setSuggestedRelativeCaretOffset(int suggestedRelativeCaretOffset)

Set the offset were the caret should be placed, relative to the beginning of the fragment.
  Parameters: suggestedRelativeCaretOffset - The offset relative to the beginning of the fragment. Since: 23
### getSuggestedRelativeCaretOffset

public int getSuggestedRelativeCaretOffset()

Get the offset were the caret should be placed, relative to the beginning of the fragment.
  Returns: Returns the offset. Since: 23
### setContentNodes

public void setContentNodes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](AuthorNode.md)> nodes)

Set the content nodes.
  Parameters: nodes - The content nodes
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
