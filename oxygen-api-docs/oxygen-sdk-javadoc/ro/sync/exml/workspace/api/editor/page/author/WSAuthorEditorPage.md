Package [ro.sync.exml.workspace.api.editor.page.author](package-summary.md)

# Interface WSAuthorEditorPage
    All Superinterfaces: [AuthorTooltipCustomizerProvider](tooltip/AuthorTooltipCustomizerProvider.md), [WSAuthorEditorPageBase](WSAuthorEditorPageBase.md), [WSEditorPage](../WSEditorPage.md), [WSTextBasedEditorPage](../WSTextBasedEditorPage.md)   All Known Subinterfaces: [WSAuthorComponentEditorPage](WSAuthorComponentEditorPage.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WSAuthorEditorPageextends [WSAuthorEditorPageBase](WSAuthorEditorPageBase.md)
Author editor page.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 void [addQuickAssistProcessor](#addQuickAssistProcessor(ro.sync.exml.editor.quickassist.SimpleQuickAssistProcessor))([SimpleQuickAssistProcessor](../../../../../editor/quickassist/SimpleQuickAssistProcessor.md) processor)
Register a quick assist processor.
  [AuthorAccess](../../../../../../ecss/extensions/api/AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()
Access class to the author functions.
  [AuthorChangeTrackingController](../../../../../../ecss/extensions/api/AuthorChangeTrackingController.md) [getChangeTrackingController](#getChangeTrackingController())()  Deprecated.
Use [getReviewController()](#getReviewController()) instead.
   [AuthorDocumentController](../../../../../../ecss/extensions/api/AuthorDocumentController.md) [getDocumentController](#getDocumentController())()
Returns the Author document controller.
  [OptionsStorage](../../../../../../ecss/extensions/api/OptionsStorage.md) [getOptionsStorage](#getOptionsStorage())()
The object that manages the options stored for author extensions.
  [AuthorOutlineAccess](../../../../../../ecss/extensions/api/access/AuthorOutlineAccess.md) [getOutlineAccess](#getOutlineAccess())()
Get the author Outline access providing Outline related information.
  [AuthorReviewController](../../../../../../ecss/extensions/api/AuthorReviewController.md) [getReviewController](#getReviewController())()
Controller that can be used to toggle the change tracking state, modify the review highlight author name, the highlight painting or to obtain information about the properties used in the serialization and representation of the review highlight (author name, reviewer auto color or the current time stamp in a format identical to the one used by Oxygen for insert, delete and comment markers).
  [AuthorTableAccess](../../../../../../ecss/extensions/api/access/AuthorTableAccess.md) [getTableAccess](#getTableAccess())()
Returns the author table access provider responsible for obtaining table related information and executing table actions.
  void [removeQuickAssistProcessor](#removeQuickAssistProcessor(ro.sync.exml.editor.quickassist.SimpleQuickAssistProcessor))([SimpleQuickAssistProcessor](../../../../../editor/quickassist/SimpleQuickAssistProcessor.md) processor)
The processor to be unregistered.

### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.author.tooltip.[AuthorTooltipCustomizerProvider](tooltip/AuthorTooltipCustomizerProvider.md)
 [addTooltipCustomizer](tooltip/AuthorTooltipCustomizerProvider.md#addTooltipCustomizer(ro.sync.exml.workspace.api.editor.page.author.tooltip.AuthorTooltipCustomizer)), [removeTooltipCustomizer](tooltip/AuthorTooltipCustomizerProvider.md#removeTooltipCustomizer(ro.sync.exml.workspace.api.editor.page.author.tooltip.AuthorTooltipCustomizer))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPageBase](WSAuthorEditorPageBase.md)
 [addAuthorAttributesDisplayFilter](WSAuthorEditorPageBase.md#addAuthorAttributesDisplayFilter(ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter)), [addAuthorCaretListener](WSAuthorEditorPageBase.md#addAuthorCaretListener(ro.sync.ecss.extensions.api.AuthorCaretListener)), [addAuthorMouseListener](WSAuthorEditorPageBase.md#addAuthorMouseListener(ro.sync.ecss.extensions.api.AuthorMouseListener)), [addDNDListener](WSAuthorEditorPageBase.md#addDNDListener(java.lang.Object)), [addPopUpMenuCustomizer](WSAuthorEditorPageBase.md#addPopUpMenuCustomizer(ro.sync.ecss.extensions.api.structure.AuthorPopupMenuCustomizer)), [buildURLForReferencedContent](WSAuthorEditorPageBase.md#buildURLForReferencedContent(int,boolean)), [deleteSelection](WSAuthorEditorPageBase.md#deleteSelection()), [editAttribute](WSAuthorEditorPageBase.md#editAttribute(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String)), [getActionsProvider](WSAuthorEditorPageBase.md#getActionsProvider()), [getAuthorComponent](WSAuthorEditorPageBase.md#getAuthorComponent()), [getAuthorFoldManager](WSAuthorEditorPageBase.md#getAuthorFoldManager()), [getAuthorSelectionModel](WSAuthorEditorPageBase.md#getAuthorSelectionModel()), [getBalancedSelection](WSAuthorEditorPageBase.md#getBalancedSelection(int,int)), [getBalancedSelectionEnd](WSAuthorEditorPageBase.md#getBalancedSelectionEnd()), [getBalancedSelectionStart](WSAuthorEditorPageBase.md#getBalancedSelectionStart()), [getDefaultAuthorSchemaAwareEditingHandler](WSAuthorEditorPageBase.md#getDefaultAuthorSchemaAwareEditingHandler()), [getFullySelectedNode](WSAuthorEditorPageBase.md#getFullySelectedNode()), [getFullySelectedNode](WSAuthorEditorPageBase.md#getFullySelectedNode(int,int)), [getHighlighter](WSAuthorEditorPageBase.md#getHighlighter()), [getPersistentHighlighter](WSAuthorEditorPageBase.md#getPersistentHighlighter()), [getPseudoElementStyles](WSAuthorEditorPageBase.md#getPseudoElementStyles(ro.sync.ecss.extensions.api.node.AuthorParentNode)), [getSelectedText](WSAuthorEditorPageBase.md#getSelectedText()), [getSelectionEnd](WSAuthorEditorPageBase.md#getSelectionEnd()), [getSelectionStart](WSAuthorEditorPageBase.md#getSelectionStart()), [getStyles](WSAuthorEditorPageBase.md#getStyles(ro.sync.ecss.extensions.api.node.AuthorNode)), [getTagsDisplayMode](WSAuthorEditorPageBase.md#getTagsDisplayMode()), [goToNextEditablePosition](WSAuthorEditorPageBase.md#goToNextEditablePosition(int,int)), [hasSelection](WSAuthorEditorPageBase.md#hasSelection()), [isOffsetInInvisibleBounds](WSAuthorEditorPageBase.md#isOffsetInInvisibleBounds(int)), [moveOutOfInvisibleBounds](WSAuthorEditorPageBase.md#moveOutOfInvisibleBounds(int,boolean)), [refresh](WSAuthorEditorPageBase.md#refresh()), [refresh](WSAuthorEditorPageBase.md#refresh(ro.sync.ecss.extensions.api.node.AuthorNode)), [removeAuthorAttributesDisplayFilter](WSAuthorEditorPageBase.md#removeAuthorAttributesDisplayFilter(ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter)), [removeAuthorCaretListener](WSAuthorEditorPageBase.md#removeAuthorCaretListener(ro.sync.ecss.extensions.api.AuthorCaretListener)), [removeAuthorMouseListener](WSAuthorEditorPageBase.md#removeAuthorMouseListener(ro.sync.ecss.extensions.api.AuthorMouseListener)), [removeDNDListener](WSAuthorEditorPageBase.md#removeDNDListener(java.lang.Object)), [removePopUpMenuCustomizer](WSAuthorEditorPageBase.md#removePopUpMenuCustomizer(ro.sync.ecss.extensions.api.structure.AuthorPopupMenuCustomizer)), [scrollToRectangle](WSAuthorEditorPageBase.md#scrollToRectangle(ro.sync.exml.view.graphics.Rectangle)), [select](WSAuthorEditorPageBase.md#select(int,int)), [setPopUpMenuCustomizer](WSAuthorEditorPageBase.md#setPopUpMenuCustomizer(ro.sync.ecss.extensions.api.structure.AuthorPopupMenuCustomizer)), [setTagsDisplayMode](WSAuthorEditorPageBase.md#setTagsDisplayMode(int)), [viewToModel](WSAuthorEditorPageBase.md#viewToModel(int,int))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSEditorPage](../WSEditorPage.md)
 [getParentEditor](../WSEditorPage.md#getParentEditor()), [hasFocus](../WSEditorPage.md#hasFocus()), [isEditable](../WSEditorPage.md#isEditable()), [requestFocus](../WSEditorPage.md#requestFocus()), [setEditable](../WSEditorPage.md#setEditable(boolean)), [setReadOnly](../WSEditorPage.md#setReadOnly(java.lang.String)), [setReadOnly](../WSEditorPage.md#setReadOnly(ro.sync.exml.workspace.api.editor.ReadOnlyReason))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSTextBasedEditorPage](../WSTextBasedEditorPage.md)
 [copy](../WSTextBasedEditorPage.md#copy()), [createAnchor](../WSTextBasedEditorPage.md#createAnchor(int)), [getCaretOffset](../WSTextBasedEditorPage.md#getCaretOffset()), [getColumnOfOffset](../WSTextBasedEditorPage.md#getColumnOfOffset(int)), [getLineOfOffset](../WSTextBasedEditorPage.md#getLineOfOffset(int)), [getLocationOnScreenAsPoint](../WSTextBasedEditorPage.md#getLocationOnScreenAsPoint(int,int)), [getLocationRelativeToEditorFromScreen](../WSTextBasedEditorPage.md#getLocationRelativeToEditorFromScreen(int,int)), [getOffsetForAnchor](../WSTextBasedEditorPage.md#getOffsetForAnchor(ro.sync.exml.workspace.api.editor.page.Anchor)), [getStartEndOffsets](../WSTextBasedEditorPage.md#getStartEndOffsets(ro.sync.document.DocumentPositionedInfo)), [getWordAtCaret](../WSTextBasedEditorPage.md#getWordAtCaret()), [modelToViewRectangle](../WSTextBasedEditorPage.md#modelToViewRectangle(int)), [scrollCaretToVisible](../WSTextBasedEditorPage.md#scrollCaretToVisible()), [selectWord](../WSTextBasedEditorPage.md#selectWord()), [setCaretPosition](../WSTextBasedEditorPage.md#setCaretPosition(int)), [viewToModelOffset](../WSTextBasedEditorPage.md#viewToModelOffset(int,int))
## Method Details

### getDocumentController

[AuthorDocumentController](../../../../../../ecss/extensions/api/AuthorDocumentController.md) getDocumentController()

Returns the Author document controller. It has methods for changing the document model.
  Returns: The controller for Author document. Cannot be null.
### getTableAccess

[AuthorTableAccess](../../../../../../ecss/extensions/api/access/AuthorTableAccess.md) getTableAccess()

Returns the author table access provider responsible for obtaining table related information and executing table actions.
  Returns: The table related information and actions provider. Cannot be null.
### getChangeTrackingController

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [AuthorChangeTrackingController](../../../../../../ecss/extensions/api/AuthorChangeTrackingController.md) getChangeTrackingController()
 Deprecated.
Use [getReviewController()](#getReviewController()) instead.

The change tracking controller used to toggle change tracking on and off and check its state.
  Returns: The change tracking controller. Cannot be null.
### getReviewController

[AuthorReviewController](../../../../../../ecss/extensions/api/AuthorReviewController.md) getReviewController()

Controller that can be used to toggle the change tracking state, modify the review highlight author name, the highlight painting or to obtain information about the properties used in the serialization and representation of the review highlight (author name, reviewer auto color or the current time stamp in a format identical to the one used by Oxygen for insert, delete and comment markers).
  Returns: The review controller. Cannot be null. Since: 12
### getOptionsStorage

[OptionsStorage](../../../../../../ecss/extensions/api/OptionsStorage.md) getOptionsStorage()

The object that manages the options stored for author extensions. This is also responsible for adding and removing listeners that are notified about the option changes.
  Returns: The object that manages the options stored for author extensions.
### getOutlineAccess

[AuthorOutlineAccess](../../../../../../ecss/extensions/api/access/AuthorOutlineAccess.md) getOutlineAccess()

Get the author Outline access providing Outline related information.
  Returns: The Outline related informations and actions provider. Cannot be null.
### getAuthorAccess

[AuthorAccess](../../../../../../ecss/extensions/api/AuthorAccess.md) getAuthorAccess()

Access class to the author functions. The WSAuthorEditorPage has most of the methods which can also be found in the AuthorAccess. This method is offered only as an useful way to have utility methods which take AuthorAccess as a parameter and to use them both from a plugin and from a framework. Provides access to specific components corresponding to editor, document, workspace, tables, change tracking and utility informations and actions.
  Returns: The author access. Since: 14.1
### addQuickAssistProcessor

void addQuickAssistProcessor([SimpleQuickAssistProcessor](../../../../../editor/quickassist/SimpleQuickAssistProcessor.md) processor)

Register a quick assist processor. This allow you to provide quick custom quick assist proposals in the current editor page quick assist menu. The quick assist processor cannot be registered for WebAuthor application.
  Parameters: processor - The processor to be registered. Since: 26.1
### removeQuickAssistProcessor

void removeQuickAssistProcessor([SimpleQuickAssistProcessor](../../../../../editor/quickassist/SimpleQuickAssistProcessor.md) processor)

The processor to be unregistered.
  Parameters: processor - The processor to be unregistered. Since: 26.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
