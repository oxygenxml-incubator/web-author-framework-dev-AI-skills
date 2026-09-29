Package [ro.sync.exml.workspace.api.editor.page.ditamap](package-summary.md)

# Interface WSDITAMapEditorPage
    All Superinterfaces: [WSEditorPage](../WSEditorPage.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WSDITAMapEditorPageextends [WSEditorPage](../WSEditorPage.md)
DITA Maps Manager editor page.
  Since: 12.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addAuthorAttributesDisplayFilter](#addAuthorAttributesDisplayFilter(ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter))([AuthorAttributesDisplayFilter](../../../../../../ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md) attributesDisplayFilter)
Adds a filter for displaying attributes to the current DITA Map Tree.
  void [addDropHandler](#addDropHandler(ro.sync.exml.workspace.api.editor.page.ditamap.dnd.DITAMapTreeDropHandler))([DITAMapTreeDropHandler](dnd/DITAMapTreeDropHandler.md) dropHandler)
Add a drop handler to the DITA Map tree.
  void [addNodeRendererCustomizer](#addNodeRendererCustomizer(ro.sync.exml.workspace.api.editor.page.ditamap.DITAMapNodeRendererCustomizer))([DITAMapNodeRendererCustomizer](DITAMapNodeRendererCustomizer.md) customizer)
Add a node renderer customizer.
  [DITAMapActionsProvider](actions/DITAMapActionsProvider.md) [getActionsProvider](#getActionsProvider())()
Provides access to actions already defined in the DITA Map page like: Undo, Redo, etc.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] [getCurrentSelectedURLs](#getCurrentSelectedURLs(boolean,boolean))(boolean recurseReferences, boolean includeBinaryAndExternalResources)
Gather all the files referenced from the selection.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getDITAMapTreeComponent](#getDITAMapTreeComponent())()
Get the internal component on which the DITA Map page is rendered (a javax.swing.JTree).
  [AuthorDocumentController](../../../../../../ecss/extensions/api/AuthorDocumentController.md) [getDocumentController](#getDocumentController())()
Returns the DITA Map document controller.
  [OptionsStorage](../../../../../../ecss/extensions/api/OptionsStorage.md) [getOptionsStorage](#getOptionsStorage())()
The object that manages the options stored for DITA Map extensions.
  [DITAMapReviewController](review/DITAMapReviewController.md) [getReviewController](#getReviewController())()
Retrieve a controller that can be used to toggle the change tracking state.
  [AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md)[] [getSelectedNodes](#getSelectedNodes(boolean))(boolean minimizeSelection)
Get the selected nodes from DITA Map tree.
  [UnsavedContentReferenceManager](../../../../../../ecss/extensions/api/access/UnsavedContentReferenceManager.md) [getUnsavedContentReferenceManager](#getUnsavedContentReferenceManager())()
Get the manager that can be used to find (and save) the resources whose content has been modified in-place, by editing the expanded references.
  boolean [isEditable](#isEditable())()
Checks whether or not the DITA Map page is editable.
  void [refreshReferences](#refreshReferences())()
Refresh all references in the opened DITA Map.
  void [removeAuthorAttributesDisplayFilter](#removeAuthorAttributesDisplayFilter(ro.sync.ecss.extensions.api.attributes.AuthorAttributesDisplayFilter))([AuthorAttributesDisplayFilter](../../../../../../ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md) attributesDisplayFilter)
Remove a filter for displaying attributes to the current DITA Map Tree.
  void [removeDropHandler](#removeDropHandler(ro.sync.exml.workspace.api.editor.page.ditamap.dnd.DITAMapTreeDropHandler))([DITAMapTreeDropHandler](dnd/DITAMapTreeDropHandler.md) dropHandler)
Remove a drop handler from the DITA Map tree.
  void [removeNodeRendererCustomizer](#removeNodeRendererCustomizer(ro.sync.exml.workspace.api.editor.page.ditamap.DITAMapNodeRendererCustomizer))([DITAMapNodeRendererCustomizer](DITAMapNodeRendererCustomizer.md) customizer)
Remove a node renderer customizer.
  void [setEditable](#setEditable(boolean))(boolean editable)
Sets the specified flag to indicate whether or not the DITA Map page should be editable.
  void [setPopUpMenuCustomizer](#setPopUpMenuCustomizer(ro.sync.exml.workspace.api.editor.page.ditamap.DITAMapPopupMenuCustomizer))([DITAMapPopupMenuCustomizer](DITAMapPopupMenuCustomizer.md) popUpCustomizer)
Set the pop-up menu customizer which can be used to customize the pop-up menu (add/remove actions) before showing it in the DITA Mapa Manager page.

### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSEditorPage](../WSEditorPage.md)
 [getParentEditor](../WSEditorPage.md#getParentEditor()), [hasFocus](../WSEditorPage.md#hasFocus()), [requestFocus](../WSEditorPage.md#requestFocus()), [setReadOnly](../WSEditorPage.md#setReadOnly(java.lang.String)), [setReadOnly](../WSEditorPage.md#setReadOnly(ro.sync.exml.workspace.api.editor.ReadOnlyReason))
## Method Details

### getDocumentController

[AuthorDocumentController](../../../../../../ecss/extensions/api/AuthorDocumentController.md) getDocumentController()

Returns the DITA Map document controller. It has methods for changing the document model. The insertions of XML content using the controller are not schema aware.
  Returns: The controller for DITA Map structure. Cannot be null.
### getOptionsStorage

[OptionsStorage](../../../../../../ecss/extensions/api/OptionsStorage.md) getOptionsStorage()

The object that manages the options stored for DITA Map extensions. This is also responsible for adding and removing listeners that are notified about the option changes.
  Returns: The object that manages the options stored for DITA Map extensions.
### setPopUpMenuCustomizer

void setPopUpMenuCustomizer([DITAMapPopupMenuCustomizer](DITAMapPopupMenuCustomizer.md) popUpCustomizer)

Set the pop-up menu customizer which can be used to customize the pop-up menu (add/remove actions) before showing it in the DITA Mapa Manager page.
  Parameters: popUpCustomizer - the pop-up menu customizer.
### getDITAMapTreeComponent

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getDITAMapTreeComponent()

Get the internal component on which the DITA Map page is rendered (a javax.swing.JTree).
  Returns: for the stand alone version, a javax.swing.JTree, for the Oxygen plugin for Eclipse an instance of TreeViewer
### addAuthorAttributesDisplayFilter

void addAuthorAttributesDisplayFilter([AuthorAttributesDisplayFilter](../../../../../../ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md) attributesDisplayFilter)

Adds a filter for displaying attributes to the current DITA Map Tree. The filter will be applied when editing the attributes for a topic reference.
  Parameters: attributesDisplayFilter - The [AuthorAttributesDisplayFilter](../../../../../../ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md) to be added. Since: 13.1
### removeAuthorAttributesDisplayFilter

void removeAuthorAttributesDisplayFilter([AuthorAttributesDisplayFilter](../../../../../../ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md) attributesDisplayFilter)

Remove a filter for displaying attributes to the current DITA Map Tree.
  Parameters: attributesDisplayFilter - The [AuthorAttributesDisplayFilter](../../../../../../ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md) to be removed. Since: 13.1
### setEditable

void setEditable(boolean editable)

Sets the specified flag to indicate whether or not the DITA Map page should be editable.
  Specified by: [setEditable](../WSEditorPage.md#setEditable(boolean)) in interface [WSEditorPage](../WSEditorPage.md) Parameters: editable - true if the DITA Map page should be editable. Since: 13.1
### isEditable

boolean isEditable()

Checks whether or not the DITA Map page is editable.
  Specified by: [isEditable](../WSEditorPage.md#isEditable()) in interface [WSEditorPage](../WSEditorPage.md) Returns: true if the DITA Map page is editable, false otherwise. Since: 15
### getSelectedNodes

[AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md)[] getSelectedNodes(boolean minimizeSelection)

Get the selected nodes from DITA Map tree.
  Parameters: minimizeSelection - If true and a parent and a child is selected, then only the parent is the list. Returns: The selected nodes from DITA Map tree.
### getActionsProvider

[DITAMapActionsProvider](actions/DITAMapActionsProvider.md) getActionsProvider()

Provides access to actions already defined in the DITA Map page like: Undo, Redo, etc.
  Returns: access to actions already defined in the DITA Map page. Since: 15.2
### addDropHandler

void addDropHandler([DITAMapTreeDropHandler](dnd/DITAMapTreeDropHandler.md) dropHandler)

Add a drop handler to the DITA Map tree.
  Parameters: dropHandler - The newly added drop handler Since: 17
### removeDropHandler

void removeDropHandler([DITAMapTreeDropHandler](dnd/DITAMapTreeDropHandler.md) dropHandler)

Remove a drop handler from the DITA Map tree.
  Parameters: dropHandler - The newly added drop handler Since: 17
### refreshReferences

void refreshReferences()

Refresh all references in the opened DITA Map. This is equivalent to pressing F5 in the map tree.
  Since: 17.1
### getReviewController

[DITAMapReviewController](review/DITAMapReviewController.md) getReviewController()

Retrieve a controller that can be used to toggle the change tracking state.
  Returns: The review controller. Cannot be null. Since: 18
### addNodeRendererCustomizer

void addNodeRendererCustomizer([DITAMapNodeRendererCustomizer](DITAMapNodeRendererCustomizer.md) customizer)

Add a node renderer customizer. The customizer can customize the icon and title which appears for each topicref in the DITA Maps Manager view.
  Parameters: customizer - The customizer can customize the icon and title which appears for each topicref in the DITA Maps Manager view. Since: 18.1
### removeNodeRendererCustomizer

void removeNodeRendererCustomizer([DITAMapNodeRendererCustomizer](DITAMapNodeRendererCustomizer.md) customizer)

Remove a node renderer customizer. The customizer can customize the icon and title which appears for each topicref in the DITA Maps Manager view.
  Parameters: customizer - The customizer can customize the icon and title which appears for each topicref in the DITA Maps Manager view. Since: 18.1
### getUnsavedContentReferenceManager

[UnsavedContentReferenceManager](../../../../../../ecss/extensions/api/access/UnsavedContentReferenceManager.md) getUnsavedContentReferenceManager()

Get the manager that can be used to find (and save) the resources whose content has been modified in-place, by editing the expanded references.
  Returns: The unsaved reference manager. Can be null, if the references cannot be edited in place in this editor. Since: 23
### getCurrentSelectedURLs

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] getCurrentSelectedURLs(boolean recurseReferences, boolean includeBinaryAndExternalResources)

Gather all the files referenced from the selection.
  Parameters: recurseReferences - true to recursively collect references. false to limit to the first level of references. includeBinaryAndExternalResources - true to include also resources which are possibly binary, for example they have the format attribute set to a binary extension or which have external scope. Returns: all dita map selected resources as URLs. Since: 24
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
