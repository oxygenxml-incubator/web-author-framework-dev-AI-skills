Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorDocumentFilter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorDocumentFilter
   @API(type=EXTENDABLE, src=PUBLIC) public class AuthorDocumentFilter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
AuthorDocumentFilter, is a filter for the methods which modify the AuthorDocument. When the AuthorDocumentis modified through the methods from the AuthorDocumentController, the appropriate method invocation is forwarded to the AuthorDocumentFilter. The default implementation allows the modification to occur. Subclasses can filter the modifications by conditionally invoking methods on the superclass, or invoking the necessary methods on the passed in AuthorDocumentFilterBypass.
**Warning: Subclasses should NOT call back into the AuthorDocumentController for modifications in the document instead call into the superclass or the AuthorDocumentFilterBypass!**

When methods are invoked on the AuthorDocumentFilter, the AuthorDocumentFilter may callback into the AuthorDocumentFilterBypass multiple times, or for different regions, but it should not callback into the AuthorDocumentFilterBypass after returning from the initially called method.

If you are working with framework level API, a good place to add an AuthorDocumentFilter in on [AuthorExtensionStateListener.activated(AuthorAccess)](AuthorExtensionStateListener.md#activated(ro.sync.ecss.extensions.api.AuthorAccess)) notification.

If you are working with plugin level API you can add an AuthorDocumentFilter in an Workspace Access plugin:

```

   public void applicationStarted(final StandalonePluginWorkspace pluginWorkspaceAccess) {
    pluginWorkspaceAccess.addEditorChangeListener(
        new WSEditorChangeListener() {
          public void editorOpened(URL editorLocation) {
            WSEditor editorAccess = pluginWorkspaceAccess.getEditorAccess(editorLocation, PluginWorkspace.MAIN_EDITING_AREA);
            WSEditorPage currentPage = editorAccess.getCurrentPage();
            if (currentPage instanceof WSAuthorEditorPage) {
              WSAuthorEditorPage authorEditorPage = (WSAuthorEditorPage) currentPage;
              authorEditorPage.getAuthorAccess().getDocumentController().setDocumentFilter(authorDocumentFilter);
            }
            // It's also a good idea to listener for page changes on the editor.
            // Perhaps the editor opens in the text page and the user switches later on to author.
            editorAccess.addPageChangedListener(new WSEditorPageChangedListener() {
              public void editorPageChanged() {
                // Same code here to add the filter.
              }
            });
          }
        },
        PluginWorkspace.MAIN_EDITING_AREA);

```

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorDocumentFilter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) [addCommentMarker](#addCommentMarker(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,int,int,java.lang.String,java.lang.String))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) comment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentID)
Add a comment marker for the given interval.
  [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) [addPersistentMarker](#addPersistentMarker(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight.PersistentHighlightType,int,int,java.util.Map))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorPersistentHighlight.PersistentHighlightType](highlights/AuthorPersistentHighlight.PersistentHighlightType.md) type, int startOffset, int endOffset, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties)
Add a comment marker for the given interval.
  boolean [delete](#delete(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,int,int,boolean))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int startOffset, int endOffset, boolean withBackspace)
Invoked before deleting the fragment between the specified offsets from the document.
  boolean [deleteNode](#deleteNode(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorNode](node/AuthorNode.md) node)
Invoked before deleting the specified node from the document.
  void [insertFragment](#insertFragment(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,int,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int offset, [AuthorDocumentFragment](node/AuthorDocumentFragment.md) frag)
Invoked before inserting an [AuthorDocumentFragment](node/AuthorDocumentFragment.md) at the specified offset.
  void [insertMultipleElements](#insertMultipleElements(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String%5B%5D,int%5B%5D,java.lang.String))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorElement](node/AuthorElement.md) parentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementNames, int[] offsets, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Invoked before inserting multiple elements at the given offsets.
  boolean [insertMultipleFragments](#insertMultipleFragments(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,ro.sync.ecss.extensions.api.node.AuthorElement,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,int%5B%5D))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorElement](node/AuthorElement.md) parentElement, [AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragments, int[] offsets)
Invoked before inserting multiple fragments at the given offsets.
  boolean [insertNode](#insertNode(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,int,ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int offset, [AuthorNode](node/AuthorNode.md) node)
Invoked before inserting a simple node into the document.
  void [insertText](#insertText(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,int,java.lang.String))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int offset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toInsert)
Invoked before inserting the specified text at the given offset.
  void [multipleDelete](#multipleDelete(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,ro.sync.ecss.extensions.api.node.AuthorElement,int%5B%5D,int%5B%5D))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorElement](node/AuthorElement.md) parentElement, int[] startOffsets, int[] endOffsets)
Invoked before deleting the given intervals from the document.
  void [removeAttribute](#removeAttribute(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AuthorElement](node/AuthorElement.md) element)
Invoked before removing an attribute from the specified element.
  boolean [removeMarker](#removeMarker(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) marker)
Remove a persistent marker.
  void [renameElement](#renameElement(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.Object))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorElement](node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newName, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) infoProvider)
Invoked before renaming the given element.
  void [setAttribute](#setAttribute(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,java.lang.String,ro.sync.ecss.extensions.api.node.AttrValue,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AttrValue](node/AttrValue.md) value, [AuthorElement](node/AuthorElement.md) element)
Invoked before setting the value of an attribute in the specified element.
  void [setDoctype](#setDoctype(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,ro.sync.ecss.extensions.api.AuthorDocumentType))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorDocumentType](AuthorDocumentType.md) docType)
Invoked before setting a new internal document type to the Author content.
  void [setMultipleAttributes](#setMultipleAttributes(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,int,int%5B%5D,java.util.Map))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int parentElementStartOffset, int[] elementOffsets, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](node/AttrValue.md)> attributes)
Sets the value of the given attribute in the specified elements.
  void [setMultipleDistinctAttributes](#setMultipleDistinctAttributes(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,int,int%5B%5D,java.util.List))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int parentElementStartOffset, int[] elementOffsets, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](node/AttrValue.md)>> attributes)
Sets the value of the given attribute in the specified elements.
  boolean [split](#split(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,ro.sync.ecss.extensions.api.node.AuthorNode,int))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorNode](node/AuthorNode.md) toSplit, int splitOffset)
Invoked before splitting the specified node into two similar nodes.
  void [surroundInFragment](#surroundInFragment(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,java.lang.String,int,int))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int startOffset, int endOffset)
Invoked before surrounding the content between the given offsets with the xmlFragment.
  void [surroundInFragment](#surroundInFragment(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment,int,int))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorDocumentFragment](node/AuthorDocumentFragment.md) xmlFragment, int startOffset, int endOffset)
Invoked before surrounding the content between the given offsets with the xmlFragment.
  void [surroundInText](#surroundInText(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,java.lang.String,java.lang.String,int,int))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) header, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) footer, int startOffset, int endOffset)
Invoked before surrounding the content between the given offsets with plain text fragments(without XML parsing).
  void [surroundWithNode](#surroundWithNode(ro.sync.ecss.extensions.api.AuthorDocumentFilterBypass,ro.sync.ecss.extensions.api.node.AuthorNode,int,int,boolean))([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorNode](node/AuthorNode.md) node, int startOffset, int endOffset, boolean leftToRight)
Invoked before surrounding the fragment between the specified offset with the specified node.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorDocumentFilter

public AuthorDocumentFilter()

## Method Details

### insertText

public void insertText([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int offset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toInsert)

Invoked before inserting the specified text at the given offset.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. offset - The offset where the text will be inserted. 0 based. toInsert - The text to be inserted.
### insertFragment

public void insertFragment([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int offset, [AuthorDocumentFragment](node/AuthorDocumentFragment.md) frag)

Invoked before inserting an [AuthorDocumentFragment](node/AuthorDocumentFragment.md) at the specified offset.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. offset - The offset where the fragment will be inserted. 0 based. frag - The [AuthorDocumentFragment](node/AuthorDocumentFragment.md) to be inserted.
### insertNode

public boolean insertNode([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int offset, [AuthorNode](node/AuthorNode.md) node)

Invoked before inserting a simple node into the document.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. offset - The offset where the node should be inserted. 0 based. node - The [AuthorNode](node/AuthorNode.md) to be inserted. Returns: true if the insert node operation succeeded.
### insertMultipleElements

public void insertMultipleElements([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorElement](node/AuthorElement.md) parentElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementNames, int[] offsets, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)

Invoked before inserting multiple elements at the given offsets. Note: *The offsets and elements are in document order and this rule must also be followed by the filter processing.*
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. parentElement - The parent element that contains all the new inserted elements. elementNames - The element names to be inserted. offsets - The absolute offsets where the elements will be inserted. 0 based. namespace - The namespace of the new inserted elements.
### insertMultipleFragments

public boolean insertMultipleFragments([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorElement](node/AuthorElement.md) parentElement, [AuthorDocumentFragment](node/AuthorDocumentFragment.md)[] fragments, int[] offsets)

Invoked before inserting multiple fragments at the given offsets. Note: *The offsets and fragments are in document order and this rule must also be followed by the filter processing.*
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. parentElement - The parent element that contains all the new inserted elements. fragments - The fragments to be inserted. offsets - The absolute offsets where the fragments will be inserted. 0 based. Returns: true if the insert operation succeed. Since: 14
### delete

public boolean delete([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int startOffset, int endOffset, boolean withBackspace)

Invoked before deleting the fragment between the specified offsets from the document.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. startOffset - Start offset of the fragment, 0 based and inclusive. endOffset - End offset of the fragment, 0 based and inclusive. withBackspace - true if BACKSPACE key was used for deleting the fragment. Returns: true If the delete operation succeeded.
### deleteNode

public boolean deleteNode([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorNode](node/AuthorNode.md) node)

Invoked before deleting the specified node from the document.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. node - The [AuthorNode](node/AuthorNode.md) to delete. Returns: true if the delete node operation was successful.
### multipleDelete

public void multipleDelete([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorElement](node/AuthorElement.md) parentElement, int[] startOffsets, int[] endOffsets)

Invoked before deleting the given intervals from the document. Note: *The offsets must be in document order and the intervals must not intersect with each other. This rule must also be followed by the filter processing.*
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. parentElement - The element that contains all the deleted intervals. startOffsets - The start offset for each interval. Must be in document order. 0 based and inclusive. endOffsets - The end offset for each interval. Must be in document order. 0 based and inclusive.
### renameElement

public void renameElement([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorElement](node/AuthorElement.md) element, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newName, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) infoProvider)

Invoked before renaming the given element.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. element - The [AuthorElement](node/AuthorElement.md) that is renamed. newName - The new name for the element. infoProvider - Information provider used for internal processing. It must NOT be altered inside this [AuthorDocumentFilter](AuthorDocumentFilter.md) method.
### setAttribute

public void setAttribute([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AttrValue](node/AttrValue.md) value, [AuthorElement](node/AuthorElement.md) element)

Invoked before setting the value of an attribute in the specified element.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. attributeName - Name of the attribute being changed. value - New [AttrValue](node/AttrValue.md) for the attribute. If null, the attribute is removed from the element. element - The [AuthorElement](node/AuthorElement.md) whose attribute we are editing.
### removeAttribute

public void removeAttribute([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [AuthorElement](node/AuthorElement.md) element)

Invoked before removing an attribute from the specified element.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. attributeName - Name of the attribute to remove. element - The [AuthorElement](node/AuthorElement.md) whose attribute will be removed.
### split

public boolean split([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorNode](node/AuthorNode.md) toSplit, int splitOffset)

Invoked before splitting the specified node into two similar nodes. The node to split is the first ancestor block level node containing the splitOffset. The attributes of the splitted node will also be copied excepting the unique ones. The unique attributes are identified by the [UniqueAttributesRecognizer](UniqueAttributesRecognizer.md).
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. toSplit - The [AuthorNode](node/AuthorNode.md) to split. splitOffset - The split offset. The given offset is greater or equal to 1 and less than the current document length. Returns: true if the node was split.
### surroundWithNode

public void surroundWithNode([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorNode](node/AuthorNode.md) node, int startOffset, int endOffset, boolean leftToRight)

Invoked before surrounding the fragment between the specified offset with the specified node. The fragment between the start and end offsets will become the node actual content.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. node - The [AuthorNode](node/AuthorNode.md) that will surround the fragment. startOffset - Start offset of the surrounded fragment. 0 based and inclusive. endOffset - End offset of the surrounded fragment. 0 based and inclusive. leftToRight - true if after the operation the selection in the author page is done from the left to the right.
### surroundInFragment

public void surroundInFragment([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int startOffset, int endOffset)throws [AuthorOperationException](AuthorOperationException.md)

Invoked before surrounding the content between the given offsets with the xmlFragment. If endOffset < startOffset the xmlFragment will be inserted at startOffset.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. xmlFragment - The XML fragment which will surround the given interval. The first leaf node of the XML fragment will be the parent of the surrounded content. startOffset - The start offset of the content to be surrounded, 0 based and inclusive. endOffset - The end offset of the content to be surrounded, 0 based and inclusive. Throws: [AuthorOperationException](AuthorOperationException.md) - If the content between start and end offset could not be surrounded.
### surroundInFragment

public void surroundInFragment([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorDocumentFragment](node/AuthorDocumentFragment.md) xmlFragment, int startOffset, int endOffset)throws [AuthorOperationException](AuthorOperationException.md)

Invoked before surrounding the content between the given offsets with the xmlFragment. If endOffset < startOffset the xmlFragment will be inserted at startOffset.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. xmlFragment - The XML fragment which will surround the given interval. The first leaf node of the XML fragment will be the parent of the surrounded content. startOffset - The start offset of the content to be surrounded, 0 based and inclusive. endOffset - The end offset of the content to be surrounded, 0 based and inclusive. Throws: [AuthorOperationException](AuthorOperationException.md) Since: 12.1
### surroundInText

public void surroundInText([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) header, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) footer, int startOffset, int endOffset)throws [AuthorOperationException](AuthorOperationException.md)

Invoked before surrounding the content between the given offsets with plain text fragments(without XML parsing). The method inserts the header at startOffset and the footer at endOffset.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. header - The header to be inserted before the surrounded text. footer - The footer to be inserted after the surrounded text. startOffset - The start offset of the text to be surrounded, 0 based and inclusive. endOffset - The end offset of the text to be surrounded, 0 based and inclusive. Throws: [AuthorOperationException](AuthorOperationException.md) - If the operation failed.
### setDoctype

public void setDoctype([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorDocumentType](AuthorDocumentType.md) docType)

Invoked before setting a new internal document type to the Author content.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. docType - The document type information to set.
### setMultipleDistinctAttributes

public void setMultipleDistinctAttributes([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int parentElementStartOffset, int[] elementOffsets, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](node/AttrValue.md)>> attributes)

Sets the value of the given attribute in the specified elements. Attributes set in this manner will be subject to undo/redo.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. parentElementStartOffset - The start offset of the parent element. elementOffsets - The start offset for each element. attributes - The list with attributes. Every attribute name is mapped to an [AttrValue](node/AttrValue.md) object. If the value is null, the attribute will be removed.
### setMultipleAttributes

public void setMultipleAttributes([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int parentElementStartOffset, int[] elementOffsets, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[AttrValue](node/AttrValue.md)> attributes)

Sets the value of the given attribute in the specified elements. Attributes set in this manner will be subject to undo/redo.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. parentElementStartOffset - The start offset of the parent element. elementOffsets - The start offset for each element. attributes - The list with attributes. Every attribute name is mapped to an [AttrValue](node/AttrValue.md) object. If the value is null, the attribute will be removed.
### removeMarker

public boolean removeMarker([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) marker)

Remove a persistent marker.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. marker - The persistent marker to remove. Returns: true if the marker was removed Since: 22
### addCommentMarker

public [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) addCommentMarker([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, int startOffset, int endOffset, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) comment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentID)

Add a comment marker for the given interval.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. startOffset - Start offset of marker endOffset - End offset of marker comment - The comment to be added. parentID - The comment parent id (not null for replies). Returns: The added comment highlight if the comment was added or null. Since: 22
### addPersistentMarker

public [AuthorPersistentHighlight](highlights/AuthorPersistentHighlight.md) addPersistentMarker([AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) filterBypass, [AuthorPersistentHighlight.PersistentHighlightType](highlights/AuthorPersistentHighlight.PersistentHighlightType.md) type, int startOffset, int endOffset, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> properties)

Add a comment marker for the given interval.
Subclasses that want to conditionally modify the default processing should override this and only call super implementation as necessary, or call directly into the [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md) as necessary.

  Parameters: filterBypass - The document filter bypass used for executing operations directly, without additional filtering. type - The persistent marker type (comment or custom) startOffset - Start offset of marker endOffset - End offset of marker properties - The comment properties. See [AuthorPersistentHighlightConstants](highlights/AuthorPersistentHighlightConstants.md) for properties that are meaningful in Oxygen. Returns: The added comment highlight if the comment was added or null. Since: 23
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
