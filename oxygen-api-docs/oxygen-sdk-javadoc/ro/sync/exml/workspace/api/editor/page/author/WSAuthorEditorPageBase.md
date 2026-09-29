Package [ro.sync.exml.workspace.api.editor.page.author](package-summary.md)

# Interface WSAuthorEditorPageBase
    All Superinterfaces: [AuthorTooltipCustomizerProvider](tooltip/AuthorTooltipCustomizerProvider.md), [WSEditorPage](../WSEditorPage.md), [WSTextBasedEditorPage](../WSTextBasedEditorPage.md)   All Known Subinterfaces: [AuthorEditorAccess](../../../../../../ecss/extensions/api/access/AuthorEditorAccess.md), [IWebappAuthorEditorAccess](../../../../../../ecss/extensions/api/webapp/access/IWebappAuthorEditorAccess.md), [WSAuthorComponentEditorPage](WSAuthorComponentEditorPage.md), [WSAuthorEditorPage](WSAuthorEditorPage.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WSAuthorEditorPageBaseextends [WSTextBasedEditorPage](../WSTextBasedEditorPage.md), [AuthorTooltipCustomizerProvider](tooltip/AuthorTooltipCustomizerProvider.md)
Provides access to methods related to the Author editor actions and information.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 void [addAuthorAttributesDisplayFilter](#addAuthorAttributesDisplayFilter(ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter))([AuthorAttributesDisplayFilter](../../../../../../ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md) attributesDisplayFilter)
Adds a filter for displaying attributes to the current author page.
  void [addAuthorCaretListener](#addAuthorCaretListener(ro.sync.ecss.extensions.api.AuthorCaretListener))([AuthorCaretListener](../../../../../../ecss/extensions/api/AuthorCaretListener.md) caretListener)
Adds a caret listener to the Author page.
  void [addAuthorMouseListener](#addAuthorMouseListener(ro.sync.ecss.extensions.api.AuthorMouseListener))([AuthorMouseListener](../../../../../../ecss/extensions/api/AuthorMouseListener.md) mouseListener)
Adds a mouse listener to the current author page.
  void [addDNDListener](#addDNDListener(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) dndListener)
Add a drag and drop listener in the Author editing mode.
  void [addPopUpMenuCustomizer](#addPopUpMenuCustomizer(ro.sync.ecss.extensions.api.structure.AuthorPopupMenuCustomizer))([AuthorPopupMenuCustomizer](../../../../../../ecss/extensions/api/structure/AuthorPopupMenuCustomizer.md) popUpCustomizer)
Add the pop-up menu customizer which can be used to customize the pop-up menu (add/remove actions) before showing it in the Author page.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [buildURLForReferencedContent](#buildURLForReferencedContent(int,boolean))(int caretOffset, boolean shortAnchor)
If the caret offset is somewhere inside an entity reference, an xi:include reference or a DITA content reference, this method will return an URL which when used with Oxygen's API (ro.sync.exml.workspace.api.Workspace.open(URL)) will open the target resource and then place the caret in the opened editor precisely at the location where it was in the original XML document which referenced the content.
  void [deleteSelection](#deleteSelection())()
Delete the current selected text, if any.
  void [editAttribute](#editAttribute(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String))([AuthorElement](../../../../../../ecss/extensions/api/node/AuthorElement.md) targetElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
Searches through the in-place editors added on the given element for the first one that edits the given attribute.
  [AuthorActionsProvider](actions/AuthorActionsProvider.md) [getActionsProvider](#getActionsProvider())()
Provides access to actions already defined in the Author page like: Undo, Redo, Display Full Tags, Edit Attributes, etc.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getAuthorComponent](#getAuthorComponent())()
Get the internal component on which the Author page is rendered.
  [AuthorFoldManager](fold/AuthorFoldManager.md) [getAuthorFoldManager](#getAuthorFoldManager())()
Get the fold manager which can be used to expand or collapse a fold.
  [AuthorSelectionModel](../../../../../../ecss/extensions/api/AuthorSelectionModel.md) [getAuthorSelectionModel](#getAuthorSelectionModel())()
Get the Author selection model containing access to all Author selection intervals and methods for adding simple and multiple selections.
  int[] [getBalancedSelection](#getBalancedSelection(int,int))(int selectionStart, int selectionEnd)
Usually returns the selection.
  int [getBalancedSelectionEnd](#getBalancedSelectionEnd())()
Usually returns the same value as [getSelectionEnd()](#getSelectionEnd()).
  int [getBalancedSelectionStart](#getBalancedSelectionStart())()
Usually returns the same value as [getSelectionStart()](#getSelectionStart()).
  [AuthorSchemaAwareEditingHandler](../../../../../../ecss/extensions/api/AuthorSchemaAwareEditingHandler.md) [getDefaultAuthorSchemaAwareEditingHandler](#getDefaultAuthorSchemaAwareEditingHandler())()
Get the default schema aware editing handler.
  [AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) [getFullySelectedNode](#getFullySelectedNode())()
Get the node which is fully and perfectly surrounded by the current selection in the Author editor. If the selection surrounds perfectly the node (the selection starts at the node start offset and ends immediately after the node end offset), the node will be returned, otherwise null will be returned.For example if a node is selected using Outline or the Breadcrumb, the method will return the corresponding node.
  [AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) [getFullySelectedNode](#getFullySelectedNode(int,int))(int selectionStart, int selectionEnd)
Get the node which is fully and perfectly surrounded by the given selection in the Author editor. If the selection surrounds perfectly the node (the selection starts at the node start offset and ends immediately after the node end offset), the node will be returned, otherwise null will be returned.For example if a node is selected using Outline or the Breadcrumb, the method will return the corresponding node.
  [AuthorHighlighter](../../../../../../ecss/extensions/api/highlights/AuthorHighlighter.md) [getHighlighter](#getHighlighter())()
Get the highlighter which can be used to add/remove/manage the custom user highlights
  [AuthorPersistentHighlighter](../../../../../../ecss/extensions/api/highlights/AuthorPersistentHighlighter.md) [getPersistentHighlighter](#getPersistentHighlighter())()
Get the persistent highlighter which can be used to add/remove/manage the custom persistent user highlights.
  [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[PseudoElementDescriptor](PseudoElementDescriptor.md),[Styles](../../../../../../ecss/css/Styles.md)> [getPseudoElementStyles](#getPseudoElementStyles(ro.sync.ecss.extensions.api.node.AuthorParentNode))([AuthorParentNode](../../../../../../ecss/extensions/api/node/AuthorParentNode.md) node)
Get the CSS styles used to render the pseudo-elements of an Author node.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSelectedText](#getSelectedText())()
Get the current selected text.
  int [getSelectionEnd](#getSelectionEnd())()
Get end offset of the current selection.
  int [getSelectionStart](#getSelectionStart())()
Get start offset of the current selection.
  [Styles](../../../../../../ecss/css/Styles.md) [getStyles](#getStyles(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) node)
Get the CSS styles which are used to render a particular Author node.
  int [getTagsDisplayMode](#getTagsDisplayMode())()
Get the display mode of the tags in the Author editor.
  void [goToNextEditablePosition](#goToNextEditablePosition(int,int))(int startOffset, int endOffset)
Identifies and goes to the next edit position.
  boolean [hasSelection](#hasSelection())()
Check if the editor page has a selection  Use [AuthorSelectionModel](../../../../../../ecss/extensions/api/AuthorSelectionModel.md) to get more information and access to the Author editor page selection.
  boolean [isOffsetInInvisibleBounds](#isOffsetInInvisibleBounds(int))(int offset)
Check whether the offset is in a region in the document which is not rendered.
  int [moveOutOfInvisibleBounds](#moveOutOfInvisibleBounds(int,boolean))(int offset, boolean forward)
Check whether the offset is in a region in the document which is not rendered.
  void [refresh](#refresh())()
Reload the CSS files and perform a refresh on the whole document to recompute the layout and the styles for all the nodes based on the new CSS files content.
  void [refresh](#refresh(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) authorNode)
Refresh the rendering layout and CSS styles for this node and all its contents.
  void [removeAuthorAttributesDisplayFilter](#removeAuthorAttributesDisplayFilter(ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter))([AuthorAttributesDisplayFilter](../../../../../../ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md) attributesDisplayFilter)
Remove a filter for displaying attributes to the current author page.
  void [removeAuthorCaretListener](#removeAuthorCaretListener(ro.sync.ecss.extensions.api.AuthorCaretListener))([AuthorCaretListener](../../../../../../ecss/extensions/api/AuthorCaretListener.md) caretListener)
Removes the specified caret listener from the Author page.
  void [removeAuthorMouseListener](#removeAuthorMouseListener(ro.sync.ecss.extensions.api.AuthorMouseListener))([AuthorMouseListener](../../../../../../ecss/extensions/api/AuthorMouseListener.md) mouseListener)
Removes the specified mouse listener from the current author page.
  void [removeDNDListener](#removeDNDListener(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) dndListener)
Remove a drag and drop listener.
  void [removePopUpMenuCustomizer](#removePopUpMenuCustomizer(ro.sync.ecss.extensions.api.structure.AuthorPopupMenuCustomizer))([AuthorPopupMenuCustomizer](../../../../../../ecss/extensions/api/structure/AuthorPopupMenuCustomizer.md) popUpCustomizer)
Add the pop-up menu customizer which can be used to customize the pop-up menu (add/remove actions) before showing it in the Author page.
  void [scrollToRectangle](#scrollToRectangle(ro.sync.exml.view.graphics.Rectangle))([Rectangle](../../../../../view/graphics/Rectangle.md) rectangle)
Scroll the Author viewport to a specific rectangle.
  void [select](#select(int,int))(int startOffset, int endOffset)
Select the interval between start and end offset.
  void [setPopUpMenuCustomizer](#setPopUpMenuCustomizer(ro.sync.ecss.extensions.api.structure.AuthorPopupMenuCustomizer))([AuthorPopupMenuCustomizer](../../../../../../ecss/extensions/api/structure/AuthorPopupMenuCustomizer.md) popUpCustomizer)  Deprecated.
This method removes all pop-up menu customizers already registered, please use the "addPopUpMenuCustomizer" method instead.
   void [setTagsDisplayMode](#setTagsDisplayMode(int))(int displayMode)
Set the display mode of the tags in the Author editor.
  [AuthorViewToModelInfo](../../../../../../ecss/extensions/api/AuthorViewToModelInfo.md) [viewToModel](#viewToModel(int,int))(int x, int y)
Get the position in the document corresponding to the point in the author viewport component.

### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.author.tooltip.[AuthorTooltipCustomizerProvider](tooltip/AuthorTooltipCustomizerProvider.md)
 [addTooltipCustomizer](tooltip/AuthorTooltipCustomizerProvider.md#addTooltipCustomizer(ro.sync.exml.workspace.api.editor.page.author.tooltip.AuthorTooltipCustomizer)), [removeTooltipCustomizer](tooltip/AuthorTooltipCustomizerProvider.md#removeTooltipCustomizer(ro.sync.exml.workspace.api.editor.page.author.tooltip.AuthorTooltipCustomizer))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSEditorPage](../WSEditorPage.md)
 [getParentEditor](../WSEditorPage.md#getParentEditor()), [hasFocus](../WSEditorPage.md#hasFocus()), [isEditable](../WSEditorPage.md#isEditable()), [requestFocus](../WSEditorPage.md#requestFocus()), [setEditable](../WSEditorPage.md#setEditable(boolean)), [setReadOnly](../WSEditorPage.md#setReadOnly(java.lang.String)), [setReadOnly](../WSEditorPage.md#setReadOnly(ro.sync.exml.workspace.api.editor.ReadOnlyReason))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSTextBasedEditorPage](../WSTextBasedEditorPage.md)
 [copy](../WSTextBasedEditorPage.md#copy()), [createAnchor](../WSTextBasedEditorPage.md#createAnchor(int)), [getCaretOffset](../WSTextBasedEditorPage.md#getCaretOffset()), [getColumnOfOffset](../WSTextBasedEditorPage.md#getColumnOfOffset(int)), [getLineOfOffset](../WSTextBasedEditorPage.md#getLineOfOffset(int)), [getLocationOnScreenAsPoint](../WSTextBasedEditorPage.md#getLocationOnScreenAsPoint(int,int)), [getLocationRelativeToEditorFromScreen](../WSTextBasedEditorPage.md#getLocationRelativeToEditorFromScreen(int,int)), [getOffsetForAnchor](../WSTextBasedEditorPage.md#getOffsetForAnchor(ro.sync.exml.workspace.api.editor.page.Anchor)), [getStartEndOffsets](../WSTextBasedEditorPage.md#getStartEndOffsets(ro.sync.document.DocumentPositionedInfo)), [getWordAtCaret](../WSTextBasedEditorPage.md#getWordAtCaret()), [modelToViewRectangle](../WSTextBasedEditorPage.md#modelToViewRectangle(int)), [scrollCaretToVisible](../WSTextBasedEditorPage.md#scrollCaretToVisible()), [selectWord](../WSTextBasedEditorPage.md#selectWord()), [setCaretPosition](../WSTextBasedEditorPage.md#setCaretPosition(int)), [viewToModelOffset](../WSTextBasedEditorPage.md#viewToModelOffset(int,int))
## Method Details

### viewToModel

[AuthorViewToModelInfo](../../../../../../ecss/extensions/api/AuthorViewToModelInfo.md) viewToModel(int x, int y)

Get the position in the document corresponding to the point in the author viewport component.
  Parameters: x - The "x" coordinate relative to the viewport origin. y - The "y" coordinate relative to the viewport origin. Returns: The [AuthorViewToModelInfo](../../../../../../ecss/extensions/api/AuthorViewToModelInfo.md) containing the offset and the node at offset corresponding to the given point. The method does not return null, instead an undefined view to model info object is returned if a valid one could not be determined.
### setPopUpMenuCustomizer

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void setPopUpMenuCustomizer([AuthorPopupMenuCustomizer](../../../../../../ecss/extensions/api/structure/AuthorPopupMenuCustomizer.md) popUpCustomizer)
 Deprecated.
This method removes all pop-up menu customizers already registered, please use the "addPopUpMenuCustomizer" method instead.

Set the pop-up menu customizer which can be used to customize the pop-up menu (add/remove actions) before showing it in the Author page.
  Parameters: popUpCustomizer - the pop-up menu customizer.
### addPopUpMenuCustomizer

void addPopUpMenuCustomizer([AuthorPopupMenuCustomizer](../../../../../../ecss/extensions/api/structure/AuthorPopupMenuCustomizer.md) popUpCustomizer)

Add the pop-up menu customizer which can be used to customize the pop-up menu (add/remove actions) before showing it in the Author page.
  Parameters: popUpCustomizer - the pop-up menu customizer. If the customizer is already added, it will not be added again. Since: 14.1
### removePopUpMenuCustomizer

void removePopUpMenuCustomizer([AuthorPopupMenuCustomizer](../../../../../../ecss/extensions/api/structure/AuthorPopupMenuCustomizer.md) popUpCustomizer)

Add the pop-up menu customizer which can be used to customize the pop-up menu (add/remove actions) before showing it in the Author page.
  Parameters: popUpCustomizer - the pop-up menu customizer. Since: 14.1
### addAuthorMouseListener

void addAuthorMouseListener([AuthorMouseListener](../../../../../../ecss/extensions/api/AuthorMouseListener.md) mouseListener)

Adds a mouse listener to the current author page.
  Parameters: mouseListener - The [AuthorMouseListener](../../../../../../ecss/extensions/api/AuthorMouseListener.md) to be added.
### removeAuthorMouseListener

void removeAuthorMouseListener([AuthorMouseListener](../../../../../../ecss/extensions/api/AuthorMouseListener.md) mouseListener)

Removes the specified mouse listener from the current author page.
  Parameters: mouseListener - The [AuthorMouseListener](../../../../../../ecss/extensions/api/AuthorMouseListener.md) to be removed.
### addAuthorCaretListener

void addAuthorCaretListener([AuthorCaretListener](../../../../../../ecss/extensions/api/AuthorCaretListener.md) caretListener)

Adds a caret listener to the Author page.
  Parameters: caretListener - The [AuthorCaretListener](../../../../../../ecss/extensions/api/AuthorCaretListener.md) to be added.
### removeAuthorCaretListener

void removeAuthorCaretListener([AuthorCaretListener](../../../../../../ecss/extensions/api/AuthorCaretListener.md) caretListener)

Removes the specified caret listener from the Author page.
  Parameters: caretListener - The [AuthorCaretListener](../../../../../../ecss/extensions/api/AuthorCaretListener.md) to be removed.
### refresh

void refresh([AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) authorNode)

Refresh the rendering layout and CSS styles for this node and all its contents.
**Note:** This should be called on the AWT thread because it will generate a layout event.

  Parameters: authorNode - The node for which the layout and styles will be recomputed.
### refresh

void refresh()

Reload the CSS files and perform a refresh on the whole document to recompute the layout and the styles for all the nodes based on the new CSS files content.

### getHighlighter

[AuthorHighlighter](../../../../../../ecss/extensions/api/highlights/AuthorHighlighter.md) getHighlighter()

Get the highlighter which can be used to add/remove/manage the custom user highlights
  Returns: The highlighter which can be used to add/remove/manage the custom user highlights.
### getPersistentHighlighter

[AuthorPersistentHighlighter](../../../../../../ecss/extensions/api/highlights/AuthorPersistentHighlighter.md) getPersistentHighlighter()

Get the persistent highlighter which can be used to add/remove/manage the custom persistent user highlights. Persistent highlights get serialized in the XML as processing instructions with the form:  <?oxy_custom_start prop1="val1"....?> xml content <?oxy_custom_end?>
  Returns: The persistent highlighter which can be used to add/remove/manage the custom user highlights. Since: 12
### getBalancedSelectionStart

int getBalancedSelectionStart()

Usually returns the same value as [getSelectionStart()](#getSelectionStart()). If the selection start is immediately to the right of a start tag and the corresponding end tag is contained in the selection, then the balanced selection start will be obtained by extending the selection start to contain the start tag.
  Returns: The balanced selection start offset, 0 based. Since: 12
### getBalancedSelectionEnd

int getBalancedSelectionEnd()

Usually returns the same value as [getSelectionEnd()](#getSelectionEnd()). The offset is **exclusive** If the selection end is immediately to the left of a end tag and the corresponding start tag is contained in the selection, then the balanced selection end will be obtained by extending the selection end to contain the end tag. If the selection end is to the right of a tag which does not have the start included in the selection, then the selection end is decreased.
  Returns: The balanced selection end offset, 0 based. Since: 12
### getBalancedSelection

int[] getBalancedSelection(int selectionStart, int selectionEnd)

Usually returns the selection. If the selection start is immediately to the right of a start tag and the corresponding end tag is contained in the selection, then the balanced selection start will be obtained by extending the selection start to contain the start tag. If the selection end is immediately to the left of a end tag and the corresponding start tag is contained in the selection, then the balanced selection end will be obtained by extending the selection end to contain the end tag.
  Parameters: selectionStart - The inclusive selection start. selectionEnd - The exclusive selection end. Returns: The balanced selection obtained from the given selection, 0 based. The first element of the returned array represents the selection start. and the second element represents the selection end. Since: 16
### getDefaultAuthorSchemaAwareEditingHandler

[AuthorSchemaAwareEditingHandler](../../../../../../ecss/extensions/api/AuthorSchemaAwareEditingHandler.md) getDefaultAuthorSchemaAwareEditingHandler()

Get the default schema aware editing handler. This can be used from a custom AuthorSchemaAwareEditingHandler implementation from an ExtensionsBundle to delegate various operations to.
  Returns: the default schema aware editing handler. Since: 12.1
### getActionsProvider

[AuthorActionsProvider](actions/AuthorActionsProvider.md) getActionsProvider()

Provides access to actions already defined in the Author page like: Undo, Redo, Display Full Tags, Edit Attributes, etc.
  Returns: access to actions already defined in the Author page. Since: 12.1
### getAuthorComponent

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getAuthorComponent()

Get the internal component on which the Author page is rendered. Use of this method is discouraged but it may be useful in some cases like: This can be helpful when you want to set a busy cursor on the component for example or when you want to get access to the scroll bars. You can also request focus in the component by casting it to its native equivalent.
  Returns: for the stand alone version, a javax.swing.JPanel and for the eclipse implementation a org.eclipse.swt.widgets.Canvas. Since: 12.2
### getStyles

[Styles](../../../../../../ecss/css/Styles.md) getStyles([AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) node)

Get the CSS styles which are used to render a particular Author node. This method **MUST** only be used to query styles. If you want to modify styles please use the [StylesFilter](../../../../../../ecss/extensions/api/StylesFilter.md).
  Parameters: node - The node for which we want to obtain the styles. Returns: the styles associated with the node. Since: 12.2
### getPseudoElementStyles

[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[PseudoElementDescriptor](PseudoElementDescriptor.md),[Styles](../../../../../../ecss/css/Styles.md)> getPseudoElementStyles([AuthorParentNode](../../../../../../ecss/extensions/api/node/AuthorParentNode.md) node)

Get the CSS styles used to render the pseudo-elements of an Author node. This method **MUST** only be used to query styles. If you want to modify styles, use the [StylesFilter](../../../../../../ecss/extensions/api/StylesFilter.md).
  Parameters: node - The node for which we want to obtain the pseudo-element styles. Returns: the styles of the pseudo-elements or an empty map. Never null. Since: 23
### addAuthorAttributesDisplayFilter

void addAuthorAttributesDisplayFilter([AuthorAttributesDisplayFilter](../../../../../../ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md) attributesDisplayFilter)

Adds a filter for displaying attributes to the current author page.
  Parameters: attributesDisplayFilter - The [AuthorAttributesDisplayFilter](../../../../../../ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md) to be added. Since: 13
### removeAuthorAttributesDisplayFilter

void removeAuthorAttributesDisplayFilter([AuthorAttributesDisplayFilter](../../../../../../ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md) attributesDisplayFilter)

Remove a filter for displaying attributes to the current author page.
  Parameters: attributesDisplayFilter - The [AuthorAttributesDisplayFilter](../../../../../../ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md) to be added. Since: 13
### getFullySelectedNode

[AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) getFullySelectedNode()

Get the node which is fully and perfectly surrounded by the current selection in the Author editor. If the selection surrounds perfectly the node (the selection starts at the node start offset and ends immediately after the node end offset), the node will be returned, otherwise null will be returned.For example if a node is selected using Outline or the Breadcrumb, the method will return the corresponding node. In such cases the method [AuthorDocumentController.getNodeAtOffset(int)](../../../../../../ecss/extensions/api/AuthorDocumentController.md#getNodeAtOffset(int)) called for the caret offset always returns the parent of the selected element as the caret is actually outside the selected element. Thus, in order to obtain the context node, this method should be used and if it returns null you can use the [AuthorDocumentController.getNodeAtOffset(int)](../../../../../../ecss/extensions/api/AuthorDocumentController.md#getNodeAtOffset(int)) method.
  Returns: The selected node if the selection surrounds perfectly the node, null otherwise. Since: 13.1
### getFullySelectedNode

[AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) getFullySelectedNode(int selectionStart, int selectionEnd)

Get the node which is fully and perfectly surrounded by the given selection in the Author editor. If the selection surrounds perfectly the node (the selection starts at the node start offset and ends immediately after the node end offset), the node will be returned, otherwise null will be returned.For example if a node is selected using Outline or the Breadcrumb, the method will return the corresponding node. In such cases the method [AuthorDocumentController.getNodeAtOffset(int)](../../../../../../ecss/extensions/api/AuthorDocumentController.md#getNodeAtOffset(int)) called for the caret offset always returns the parent of the selected element as the caret is actually outside the selected element. Thus, in order to obtain the context node, this method should be used and if it returns null you can use the [AuthorDocumentController.getNodeAtOffset(int)](../../../../../../ecss/extensions/api/AuthorDocumentController.md#getNodeAtOffset(int)) method.
  Parameters: selectionStart - **Inclusive** start offset. selectionEnd - **Exclusive** end offset. Returns: The selected node if the given selection surrounds perfectly the node, null otherwise. Since: 16
### getAuthorSelectionModel

[AuthorSelectionModel](../../../../../../ecss/extensions/api/AuthorSelectionModel.md) getAuthorSelectionModel()

Get the Author selection model containing access to all Author selection intervals and methods for adding simple and multiple selections.
  Returns: The Author selection model. Since: 14
### getSelectionStart

int getSelectionStart()

Get start offset of the current selection. It is **inclusive**.  If the Author editor page has multiple selection intervals, this method returns the start offset of the last selected content interval. Use [AuthorSelectionModel](../../../../../../ecss/extensions/api/AuthorSelectionModel.md) to get more information and access to the Author editor page selection.  If there is no selection in Author editor page, the caret offset is returned.
  Specified by: [getSelectionStart](../WSTextBasedEditorPage.md#getSelectionStart()) in interface [WSTextBasedEditorPage](../WSTextBasedEditorPage.md) Returns: The selection start offset, 0 based.
### getSelectionEnd

int getSelectionEnd()

Get end offset of the current selection. It is **exclusive**  If the Author editor page has multiple selection intervals, this method returns the end offset of the last selected content interval. Use [AuthorSelectionModel](../../../../../../ecss/extensions/api/AuthorSelectionModel.md) to get more information and access to the Author editor page selection.  If there is no selection in Author editor page, the caret offset is returned.
  Specified by: [getSelectionEnd](../WSTextBasedEditorPage.md#getSelectionEnd()) in interface [WSTextBasedEditorPage](../WSTextBasedEditorPage.md) Returns: The selection end offset, 0 based.
### getSelectedText

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSelectedText()

Get the current selected text. The text does not contain XML tags for the Author page.  If the Author editor page has multiple selection intervals, this method returns the text from the last selected content interval. Use [AuthorSelectionModel](../../../../../../ecss/extensions/api/AuthorSelectionModel.md) to get more information and access to the Author editor page selection.
  Specified by: [getSelectedText](../WSTextBasedEditorPage.md#getSelectedText()) in interface [WSTextBasedEditorPage](../WSTextBasedEditorPage.md) Returns: The selected text or an empty string if no selection is present.
### deleteSelection

void deleteSelection()

Delete the current selected text, if any.  If the Author editor page has multiple selection intervals, this method deletes the content from the last selected interval. Use [AuthorSelectionModel](../../../../../../ecss/extensions/api/AuthorSelectionModel.md) to get more information and access to the Author editor page selection.
  Specified by: [deleteSelection](../WSTextBasedEditorPage.md#deleteSelection()) in interface [WSTextBasedEditorPage](../WSTextBasedEditorPage.md)
### hasSelection

boolean hasSelection()

Check if the editor page has a selection  Use [AuthorSelectionModel](../../../../../../ecss/extensions/api/AuthorSelectionModel.md) to get more information and access to the Author editor page selection.
  Specified by: [hasSelection](../WSTextBasedEditorPage.md#hasSelection()) in interface [WSTextBasedEditorPage](../WSTextBasedEditorPage.md) Returns: true if there is a selection, false otherwise.
### select

void select(int startOffset, int endOffset)

Select the interval between start and end offset.  Use [AuthorSelectionModel](../../../../../../ecss/extensions/api/AuthorSelectionModel.md) to get more information and access to the Author editor page selection.
  Specified by: [select](../WSTextBasedEditorPage.md#select(int,int)) in interface [WSTextBasedEditorPage](../WSTextBasedEditorPage.md) Parameters: startOffset - **Inclusive** start offset endOffset - **Exclusive** end offset
### isOffsetInInvisibleBounds

boolean isOffsetInInvisibleBounds(int offset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Check whether the offset is in a region in the document which is not rendered. For example: oxy-collapse-text nodes, 'display: none' nodes or tracked deleted content which is not presented in 'Final' mode.
  Parameters: offset - The offset to check. Returns: true if the offset is in an invisible region. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If the offset is outside the document.
### moveOutOfInvisibleBounds

int moveOutOfInvisibleBounds(int offset, boolean forward)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Check whether the offset is in a region in the document which is not rendered. If this is the case, this method returns an offset which is outside that region in the specified direction. For example: oxy-collapse-text nodes, 'display: none' nodes or tracked deleted content which is not presented in 'Final' mode are considered invisible.
  Parameters: offset - The offset to check. forward - true if we should move to a position in a forward direction. Returns: an offset that is outside of the invisible region in the specified direction. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If the offset is outside the document. Since: 17
### goToNextEditablePosition

void goToNextEditablePosition(int startOffset, int endOffset)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Identifies and goes to the next edit position. Depending on which is first, this can be:
        * An offset inside the first leaf element or the first element with mixed content.
        * An in-place editor used to edit the value of an attribute (for example a checkbox). In this case the editor will be activated.
The offset should be in the given interval specified by startOffset and endOffset exclusive.
  Parameters: startOffset - The offset from where to start looking. endOffset - The offset where to stop looking for. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - The given offset is invalid. Since: 14.1
### editAttribute

void editAttribute([AuthorElement](../../../../../../ecss/extensions/api/node/AuthorElement.md) targetElement, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)

Searches through the in-place editors added on the given element for the first one that edits the given attribute. If such an editor is found it will activate the editor to start editing. Hypothetically there could be more than one editor for the same attribute (even though is not a real use case nor is it encouraged) but we'll activate the first one we encounter. The search will first look at the BEFORE styles, then the element styles and finally the AFTER styles.
  Parameters: targetElement - The parent element of the attribute. attributeName - The QName of the searched attribute. Since: 14.1
### scrollToRectangle

void scrollToRectangle([Rectangle](../../../../../view/graphics/Rectangle.md) rectangle)

Scroll the Author viewport to a specific rectangle. To find the rectangle that corresponds to a specific offset in the Author document you can use the [WSTextBasedEditorPage.modelToViewRectangle(int)](../WSTextBasedEditorPage.md#modelToViewRectangle(int)) method.
  Parameters: rectangle - The rectangle to scroll to. Since: 14.1
### getAuthorFoldManager

[AuthorFoldManager](fold/AuthorFoldManager.md) getAuthorFoldManager()

Get the fold manager which can be used to expand or collapse a fold.
  Returns: the fold manager. Since: 17
### addDNDListener

void addDNDListener([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) dndListener)

Add a drag and drop listener in the Author editing mode.
  Parameters: dndListener - The drag and drop listener. Needs to be an instance of "ro.sync.exml.editor.xmleditor.pageauthor.AuthorDnDListener" for the standalone implementation and com.oxygenxml.editor.editors.author.AuthorDnDListener for the Eclipse implementation. Since: 17.1
### removeDNDListener

void removeDNDListener([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) dndListener)

Remove a drag and drop listener.
  Parameters: dndListener - The drag and drop listener to remove. Since: 17.1
### setTagsDisplayMode

void setTagsDisplayMode(int displayMode)

Set the display mode of the tags in the Author editor.
  Parameters: displayMode - The tags display mode, one of [DisplayModeConstants](DisplayModeConstants.md) constants. Since: 17.1
### getTagsDisplayMode

int getTagsDisplayMode()

Get the display mode of the tags in the Author editor.
  Returns: The tags display mode (one of [DisplayModeConstants](DisplayModeConstants.md) constants). Since: 17.1
### buildURLForReferencedContent

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) buildURLForReferencedContent(int caretOffset, boolean shortAnchor)

If the caret offset is somewhere inside an entity reference, an xi:include reference or a DITA content reference, this method will return an URL which when used with Oxygen's API (ro.sync.exml.workspace.api.Workspace.open(URL)) will open the target resource and then place the caret in the opened editor precisely at the location where it was in the original XML document which referenced the content.
  Parameters: caretOffset - The offset at which the caret is currently located. shortAnchor - Flag telling whether to build a short version of the referenced content URL or not. This format is used in Web Author. Returns: A URL with a precise localization anchor included or null if the caret position is not inside a reference. Since: 19.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
