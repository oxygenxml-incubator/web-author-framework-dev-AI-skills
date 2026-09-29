Package [ro.sync.exml.workspace.api.editor.page.author](package-summary.md)

# Interface WSAuthorComponentEditorPage
    All Superinterfaces: [AuthorTooltipCustomizerProvider](tooltip/AuthorTooltipCustomizerProvider.md), [WSAuthorEditorPage](WSAuthorEditorPage.md), [WSAuthorEditorPageBase](WSAuthorEditorPageBase.md), [WSEditorPage](../WSEditorPage.md), [WSTextBasedEditorPage](../WSTextBasedEditorPage.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WSAuthorComponentEditorPageextends [WSAuthorEditorPage](WSAuthorEditorPage.md)
Provides enhanced access (with additional methods) to the author page from an Author Component editor.
  Since: 14.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [JToolBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolBar.html) [createBasicAuthorToolbar](#createBasicAuthorToolbar())()
Create the toolbar which contains Refresh, Change Element Tags and Profiling Sets switch button.
  [JToolBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolBar.html) [createCSSAlternativesToolbar](#createCSSAlternativesToolbar())()
Retrieve the toolbar containing the drop-down button for CSS alternative stylesheets.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[JToolBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolBar.html)> [createExtensionActionsToolbars](#createExtensionActionsToolbars())()
Create toolbars with all the actions defined at the framework level in exactly the same order in which they have been added to the toolbars from the Document Type Edit dialog.
  [JToolBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolBar.html) [createReviewToolbar](#createReviewToolbar())()
Retrieve the toolbar for author review.
  void [setBreadCrumbPopUpCustomizer](#setBreadCrumbPopUpCustomizer(ro.sync.ecss.extensions.api.component.PopupMenuCustomizer))([PopupMenuCustomizer](../../../../../../ecss/extensions/api/component/PopupMenuCustomizer.md) popUpCustomizer)
The Pop-up customizer can be used to add/remove actions from the pop-up menu in the Author bread crumb before showing it.
  void [setOutlinerPopUpCustomizer](#setOutlinerPopUpCustomizer(ro.sync.ecss.extensions.api.component.PopupMenuCustomizer))([PopupMenuCustomizer](../../../../../../ecss/extensions/api/component/PopupMenuCustomizer.md) popUpCustomizer)
The Pop-up customizer can be used to add/remove actions from the pop-up menu in the Author Outliner view before showing it.
  void [showBreadCrumb](#showBreadCrumb(boolean))(boolean showBreadCrumb)
Show or hide the Bread Crumb panel in Author component.
  void [showRangeRuler](#showRangeRuler(boolean))(boolean showRangeRuler)
Hide or show the vertical stripe located on the right side of the editing area which presents ranges for errors or various other highlights.
  void [showValidationStatusBar](#showValidationStatusBar(boolean))(boolean showValidationStatus)
Hide or show the validation status bar which appears at the bottom of the editing area when placing the caret inside an error highlight.

### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.author.tooltip.[AuthorTooltipCustomizerProvider](tooltip/AuthorTooltipCustomizerProvider.md)
 [addTooltipCustomizer](tooltip/AuthorTooltipCustomizerProvider.md#addTooltipCustomizer(ro.sync.exml.workspace.api.editor.page.author.tooltip.AuthorTooltipCustomizer)), [removeTooltipCustomizer](tooltip/AuthorTooltipCustomizerProvider.md#removeTooltipCustomizer(ro.sync.exml.workspace.api.editor.page.author.tooltip.AuthorTooltipCustomizer))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPage](WSAuthorEditorPage.md)
 [addQuickAssistProcessor](WSAuthorEditorPage.md#addQuickAssistProcessor(ro.sync.exml.editor.quickassist.SimpleQuickAssistProcessor)), [getAuthorAccess](WSAuthorEditorPage.md#getAuthorAccess()), [getChangeTrackingController](WSAuthorEditorPage.md#getChangeTrackingController()), [getDocumentController](WSAuthorEditorPage.md#getDocumentController()), [getOptionsStorage](WSAuthorEditorPage.md#getOptionsStorage()), [getOutlineAccess](WSAuthorEditorPage.md#getOutlineAccess()), [getReviewController](WSAuthorEditorPage.md#getReviewController()), [getTableAccess](WSAuthorEditorPage.md#getTableAccess()), [removeQuickAssistProcessor](WSAuthorEditorPage.md#removeQuickAssistProcessor(ro.sync.exml.editor.quickassist.SimpleQuickAssistProcessor))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPageBase](WSAuthorEditorPageBase.md)
 [addAuthorAttributesDisplayFilter](WSAuthorEditorPageBase.md#addAuthorAttributesDisplayFilter(ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter)), [addAuthorCaretListener](WSAuthorEditorPageBase.md#addAuthorCaretListener(ro.sync.ecss.extensions.api.AuthorCaretListener)), [addAuthorMouseListener](WSAuthorEditorPageBase.md#addAuthorMouseListener(ro.sync.ecss.extensions.api.AuthorMouseListener)), [addDNDListener](WSAuthorEditorPageBase.md#addDNDListener(java.lang.Object)), [addPopUpMenuCustomizer](WSAuthorEditorPageBase.md#addPopUpMenuCustomizer(ro.sync.ecss.extensions.api.structure.AuthorPopupMenuCustomizer)), [buildURLForReferencedContent](WSAuthorEditorPageBase.md#buildURLForReferencedContent(int,boolean)), [deleteSelection](WSAuthorEditorPageBase.md#deleteSelection()), [editAttribute](WSAuthorEditorPageBase.md#editAttribute(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String)), [getActionsProvider](WSAuthorEditorPageBase.md#getActionsProvider()), [getAuthorComponent](WSAuthorEditorPageBase.md#getAuthorComponent()), [getAuthorFoldManager](WSAuthorEditorPageBase.md#getAuthorFoldManager()), [getAuthorSelectionModel](WSAuthorEditorPageBase.md#getAuthorSelectionModel()), [getBalancedSelection](WSAuthorEditorPageBase.md#getBalancedSelection(int,int)), [getBalancedSelectionEnd](WSAuthorEditorPageBase.md#getBalancedSelectionEnd()), [getBalancedSelectionStart](WSAuthorEditorPageBase.md#getBalancedSelectionStart()), [getDefaultAuthorSchemaAwareEditingHandler](WSAuthorEditorPageBase.md#getDefaultAuthorSchemaAwareEditingHandler()), [getFullySelectedNode](WSAuthorEditorPageBase.md#getFullySelectedNode()), [getFullySelectedNode](WSAuthorEditorPageBase.md#getFullySelectedNode(int,int)), [getHighlighter](WSAuthorEditorPageBase.md#getHighlighter()), [getPersistentHighlighter](WSAuthorEditorPageBase.md#getPersistentHighlighter()), [getPseudoElementStyles](WSAuthorEditorPageBase.md#getPseudoElementStyles(ro.sync.ecss.extensions.api.node.AuthorParentNode)), [getSelectedText](WSAuthorEditorPageBase.md#getSelectedText()), [getSelectionEnd](WSAuthorEditorPageBase.md#getSelectionEnd()), [getSelectionStart](WSAuthorEditorPageBase.md#getSelectionStart()), [getStyles](WSAuthorEditorPageBase.md#getStyles(ro.sync.ecss.extensions.api.node.AuthorNode)), [getTagsDisplayMode](WSAuthorEditorPageBase.md#getTagsDisplayMode()), [goToNextEditablePosition](WSAuthorEditorPageBase.md#goToNextEditablePosition(int,int)), [hasSelection](WSAuthorEditorPageBase.md#hasSelection()), [isOffsetInInvisibleBounds](WSAuthorEditorPageBase.md#isOffsetInInvisibleBounds(int)), [moveOutOfInvisibleBounds](WSAuthorEditorPageBase.md#moveOutOfInvisibleBounds(int,boolean)), [refresh](WSAuthorEditorPageBase.md#refresh()), [refresh](WSAuthorEditorPageBase.md#refresh(ro.sync.ecss.extensions.api.node.AuthorNode)), [removeAuthorAttributesDisplayFilter](WSAuthorEditorPageBase.md#removeAuthorAttributesDisplayFilter(ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter)), [removeAuthorCaretListener](WSAuthorEditorPageBase.md#removeAuthorCaretListener(ro.sync.ecss.extensions.api.AuthorCaretListener)), [removeAuthorMouseListener](WSAuthorEditorPageBase.md#removeAuthorMouseListener(ro.sync.ecss.extensions.api.AuthorMouseListener)), [removeDNDListener](WSAuthorEditorPageBase.md#removeDNDListener(java.lang.Object)), [removePopUpMenuCustomizer](WSAuthorEditorPageBase.md#removePopUpMenuCustomizer(ro.sync.ecss.extensions.api.structure.AuthorPopupMenuCustomizer)), [scrollToRectangle](WSAuthorEditorPageBase.md#scrollToRectangle(ro.sync.exml.view.graphics.Rectangle)), [select](WSAuthorEditorPageBase.md#select(int,int)), [setPopUpMenuCustomizer](WSAuthorEditorPageBase.md#setPopUpMenuCustomizer(ro.sync.ecss.extensions.api.structure.AuthorPopupMenuCustomizer)), [setTagsDisplayMode](WSAuthorEditorPageBase.md#setTagsDisplayMode(int)), [viewToModel](WSAuthorEditorPageBase.md#viewToModel(int,int))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSEditorPage](../WSEditorPage.md)
 [getParentEditor](../WSEditorPage.md#getParentEditor()), [hasFocus](../WSEditorPage.md#hasFocus()), [isEditable](../WSEditorPage.md#isEditable()), [requestFocus](../WSEditorPage.md#requestFocus()), [setEditable](../WSEditorPage.md#setEditable(boolean)), [setReadOnly](../WSEditorPage.md#setReadOnly(java.lang.String)), [setReadOnly](../WSEditorPage.md#setReadOnly(ro.sync.exml.workspace.api.editor.ReadOnlyReason))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSTextBasedEditorPage](../WSTextBasedEditorPage.md)
 [copy](../WSTextBasedEditorPage.md#copy()), [createAnchor](../WSTextBasedEditorPage.md#createAnchor(int)), [getCaretOffset](../WSTextBasedEditorPage.md#getCaretOffset()), [getColumnOfOffset](../WSTextBasedEditorPage.md#getColumnOfOffset(int)), [getLineOfOffset](../WSTextBasedEditorPage.md#getLineOfOffset(int)), [getLocationOnScreenAsPoint](../WSTextBasedEditorPage.md#getLocationOnScreenAsPoint(int,int)), [getLocationRelativeToEditorFromScreen](../WSTextBasedEditorPage.md#getLocationRelativeToEditorFromScreen(int,int)), [getOffsetForAnchor](../WSTextBasedEditorPage.md#getOffsetForAnchor(ro.sync.exml.workspace.api.editor.page.Anchor)), [getStartEndOffsets](../WSTextBasedEditorPage.md#getStartEndOffsets(ro.sync.document.DocumentPositionedInfo)), [getWordAtCaret](../WSTextBasedEditorPage.md#getWordAtCaret()), [modelToViewRectangle](../WSTextBasedEditorPage.md#modelToViewRectangle(int)), [scrollCaretToVisible](../WSTextBasedEditorPage.md#scrollCaretToVisible()), [selectWord](../WSTextBasedEditorPage.md#selectWord()), [setCaretPosition](../WSTextBasedEditorPage.md#setCaretPosition(int)), [viewToModelOffset](../WSTextBasedEditorPage.md#viewToModelOffset(int,int))
## Method Details

### createExtensionActionsToolbars

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[JToolBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolBar.html)> createExtensionActionsToolbars()

Create toolbars with all the actions defined at the framework level in exactly the same order in which they have been added to the toolbars from the Document Type Edit dialog. The toolbars will look almost identical with the ones which appear when the XML is opened in an Oxygen standalone version.
  Returns: toolbars with all the actions defined at the framework level.
### setBreadCrumbPopUpCustomizer

void setBreadCrumbPopUpCustomizer([PopupMenuCustomizer](../../../../../../ecss/extensions/api/component/PopupMenuCustomizer.md) popUpCustomizer)

The Pop-up customizer can be used to add/remove actions from the pop-up menu in the Author bread crumb before showing it. If everything is removed then the menu will not be shown.
  Parameters: popUpCustomizer - The pop Up Customizer.
### showBreadCrumb

void showBreadCrumb(boolean showBreadCrumb)

Show or hide the Bread Crumb panel in Author component.
  Parameters: showBreadCrumb - true to show the Bread Crumb.
### setOutlinerPopUpCustomizer

void setOutlinerPopUpCustomizer([PopupMenuCustomizer](../../../../../../ecss/extensions/api/component/PopupMenuCustomizer.md) popUpCustomizer)

The Pop-up customizer can be used to add/remove actions from the pop-up menu in the Author Outliner view before showing it. If everything is removed then the menu will not be shown.
  Parameters: popUpCustomizer - The pop Up Customizer.
### createReviewToolbar

[JToolBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolBar.html) createReviewToolbar()

Retrieve the toolbar for author review.
  Returns: The toolbar for author review.
### createCSSAlternativesToolbar

[JToolBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolBar.html) createCSSAlternativesToolbar()

Retrieve the toolbar containing the drop-down button for CSS alternative stylesheets.
  Returns: The toolbar containing the drop-down button for CSS alternative stylesheets. Since: 15.2
### createBasicAuthorToolbar

[JToolBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolBar.html) createBasicAuthorToolbar()

Create the toolbar which contains Refresh, Change Element Tags and Profiling Sets switch button.
  Returns: The toolbar which contains Refresh, Change Element Tags and Profiling Sets switch button. Since: 16.1
### showRangeRuler

void showRangeRuler(boolean showRangeRuler)

Hide or show the vertical stripe located on the right side of the editing area which presents ranges for errors or various other highlights. By default the validation stripe is shown.
  Parameters: showRangeRuler - true to show the validation stripe, false to hide it. Since: 23
### showValidationStatusBar

void showValidationStatusBar(boolean showValidationStatus)

Hide or show the validation status bar which appears at the bottom of the editing area when placing the caret inside an error highlight. By default it is shown.
  Parameters: showValidationStatus - true to show the validation status bar. false to always hide it. Since: 23
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
