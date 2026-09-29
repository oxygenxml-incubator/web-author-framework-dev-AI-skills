# All Classes and Interfaces
   All Classes and InterfacesInterfacesClassesEnum ClassesExceptionsAnnotation Interfaces
Class

Description
 [AbstractComponentProvider](ro/sync/ecss/extensions/api/component/AbstractComponentProvider.md)
A component encapsulating all the editing part.
  [AbstractDocumentTypeHelper](ro/sync/ecss/extensions/commons/AbstractDocumentTypeHelper.md)
Abstract implementation of the document type helper.
  [AbstractInplaceEditor](ro/sync/ecss/extensions/api/editor/AbstractInplaceEditor.md)
An abstract implementation that handles listeners fire.
  [AbstractInplaceEditorWrapper](ro/sync/ecss/extensions/api/editor/AbstractInplaceEditorWrapper.md)
It can be used when more than one editor types are needed depending on the received context and it can choose at runtime an appropriate editor implementation.
  [AbstractTableOperation](ro/sync/ecss/extensions/commons/table/operations/AbstractTableOperation.md)
Base class for table operations.
  [ActionBarContributorCustomizer](com/oxygenxml/editor/editors/ActionBarContributorCustomizer.md)
Abstract class allowed as an extension point to customize the menu and toolbar buttons added by our editors.
  [ActionPerformedListener](ro/sync/exml/workspace/api/editor/page/author/actions/ActionPerformedListener.md)
This listener can be registered for a certain action.
  [ActionsListFilter](com/oxygenxml/editor/editors/xml/ActionsListFilter.md)
Access to the drop down tool item, allows configuring the set of available actions.
  [ActionsProvider](ro/sync/exml/workspace/api/editor/page/author/actions/ActionsProvider.md)
Provides access to actions defined in the Author page.
  [ActionsProvider](ro/sync/exml/workspace/api/standalone/actions/ActionsProvider.md)
Provides access to global actions in the entire workbench.
  [AddEditConrefOperation](ro/sync/ecss/extensions/dita/conref/AddEditConrefOperation.md)
Operation used to add or edit a conref from an element in DITA documents.
  [AIConnectorsPluginExtension](ro/sync/exml/plugin/ai/AIConnectorsPluginExtension.md)
Plug-in extension that provides external AI connectors to AI services
  [AIFunctionsPluginExtension](ro/sync/exml/plugin/ai/AIFunctionsPluginExtension.md)
Plug-in extension that provides external AI functions
  [AIHooksHandlerPluginExtension](ro/sync/exml/plugin/ai/AIHooksHandlerPluginExtension.md)
Plug-in extension that provides a handler for the AI hooks
  [Anchor](ro/sync/exml/workspace/api/editor/page/Anchor.md)
This is a marker interface for an anchor which can be created either in the Text or Author editing modes and then used to located the same content in another editing mode (Author or Text).
  [AntExtensionsBundle](ro/sync/ecss/extensions/ant/AntExtensionsBundle.md)
The Ant framework extensions bundle.
  [AntNodeRendererCustomizer](ro/sync/ecss/extensions/ant/AntNodeRendererCustomizer.md)
Class used to customize the way a Ant node is rendered in the UI.
  [APIAccessibleOptionTags](ro/sync/exml/options/APIAccessibleOptionTags.md)
Global Oxygen options which can be read and set via the API.
  [APIOptionConstants](ro/sync/exml/options/APIOptionConstants.md)
Global Oxygen constants which are accessible via the API.
  [ApplicationInformationAccess](ro/sync/exml/workspace/api/application/ApplicationInformationAccess.md)
Access to various details about the application.
  [ApplicationType](ro/sync/exml/workspace/api/application/ApplicationType.md)
Application type enumeration.
  [ArgumentDescriptor](ro/sync/ecss/extensions/api/ArgumentDescriptor.md)
Descriptor class for an author operation argument.
  [ArgumentsMap](ro/sync/ecss/extensions/api/ArgumentsMap.md)
Map between argument names and values.
  [ArtificialNode](ro/sync/ecss/extensions/api/node/ArtificialNode.md)
Marker interface for artificial elements which wrap Processing Instructions, CData and Comments allowing access to the wrapped node.
  [AskDescriptor](ro/sync/ecss/extensions/AskDescriptor.md)

 [Attr](ro/sync/ecss/extensions/api/link/Attr.md)
Contains informations about an attribute.
  [Attribute](ro/sync/outline/xml/Attribute.md)
An attribute representation used mainly in the content completion process.
  [AttributeChangedEvent](ro/sync/ecss/extensions/api/AttributeChangedEvent.md)
Event received by the [AuthorListener](ro/sync/ecss/extensions/api/AuthorListener.md) when an Author attribute has been changed.
  [AttributedString](ro/sync/exml/view/graphics/AttributedString.md)
A string annotated with attributes.
  [AttributedString.AttributedInterval](ro/sync/exml/view/graphics/AttributedString.AttributedInterval.md)
A text interval from the string, with a specific attribute.
  [AttributeEditingContextDescription](ro/sync/exml/workspace/api/standalone/AttributeEditingContextDescription.md)
Provides language-independent information about the element and attribute name for which the value is edited.
  [AttributeReferenceValueDetector](ro/sync/ecss/extensions/dita/id/AttributeReferenceValueDetector.md)
Detects the [AttrValue](ro/sync/ecss/extensions/api/node/AttrValue.md) of a node and the name of the attribute.
  [AttributesManager](ro/sync/ecss/extensions/api/webapp/attributes/AttributesManager.md)
Offers support for element attributes operations.
  [AttributesValueEditor](ro/sync/ecss/extensions/api/AttributesValueEditor.md)
Deprecated.
Starting with version 15 the [CustomAttributeValueEditor](ro/sync/ecss/extensions/api/CustomAttributeValueEditor.md) can be used instead to edit only specific attributes using a custom editor.

 [AttrValue](ro/sync/ecss/extensions/api/node/AttrValue.md)
Contains informations about an attribute value.
  [AuthorAccess](ro/sync/ecss/extensions/api/AuthorAccess.md)
Access class to the author functions.
  [AuthorAccessDeprecated](ro/sync/ecss/extensions/api/AuthorAccessDeprecated.md)
Contains methods that are deprecated in the [AuthorAccess](ro/sync/ecss/extensions/api/AuthorAccess.md) and should no longer be used.
  [AuthorActionEventDetails](ro/sync/ecss/extensions/api/AuthorActionEventDetails.md)
Class offering details about an author action event.
  [AuthorActionEventHandler](ro/sync/ecss/extensions/api/AuthorActionEventHandler.md)
Intercepts action events in the Author mode and can handle them in a special manner.
  [AuthorActionEventHandler.AuthorActionEventType](ro/sync/ecss/extensions/api/AuthorActionEventHandler.AuthorActionEventType.md)
Events that are delegated to this handler.
  [AuthorActionEventHandlerBase](ro/sync/ecss/extensions/api/AuthorActionEventHandlerBase.md)
Adds various API methods, for example it adds a method which intercepts action events in the Author mode and can handle them in a special manner.
  [AuthorActionsProvider](ro/sync/exml/workspace/api/editor/page/author/actions/AuthorActionsProvider.md)
Provides access to actions defined in the Author page.
  [AuthorAttributesController](ro/sync/ecss/extensions/api/AuthorAttributesController.md)
Helper used to set attributes
  [AuthorAttributesDisplayFilter](ro/sync/ecss/extensions/api/attributes/AuthorAttributesDisplayFilter.md)
Filter certain attributes from being displayed in certain parts of the Author editor (the Attributes view, the Attributes editor, the Outline).
  [AuthorBreadCrumbCustomizer](ro/sync/ecss/extensions/api/structure/AuthorBreadCrumbCustomizer.md)
Author Bread Crumb (components path which appears in the top of the Author editor) customizer used for nodes rendering and pop-up customization.
  [AuthorCalloutRenderingInformation](ro/sync/ecss/extensions/api/callouts/AuthorCalloutRenderingInformation.md)
The callouts are representations of Track Changes insert and delete highlights, review comment highlights and custom review highlights in Author mode.
  [AuthorCalloutsController](ro/sync/ecss/extensions/api/callouts/AuthorCalloutsController.md)
The callouts are representations of Track Changes insert and delete highlights, review comment highlights and custom review highlights in the Author mode on a side bar.
  [AuthorCaretEvent](ro/sync/ecss/extensions/api/AuthorCaretEvent.md)
AuthorCaretEvent is used to notify interested [AuthorCaretListener](ro/sync/ecss/extensions/api/AuthorCaretListener.md) that the position of the caret has changed in the Author editor page.
  [AuthorCaretListener](ro/sync/ecss/extensions/api/AuthorCaretListener.md)
Listener for changes in the caret position of the Author editor page.
  [AuthorCCItemTypes](ro/sync/ecss/contentcompletion/ccitems/AuthorCCItemTypes.md)
Types of the items that are shown in the content completion menu.
  [AuthorChangeTrackingController](ro/sync/ecss/extensions/api/AuthorChangeTrackingController.md)
Controls the change tracking mode.
  [AuthorClipboardAccess](ro/sync/ecss/extensions/api/AuthorClipboardAccess.md)
Access to various content data in the system clipboard.
  [AuthorComponentException](ro/sync/ecss/extensions/api/component/AuthorComponentException.md)
Thrown by the [AuthorComponentProvider](ro/sync/ecss/extensions/api/component/AuthorComponentProvider.md) whenever the component is not used/initialized propertly.
  [AuthorComponentFactory](ro/sync/ecss/extensions/api/component/AuthorComponentFactory.md)
This factory creates author components.
  [AuthorComponentListener](ro/sync/ecss/extensions/api/component/listeners/AuthorComponentListener.md)
Author component listener
  [AuthorComponentProvider](ro/sync/ecss/extensions/api/component/AuthorComponentProvider.md)
A component encapsulating all the visual editing part.
  [AuthorConstants](ro/sync/ecss/extensions/api/AuthorConstants.md)
Interface containing the constants used in Author API.
  [AuthorContentMetadata](ro/sync/ecss/component/AuthorContentMetadata.md)
Marker interface for objects holding metadata associated with Author content.
  [AuthorCSSAlternativesCustomizer](ro/sync/exml/workspace/api/editor/page/author/css/AuthorCSSAlternativesCustomizer.md)
Provides the list of CSS alternatives which can be selected in the Styles drop-down by the end user.
  [AuthorDiffChangeTrackingMerger](ro/sync/diff/api/AuthorDiffChangeTrackingMerger.md)
Extracts the differences reported when comparing two XML documents ('Two-Way' Author comparison mode) as a document with change tracking, which can be used to review the differences and merge the two documents.
  [AuthorDiffChangeTrackingMergerFactory](ro/sync/diff/api/AuthorDiffChangeTrackingMergerFactory.md)
Factory for creating mergers with change tracking highlights.
  [AuthorDiffDirectoriesChangeTrackingMerger](ro/sync/diff/api/AuthorDiffDirectoriesChangeTrackingMerger.md)
Merger based on 2-way mode directory comparison which saves the results in a specified directory.
  [AuthorDifferencePerformer](ro/sync/diff/api/AuthorDifferencePerformer.md)
The [AuthorDifferencePerformer](ro/sync/diff/api/AuthorDifferencePerformer.md) is used to compare two Author documents using a set of options.
  [AuthorDnDListener](com/oxygenxml/editor/editors/author/AuthorDnDListener.md)
Author Drag and Drop listener interface for the SWT implementation.
  [AuthorDnDListener](ro/sync/exml/editor/xmleditor/pageauthor/AuthorDnDListener.md)
Author Drag and Drop listener interface for the AWT implementation.
  [AuthorDocument](ro/sync/ecss/extensions/api/node/AuthorDocument.md)
The Document interface represents the entire XML document.
  [AuthorDocumentController](ro/sync/ecss/extensions/api/AuthorDocumentController.md)
Provides methods for modifying the Author document.
  [AuthorDocumentEvent](ro/sync/ecss/extensions/api/AuthorDocumentEvent.md)
Marker interface for all document change related events.
  [AuthorDocumentFilter](ro/sync/ecss/extensions/api/AuthorDocumentFilter.md)
AuthorDocumentFilter, is a filter for the methods which modify the AuthorDocument.
  [AuthorDocumentFilterBypass](ro/sync/ecss/extensions/api/AuthorDocumentFilterBypass.md)
Used as a way to circumvent calling back into the AuthorDocumentController to change the AuthorDocument.
  [AuthorDocumentFragment](ro/sync/ecss/extensions/api/node/AuthorDocumentFragment.md)
Represents a fragment of an XML document.
  [AuthorDocumentModel](ro/sync/ecss/extensions/api/webapp/AuthorDocumentModel.md)
The model of an XML document to be edited.
  [AuthorDocumentModelContextManager](ro/sync/ecss/extensions/api/webapp/AuthorDocumentModelContextManager.md)
A helper class that handles the current editing context.
  [AuthorDocumentNodesCollector](ro/sync/ecss/dita/topic/ref/AuthorDocumentNodesCollector.md)
Collects nodes in an author document.
  [AuthorDocumentPositionedInfo](ro/sync/ecss/component/validation/AuthorDocumentPositionedInfo.md)
A document position info usually needs a line and column for the error.
  [AuthorDocumentProvider](ro/sync/ecss/extensions/api/node/AuthorDocumentProvider.md)
Use this API to access an "in memory" representation of an author document over a resource and customize the document in a non visual way using the [AuthorDocumentController](ro/sync/ecss/extensions/api/AuthorDocumentController.md) and [AuthorDocument](ro/sync/ecss/extensions/api/node/AuthorDocument.md) API.
  [AuthorDocumentType](ro/sync/ecss/extensions/api/AuthorDocumentType.md)
Author structure representing DOCTYPE information as present in the Author document.
  [AuthorEditorAccess](ro/sync/ecss/extensions/api/access/AuthorEditorAccess.md)
Provides access to methods related to the Author editor actions and information.
  [AuthorElement](ro/sync/ecss/extensions/api/node/AuthorElement.md)
The Author Element represents an XML element.
  [AuthorElementBaseInterface](ro/sync/ecss/extensions/api/AuthorElementBaseInterface.md)
Element represents a tag in an XML document.
  [AuthorExtensionActionProvider](ro/sync/ecss/extensions/api/AuthorExtensionActionProvider.md)
Provides an author extension action for a given action ID.
  [AuthorExtensionAskAction](ro/sync/ecss/extensions/api/editor/AuthorExtensionAskAction.md)
An author action created over an author operation who does not handle the ask variables expansion.
  [AuthorExtensionStateAdapter](ro/sync/ecss/extensions/api/AuthorExtensionStateAdapter.md)
Adapter class for [AuthorExtensionStateListener](ro/sync/ecss/extensions/api/AuthorExtensionStateListener.md).
  [AuthorExtensionStateListener](ro/sync/ecss/extensions/api/AuthorExtensionStateListener.md)
Notified when the Author extension, where the listener is defined, was activated or deactivated in the detection process.
  [AuthorExtensionStateListenerDelegator](ro/sync/ecss/extensions/api/AuthorExtensionStateListenerDelegator.md)
A single Author extension state listeners which delegates to other registered listeners.
  [AuthorExternalObjectInsertionHandler](ro/sync/ecss/extensions/api/AuthorExternalObjectInsertionHandler.md)
This class is notified when URLs are dropped or pasted to an Author Editor page or when XHTML fragments are pasted or dropped from external applications (like web browsers or office applications) to the Author page.If you want to use a stylesheet to convert the pasted XHTML to your own XML vocabulary you can just overwrite the method: "ro.sync.ecss.extensions.api.AuthorExternalObjectInsertionHandler.getImporterStylesheetFileName(AuthorAccess)" and return the file name of the stylesheet which will be applied.
  [AuthorFilteredContent](ro/sync/ecss/extensions/api/filter/AuthorFilteredContent.md)
The char sequence representing the filtered Author content.
  [AuthorFoldManager](ro/sync/exml/workspace/api/editor/page/author/fold/AuthorFoldManager.md)
Interface which can be used to expand/collapse foldable nodes.
  [AuthorFormatCompatibilityModeConstants](ro/sync/ecss/dom/builder/AuthorFormatCompatibilityModeConstants.md)
The way formatting when passing from author in text or on save.
  [AuthorHighlighter](ro/sync/ecss/extensions/api/highlights/AuthorHighlighter.md)
The highlighter which will be available to users to add, remove and check highlights.
  [AuthorHighlighterListener](ro/sync/ecss/extensions/api/highlights/AuthorHighlighterListener.md)
Listener for the author highlighter events.

[AuthorIdIndex](ro/sync/ecss/extensions/api/webapp/AuthorIdIndex.md)<[T](ro/sync/ecss/extensions/api/webapp/AuthorIdIndex.md)>

An index that maps from IDs to objects and viceversa.
  [AuthorImageDecorator](ro/sync/ecss/extensions/api/AuthorImageDecorator.md)
Permits decoration of the images that are displayed in the Author view.
  [AuthorImageMapDecorator](ro/sync/ecss/extensions/commons/imagemap/AuthorImageMapDecorator.md)
Image map decorator base for Author.
  [AuthorInplaceContext](ro/sync/ecss/extensions/api/editor/AuthorInplaceContext.md)
Context where an edit component will be used.
  [AuthorInputEvent](ro/sync/ecss/extensions/api/AuthorInputEvent.md)
Base class for Author input events.
  [AuthorListener](ro/sync/ecss/extensions/api/AuthorListener.md)
Listener notified about Author document changes, document structure changes and document content changes. **DANGER:** You must avoid making live document changes on the received call backs.
  [AuthorListenerAdapter](ro/sync/ecss/extensions/api/AuthorListenerAdapter.md)
Convenience implementation of the [AuthorListener](ro/sync/ecss/extensions/api/AuthorListener.md).
  [AuthorMouseAdapter](ro/sync/ecss/extensions/api/AuthorMouseAdapter.md)
Empty implementation of the [AuthorMouseListener](ro/sync/ecss/extensions/api/AuthorMouseListener.md).
  [AuthorMouseEvent](ro/sync/ecss/extensions/api/AuthorMouseEvent.md)
Mouse event received by the [AuthorMouseListener](ro/sync/ecss/extensions/api/AuthorMouseListener.md).
  [AuthorMouseListener](ro/sync/ecss/extensions/api/AuthorMouseListener.md)
Interface for the author mouse listeners.
  [AuthorNode](ro/sync/ecss/extensions/api/node/AuthorNode.md)
Base interface for all Author nodes.
  [AuthorNodeRendererCustomizer](ro/sync/ecss/extensions/api/structure/AuthorNodeRendererCustomizer.md)
Customize rendering information for an AuthorNode
  [AuthorNodeRendererCustomizerContext](ro/sync/exml/workspace/api/editor/page/author/AuthorNodeRendererCustomizerContext.md)
Offers access to the current Author node (the one for which we are customizing the renderer).
  [AuthorNodesFilter](ro/sync/ecss/extensions/api/filter/AuthorNodesFilter.md)
Provides information about the Author nodes that should be filtered.
  [AuthorNodeUtil](ro/sync/ecss/extensions/api/node/AuthorNodeUtil.md)
Utility functions for working with AuthorNodes.
  [AuthorOperation](ro/sync/ecss/extensions/api/AuthorOperation.md)
Interface defining an author extension operation.
  [AuthorOperationException](ro/sync/ecss/extensions/api/AuthorOperationException.md)
An exception thrown by an [AuthorOperation](ro/sync/ecss/extensions/api/AuthorOperation.md) when it fails.
  [AuthorOperationStoppedByUserException](ro/sync/ecss/extensions/api/AuthorOperationStoppedByUserException.md)
An exception thrown by an [AuthorOperation](ro/sync/ecss/extensions/api/AuthorOperation.md) when it interacts with the user and the user cancels it.
  [AuthorOperationWithCustomUndoBehavior](ro/sync/ecss/extensions/api/AuthorOperationWithCustomUndoBehavior.md)
Marker interface that specifies that a particular operation should not be wrapped in a compound undoable edit.
  [AuthorOperationWithResult](ro/sync/ecss/extensions/api/webapp/AuthorOperationWithResult.md)
Operation that returns a result when invoked from the Web Author JS API.
  [AuthorOutlineAccess](ro/sync/ecss/extensions/api/access/AuthorOutlineAccess.md)
Author Outline access.
  [AuthorOutlineCustomizer](ro/sync/ecss/extensions/api/structure/AuthorOutlineCustomizer.md)
Author Outline customizer used for custom filtering and nodes rendering in the Outline.
  [AuthorParentNode](ro/sync/ecss/extensions/api/node/AuthorParentNode.md)
An author parent node contains a list of children.
  [AuthorPersistentHighlight](ro/sync/ecss/extensions/api/highlights/AuthorPersistentHighlight.md)
Defines the Author Persistent Highlight which get serialized in the XML as processing instruction.
  [AuthorPersistentHighlight.PersistentHighlightType](ro/sync/ecss/extensions/api/highlights/AuthorPersistentHighlight.PersistentHighlightType.md)
The Author Persistent Highlight type.
  [AuthorPersistentHighlightActionsProvider](ro/sync/ecss/extensions/api/highlights/AuthorPersistentHighlightActionsProvider.md)
The provider for contextual actions that are shown on the contextual menu of the persistent highlight (in the main editor area - not yet supported) and on the associated callout.
  [AuthorPersistentHighlightConstants](ro/sync/ecss/extensions/api/highlights/AuthorPersistentHighlightConstants.md)
Constants used in the serialization process of the Author Persistent Highlights.
  [AuthorPersistentHighlighter](ro/sync/ecss/extensions/api/highlights/AuthorPersistentHighlighter.md)
Manage the user custom persistent highlights which get serialized in the XML as processing instructions with the form:  <?oxy_custom_start prop1="val1"....?> xml content <?oxy_custom_end?> The Highlighter is accessible from [WSAuthorEditorPageBase.getPersistentHighlighter()](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#getPersistentHighlighter()).
  [AuthorPersistentHighlightsFilter](ro/sync/ecss/extensions/api/highlights/AuthorPersistentHighlightsFilter.md)
Filter for the [AuthorPersistentHighlight](ro/sync/ecss/extensions/api/highlights/AuthorPersistentHighlight.md) presented in the author page, callouts section and review panel.
  [AuthorPersistentHighlightsListener](ro/sync/ecss/extensions/api/highlights/AuthorPersistentHighlightsListener.md)
Listener for all the events related to the [AuthorPersistentHighlight](ro/sync/ecss/extensions/api/highlights/AuthorPersistentHighlight.md).
  [AuthorPopupMenuCustomizer](ro/sync/ecss/extensions/api/structure/AuthorPopupMenuCustomizer.md)
Can be used to customize a pop-up menu before showing it.
  [AuthorPreloadProcessor](ro/sync/ecss/extensions/api/AuthorPreloadProcessor.md)
This processor is notified before the Author document is loaded and renderer.
  [AuthorPreviewComponentProvider](ro/sync/exml/workspace/api/editor/page/author/AuthorPreviewComponentProvider.md)
A simple read only Author preview component.
  [AuthorPseudoClassController](ro/sync/ecss/extensions/api/AuthorPseudoClassController.md)
Controls setting and resetting pseudo classes.
  [AuthorReferenceNode](ro/sync/ecss/extensions/api/node/AuthorReferenceNode.md)
Interface for reference nodes that have a content expanded when displayed in the Author mode.
  [AuthorReferenceResolver](ro/sync/ecss/extensions/api/AuthorReferenceResolver.md)
Interface for the custom handlers used to expand content references.
  [AuthorReferenceResolverWrapper](ro/sync/ecss/component/resolvers/AuthorReferenceResolverWrapper.md)
Adapter used to make wrappers over [AuthorReferenceResolver](ro/sync/ecss/extensions/api/AuthorReferenceResolver.md).
  [AuthorResourceBundle](ro/sync/ecss/extensions/api/AuthorResourceBundle.md)
Gives access to translate keys.
  [AuthorReviewController](ro/sync/ecss/extensions/api/AuthorReviewController.md)
Controller that can be used to toggle the change tracking state, modify the review highlight author name, the highlight painting or to obtain information about the properties used in the serialization and representation of the review highlight (author name, reviewer auto color or the current time stamp in a format identical to the one used by Oxygen for insert, delete and comment review highlights).
  [AuthorReviewerNameController](ro/sync/ecss/extensions/api/AuthorReviewerNameController.md)
Provides access to reviewer author name, used in the processing instruction that results when a tracked change or a comment is serialized.
  [AuthorReviewRenderingInformation](ro/sync/ecss/extensions/api/review/AuthorReviewRenderingInformation.md)
The review view entries are representations of Track Changes insert and delete highlights and review comment highlights highlights in Author mode.
  [AuthorReviewViewController](ro/sync/ecss/extensions/api/review/AuthorReviewViewController.md)
The review view presents Track Changes insert and delete highlights and review comment highlights in the Author mode.
  [AuthorSchemaAwareEditingHandler](ro/sync/ecss/extensions/api/AuthorSchemaAwareEditingHandler.md)
If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this handler.
  [AuthorSchemaAwareEditingHandlerAdapter](ro/sync/ecss/extensions/api/AuthorSchemaAwareEditingHandlerAdapter.md)
Adapter class.
  [AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions](ro/sync/ecss/extensions/api/AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions.md)
One of the default smart paste strategies involves detecting an path o ancestors from the context element to the inserted one.
  [AuthorSchemaManager](ro/sync/ecss/extensions/api/AuthorSchemaManager.md)
Author schema manager.
  [AuthorSelectionAndCaretModel](ro/sync/ecss/extensions/api/AuthorSelectionAndCaretModel.md)
Interface to the author selection and caret model providing methods to query and modify the selection intervals and caret position.
  [AuthorSelectionModel](ro/sync/ecss/extensions/api/AuthorSelectionModel.md)
Get the Author selection model containing access to all Author selection intervals and methods for adding simple and multiple selections.
  [AuthorSource](ro/sync/ecss/dom/wrappers/mutable/AuthorSource.md)
A DOM-like source over a author document model.
  [AuthorTableAccess](ro/sync/ecss/extensions/api/access/AuthorTableAccess.md)
Provides methods for table actions and informations regarding the table content.
  [AuthorTableArguments](ro/sync/ecss/extensions/api/table/operations/AuthorTableArguments.md)
Holds the arguments for [AuthorTableOperationsHandler.handleCreateTable(AuthorTableArguments)](ro/sync/ecss/extensions/api/table/operations/AuthorTableOperationsHandler.md#handleCreateTable(ro.sync.ecss.extensions.api.table.operations.AuthorTableArguments)) method.
  [AuthorTableCellSepProvider](ro/sync/ecss/extensions/api/AuthorTableCellSepProvider.md)
This is an interface for classes which are responsible for providing information about the cell separators: "rowsep" and "colsep".
  [AuthorTableCellSpanProvider](ro/sync/ecss/extensions/api/AuthorTableCellSpanProvider.md)
This is an interface for classes which are responsible for providing information about the cell spanning.
  [AuthorTableColumnWidthProvider](ro/sync/ecss/extensions/api/AuthorTableColumnWidthProvider.md)
This is an interface for classes which are responsible for providing information and handling modifications regarding table and column widths.
  [AuthorTableColumnWidthProviderBase](ro/sync/ecss/extensions/api/AuthorTableColumnWidthProviderBase.md)
This is an interface for classes which are responsible for providing information and handling modifications regarding table and column widths.
  [AuthorTableDeleteColumnArguments](ro/sync/ecss/extensions/api/table/operations/AuthorTableDeleteColumnArguments.md)
Holds the arguments for [AuthorTableOperationsHandler.handleDeleteColumn(AuthorTableDeleteColumnArguments)](ro/sync/ecss/extensions/api/table/operations/AuthorTableOperationsHandler.md#handleDeleteColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteColumnArguments)) method.
  [AuthorTableDeleteRowArguments](ro/sync/ecss/extensions/api/table/operations/AuthorTableDeleteRowArguments.md)
Holds the arguments for [AuthorTableOperationsHandler.handleDeleteRow(AuthorTableDeleteRowArguments)](ro/sync/ecss/extensions/api/table/operations/AuthorTableOperationsHandler.md#handleDeleteRow(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowArguments)) method.
  [AuthorTableDeleteRowsArguments](ro/sync/ecss/extensions/api/table/operations/AuthorTableDeleteRowsArguments.md)
Holds the arguments for [AuthorTableOperationsHandler.handleDeleteRows(AuthorTableDeleteRowsArguments)](ro/sync/ecss/extensions/api/table/operations/AuthorTableOperationsHandler.md#handleDeleteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableDeleteRowsArguments)) method.
  [AuthorTableHelper](ro/sync/ecss/extensions/commons/table/operations/AuthorTableHelper.md)
Document type specific table information helper.
  [AuthorTableInsertColumnArguments](ro/sync/ecss/extensions/api/table/operations/AuthorTableInsertColumnArguments.md)
Holds the arguments for [AuthorTableOperationsHandler.handleInsertColumn(AuthorTableInsertColumnArguments)](ro/sync/ecss/extensions/api/table/operations/AuthorTableOperationsHandler.md#handleInsertColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertColumnArguments)) method.
  [AuthorTableInsertRowArguments](ro/sync/ecss/extensions/api/table/operations/AuthorTableInsertRowArguments.md)
Holds the arguments for [AuthorTableOperationsHandler.handlePasteRows(AuthorTableInsertRowArguments)](ro/sync/ecss/extensions/api/table/operations/AuthorTableOperationsHandler.md#handlePasteRows(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertRowArguments)) method.
  [AuthorTableOperationsHandler](ro/sync/ecss/extensions/api/table/operations/AuthorTableOperationsHandler.md)
Handler for Author table operations.
  [AuthorTooltipCustomizer](ro/sync/exml/workspace/api/editor/page/author/tooltip/AuthorTooltipCustomizer.md)
Customize the tooltips which appear when hovering in the Author page.
  [AuthorTooltipCustomizerProvider](ro/sync/exml/workspace/api/editor/page/author/tooltip/AuthorTooltipCustomizerProvider.md)
Allow developers to add tooltip customizers for customizing the tooltips which appear when hovering in the visual Author editing mode.
  [AuthorUndoManager](ro/sync/ecss/extensions/api/AuthorUndoManager.md)
Undo manager for Author edits.
  [AuthorUtilAccess](ro/sync/ecss/extensions/api/access/AuthorUtilAccess.md)
Provides access to utility methods related to author access.
  [AuthorViewToModelInfo](ro/sync/ecss/extensions/api/AuthorViewToModelInfo.md)
An implementation of this interface is returned by the [WSAuthorEditorPageBase.viewToModel(int, int)](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#viewToModel(int,int))method.
  [AuthorWorkspaceAccess](ro/sync/ecss/extensions/api/access/AuthorWorkspaceAccess.md)
Provides access to workspace specific information and actions.
  [AuthorXMLUtilAccess](ro/sync/ecss/extensions/api/access/AuthorXMLUtilAccess.md)
Author XML Utilities.
  [AuthorXPathExpressionBuilder](ro/sync/ecss/extensions/api/AuthorXPathExpressionBuilder.md)
Generates an XPath expression for an XML node.
  [AWTExtension](ro/sync/ecss/extensions/api/AWTExtension.md)
The base interface for all AWT Oxygen extension classes.
  [BaseShape](ro/sync/exml/view/graphics/BaseShape.md)
Base for shapes.
  [BasicRenderingInformation](ro/sync/exml/workspace/api/node/customizer/BasicRenderingInformation.md)
The rendering information used to display a node in the Outline view, Author bread crumb, Content Completion popup window, Elements view and DITA Map view.
  [BatchEditListener](ro/sync/ecss/component/BatchEditListener.md)
The edit events sometimes come in batches, for example when an undo is executed.
  [BatchOperationInfo](ro/sync/exml/workspace/api/listeners/BatchOperationInfo.md)
The type of batch operation.
  [BatchOperationInfo.Type](ro/sync/exml/workspace/api/listeners/BatchOperationInfo.Type.md)
The type of the batch operation.
  [BatchOperationsListener](ro/sync/exml/workspace/api/listeners/BatchOperationsListener.md)
Listener which can be notified before and after a batch operation which will modify lots of resources (Replace All in Files, Rename in Files) is started.
  [BinaryImageHandler](ro/sync/exml/workspace/api/images/handlers/BinaryImageHandler.md)
Special handler for binary images like EPS or AI...
  [Button](ro/sync/exml/workspace/api/standalone/ui/Button.md)
Button which has proper support for retina icons.
  [ButtonEditor](ro/sync/ecss/component/editor/ButtonEditor.md)
A button that can be used to invoke an author extension action.
  [ButtonGroupEditor](ro/sync/ecss/component/editor/ButtonGroupEditor.md)
Inplace editor that uses a button to trigger a pop-up menu with multiple actions.
  [CacheableAuthorReferencesResolver](ro/sync/ecss/extensions/api/CacheableAuthorReferencesResolver.md)
Marker for cachable references resolvers.
  [CacheableUrlConnection](ro/sync/exml/plugin/urlstreamhandler/CacheableUrlConnection.md)
Marker interface that should be implemented by a URL connection and which instructs oXygen that it makes sense to cache data read from such a connection.
  [CalloutActionsProvider](ro/sync/ecss/extensions/api/callouts/CalloutActionsProvider.md)
Provides a set of custom actions for a certain highlight.
  [CalloutsRenderingInformationProvider](ro/sync/ecss/extensions/api/callouts/CalloutsRenderingInformationProvider.md)
Provider for data that will be rendered as callouts, in Author mode.
  [CALSAndHTMLShowTablePropertiesBase](ro/sync/ecss/extensions/commons/table/properties/CALSAndHTMLShowTablePropertiesBase.md)
Base class for edit properties on CALS and HTML tables.
  [CALSandHTMLTableCellInfoProvider](ro/sync/ecss/extensions/commons/table/support/CALSandHTMLTableCellInfoProvider.md)
A table cell span and column width info provider used for frameworks that have both CALS and HTML tables.
  [CALSandHTMLTableCellSpanProvider](ro/sync/ecss/extensions/commons/table/spansupport/CALSandHTMLTableCellSpanProvider.md)
Empty implementation for backward compatibility .
  [CALSAndHTMLTableLayoutProblem](ro/sync/ecss/extensions/commons/table/support/errorscanner/CALSAndHTMLTableLayoutProblem.md)
CALS table layout problem
  [CALSAndHTMLTableSortOperation](ro/sync/ecss/extensions/commons/table/operations/cals/CALSAndHTMLTableSortOperation.md)
Table sort operation base for CALS and HTML tables.
  [CALSColSpanSpec](ro/sync/ecss/extensions/commons/table/support/CALSColSpanSpec.md)
Contains information about column span for the CALS table model (e.g.
  [CALSColSpec](ro/sync/ecss/extensions/commons/table/support/CALSColSpec.md)
The column specification for a CALS table model (e.g.
  [CALSConstants](ro/sync/ecss/extensions/commons/table/operations/cals/CALSConstants.md)
Contains the names of the elements and attributes used in CALS table model (e.g.
  [CALSDocumentTypeHelper](ro/sync/ecss/extensions/commons/table/operations/cals/CALSDocumentTypeHelper.md)
Implementation of the document type helper for CALS table model(DocBook, DITA and S1000D).
  [CALSShowTableProperties](ro/sync/ecss/extensions/commons/table/properties/CALSShowTableProperties.md)

 [CALSTableCellInfoProvider](ro/sync/ecss/extensions/commons/table/support/CALSTableCellInfoProvider.md)
Provides informations about the cell spanning and column width for Docbook CALS tables.
  [CALSTableCellSpanProvider](ro/sync/ecss/extensions/commons/table/spansupport/CALSTableCellSpanProvider.md)
Empty implementation for backward compatibility.
  [CALSTableColumnSpecificationInformation](ro/sync/ecss/extensions/commons/table/operations/cals/CALSTableColumnSpecificationInformation.md)
Information about CALS table column specification.
  [CancelledByUserException](ro/sync/ecss/extensions/api/CancelledByUserException.md)
A custom class used for the exceptions generated by an operation canceled by user.
  [CannotEditException](ro/sync/ecss/extensions/commons/CannotEditException.md)
Deprecated.
 [CannotEditException](ro/sync/exml/workspace/api/images/handlers/CannotEditException.md)
Exception thrown when an attempt to edit an resource is made with a handler that does not support this, or that gets an error when editing.
  [CannotHandleException](ro/sync/diff/factory/CannotHandleException.md)
Thrown when an algorithm cannont handle the documents it is supposed to diff.
  [CannotRecognizeIDException](ro/sync/ecss/extensions/api/link/CannotRecognizeIDException.md)
Exception that is thrown when an ID cannot be recognized in the current context.
  [CapitalizeSentencesOperation](ro/sync/ecss/extensions/commons/operations/text/CapitalizeSentencesOperation.md)
The class provides an operation for forming sentences over a selection.
  [CapitalizeWordsOperation](ro/sync/ecss/extensions/commons/operations/text/CapitalizeWordsOperation.md)
The class provides an operation for forming words over a selection.
  [CCItemProxy](ro/sync/ecss/extensions/api/webapp/cc/CCItemProxy.md)
An item proposed by the content completion manager, and which can be selected by the user.
  [ChangeAttributeOperation](ro/sync/ecss/extensions/commons/operations/ChangeAttributeOperation.md)
An implementation of an operation to change the value of an attribute.
  [ChangeAttributesOperation](ro/sync/ecss/extensions/commons/operations/ChangeAttributesOperation.md)
Operation that can change/insert/remove one or more attributes of one or more elements.
  [ChangePseudoClassesOperation](ro/sync/ecss/extensions/commons/operations/ChangePseudoClassesOperation.md)
An implementation of an operation to set a list of pseudo class values to nodes identified by an XPath expression and to remove a list of values from nodes identified by an XPath expression.
  [ChangeTrackingController](ro/sync/ecss/extensions/api/ChangeTrackingController.md)
Controls the change tracking mode.
  [CheckBoxEditor](ro/sync/ecss/component/editor/CheckBoxEditor.md)
A panel with checkboxes that can be used to render boolean values but also lists of values.
  [ChoiceTableHelper](ro/sync/ecss/extensions/dita/topic/table/simpletable/properties/ChoiceTableHelper.md)
Helper class for edit properties on DITA Simple tables.
  [ChoiceTableShowPropertiesOperation](ro/sync/ecss/extensions/dita/topic/table/simpletable/properties/ChoiceTableShowPropertiesOperation.md)
Class for edit properties on DITA choice tables.
  [CIAttribute](ro/sync/contentcompletion/xml/CIAttribute.md)
Interface for objects holding information about attributes used in the content completion process.
  [CIAttribute.DefaultValueProvider](ro/sync/contentcompletion/xml/CIAttribute.DefaultValueProvider.md)
Default value provider for an attribute.
  [CIAttribute.EditableState](ro/sync/contentcompletion/xml/CIAttribute.EditableState.md)
The editable state of the attribute.
  [CIElement](ro/sync/contentcompletion/xml/CIElement.md)
Interface for objects holding information about element proposals used in the content completion process.
  [CIElementAdapter](ro/sync/contentcompletion/xml/CIElementAdapter.md)
A CIElement adapter.
  [CILevelValue](ro/sync/ecss/dita/CILevelValue.md)
CI Value which also has a level.
  [Circle](ro/sync/exml/view/graphics/Circle.md)
The class describes a circle
  [CIValue](ro/sync/contentcompletion/xml/CIValue.md)
Interface for objects holding information about element or attribute values used in the content completion process.
  [ClassPathResourcesAccess](ro/sync/ecss/extensions/api/ClassPathResourcesAccess.md)
Provides access to all URLs which were added in the classpath for the specific framework when the document type was edited from the Oxygen preferences.
  [ClipboardFragmentInformation](ro/sync/ecss/extensions/api/content/ClipboardFragmentInformation.md)
Provides information about a fragment in the clipboard.
  [ClipboardFragmentProcessor](ro/sync/ecss/extensions/api/content/ClipboardFragmentProcessor.md)
Process a document fragment from the clipboard (pasted or dropped in the Author page).
  [CollectingError](ro/sync/exml/workspace/api/references/CollectingError.md)
CollectingError is an interface that describes an error that happens while collecting references
  [CollectingError.Severity](ro/sync/exml/workspace/api/references/CollectingError.Severity.md)
The severity of the error
  [Color](ro/sync/exml/view/graphics/Color.md)
The class used to represent a Color.
  [ColorButton](ro/sync/exml/workspace/api/standalone/ui/ColorButton.md)
A button which presents a color chooser
  [ColorHighlightPainter](ro/sync/ecss/extensions/api/highlights/ColorHighlightPainter.md)
Painter that can be used to customize the way that a highlight is displayed by setting custom text decoration, text decoration stroke, background color or stroke color.
  [ColorHighlightPainter.TextDecoration](ro/sync/ecss/extensions/api/highlights/ColorHighlightPainter.TextDecoration.md)
The decoration added to text.
  [ColorTheme](ro/sync/exml/workspace/api/util/ColorTheme.md)
A theme manager is an object that is able to provide information about the color theme used by oXygen.
  [ColorThemeUtilities](ro/sync/exml/workspace/api/util/ColorThemeUtilities.md)
A theme manager is an object that is able to provide information about the color theme used by oXygen.
  [ComboBoxEditor](ro/sync/ecss/component/editor/ComboBoxEditor.md)
Combo box value editor.
  [CommonActionsProvider](ro/sync/exml/workspace/api/actions/CommonActionsProvider.md)
Provides access to actions.
  [CommonsOperationsUtil](ro/sync/ecss/extensions/commons/operations/CommonsOperationsUtil.md)
Util methods for common Author operations.
  [CommonsOperationsUtil.ConversionElementHelper](ro/sync/ecss/extensions/commons/operations/CommonsOperationsUtil.ConversionElementHelper.md)
Interface used to check the elements that will be converted in other elements (table cells or list entries)
  [CommonsOperationsUtil.SelectedFragmentInfo](ro/sync/ecss/extensions/commons/operations/CommonsOperationsUtil.SelectedFragmentInfo.md)
Class containing the new fragment and info about it.
  [CompareUtilAccess](ro/sync/exml/workspace/api/util/CompareUtilAccess.md)
Compare utilities.
  [CompletionProposal](ro/sync/exml/workspace/api/standalone/project/textcompletions/CompletionProposal.md)
Represents a text completion proposal.
  [CompletionProposalsOptions](ro/sync/exml/workspace/api/standalone/project/textcompletions/CompletionProposalsOptions.md)
A set of options for the completion selection algorithm.
  [CompletionProposalsOptions.Builder](ro/sync/exml/workspace/api/standalone/project/textcompletions/CompletionProposalsOptions.Builder.md)
Builder.
  [ComponentProvider](ro/sync/ecss/extensions/api/component/ComponentProvider.md)
Base interface for Editor and for DITA Map component providers with common methods.
  [ComponentsValidator](ro/sync/exml/ComponentsValidator.md)
Validator interface for menus, toolbars and their actions.
  [ComponentsValidatorPluginExtension](ro/sync/exml/plugin/startup/ComponentsValidatorPluginExtension.md)
Startup plugin.
  [CompoundEditListener](ro/sync/ecss/extensions/api/CompoundEditListener.md)
Listener notified when compound edits are started and ended.
  [ConfigurationProperties](ro/sync/exml/plugin/transform/ConfigurationProperties.md)
Interface with transformer properties that can be passed externally.
  [ConfigureAutoIDElementsOperation](ro/sync/ecss/extensions/commons/id/ConfigureAutoIDElementsOperation.md)
Operation used to configure elements for which ID generation is auto.
  [Content](ro/sync/ecss/extensions/api/Content.md)
Interface to describe a sequence of character content that can be edited.
  [ContentCompletionManager](ro/sync/ecss/extensions/api/webapp/cc/ContentCompletionManager.md)
This class offers support for actions with content completion such as: insert element, surround with tags and rename element.
  [ContentCompletionSortPriorityAssigner](ro/sync/ecss/extensions/api/webapp/cc/ContentCompletionSortPriorityAssigner.md)
Extension that can be used to assign sorting priorities for elements. The elements in the content completion menu will be sorted according to this priority and in case of equality the display name is used. By default, all entries have priority 0 except for "Split" / "New" - type entries which have priority [CCItemProxy.SPLIT_ITEM_PRIORITY](ro/sync/ecss/extensions/api/webapp/cc/CCItemProxy.md#SPLIT_ITEM_PRIORITY). The instance can be returned from a [WebappExtensionsProvider](ro/sync/ecss/extensions/api/WebappExtensionsProvider.md) implementation, by implementing the [WebappExtensionsProvider.getSortPriorityAssigner()](ro/sync/ecss/extensions/api/WebappExtensionsProvider.md#getSortPriorityAssigner()) method. The [WebappExtensionsProvider](ro/sync/ecss/extensions/api/WebappExtensionsProvider.md) instance can be returned from an [ExtensionsBundle](ro/sync/ecss/extensions/api/ExtensionsBundle.md) implementation, by implementing the [ExtensionsBundle.getWebappExtensionsProvier()](ro/sync/ecss/extensions/api/ExtensionsBundle.md#getWebappExtensionsProvier()) method.
  [ContentInterval](ro/sync/ecss/extensions/api/ContentInterval.md)
A content interval containing the **inclusive** start offset and **exclusive** end offset.
  [ContentIterator](ro/sync/ecss/extensions/api/node/ContentIterator.md)
Iterator over the content of a node.
  [Context](ro/sync/contentcompletion/xml/Context.md)
The context for a node contains: elementStack - the stack with [ContextElement](ro/sync/contentcompletion/xml/ContextElement.md) up to the root.
  [ContextDescriptionProvider](ro/sync/exml/workspace/api/standalone/ContextDescriptionProvider.md)
Provides language-independent information about a certain context.
  [ContextElement](ro/sync/contentcompletion/xml/ContextElement.md)
Store information about an element inside a context, involved in the content completion process.
  [ContextKeyManager](ro/sync/ecss/dita/ContextKeyManager.md)
Context aware key manager.
  [ContextKeyManagerProvider](ro/sync/ecss/dita/ContextKeyManagerProvider.md)
Provider of a context key manager.
  [ConversionProvider](ro/sync/net/protocol/convert/ConversionProvider.md)
Provides conversion for a certain type of processor
  [ConvertHexToCharOperation](ro/sync/ecss/extensions/commons/operations/text/ConvertHexToCharOperation.md)
Operation for converting a hexadecimal sequence of digits from the left of the caret to the equivalent Unicode character.
  [Cookie](ro/sync/ecss/extensions/api/webapp/plugin/servlet/http/Cookie.md)
Cookie interface inspired from HTTP Servlet 5.0.
  [CountWordsOperation](ro/sync/ecss/extensions/commons/operations/text/CountWordsOperation.md)
Count words either in the whole document or in the selection.
  [CreateAndInsertTopicRef](ro/sync/ecss/extensions/dita/map/topicref/CreateAndInsertTopicRef.md)
Action to create a new topic and insert a reference to it.
  [CreateAndInsertTopicRef.Arguments](ro/sync/ecss/extensions/dita/map/topicref/CreateAndInsertTopicRef.Arguments.md)
Handles argument retrieval.
  [CreateNewTopicFromSelectionOperation](ro/sync/ecss/extensions/dita/topic/CreateNewTopicFromSelectionOperation.md)
Author operation that will create a new document using the selected text from current document
  [CreateReusableComponentOperation](ro/sync/ecss/extensions/dita/reuse/CreateReusableComponentOperation.md)
Operation used to create a reusable component in DITA documents.
  [CriterionComposite](ro/sync/ecss/extensions/commons/sort/CriterionComposite.md)
This class will add to the given parent container a checkbox to enable the criterion, a combobox to select the key, a type combobox and order combobox.
  [CriterionInformation](ro/sync/ecss/extensions/commons/sort/CriterionInformation.md)
Holds information about a single sorting criterion.
  [CriterionInformation.ORDER](ro/sync/ecss/extensions/commons/sort/CriterionInformation.ORDER.md)
Order enumeration.
  [CriterionInformation.TYPE](ro/sync/ecss/extensions/commons/sort/CriterionInformation.TYPE.md)
Type enumeration.
  [CriterionPanel](ro/sync/ecss/extensions/commons/sort/CriterionPanel.md)
This class will add to the given parent container a checkbox to enable the criterion, a combobox to select the key, a type combobox and order combobox.
  [CspDirective](ro/sync/exml/plugin/workspace/security/CspDirective.md)
Enum for Content Security Policy (CSP) directives.
  [CspProviderExtension](ro/sync/exml/plugin/workspace/security/CspProviderExtension.md)
Extension that can be used by plugins to contribute to the Content-Security-Policy header.
  [CSSCounter](ro/sync/ecss/css/CSSCounter.md)
A CSS counter identified by it's name.
  [CSSCounterIncrement](ro/sync/ecss/css/CSSCounterIncrement.md)
A CSS counter increment data.
  [CSSGroup](ro/sync/exml/workspace/api/editor/page/author/css/CSSGroup.md)
Represents a group of CSS resources that will all be used at once to style the Author interface.
  [CSSResource](ro/sync/exml/workspace/api/editor/page/author/css/CSSResource.md)
The CSS resource contains an URI to the CSS resource and its origin.
  [CursorType](ro/sync/ecss/extensions/api/CursorType.md)
Supported cursor types for author.
  [CustomAttributeValueContext](ro/sync/ecss/extensions/api/CustomAttributeValueContext.md)
Context for a custom attribute.
  [CustomAttributeValueEditingContext](ro/sync/ecss/extensions/api/CustomAttributeValueEditingContext.md)
Provides the contexts for the custom attribute value editing.
  [CustomAttributeValueEditor](ro/sync/ecss/extensions/api/CustomAttributeValueEditor.md)
A custom editor which gets invoked to edit the value for an attribute.
  [CustomEditorInputCreator](com/oxygenxml/editor/editors/CustomEditorInputCreator.md)
Abstract class allowed as an extension point to create a custom editor input for resources that the Oxygen plugin tries to open (by clicking on a link in the Author page for example).
  [CustomResolverException](ro/sync/ecss/extensions/api/CustomResolverException.md)
Signals an custom reference that wasn't resolved.
  [DataSourceConnectionInfo](ro/sync/exml/workspace/api/options/DataSourceConnectionInfo.md)
Provides properties values for a Data source.
  [DatePickerEditor](ro/sync/ecss/component/editor/DatePickerEditor.md)
Date picker form control.
  [DB4InsertListOperation](ro/sync/ecss/extensions/docbook/DB4InsertListOperation.md)
Insert list operation for Docbook 4.
  [DB5InsertListOperation](ro/sync/ecss/extensions/docbook/DB5InsertListOperation.md)
Insert List operation for Docbook 5.
  [DefaultAuthorActionEventHandler](ro/sync/ecss/extensions/api/DefaultAuthorActionEventHandler.md)
Intercepts TAB and SHIFT+TAB events inside a list item and promotes or demotes it.
  [DefaultAuthorActionEventHandler.CiElementAndOffset](ro/sync/ecss/extensions/api/DefaultAuthorActionEventHandler.CiElementAndOffset.md)
A simple structure to return from the method getInsertableFormForElement both the CIElement that can be inserted for a given element and the offset that should be applied to the insertion position in order to insert it.
  [DefaultElementLocatorProvider](ro/sync/ecss/extensions/commons/DefaultElementLocatorProvider.md)
Default implementation for locating elements based on a given link.
  [DefaultExtensions](ro/sync/ecss/extensions/commons/operations/DefaultExtensions.md)
Interface containing all the default operation distributed with Oxygen.
  [DefaultIDTypeIdentifier](ro/sync/ecss/extensions/api/link/DefaultIDTypeIdentifier.md)
Default implementation for [IDTypeIdentifier](ro/sync/ecss/extensions/api/link/IDTypeIdentifier.md).
  [DefaultSaveStrategy](ro/sync/ecss/extensions/api/webapp/ce/DefaultSaveStrategy.md)
Default save strategy used when no save strategy is explicitly specified when creating a room.
  [DefaultUniqueAttributesRecognizer](ro/sync/ecss/extensions/commons/id/DefaultUniqueAttributesRecognizer.md)
Default unique attributes recognizer
  [DeleteColumnOperation](ro/sync/ecss/extensions/commons/table/operations/cals/DeleteColumnOperation.md)
Operation used to delete a CALS table column.
  [DeleteColumnOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/DeleteColumnOperation.md)
Operation used to delete an XHTML table column.
  [DeleteColumnOperation](ro/sync/ecss/extensions/dita/map/table/DeleteColumnOperation.md)
Operation used to delete a DITA map reltable column.
  [DeleteColumnOperation](ro/sync/ecss/extensions/dita/topic/table/cals/DeleteColumnOperation.md)
Operation used to delete a DITA CALS table column.
  [DeleteColumnOperation](ro/sync/ecss/extensions/dita/topic/table/simpletable/DeleteColumnOperation.md)
Operation used to delete a DITA simple table column.
  [DeleteColumnOperation](ro/sync/ecss/extensions/tei/table/DeleteColumnOperation.md)
Operation used to delete a TEI table column.
  [DeleteColumnOperationBase](ro/sync/ecss/extensions/commons/table/operations/DeleteColumnOperationBase.md)
Base implementation for operations used to delete table columns.
  [DeleteElementOperation](ro/sync/ecss/extensions/commons/operations/DeleteElementOperation.md)
An implementation of a delete operation that deletes the node at caret.
  [DeleteElementsOperation](ro/sync/ecss/extensions/commons/operations/DeleteElementsOperation.md)
An implementation of a delete operation that deletes all the nodes identified by a XPath expression.
  [DeleteRowOperation](ro/sync/ecss/extensions/commons/table/operations/cals/DeleteRowOperation.md)
Operation used to delete a CALS table row.
  [DeleteRowOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/DeleteRowOperation.md)
Operation used to delete an XHTML table row.
  [DeleteRowOperation](ro/sync/ecss/extensions/dita/map/table/DeleteRowOperation.md)
Operation used to delete a DITA map reltable row.
  [DeleteRowOperation](ro/sync/ecss/extensions/dita/topic/table/cals/DeleteRowOperation.md)
Operation used to delete a DITA CALS table row.
  [DeleteRowOperation](ro/sync/ecss/extensions/dita/topic/table/simpletable/DeleteRowOperation.md)
Operation used to delete a DITA simple table row.
  [DeleteRowOperation](ro/sync/ecss/extensions/tei/table/DeleteRowOperation.md)
Operation used to delete a TEI table row.
  [DeleteRowOperationBase](ro/sync/ecss/extensions/commons/table/operations/DeleteRowOperationBase.md)
Operation used to delete table rows.
  [DemoteTopicrefOperation](ro/sync/ecss/extensions/dita/map/topicref/DemoteTopicrefOperation.md)
Implements a demote operation.
  [Dictionary](ro/sync/exml/workspace/api/spell/Dictionary.md)
This interface can be used to set an extra terms dictionary to be used on spell checking actions.
  [DiffAndMergeTools](ro/sync/exml/workspace/api/standalone/DiffAndMergeTools.md)
Tools used for executing operations like finding differences between files and folders, or merging different files.
  [DiffContentTypes](ro/sync/diff/api/DiffContentTypes.md)
Content types for the documents used in the diff process.
  [Difference](ro/sync/diff/api/Difference.md)
Represents a difference generated by the diff performer.
  [DifferenceParent](ro/sync/diff/api/DifferenceParent.md)
Represents a difference generated by the diff performer.
  [DifferencePerformer](ro/sync/diff/api/DifferencePerformer.md)
The [DifferencePerformer](ro/sync/diff/api/DifferencePerformer.md) is used to compare two resources of a given content type using a set of options.
  [DifferenceType](ro/sync/diff/api/DifferenceType.md)
Represents the type a [Difference](ro/sync/diff/api/Difference.md) can have.
  [DiffException](ro/sync/diff/api/DiffException.md)
Exception thrown by the diff performer when a problem is encountered and the operation fails or if the operation was stopped.
  [DiffMergeResult](ro/sync/exml/workspace/api/util/diff/DiffMergeResult.md)
The result of merging new content over an Author document using [CompareUtilAccess.mergeAuthorContent(ro.sync.ecss.extensions.api.AuthorAccess, java.lang.String, java.lang.String, ro.sync.exml.workspace.api.util.diff.TrackChangesMode)](ro/sync/exml/workspace/api/util/CompareUtilAccess.md#mergeAuthorContent(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.exml.workspace.api.util.diff.TrackChangesMode)).
  [DiffMergeResult.ResultType](ro/sync/exml/workspace/api/util/diff/DiffMergeResult.ResultType.md)
The type of the merge result.
  [DiffOptions](ro/sync/diff/api/DiffOptions.md)
Holds options needed to decide which diff algorithm and which diff options will be used.
  [DiffPerformerFactory](ro/sync/diff/api/DiffPerformerFactory.md)
Factory used to create a difference performer, used to compare two resources using different algorithms and options.
  [DiffProgressEvent](ro/sync/diff/api/DiffProgressEvent.md)
Event used by the [DiffProgressListener](ro/sync/diff/api/DiffProgressListener.md) to signal when the diff progress is incremented.
  [DiffProgressListener](ro/sync/diff/api/DiffProgressListener.md)
Listener to the diff performer.
  [Dimension](ro/sync/exml/view/graphics/Dimension.md)
Dimension.
  [DisplayModeConstants](ro/sync/exml/workspace/api/editor/page/author/DisplayModeConstants.md)
Constants for display modes of Author editor.
  [DITAAccess](ro/sync/ecss/dita/DITAAccess.md)
Utility methods for DITA interaction.
  [DITAAccess.InsertLinkReferenceShortcut](ro/sync/ecss/dita/DITAAccess.InsertLinkReferenceShortcut.md)
Short cut for the insert link operation.
  [DITAAccess.PasteInfo](ro/sync/ecss/dita/DITAAccess.PasteInfo.md)
Paste type of clipboard fragments.
  [DITAAuthorActionEventHandler](ro/sync/ecss/extensions/api/DITAAuthorActionEventHandler.md)
Author action event handler for DITA.
  [DITAAuthorImageDecorator](ro/sync/ecss/extensions/dita/DITAAuthorImageDecorator.md)
Handles a DITA vocabulary image map.
  [DITAAuthorTableOperationsHandler](ro/sync/ecss/extensions/dita/DITAAuthorTableOperationsHandler.md)
Author table operations handler for DITA framework.
  [DITACALSShowTablePropertiesOperation](ro/sync/ecss/extensions/dita/topic/table/cals/properties/DITACALSShowTablePropertiesOperation.md)
Class for dita CALS table properties action.
  [DITACALSTableCellInfoProvider](ro/sync/ecss/extensions/commons/table/support/DITACALSTableCellInfoProvider.md)
DITA CALS table cell info provider, should work with specializations.
  [DITACALSTableHelper](ro/sync/ecss/extensions/dita/topic/table/cals/properties/DITACALSTableHelper.md)
Helper class for edit properties on DITA CALS tables.
  [DITACALSTableSortOperation](ro/sync/ecss/extensions/dita/topic/table/DITACALSTableSortOperation.md)
DITA CALS table sort operation implementation.
  [DITAConfigureAutoIDElementsOperation](ro/sync/ecss/extensions/dita/id/DITAConfigureAutoIDElementsOperation.md)
Operation used to insert a Link in DITA documents.
  [DITAConRefResolver](ro/sync/ecss/extensions/dita/conref/DITAConRefResolver.md)
Resolver for content referred using conref attribute.
  [DITAConrefsResolverBase](ro/sync/ecss/extensions/api/DITAConrefsResolverBase.md)
Resolve references when showing DITA content in the editor
  [DITAConstants](ro/sync/ecss/dita/DITAConstants.md)
DITA constants.
  [DITACustomRuleMatcher](ro/sync/ecss/extensions/dita/DITACustomRuleMatcher.md)
DITA custom rule matcher abstract class.
  [DITAEditImageMapCore](ro/sync/ecss/extensions/dita/DITAEditImageMapCore.md)
Edit Image Map Core for DITA.
  [DITAElementLocator](ro/sync/ecss/extensions/dita/DITAElementLocator.md)
An implementation for a DITA element when the referred element is not a topic.
  [DITAElementLocatorProvider](ro/sync/ecss/extensions/dita/DITAElementLocatorProvider.md)
Implementation for locating elements based on a link from a DITA document.
  [DITAExtensionsBundle](ro/sync/ecss/extensions/dita/DITAExtensionsBundle.md)
The DITA framework extensions bundle.
  [DITAExternalObjectInsertionHandler](ro/sync/ecss/extensions/dita/DITAExternalObjectInsertionHandler.md)
Dropped URLs handler
  [DITAExternalObjectInsertionHandlerUtil](ro/sync/ecss/extensions/dita/DITAExternalObjectInsertionHandlerUtil.md)
Utility class for the DITA and DITA Map external object insertion handlers.
  [DITAFilteringContentHandler](ro/sync/ecss/extensions/dita/conref/DITAFilteringContentHandler.md)
Content and lexical handler used to filter parser events outside the given topic IDs path.
  [DITAIDElementLocator](ro/sync/ecss/extensions/dita/DITAIDElementLocator.md)
Implementation of an ElementLocator that locates elements based on a given link and checks if the attribute with the type ID matches the provided link and the class attribute contains 'topic/topic'.
  [DITAIDTypeRecognizer](ro/sync/ecss/extensions/dita/id/DITAIDTypeRecognizer.md)
Implementation of ID declarations and references recognizer for DITA framework.
  [DITAImposedReferenceType](ro/sync/ecss/dita/DITAImposedReferenceType.md)
Specifies how a reference should be inserted in a document: xref, figure, variable, etc
  [DITAInsertListOperation](ro/sync/ecss/extensions/dita/DITAInsertListOperation.md)
Insert List operation for DITA.
  [DITAKeyNameGenerator](ro/sync/ecss/dita/DITAKeyNameGenerator.md)
Used to generate key names based on file names.
  [DitaLinkTextResolver](ro/sync/ecss/extensions/dita/link/DitaLinkTextResolver.md)
Can resolve DITA references to another topic made through the href attribute on elements of classes: map/topicref , topic/xref and topic/link .
  [DITAListSortOperation](ro/sync/ecss/extensions/commons/sort/DITAListSortOperation.md)
DITA list sort operation implementation.
  [DITAMap2_xCustomRuleMatcher](ro/sync/ecss/extensions/dita/map/DITAMap2_xCustomRuleMatcher.md)
Matches a specific DITA Map 2.x framework
  [DITAMapActionsProvider](ro/sync/exml/workspace/api/editor/page/ditamap/actions/DITAMapActionsProvider.md)
Provides access to actions defined in the DITA Map editor page.
  [DITAMapAuthorTableOperationsHandler](ro/sync/ecss/extensions/dita/map/DITAMapAuthorTableOperationsHandler.md)
Author table operations handler for DITAMap framework.
  [DITAMapCustomRuleMatcher](ro/sync/ecss/extensions/dita/map/DITAMapCustomRuleMatcher.md)
DITA map custom rule matcher.
  [DITAMapDocumentModel](ro/sync/ecss/webapp/ditamap/DITAMapDocumentModel.md)
The editable DITA Map document model
  [DITAMapExtensionsBundle](ro/sync/ecss/extensions/dita/map/DITAMapExtensionsBundle.md)
DITA Map extensions bundle
  [DITAMapExternalObjectInsertionHandler](ro/sync/ecss/extensions/dita/map/DITAMapExternalObjectInsertionHandler.md)
Dropped URLs handler
  [DITAMapKeyDefElementLocator](ro/sync/ecss/extensions/dita/DITAMapKeyDefElementLocator.md)
An implementation for a DITA element searching for a key definition.
  [DITAMapModel](ro/sync/exml/workspace/api/editor/page/ditamap/model/DITAMapModel.md)
The DITA Map Model.
  [DITAMapNodeRendererCustomizer](ro/sync/exml/workspace/api/editor/page/ditamap/DITAMapNodeRendererCustomizer.md)
Node renderer customizer specific for the DITA Maps Manager.
  [DITAMapNodeRendererCustomizerContext](ro/sync/exml/workspace/api/editor/page/ditamap/DITAMapNodeRendererCustomizerContext.md)
Offers more information about the class of the target topics.
  [DITAMapPopupMenuCustomizer](ro/sync/exml/workspace/api/editor/page/ditamap/DITAMapPopupMenuCustomizer.md)
Can be used to customize a pop-up menu before showing it.
  [DITAMapReferencesResolver](ro/sync/ecss/extensions/api/DITAMapReferencesResolver.md)
Resolve references when showing a DITA Map in the editor
  [DITAMapRefResolver](ro/sync/ecss/extensions/dita/map/topicref/DITAMapRefResolver.md)
Resolves the hrefs to other maps.
  [DITAMapResolvedReferencesCustomRuleMatcher](ro/sync/ecss/extensions/dita/map/DITAMapResolvedReferencesCustomRuleMatcher.md)
Matches a specific DITA Map opened with resolved topics
  [DITAMapReviewController](ro/sync/exml/workspace/api/editor/page/ditamap/review/DITAMapReviewController.md)
The DITA Map Change tracking controller.
  [DITAMapSchemaAwareEditingHandler](ro/sync/ecss/extensions/dita/map/DITAMapSchemaAwareEditingHandler.md)
DITA Map Schema aware editing handler.
  [DITAMapTextPageExternalObjectInsertionHandler](ro/sync/ecss/extensions/dita/map/DITAMapTextPageExternalObjectInsertionHandler.md)
The DITA Map text page external object insertion handler.
  [DITAMapTopicTitlesResolveListener](ro/sync/ecss/extensions/dita/map/DITAMapTopicTitlesResolveListener.md)
Listener handling the 'showTopicTitles' editing context attribute.
  [DITAMapTreeComponentListener](ro/sync/ecss/extensions/api/component/listeners/DITAMapTreeComponentListener.md)
DITA Map tree component listener.
  [DITAMapTreeComponentProvider](ro/sync/ecss/extensions/api/component/ditamap/DITAMapTreeComponentProvider.md)
A component encapsulating editing a DITA Map in a DITA Maps Manager tree-like structure.
  [DITAMapTreeDropHandler](ro/sync/exml/workspace/api/editor/page/ditamap/dnd/DITAMapTreeDropHandler.md)
A handler which can be installed to override handling of drop events in the DITA Map Tree.
  [DITANodeRendererCustomizer](ro/sync/ecss/extensions/dita/DITANodeRendererCustomizer.md)
Class used to customize the way a DITA node is rendered in the UI.
  [DITANodeRendererCustomizer.DitaClass](ro/sync/ecss/extensions/dita/DITANodeRendererCustomizer.DitaClass.md)
DITA classes constants.
  [DitaReferenceTargetDescriptor](ro/sync/ecss/dita/DitaReferenceTargetDescriptor.md)
Descriptor for a conref target.
  [DITARelTableDocumentTypeHelper](ro/sync/ecss/extensions/dita/map/table/DITARelTableDocumentTypeHelper.md)
Implementation of the document type helper for DITA Map reltable model
  [DITASchemaAwareEditingHandler](ro/sync/ecss/extensions/dita/DITASchemaAwareEditingHandler.md)
Specific editing support for DITA documents.
  [DITASchemaManagerFilter](ro/sync/ecss/extensions/dita/DITASchemaManagerFilter.md)
Schema manager filter which provides the available keyref + condition values.
  [DITASimpleTableCellSpanProvider](ro/sync/ecss/extensions/commons/table/support/DITASimpleTableCellSpanProvider.md)
This class is responsible for providing information about the DITA simple table cell spanning.
  [DITASimpleTableDocumentTypeHelper](ro/sync/ecss/extensions/dita/topic/table/simpletable/DITASimpleTableDocumentTypeHelper.md)
Implementation of the document type helper for DITA simple table model
  [DITASimpleTableSortOperation](ro/sync/ecss/extensions/dita/topic/table/DITASimpleTableSortOperation.md)
DITA simple table sort operation implementation.
  [DITASpellCheckerHelper](ro/sync/ecss/extensions/dita/DITASpellCheckerHelper.md)
Helps identify inline elements which should be transparent to the spell checker
  [DITATableCellInfoProvider](ro/sync/ecss/extensions/commons/table/support/DITATableCellInfoProvider.md)
Provides information about the column width for DITA tables.
  [DITATableCellSepInfoProvider](ro/sync/ecss/extensions/commons/table/support/DITATableCellSepInfoProvider.md)
A DITA cell separators provider.
  [DITATableDocumentTypeHelper](ro/sync/ecss/extensions/dita/topic/table/DITATableDocumentTypeHelper.md)
Implementation of the document type helper for DITA CALS table model.
  [DITATextAccess](ro/sync/ecss/dita/DITATextAccess.md)
Access utility methods to work with DITA in the text editing mode.
  [DITATextPageExternalObjectInsertionHandler](ro/sync/ecss/extensions/dita/DITATextPageExternalObjectInsertionHandler.md)
The DITA text page external object insertion handler.
  [DITATopic2_xCustomRuleMatcher](ro/sync/ecss/extensions/dita/topic/DITATopic2_xCustomRuleMatcher.md)
Matches a specific DITA 2.x framework which provides support for the DITA 2.x standard.
  [DITATopicCustomRuleMatcher](ro/sync/ecss/extensions/dita/topic/DITATopicCustomRuleMatcher.md)
DITA topic custom rule matcher.
  [DITATopicInsertionPosition](ro/sync/ecss/dita/DITATopicInsertionPosition.md)
The position where to insert a topic, relative to the selection.
  [DITAUniqueAttributesRecognizer](ro/sync/ecss/extensions/dita/id/DITAUniqueAttributesRecognizer.md)
Unique attributes recognizer for DITA.
  [DITAUniqueAttributesRecognizerUtil](ro/sync/ecss/extensions/dita/id/DITAUniqueAttributesRecognizerUtil.md)
Utility class for Schema Aware actions.
  [DITAUpdateImageMapOperation](ro/sync/ecss/extensions/dita/DITAUpdateImageMapOperation.md)
DITA implementation of the operation that updates an image map with shape information from an SVG.
  [DITAUpdateImageMapOperation.DITANewShapeDescriptor](ro/sync/ecss/extensions/dita/DITAUpdateImageMapOperation.DITANewShapeDescriptor.md)
Descriptor of a shape that was added client-side.
  [DITAValExtensionsBundle](ro/sync/ecss/extensions/dita/DITAValExtensionsBundle.md)
The DITAVal extensions bundle
  [DITAValSchemaManagerFilter](ro/sync/ecss/extensions/dita/DITAValSchemaManagerFilter.md)
Schema manager filter which provides the available keyref + condition values.
  [DITAXMLReaderWrapper](ro/sync/ecss/extensions/dita/conref/DITAXMLReaderWrapper.md)
Delegating XML Reader used to parse DITA 'conref' references.
  [DITAXSLTExtensionFunctionUtil](ro/sync/ecss/dita/extensions/DITAXSLTExtensionFunctionUtil.md)
Utility methods used to access information about keys referenced in DITA topics.
  [Docbook4CALSShowTablePropertiesOperation](ro/sync/ecss/extensions/docbook/table/properties/Docbook4CALSShowTablePropertiesOperation.md)
Class for edit properties on DB4 CALS tables.
  [DocBook4ExtensionsBundle](ro/sync/ecss/extensions/docbook/DocBook4ExtensionsBundle.md)
The DocBook 4 framework extensions bundle.
  [Docbook4ExternalObjectInsertionHandler](ro/sync/ecss/extensions/docbook/Docbook4ExternalObjectInsertionHandler.md)
Dropped URLs handler
  [Docbook4HTMLShowTablePropertiesOperation](ro/sync/ecss/extensions/docbook/table/properties/Docbook4HTMLShowTablePropertiesOperation.md)
Class for edit properties on DB4 CALS tables.
  [Docbook4InsertMediaDataOperation](ro/sync/ecss/extensions/docbook/Docbook4InsertMediaDataOperation.md)
Operation used to insert an media object in DocBook 4 documents.
  [Docbook4PasteAsLinkOperation](ro/sync/ecss/extensions/docbook/Docbook4PasteAsLinkOperation.md)
Operation used to paste content as <link> in Docbook 4 documents.
  [Docbook4PasteAsXIncludeOperation](ro/sync/ecss/extensions/docbook/Docbook4PasteAsXIncludeOperation.md)
Operation used to paste content as reference in Docbook5 documents.
  [Docbook4PasteAsXrefOperation](ro/sync/ecss/extensions/docbook/Docbook4PasteAsXrefOperation.md)
Operation used to paste content as <xref> in Docbook 4 documents.
  [Docbook4UniqueAttributesRecognizer](ro/sync/ecss/extensions/docbook/id/Docbook4UniqueAttributesRecognizer.md)
Unique attributes recognizer for DocBook 4
  [Docbook5CALSShowTablePropertiesOperation](ro/sync/ecss/extensions/docbook/table/properties/Docbook5CALSShowTablePropertiesOperation.md)
Class for edit properties on DB5 CALS tables.
  [Docbook5CALSTableHelper](ro/sync/ecss/extensions/docbook/table/properties/Docbook5CALSTableHelper.md)
Docbook CALS table helper.
  [Docbook5ConfigureAutoIDElementsOperation](ro/sync/ecss/extensions/docbook/id/Docbook5ConfigureAutoIDElementsOperation.md)
Operation specific for Docbook 5
  [DocBook5ExtensionsBundle](ro/sync/ecss/extensions/docbook/DocBook5ExtensionsBundle.md)
The DocBook 5 framework extensions bundle.
  [Docbook5ExternalObjectInsertionHandler](ro/sync/ecss/extensions/docbook/Docbook5ExternalObjectInsertionHandler.md)
Dropped URLs handler
  [Docbook5HTMLShowTablePropertiesOperation](ro/sync/ecss/extensions/docbook/table/properties/Docbook5HTMLShowTablePropertiesOperation.md)
Class for edit properties on DB4 CALS tables.
  [Docbook5HTMLTableHelper](ro/sync/ecss/extensions/docbook/table/properties/Docbook5HTMLTableHelper.md)
Docbook CALS table helper.
  [Docbook5InsertMediaDataOperation](ro/sync/ecss/extensions/docbook/Docbook5InsertMediaDataOperation.md)
Operation used to insert an media object in DocBook 5 documents.
  [Docbook5PasteAsLinkOperation](ro/sync/ecss/extensions/docbook/Docbook5PasteAsLinkOperation.md)
Operation used to paste content as <link> in Docbook 5 documents.
  [Docbook5PasteAsXIncludeOperation](ro/sync/ecss/extensions/docbook/Docbook5PasteAsXIncludeOperation.md)
Operation used to paste content as reference in Docbook5 documents.
  [Docbook5PasteAsXrefOperation](ro/sync/ecss/extensions/docbook/Docbook5PasteAsXrefOperation.md)
Operation used to paste content as <xref> in Docbook 5 documents.
  [Docbook5SchemaAwareEditingHandler](ro/sync/ecss/extensions/docbook/Docbook5SchemaAwareEditingHandler.md)
Specific schema aware editing cases for Docbook5.
  [Docbook5UniqueAttributesRecognizer](ro/sync/ecss/extensions/docbook/id/Docbook5UniqueAttributesRecognizer.md)
Unique attributes recognizer for DocBook 5
  [DocbookAccess](ro/sync/ecss/docbook/DocbookAccess.md)
Docbook access.
  [DocbookAuthorActionEventHandler](ro/sync/ecss/extensions/api/DocbookAuthorActionEventHandler.md)
Author action event handler for DocBook.
  [DocbookAuthorImageDecorator](ro/sync/ecss/extensions/docbook/DocbookAuthorImageDecorator.md)
Handles a Docbook vocabulary image map.
  [DocbookAuthorTableOperationsHandler](ro/sync/ecss/extensions/docbook/DocbookAuthorTableOperationsHandler.md)
Author table operations handler for Docbook framework.
  [DocbookCALSTableHelper](ro/sync/ecss/extensions/docbook/table/properties/DocbookCALSTableHelper.md)
Docbook CALS table helper.
  [DocbookCALSTableSortOperation](ro/sync/ecss/extensions/docbook/table/DocbookCALSTableSortOperation.md)
The sort operation used for Docbook CALS tables.
  [DocbookConfigureAutoIDElementsOperation](ro/sync/ecss/extensions/docbook/id/DocbookConfigureAutoIDElementsOperation.md)
Operation used to insert a Link in Docbook documents.
  [DocbookEditImageMapCore](ro/sync/ecss/extensions/docbook/DocbookEditImageMapCore.md)
Edit image ma core for Docbook.
  [DocBookExtensionsBundleBase](ro/sync/ecss/extensions/docbook/DocBookExtensionsBundleBase.md)
The DocBook framework extensions bundle.
  [DocbookHTMLShowTablePropertiesOperationBase](ro/sync/ecss/extensions/docbook/table/properties/DocbookHTMLShowTablePropertiesOperationBase.md)
Base class for edit properties on DB4 tables.
  [DocbookHTMLTableHelper](ro/sync/ecss/extensions/docbook/table/properties/DocbookHTMLTableHelper.md)
Docbook CALS table helper.
  [DocbookInsertListOperation](ro/sync/ecss/extensions/docbook/DocbookInsertListOperation.md)
Docbook Insert List operation,
  [DocbookLinkTextResolver](ro/sync/ecss/extensions/docbook/link/DocbookLinkTextResolver.md)
Resolves local docbook xrefs.
  [DocbookListSortOperation](ro/sync/ecss/extensions/commons/sort/DocbookListSortOperation.md)
Class for Docbook 'Sort list' operation.
  [DocbookNodeRendererCustomizer](ro/sync/ecss/extensions/docbook/DocbookNodeRendererCustomizer.md)
Class used to customize the way an Docbook node is rendered in the UI.
  [DocbookSchemaAwareEditingHandler](ro/sync/ecss/extensions/docbook/DocbookSchemaAwareEditingHandler.md)
Specific editing support for Docbook documents.
  [DocbookSchemaManagerFilter](ro/sync/ecss/extensions/docbook/DocbookSchemaManagerFilter.md)
Schema manager filter which provides the available condition values.
  [DocbookTableCellSepInfoProvider](ro/sync/ecss/extensions/docbook/table/DocbookTableCellSepInfoProvider.md)
A DITA cell separators provider.
  [DocbookTableCustomizerConstants](ro/sync/ecss/extensions/docbook/table/DocbookTableCustomizerConstants.md)
Constants used to choose Docbook table attributes.
  [DocBookUniqueAttributesRecognizer](ro/sync/ecss/extensions/docbook/id/DocBookUniqueAttributesRecognizer.md)
Unique attributes recognizer for DocBook.
  [DocumentContentChangedEvent](ro/sync/ecss/extensions/api/DocumentContentChangedEvent.md)
Event received by an [AuthorListener](ro/sync/ecss/extensions/api/AuthorListener.md) when changes have been made in the content of the [AuthorDocument](ro/sync/ecss/extensions/api/node/AuthorDocument.md).
  [DocumentContentDeletedEvent](ro/sync/ecss/extensions/api/DocumentContentDeletedEvent.md)
Event received by an [AuthorListener](ro/sync/ecss/extensions/api/AuthorListener.md) when a deletion has been made in the content of the [AuthorDocument](ro/sync/ecss/extensions/api/node/AuthorDocument.md).
  [DocumentContentInsertedEvent](ro/sync/ecss/extensions/api/DocumentContentInsertedEvent.md)
Event received by an [AuthorListener](ro/sync/ecss/extensions/api/AuthorListener.md) when insertion have been made in the content of the [AuthorDocument](ro/sync/ecss/extensions/api/node/AuthorDocument.md).
  [DocumentModelReferenceCollector](ro/sync/ecss/extensions/api/webapp/references/DocumentModelReferenceCollector.md)
Instances of this class are used to collect the references to external resources (images, audio, video, XInclude, etc.) from an AuthorDocumentModelTo be used when the document has been already parsed and its structure is already known See URLCollectingReader for collecting references from a document specified by a URL
  [DocumentPluginContext](ro/sync/exml/plugin/document/DocumentPluginContext.md)
Plugin context interface.
  [DocumentPluginExtension](ro/sync/exml/plugin/document/DocumentPluginExtension.md)
Plugin extension.
  [DocumentPluginResult](ro/sync/exml/plugin/document/DocumentPluginResult.md)
Plugin result interface.
  [DocumentPluginResultImpl](ro/sync/exml/plugin/document/DocumentPluginResultImpl.md)

 [DocumentPositionedInfo](ro/sync/document/DocumentPositionedInfo.md)
This class holds information related to the document, refering to some errors, or find results.
  [DocumentTypeAdvancedCustomRuleMatcher](ro/sync/ecss/extensions/api/DocumentTypeAdvancedCustomRuleMatcher.md)
Abstract class which can be implemented to provide custom matching to the document type it belongs to.
  [DocumentTypeCustomRuleMatcher](ro/sync/ecss/extensions/api/DocumentTypeCustomRuleMatcher.md)
Interface which can be implemented to provide custom matching to the document type it belongs to.
  [DocumentTypeInfo](ro/sync/ecss/extensions/api/webapp/doctype/DocumentTypeInfo.md)
Information about a document type.
  [DocumentTypeInfoParser](ro/sync/ecss/extensions/api/webapp/doctype/DocumentTypeInfoParser.md)
Can parse framework files in memory.
  [DocumentTypeInfoRepository](ro/sync/ecss/extensions/api/webapp/doctype/DocumentTypeInfoRepository.md)
Class used to retrieve information about the registered document types.
  [DocumentTypeInformation](ro/sync/exml/workspace/api/editor/documenttype/DocumentTypeInformation.md)
Provides information about the document type configuration which was loaded for the current editor ('Document Type Association' preferences page).
  [DOTProjectAuthorReferenceResolver](ro/sync/ecss/extensions/dita/DOTProjectAuthorReferenceResolver.md)
Author Reference Resolver for DITA-OT Project files.
  [DOTProjectExtensionsBundle](ro/sync/ecss/extensions/dita/DOTProjectExtensionsBundle.md)
Extensions bundle for a DITA OT Project.
  [DPILocation](ro/sync/ecss/extensions/api/webapp/DPILocation.md)
DPI location information.
  [DynamicPropertyEvaluator](ro/sync/ecss/extensions/api/editor/DynamicPropertyEvaluator.md)
Some form control properties can't be evaluated at the time the CSS is compiled.
  [ECCustomTableColumnInsertionDialog](ro/sync/ecss/extensions/commons/table/operations/ECCustomTableColumnInsertionDialog.md)
Dialog displayed when trying to insert multiple columns (using "Insert Columns...").
  [ECCustomTableRowInsertionDialog](ro/sync/ecss/extensions/commons/table/operations/ECCustomTableRowInsertionDialog.md)
Dialog displayed when trying to insert multiple rows (using "Insert Rows...").
  [ECDITARelTableCustomizer](ro/sync/ecss/extensions/dita/map/table/ECDITARelTableCustomizer.md)
Customize a DITA map reltable.
  [ECDITARelTableCustomizerDialog](ro/sync/ecss/extensions/dita/map/table/ECDITARelTableCustomizerDialog.md)
Dialog used to customize DITA table creation.
  [ECDITATableCustomizer](ro/sync/ecss/extensions/dita/topic/table/ECDITATableCustomizer.md)
Customize a DITA table.
  [ECDITATableCustomizerDialog](ro/sync/ecss/extensions/dita/topic/table/ECDITATableCustomizerDialog.md)
Dialog used to customize DITA table creation.
  [ECDocbookInnerTableCustomizer](ro/sync/ecss/extensions/docbook/table/ECDocbookInnerTableCustomizer.md)
Customize a Docbook table.
  [ECDocbookTableCustomizer](ro/sync/ecss/extensions/docbook/table/ECDocbookTableCustomizer.md)
Customize a Docbook table.
  [ECDocbookTableCustomizerDialog](ro/sync/ecss/extensions/docbook/table/ECDocbookTableCustomizerDialog.md)
Dialog used to customize DocBook table creation.
  [ECIDElementsCustomizer](ro/sync/ecss/extensions/commons/id/ECIDElementsCustomizer.md)
Customize the list of elements for auto ID generation.
  [ECIDElementsCustomizerDialog](ro/sync/ecss/extensions/commons/id/ECIDElementsCustomizerDialog.md)
Dialog used to customize DITA elements which have auto ID generation.
  [ECImageMapAccess](com/oxygenxml/editor/imagemap/ECImageMapAccess.md)
Eclipse Image Map Access.
  [EclipseActionWrapper](com/oxygenxml/editor/editors/EclipseActionWrapper.md)
Provides access to an Eclipse action wrapped in a swing action.
  [EclipsePluginWorkspace](com/oxygenxml/workspace/api/eclipse/EclipsePluginWorkspace.md)
The Eclipse **Plugin Workspace** offers access utility methods or to access (and add listeners for) all opened editors from the Main editing area or from the DITA Maps editing area.
  [EclipseWorkspaceAccessPluginExtension](com/oxygenxml/workspace/api/eclipse/EclipseWorkspaceAccessPluginExtension.md)
Workspace Access plugin extension for Eclipse.
  [ECPropertiesComposite](ro/sync/ecss/extensions/commons/table/properties/ECPropertiesComposite.md)
Composite corresponding to a tab information.
  [ECPropertyComposite](ro/sync/ecss/extensions/commons/table/properties/ECPropertyComposite.md)
The composite used to edit a table property.
  [ECSortCustomizerDialog](ro/sync/ecss/extensions/commons/sort/ECSortCustomizerDialog.md)
Eclipse implementation of the customizer used to select the criterion information used when sorting.
  [ECTableColumnInsertionCustomizerInvoker](ro/sync/ecss/extensions/commons/table/operations/ECTableColumnInsertionCustomizerInvoker.md)
Customize table columns at insertion.
  [ECTableCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/ECTableCustomizerDialog.md)
Dialog used to customize the insertion of a generic table (number of rows, columns, table caption).
  [ECTablePropertiesCustomizerDialog](ro/sync/ecss/extensions/commons/table/properties/ECTablePropertiesCustomizerDialog.md)
Dialog that allows the user to edit the table properties.
  [ECTableRowInsertionCustomizerInvoker](ro/sync/ecss/extensions/commons/table/operations/ECTableRowInsertionCustomizerInvoker.md)
Customize table rows at insertion.
  [ECTableSplitCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/ECTableSplitCustomizerDialog.md)
Dialog that allows the user to choose the information necessary for the Split operation.
  [ECTEIFigureEntityAttributeCustomizer](ro/sync/ecss/extensions/tei/ECTEIFigureEntityAttributeCustomizer.md)
Customize the value of the attribute for a TEI figure.
  [ECTEITableCustomizer](ro/sync/ecss/extensions/tei/table/ECTEITableCustomizer.md)
Customize a TEI table.
  [ECTEITableCustomizerDialog](ro/sync/ecss/extensions/tei/table/ECTEITableCustomizerDialog.md)
The dialog used to customize a TEI table.
  [ECXHTMLTableCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/xhtml/ECXHTMLTableCustomizerDialog.md)
Dialog used to customize XHTML table creation.
  [ECXHTMLTableCustomizerInvoker](ro/sync/ecss/extensions/commons/table/operations/xhtml/ECXHTMLTableCustomizerInvoker.md)
Customize a XHTML table for Eclipse application.
  [EditedAttribute](ro/sync/ecss/extensions/api/EditedAttribute.md)
Edited attribute information, like QName, element's QName and the proxy namespace mapping.
  [EditedTablePropertiesInfo](ro/sync/ecss/extensions/commons/table/properties/EditedTablePropertiesInfo.md)

 [EditedTablePropertiesInfo.TAB_TYPE](ro/sync/ecss/extensions/commons/table/properties/EditedTablePropertiesInfo.TAB_TYPE.md)
Enumeration that contains the elements for every tab type.
  [EditImageHandler](ro/sync/exml/workspace/api/images/handlers/EditImageHandler.md)
Special handler for editing images which are either embedded or referenced.
  [EditImageMapCore](ro/sync/ecss/extensions/commons/imagemap/EditImageMapCore.md)
Core methods to be used from the operations and from the image map decorators.
  [EditImageMapOperation](ro/sync/ecss/extensions/commons/operations/EditImageMapOperation.md)
Operation used to edit an ImageMap in some documents.
  [EditImageMapOperation](ro/sync/ecss/extensions/dita/EditImageMapOperation.md)
Operation used to edit an ImageMap in DITA documents.
  [EditImageMapOperation](ro/sync/ecss/extensions/docbook/EditImageMapOperation.md)
Operation used to edit an ImageMap in Docbook documents.
  [EditImageMapOperation](ro/sync/ecss/extensions/tei/EditImageMapOperation.md)
Operation used to edit an ImageMap in TEI documents.
  [EditImageMapOperation](ro/sync/ecss/extensions/xhtml/imagemap/EditImageMapOperation.md)
Operation used to edit an ImageMap in Docbook documents.
  [EditImageMapWithSurroundCore](ro/sync/ecss/extensions/commons/imagemap/EditImageMapWithSurroundCore.md)
Core for the frameworks that need to surround the "image" in an "image map".
  [EditingEvent](ro/sync/ecss/extensions/api/editor/EditingEvent.md)
The in-place editing was stopped.
  [EditingSessionContext](ro/sync/ecss/extensions/api/access/EditingSessionContext.md)
The editing session context.
  [EditingSessionOpenVetoException](ro/sync/ecss/extensions/api/webapp/access/EditingSessionOpenVetoException.md)
Exception to be thrown when the plugin decides that the editing session should not be started.
  [EditOLinkOperation](ro/sync/ecss/extensions/docbook/olink/EditOLinkOperation.md)
Edit OLink operation.
  [EditorAdapterContributor](com/oxygenxml/editor/editors/EditorAdapterContributor.md)
Abstract class allowed as an extension point to contribute an adapter to the XML editor.
  [EditorComponentProvider](ro/sync/ecss/extensions/api/component/EditorComponentProvider.md)
Provides access to a created editor + helper views and additional panels.
  [EditorContent](ro/sync/ecss/css/EditorContent.md)
The content correspondent to an oxy_editor function.
  [EditorPageConstants](ro/sync/exml/editor/EditorPageConstants.md)
Define editor page IDs.
  [EditorTemplate](ro/sync/exml/editor/EditorTemplate.md)
Used to create a new editor for a given extension.
  [EditorTemplateWithContent](ro/sync/template/EditorTemplateWithContent.md)
Editor template with predefined string content.
  [EditorVariableDescription](ro/sync/exml/workspace/api/util/EditorVariableDescription.md)
An editor variable's description (name and short desc).
  [EditorVariables](ro/sync/util/editorvars/EditorVariables.md)
Holds constants representing all editor variables defined in Oxygen.
  [EditorVariables.FrameworkRewritePolicy](ro/sync/util/editorvars/EditorVariables.FrameworkRewritePolicy.md)
Used to determine how framework variables should be expanded/rewritten.
  [EditorVariables.FunctionResolver](ro/sync/util/editorvars/EditorVariables.FunctionResolver.md)
Resolves a function
  [EditorVariablesBase](ro/sync/util/editorvars/EditorVariablesBase.md)
Base for EditorVariables.
  [EditorVariablesConstants](ro/sync/util/editorvars/EditorVariablesConstants.md)
All the editor variables constants under one roof
  [EditorVariablesResolver](ro/sync/exml/workspace/api/util/EditorVariablesResolver.md)
Such a resolver can be registered via the "ro.sync.exml.workspace.api.util.UtilAccess" API and is called to resolve custom editor variables in a string.
  [EditPropertiesHandler](ro/sync/ecss/extensions/api/EditPropertiesHandler.md)
A custom implementation to handle editing properties for an author node.
  [EditPropertiesHandlerAdapter](ro/sync/ecss/extensions/api/EditPropertiesHandlerAdapter.md)
Adapter class.
  [EditPropertiesOperation](ro/sync/ecss/extensions/dita/map/EditPropertiesOperation.md)
Operation used to edit the properties of a topic reference.
  [ElementLocator](ro/sync/ecss/extensions/api/link/ElementLocator.md)
Base class for custom elements locators used to locate an element based on a link.
  [ElementLocatorException](ro/sync/ecss/extensions/api/link/ElementLocatorException.md)
Exception thrown when an element locator fails.
  [ElementLocatorProvider](ro/sync/ecss/extensions/api/link/ElementLocatorProvider.md)
This class is able to provide an implementation of an [ElementLocator](ro/sync/ecss/extensions/api/link/ElementLocator.md) based on the structure of a link.
  [Ellipse](ro/sync/exml/view/graphics/Ellipse.md)
The class describes an ellipse that is defined by a bounding rectangle.
  [EmbeddedImageContentProvider](ro/sync/exml/workspace/api/images/handlers/providers/EmbeddedImageContentProvider.md)
Provides access to the XML image contents...
  [EntityUrlResolver](ro/sync/exml/workspace/api/util/EntityUrlResolver.md)
Extended interface to be implemented by an EntityResolver to receive a special callback when Oxygen is not interested in the content of the entity but just in its URL.
  [EnumerationDefInfo](ro/sync/exml/workspace/api/editor/page/ditamap/keys/EnumerationDefInfo.md)
An enumeration def info.
  [ErrorHandler](ro/sync/exml/workspace/api/references/ErrorHandler.md)
ErrorHandler is an interface that the ReferenceCollectorimplementation can call when reporting errors that happens while collecting the references
  [ErrorMessageEditor](ro/sync/ecss/component/editor/ErrorMessageEditor.md)
If there are errors obtaining the editor we will use this editor just to present the error.
  [ErrorResolverContextInfo](ro/sync/ecss/extensions/api/ErrorResolverContextInfo.md)
Class that contains some information about the current error.
  [ExecuteCommandLineOperation](ro/sync/ecss/extensions/commons/operations/ExecuteCommandLineOperation.md)
Author operation allowing the execution of command lines.
  [ExecuteCustomizableTransformationScenarioOperation](ro/sync/ecss/extensions/commons/operations/ExecuteCustomizableTransformationScenarioOperation.md)
An implementation of an operation which runs a single transformation scenario.
  [ExecuteMultipleActionsOperation](ro/sync/ecss/extensions/commons/operations/ExecuteMultipleActionsOperation.md)
An implementation of an operation which runs a sequence of actions, defined as a list of IDs.
  [ExecuteMultipleActionsWithExtraAskValuesOperation](ro/sync/ecss/extensions/ExecuteMultipleActionsWithExtraAskValuesOperation.md)
Interface defining an author extension operation taht executes multiple actions and receive a list with expanded ask variables values, when invoked
  [ExecuteMultipleWebappCompatibleActionsOperation](ro/sync/ecss/extensions/commons/operations/ExecuteMultipleWebappCompatibleActionsOperation.md)
An implementation of an operation which runs a sequence of webapp-compatible ([WebappCompatible](ro/sync/ecss/extensions/api/WebappCompatible.md)) actions, defined as a list of IDs.
  [ExecuteTransformationScenariosOperation](ro/sync/ecss/extensions/commons/operations/ExecuteTransformationScenariosOperation.md)
An implementation of an operation which runs a certain transformation scenario.
  [ExecuteValidationScenariosOperation](ro/sync/ecss/extensions/commons/operations/ExecuteValidationScenariosOperation.md)
An implementation of an operation which runs validation scenarios.
  [ExpandableTopicrefCounter](ro/sync/ecss/dita/topic/ref/ExpandableTopicrefCounter.md)
Class that counts the number of expandable topic references.
  [ExportProgressUpdater](ro/sync/ecss/dita/mapeditor/actions/export/helper/ExportProgressUpdater.md)
Interface used to update the progress component.
  [Extension](ro/sync/ecss/extensions/api/Extension.md)
The base interface for all Oxygen extensions classes.
  [ExtensionsBundle](ro/sync/ecss/extensions/api/ExtensionsBundle.md)
Abstract class representing a bundle for all extensions handlers.
  [ExtensionsBundleContributor](com/oxygenxml/editor/editors/ExtensionsBundleContributor.md)
Provider for an extensions bundle based certain parameters.
  [ExtensionTags](ro/sync/ecss/extensions/commons/ExtensionTags.md)
The collection of the extension messages.
  [ExtensionUtil](ro/sync/ecss/extensions/api/link/ExtensionUtil.md)
Utility methods.
  [ExternalAIFunction](ro/sync/exml/plugin/ai/ExternalAIFunction.md)
Interface representing a function used by the AI to interact with the application.
  [ExternalContentCompletionProvider](ro/sync/exml/workspace/api/editor/page/text/ExternalContentCompletionProvider.md)
An external content completion provider.
  [ExternalEntityNameValue](ro/sync/contentcompletion/xml/ExternalEntityNameValue.md)
A pair class with name and value.
  [ExternalObjectInsertionSources](ro/sync/ecss/extensions/api/ExternalObjectInsertionSources.md)
Drop and paste sources
  [ExternalPersistentObject](ro/sync/exml/workspace/api/options/ExternalPersistentObject.md)
Marker interface for persistent objects which are implemented in plugins.
  [ExternalServiceException](ro/sync/exml/plugin/ai/ExternalServiceException.md)
Exception thrown when an error occurs while interacting with an external service.
  [FeatureFlags](ro/sync/ecss/webapp/FeatureFlags.md)
Feature flag names used in web author.
  [FileBrowsingConnection](ro/sync/net/protocol/FileBrowsingConnection.md)
Interface implemented by an URLConnection class that supports file browsing.
  [FileCannotBeOpenedInReviewerException](ro/sync/exml/editor/FileCannotBeOpenedInReviewerException.md)
Exception thrown when a document cannot be opened in Author Reviewer edition.
  [FileProber](ro/sync/ecss/extensions/dita/map/topicref/util/FileProber.md)
Class that checks if a file exists.
  [FileProber.Status](ro/sync/ecss/extensions/dita/map/topicref/util/FileProber.Status.md)
The status of the file.
  [FilterURLConnection](ro/sync/ecss/extensions/api/webapp/plugin/FilterURLConnection.md)
URLConnection that delegates all methods to the connection given as a parameter.
  [FindReplaceSupport](ro/sync/ecss/extensions/api/webapp/findreplace/FindReplaceSupport.md)
Support object for the Find/Replace related actions.
  [FindSimilarTopicsOperation](ro/sync/ecss/extensions/dita/FindSimilarTopicsOperation.md)
Operation used for finding possible similar topics using the "Open/Find resource" feature.
  [FolderEntryDescriptor](ro/sync/net/protocol/FolderEntryDescriptor.md)
Descriptor for a folder entry.
  [Font](ro/sync/exml/view/graphics/Font.md)
Font common class.
  [FontMetrics](ro/sync/exml/view/graphics/FontMetrics.md)
Common font metrics
  [FormControlEditingHelper](ro/sync/ecss/extensions/api/webapp/formcontrols/FormControlEditingHelper.md)
Helper class for editing using form controls.
  [FormSelectedTextOperation](ro/sync/ecss/extensions/commons/operations/text/FormSelectedTextOperation.md)
The class provides form word and form sentence operations over a selected text.
  [GeneralPluginContext](ro/sync/exml/plugin/general/GeneralPluginContext.md)
Plugin context interface.
  [GeneralPluginExtension](ro/sync/exml/plugin/general/GeneralPluginExtension.md)
Plugin interface.
  [GeneralStylesFilterExtension](ro/sync/exml/plugin/author/css/filter/GeneralStylesFilterExtension.md)
CSS properties filter plugin extension.
  [GenerateIDElementsInfo](ro/sync/ecss/extensions/commons/id/GenerateIDElementsInfo.md)
Information about the list of elements for which to generate auto ID + if the auto ID generation is activated
  [GenerateIDsDB4Operation](ro/sync/ecss/extensions/docbook/id/GenerateIDsDB4Operation.md)
Operation to auto generate IDs on the selected content.
  [GenerateIDsDB5Operation](ro/sync/ecss/extensions/docbook/id/GenerateIDsDB5Operation.md)
Operation to auto generate IDs on the selected content.
  [GenerateIDsDITAOperation](ro/sync/ecss/extensions/dita/id/GenerateIDsDITAOperation.md)
Operation to auto generate IDs on the selected content.
  [GenerateIDsOperation](ro/sync/ecss/extensions/commons/id/GenerateIDsOperation.md)
Operation used to auto generate IDs for the elements included in the selected fragment.
  [GenerateIDsTEIP5Operation](ro/sync/ecss/extensions/tei/id/GenerateIDsTEIP5Operation.md)
Operation to auto generate IDs on the selected content.
  [GenericEditorComponentProvider](ro/sync/ecss/extensions/api/component/GenericEditorComponentProvider.md)
A component encapsulating all the editing part.
  [GetCurrentElementSaxonExtension](ro/sync/ecss/extensions/commons/operations/GetCurrentElementSaxonExtension.md)
Returns the current element for an XSLT operation.
  [GhostTextProvider](ro/sync/document/GhostTextProvider.md)
Interface for providing ghost text suggestions in the editor.
  [GhostTextSuggestion](ro/sync/document/GhostTextSuggestion.md)
Represents a ghost text suggestion with its content and metadata.
  [GlobalOptionsStorage](ro/sync/exml/workspace/api/options/GlobalOptionsStorage.md)
This interface should be used to access global application options.
  [Graphics](ro/sync/exml/view/graphics/Graphics.md)
The graphics interface used to draw Author and Schema Diagram.
  [GroupChangesForMultiplePeersStrategy](ro/sync/ecss/extensions/api/webapp/ce/GroupChangesForMultiplePeersStrategy.md)
Details required when saving a concurrently edited document.
  [GroupChangesForSinglePeerStrategy](ro/sync/ecss/extensions/api/webapp/ce/GroupChangesForSinglePeerStrategy.md)
Details required when saving a concurrently edited document.
  [GuiElements](ro/sync/ecss/extensions/commons/table/properties/GuiElements.md)
Impose the GUI elements that will be used to present the values for a specific table property.
  [HelpPageProvider](ro/sync/ui/application/HelpPageProvider.md)
Provides the help page ID.
  [Highlight](ro/sync/ecss/extensions/api/highlights/Highlight.md)
The highlight interface.
  [HighlightActionsProvider](ro/sync/ecss/extensions/api/highlights/HighlightActionsProvider.md)
Provider for the actions available for a highlight.
  [HighlightActionsRenderingStyle](ro/sync/ecss/extensions/api/highlights/HighlightActionsRenderingStyle.md)
The rendering style of the actions associated with a highlight.
  [HighlightPainter](ro/sync/ecss/extensions/api/highlights/HighlightPainter.md)
Highlight renderer.
  [HighlightPainterInfo](ro/sync/ecss/extensions/api/highlights/HighlightPainterInfo.md)
Information needed by the painter.
  [HrefInfo](ro/sync/ecss/dita/HrefInfo.md)
Contains the referenced URL + information whether this is a map or a topic
  [HTML5CustomRuleMatcher](ro/sync/ecss/extensions/html/HTML5CustomRuleMatcher.md)
Check if the document is an HTML5 document.
  [HTMLClasses](ro/sync/ecss/extensions/api/webapp/HTMLClasses.md)
HTML classes used to identify the role of HTML elements.
  [HtmlContentEditor](ro/sync/ecss/component/editor/HtmlContentEditor.md)
Editor used to render HTML content.
  [HTMLTableCellInfoProvider](ro/sync/ecss/extensions/commons/table/support/HTMLTableCellInfoProvider.md)
Provides information regarding HTML table cell span and column width.
  [HTMLTableCellSpanProvider](ro/sync/ecss/extensions/commons/table/spansupport/HTMLTableCellSpanProvider.md)
Empty implementation for backward compatibility.
  [HttpExceptionWithDetails](ro/sync/net/protocol/http/HttpExceptionWithDetails.md)
HTTP Exception with details.
  [HttpServletRequest](ro/sync/ecss/extensions/api/webapp/plugin/servlet/http/HttpServletRequest.md)
HTTP Request interface inspired from HTTP Servlet 5.0.
  [HttpServletResponse](ro/sync/ecss/extensions/api/webapp/plugin/servlet/http/HttpServletResponse.md)
Response interface inspired from HTTP Servlet 5.0.
  [HttpSession](ro/sync/ecss/extensions/api/webapp/plugin/servlet/http/HttpSession.md)
HttpSession interface inspired from HTTP Servlet 5.0.
  [IAuthorDocumentPositionedInfo](ro/sync/ecss/component/validation/IAuthorDocumentPositionedInfo.md)
Interface defining the Author Mode document positioned info: allows you to specify the problem AuthorNode.
  [IAuthorExtensionAction](ro/sync/ecss/extensions/api/editor/IAuthorExtensionAction.md)
An author action created over an author operation.
  [IComponentInfo](ro/sync/exml/workspace/api/componentscollector/IComponentInfo.md)
Component information interface.
  [IComponentsProvider](ro/sync/exml/workspace/api/componentscollector/IComponentsProvider.md)
The components provider interface.
  [IDElementLocator](ro/sync/ecss/extensions/commons/IDElementLocator.md)
Implementation of an ElementLocator that locates elements based on a given link and checks if the attribute with the type ID matches the provided link.
  [IDropDownMenuAction](com/oxygenxml/editor/editors/IDropDownMenuAction.md)
Adds the possibility to add a drop down menu customizer.
  [IDropDownMenuCustomizer](com/oxygenxml/editor/editors/IDropDownMenuCustomizer.md)
Customize a drop down menu shown on an action.
  [IDropDownToolItem](com/oxygenxml/editor/editors/xml/IDropDownToolItem.md)
Access to the drop down tool item, allows configuring the set of available actions.
  [IDTypeIdentifier](ro/sync/ecss/extensions/api/link/IDTypeIdentifier.md)
Identifier for an ID declaration or reference.
  [IDTypeRecognizer](ro/sync/ecss/extensions/api/link/IDTypeRecognizer.md)
Recognizer for ID declaration and references in attribute values.
  [IDTypeVerifier](ro/sync/ecss/extensions/api/link/IDTypeVerifier.md)
Interface used to check if an attribute has the ID type.
  [IExternalContentCompletionContext](ro/sync/exml/workspace/api/editor/page/text/IExternalContentCompletionContext.md)
Contains context information about the position where the content completion is invoked.

[IImageMapWrapper](ro/sync/ecss/imagemap/IImageMapWrapper.md)<[E](ro/sync/ecss/imagemap/IImageMapWrapper.md) extends ro.sync.ecss.imagemap.IImageMap>

Marker interface for the Image Map Wraper.
  [ImageContentProvider](ro/sync/exml/workspace/api/images/handlers/providers/ImageContentProvider.md)
Provides access to the image contents...
  [ImageFileChooser](ro/sync/ecss/extensions/commons/ImageFileChooser.md)
Choose an image file.
  [ImageHandler](ro/sync/exml/workspace/api/images/handlers/ImageHandler.md)
Base class for all the image handlers.
  [ImageHolder](ro/sync/exml/workspace/api/util/ImageHolder.md)
An image holder that can be written to an OutputStream and contains additional information about the image.
  [ImageInverter](ro/sync/exml/workspace/api/util/ImageInverter.md)
Inverts certain images based on color theme.
  [ImageLayoutInformation](ro/sync/exml/workspace/api/images/handlers/ImageLayoutInformation.md)
Information about an image's dimensions and baseline.
  [ImageMapExtractor](ro/sync/ecss/extensions/api/webapp/references/ImageMapExtractor.md)
Returns an optional Reference with type Type.STATIC_CONTENT and the URL of the image map.
  [ImageMapFactory](ro/sync/ecss/imagemap/ImageMapFactory.md)
Factory for image map implementations.
  [ImageMapFormatException](ro/sync/ecss/extensions/api/webapp/imagemap/ImageMapFormatException.md)
Exception thrown when an image map cannot be parsed from an XML element.
  [ImageMapNotSuportedException](ro/sync/ecss/imagemap/ImageMapNotSuportedException.md)
Image map not supported exception.
  [ImageMapUtil](ro/sync/ecss/imagemap/ImageMapUtil.md)
Image Map Utilities.
  [ImageRenderingContext](ro/sync/exml/workspace/api/images/handlers/ImageRenderingContext.md)
Contains information about the context in which the image will be rendered..
  [ImageUtilities](ro/sync/exml/workspace/api/images/ImageUtilities.md)
Utilities related to registering image handlers...
  [ImageUtilitiesSpecificProvider](ro/sync/exml/workspace/api/images/ImageUtilitiesSpecificProvider.md)
Platform specific image utilities provider.
  [INamespaceInfo](ro/sync/exml/workspace/api/componentscollector/INamespaceInfo.md)
Namespace information interface.
  [IndexedReusableComponent](ro/sync/exml/workspace/api/standalone/project/IndexedReusableComponent.md)
Represents information about an indexed reusable component
  [InlineProposal](ro/sync/contentcompletion/editor/InlineProposal.md)
Inline proposal presented in InlineProposalsWindow.
  [InplaceEditingListener](ro/sync/ecss/extensions/api/editor/InplaceEditingListener.md)
Gets notified about edit events: [InplaceEditingListener.editingStopped(EditingEvent)](ro/sync/ecss/extensions/api/editor/InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) - a request to stop the editing and commit the value from the editor.
  [InplaceEditingTraversalListener](ro/sync/ecss/extensions/api/editor/InplaceEditingTraversalListener.md)
Gets notified about focus traversal keys TAB and SHIFT-TAB.
  [InplaceEditor](ro/sync/ecss/extensions/api/editor/InplaceEditor.md)
An author in-place editor.
  [InplaceEditorAdapter](ro/sync/ecss/extensions/api/editor/InplaceEditorAdapter.md)
Convenience implementation of the [InplaceEditor](ro/sync/ecss/extensions/api/editor/InplaceEditor.md).
  [InplaceEditorArgumentKeys](ro/sync/ecss/extensions/api/editor/InplaceEditorArgumentKeys.md)
Properties of the oxy_editor function extended with other computed properties that the renderer/editor might need.
  [InplaceEditorCSSConstants](ro/sync/ecss/extensions/api/editor/InplaceEditorCSSConstants.md)
Arguments of the oxy_editor function as well as built-in values for some of these arguments.
  [InplaceEditorRendererAdapter](ro/sync/ecss/extensions/api/editor/InplaceEditorRendererAdapter.md)
Convenience implementation of the [InplaceRenderer](ro/sync/ecss/extensions/api/editor/InplaceRenderer.md) and [InplaceEditor](ro/sync/ecss/extensions/api/editor/InplaceEditor.md).
  [InplaceEditorUtil](ro/sync/ecss/extensions/commons/editor/InplaceEditorUtil.md)
Utility methods for preparing the in-place editors for being displayed.
  [InplaceHeavyEditor](ro/sync/ecss/extensions/api/editor/InplaceHeavyEditor.md)
A form control that appears inside the author page.
  [InplaceRenderer](ro/sync/ecss/extensions/api/editor/InplaceRenderer.md)
An author in-place renderer.
  [InplaceRendererAdapter](ro/sync/ecss/extensions/api/editor/InplaceRendererAdapter.md)
Convenience implementation of the [InplaceRenderer](ro/sync/ecss/extensions/api/editor/InplaceRenderer.md).
  [InputURLChooser](ro/sync/exml/workspace/api/standalone/InputURLChooser.md)
Interface through which the CMS can set a custom URL to any Input URL Panel from Oxygen.
  [InputURLChooserCustomizer](ro/sync/exml/workspace/api/standalone/InputURLChooserCustomizer.md)
Customize the actions which appear in any Input URL chooser from Oxygen.
  [InputUrlComponentChangeListener](ro/sync/exml/workspace/api/standalone/ui/urlpanel/InputUrlComponentChangeListener.md)
Notifies changes in [InputUrlComponentProvider](ro/sync/exml/workspace/api/standalone/ui/urlpanel/InputUrlComponentProvider.md) components.
  [InputUrlComponentProvider](ro/sync/exml/workspace/api/standalone/ui/urlpanel/InputUrlComponentProvider.md)
Gives access to an URL chooser component similar to the ones in the application.
  [InputURLEditor](ro/sync/ecss/component/editor/InputURLEditor.md)
In-place editor used to select an URL.
  [InsertColumnOperation](ro/sync/ecss/extensions/commons/table/operations/cals/InsertColumnOperation.md)
Operation used to insert one or more CALS table columns.
  [InsertColumnOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/InsertColumnOperation.md)
Operation used to insert one or more XHTML table columns.
  [InsertColumnOperation](ro/sync/ecss/extensions/dita/map/table/InsertColumnOperation.md)
Operation used to insert a DITA map reltable column.
  [InsertColumnOperation](ro/sync/ecss/extensions/dita/topic/table/cals/InsertColumnOperation.md)
Operation used to insert one or more DITA table columns.
  [InsertColumnOperation](ro/sync/ecss/extensions/dita/topic/table/simpletable/InsertColumnOperation.md)
Operation used to insert one or more DITA simple table columns.
  [InsertColumnOperation](ro/sync/ecss/extensions/tei/table/InsertColumnOperation.md)
Operation used to insert a TEI table column.
  [InsertColumnOperationBase](ro/sync/ecss/extensions/commons/table/operations/InsertColumnOperationBase.md)
Operation used to insert a table column.
  [InsertConrefOperation](ro/sync/ecss/extensions/dita/conref/InsertConrefOperation.md)
Operation used to insert a conref in DITA documents.
  [InsertContentKeyrefOperation](ro/sync/ecss/extensions/dita/keyref/InsertContentKeyrefOperation.md)
Operation used to insert a conkeyref in DITA documents.
  [InsertEquationOperation](ro/sync/ecss/extensions/commons/operations/InsertEquationOperation.md)
Operation used to insert an MathML Equation in any documents.
  [InsertEquationOperation](ro/sync/ecss/extensions/docbook/InsertEquationOperation.md)
Operation used to insert an equation in Docbook documents.
  [InsertEquationOperation](ro/sync/ecss/extensions/xhtml/InsertEquationOperation.md)
Operation used to insert an MathML Equation in XHTML 1.1 documents.
  [InsertExternalLinkOperation](ro/sync/ecss/extensions/docbook/link/InsertExternalLinkOperation.md)
Insert Web Link (link).
  [InsertFragmentOperation](ro/sync/ecss/extensions/commons/operations/InsertFragmentOperation.md)
An implementation of an insert operation for an argument of type fragment.
  [InsertGraphicOperation](ro/sync/ecss/extensions/docbook/InsertGraphicOperation.md)
Operation used to insert a Docbook graphic.
  [InsertGUIButtonOperation](ro/sync/ecss/extensions/docbook/InsertGUIButtonOperation.md)
Operation used to insert a Docbook guibutton with the child elements inlinemediaobject, imageobject and imagedata.
  [InsertImageDataOperation](ro/sync/ecss/extensions/docbook/InsertImageDataOperation.md)
Operation used to insert an image in Docbook 5 documents.
  [InsertImageOperation](ro/sync/ecss/extensions/dita/topic/InsertImageOperation.md)
Operation used to insert an image in DITA documents.
  [InsertImageOperationP4](ro/sync/ecss/extensions/tei/InsertImageOperationP4.md)
Operation used to insert a TEI P4 graphic.
  [InsertImageOperationP5](ro/sync/ecss/extensions/tei/InsertImageOperationP5.md)
Operation used to insert a TEI P5 graphic.
  [InsertImgOperation](ro/sync/ecss/extensions/xhtml/InsertImgOperation.md)
Operation used to insert a XHTML graphic.
  [InsertKeydefWithKeywordOperation](ro/sync/ecss/extensions/dita/InsertKeydefWithKeywordOperation.md)
Operation used to insert a key with keyword in DITA Map documents.
  [InsertKeyrefOperation](ro/sync/ecss/extensions/dita/keyref/InsertKeyrefOperation.md)
Operation used to insert a keyref in DITA documents.
  [InsertLinkOperation](ro/sync/ecss/extensions/dita/link/InsertLinkOperation.md)
Operation used to insert a Link in DITA documents.
  [InsertLinkUtil](ro/sync/ecss/extensions/docbook/link/InsertLinkUtil.md)
Utility class for insert web link.
  [InsertListOperation](ro/sync/ecss/extensions/commons/operations/InsertListOperation.md)
Operation used to convert a selection to an ordered/unordered list.
  [InsertLocalLinkOperation](ro/sync/ecss/extensions/docbook/link/InsertLocalLinkOperation.md)
Insert local link.
  [InsertMediaDataOperationBase](ro/sync/ecss/extensions/docbook/InsertMediaDataOperationBase.md)
Operation used to insert an media object in DocBook documents.
  [InsertMediaOperation](ro/sync/ecss/extensions/dita/topic/InsertMediaOperation.md)
Operation used to insert a media object in DITA documents.
  [InsertMediaOperation](ro/sync/ecss/extensions/xhtml/InsertMediaOperation.md)
Operation used to insert a XHTML media.
  [InsertNewTopicOperation](ro/sync/ecss/extensions/dita/map/topicref/InsertNewTopicOperation.md)
Operation used to create a new topic and insert a reference to it.
  [InsertOLinkOperation](ro/sync/ecss/extensions/docbook/olink/InsertOLinkOperation.md)
Insert OLink.
  [InsertOrReplaceFragmentOperation](ro/sync/ecss/extensions/commons/operations/InsertOrReplaceFragmentOperation.md)
Identical with [InsertFragmentOperation](ro/sync/ecss/extensions/commons/operations/InsertFragmentOperation.md) with the difference that the selection will be removed.
  [InsertOrReplaceTextOperation](ro/sync/ecss/extensions/commons/operations/InsertOrReplaceTextOperation.md)
An implementation of an insert/replace operation for an argument of type [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html).
  [InsertReusableComponentOperation](ro/sync/ecss/extensions/dita/reuse/InsertReusableComponentOperation.md)
Operation used to insert a conref in DITA documents.
  [InsertRowOperation](ro/sync/ecss/extensions/commons/table/operations/cals/InsertRowOperation.md)
Operation used to insert a table row for DocBook v.4 or v.5 and for DITA CALS tables..
  [InsertRowOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/InsertRowOperation.md)
Operation used to insert a table row for XHTML documents.
  [InsertRowOperation](ro/sync/ecss/extensions/dita/map/table/InsertRowOperation.md)
Operation used to insert a reltable row for DITA.
  [InsertRowOperation](ro/sync/ecss/extensions/dita/topic/table/cals/InsertRowOperation.md)
Operation used to insert a table row for DITA.
  [InsertRowOperation](ro/sync/ecss/extensions/dita/topic/table/simpletable/InsertRowOperation.md)
Operation used to insert a simple table row for DITA.
  [InsertRowOperation](ro/sync/ecss/extensions/tei/table/InsertRowOperation.md)
Operation used to insert a table row for TEI documents.
  [InsertRowOperationBase](ro/sync/ecss/extensions/commons/table/operations/InsertRowOperationBase.md)
Abstract class for operation used to insert a table row.
  [InsertScreenshotOperation](ro/sync/ecss/extensions/docbook/InsertScreenshotOperation.md)
Operation used to insert a Docbook graphic.
  [InsertSingleColumnOperation](ro/sync/ecss/extensions/commons/table/operations/cals/InsertSingleColumnOperation.md)
Operation used to insert one or more CALS table columns.
  [InsertSingleColumnOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/InsertSingleColumnOperation.md)
Operation used to insert one or more XHTML table columns.
  [InsertSingleColumnOperation](ro/sync/ecss/extensions/dita/map/table/InsertSingleColumnOperation.md)
Operation used to insert a DITA map reltable column.
  [InsertSingleColumnOperation](ro/sync/ecss/extensions/dita/topic/table/cals/InsertSingleColumnOperation.md)
Operation used to insert one or more DITA table columns.
  [InsertSingleColumnOperation](ro/sync/ecss/extensions/dita/topic/table/simpletable/InsertSingleColumnOperation.md)
Operation used to insert one or more DITA simple table columns.
  [InsertSingleColumnOperation](ro/sync/ecss/extensions/tei/table/InsertSingleColumnOperation.md)
Operation used to insert a TEI table column.
  [InsertSingleRowOperation](ro/sync/ecss/extensions/commons/table/operations/cals/InsertSingleRowOperation.md)
Operation used to insert a table row for DocBook v.4 or v.5 and for DITA CALS tables..
  [InsertSingleRowOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/InsertSingleRowOperation.md)
Operation used to insert a table row for XHTML documents.
  [InsertSingleRowOperation](ro/sync/ecss/extensions/dita/map/table/InsertSingleRowOperation.md)
Operation used to insert a reltable row for DITA.
  [InsertSingleRowOperation](ro/sync/ecss/extensions/dita/topic/table/cals/InsertSingleRowOperation.md)
Operation used to insert a table row for DITA tables..
  [InsertSingleRowOperation](ro/sync/ecss/extensions/dita/topic/table/simpletable/InsertSingleRowOperation.md)
Operation used to insert a single simple table row for DITA.
  [InsertSingleRowOperation](ro/sync/ecss/extensions/tei/table/InsertSingleRowOperation.md)
Operation used to insert a single table row for TEI documents.
  [InsertTableCellsContentConstants](ro/sync/ecss/extensions/commons/table/operations/InsertTableCellsContentConstants.md)
Interface holding constants used in operations that insert content in table cells.
  [InsertTableOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/InsertTableOperation.md)
Operation used to insert a XHTML table.
  [InsertTableOperation](ro/sync/ecss/extensions/dita/map/table/InsertTableOperation.md)
Operation used to insert a DITA map reltable.
  [InsertTableOperation](ro/sync/ecss/extensions/dita/topic/table/InsertTableOperation.md)
Operation used to insert a DITA table.
  [InsertTableOperation](ro/sync/ecss/extensions/docbook/table/InsertTableOperation.md)
Operation used to insert a CALS Docbook table or an HTML table in a DocBook document.
  [InsertTableOperation](ro/sync/ecss/extensions/tei/table/InsertTableOperation.md)
The operation used to insert a TEI table.
  [InsertTableOperationBase](ro/sync/ecss/extensions/commons/table/operations/InsertTableOperationBase.md)
Base for insert Author table operation.
  [InsertTopicgroupOperation](ro/sync/ecss/extensions/dita/map/topicgroup/InsertTopicgroupOperation.md)
Operation used to insert a topic group in DITA documents.
  [InsertTopicheadOperation](ro/sync/ecss/extensions/dita/map/topichead/InsertTopicheadOperation.md)
Operation used to insert a topic heading in DITA documents.
  [InsertTopicrefOperation](ro/sync/ecss/extensions/dita/map/topicref/InsertTopicrefOperation.md)
Operation used to insert a topic reference in DITA documents.
  [InsertULink](ro/sync/ecss/extensions/docbook/link/InsertULink.md)
Insert Web Link (ulink).
  [InsertXIncludeOperation](ro/sync/ecss/extensions/commons/operations/InsertXIncludeOperation.md)
Insert an XInclude.
  [InsertXrefOperation](ro/sync/ecss/extensions/dita/link/InsertXrefOperation.md)
Operation used to insert an XRef in DITA documents.
  [InsertXrefOperation](ro/sync/ecss/extensions/docbook/link/InsertXrefOperation.md)
Inserts a xref element.
  [InvalidEditException](ro/sync/ecss/extensions/api/InvalidEditException.md)
Exception thrown by [AuthorSchemaAwareEditingHandler](ro/sync/ecss/extensions/api/AuthorSchemaAwareEditingHandler.md) methods when an edit is considered invalid and must be rejected.
  [InvalidLinkException](ro/sync/ecss/extensions/api/link/InvalidLinkException.md)
Signals a link that cannot be resolved.
  [InvalidPersistentObjException](ro/sync/options/InvalidPersistentObjException.md)
Thrown when we try to deserialize a persistent object.
  [InvokeAIActionOperation](ro/sync/ecss/extensions/commons/operations/InvokeAIActionOperation.md)
Author operation which invokes an AI action by ID.

[IQuickAssistInvocationContext](ro/sync/exml/editor/quickassist/IQuickAssistInvocationContext.md)<[P](ro/sync/exml/editor/quickassist/IQuickAssistInvocationContext.md)>

Platform independent(Eclipse vs SA) invocation context for the quick assists.
  [IQuickAssistProcessor](ro/sync/exml/editor/quickassist/IQuickAssistProcessor.md)
Quick assist processor for quick fixes and quick assists.

[IQuickAssistProposal](ro/sync/exml/editor/quickassist/IQuickAssistProposal.md)<[I](ro/sync/exml/editor/quickassist/IQuickAssistProposal.md)>

The interface of completion proposals generated by content assist processors.
  [IQuickFix](ro/sync/quickfix/IQuickFix.md)
The interface describing a quick fix.
  [IQuickFixableValidationProblem](ro/sync/exml/validate/IQuickFixableValidationProblem.md)
Interface defining a validation problem that would be quick fixable.
  [ItemNotFoundException](ro/sync/ecss/extensions/api/webapp/cc/ItemNotFoundException.md)
An exception thrown when the content completion item chosen by the user was not one of the proposed ones in the specified context.
  [IWebappAuthorEditorAccess](ro/sync/ecss/extensions/api/webapp/access/IWebappAuthorEditorAccess.md)
Extended [AuthorEditorAccess](ro/sync/ecss/extensions/api/access/AuthorEditorAccess.md) interface for Web Author.
  [IXSLComponentInfo](ro/sync/exml/workspace/api/componentscollector/IXSLComponentInfo.md)
XSL Component information interface.
  [JoinCellAboveBelowOperation](ro/sync/ecss/extensions/commons/table/operations/cals/JoinCellAboveBelowOperation.md)
Operation for joining the content of two cells from adjacent rows on the same column, CALS tables implementation.
  [JoinCellAboveBelowOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/JoinCellAboveBelowOperation.md)
Operation for joining the content of two cells on the same column from adjacent rows, XHTML tables implementation.
  [JoinCellAboveBelowOperation](ro/sync/ecss/extensions/dita/map/table/JoinCellAboveBelowOperation.md)
Operation for joining the content of two cells on the same column, from adjacent rows, DITA reltable implementation.
  [JoinCellAboveBelowOperation](ro/sync/ecss/extensions/dita/topic/table/cals/JoinCellAboveBelowOperation.md)
Operation for joining the content of two cells from adjacent rows on the same column, DITA CALS tables implementation.
  [JoinCellAboveBelowOperation](ro/sync/ecss/extensions/dita/topic/table/simpletable/JoinCellAboveBelowOperation.md)
Operation for joining the content of two cells from adjacent rows, DITA simpletable implementation.
  [JoinCellAboveBelowOperation](ro/sync/ecss/extensions/tei/table/JoinCellAboveBelowOperation.md)
Operation used to join the content of two cells from the same column, from adjacent rows, TEI tables implementation.
  [JoinCellAboveBelowOperationBase](ro/sync/ecss/extensions/commons/table/operations/JoinCellAboveBelowOperationBase.md)
Operation for joining the content of two cells in the same column, from adjacent rows.
  [JoinOperation](ro/sync/ecss/extensions/commons/table/operations/cals/JoinOperation.md)
Operation for joining the content of selected cells.
  [JoinOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/JoinOperation.md)
Operation for joining the content of selected cells.
  [JoinOperation](ro/sync/ecss/extensions/dita/topic/table/cals/JoinOperation.md)
Operation for joining the content of selected cells.
  [JoinOperation](ro/sync/ecss/extensions/tei/table/JoinOperation.md)
Operation for joining the content of selected cells.
  [JoinOperationBase](ro/sync/ecss/extensions/commons/table/operations/JoinOperationBase.md)
Operation for joining the content of selected cells.
  [JoinRowCellsOperation](ro/sync/ecss/extensions/commons/table/operations/cals/JoinRowCellsOperation.md)
This is the CALS tables implementation of the operation used to join the content of two or more cells from the same table row.
  [JoinRowCellsOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/JoinRowCellsOperation.md)
This is the HTML tables implementation of the operation used to join the content of two or more cells from the same table row.
  [JoinRowCellsOperation](ro/sync/ecss/extensions/dita/map/table/JoinRowCellsOperation.md)
This is the DITA tables implementation of the operation used to join the content of two or more cells from the same table row.
  [JoinRowCellsOperation](ro/sync/ecss/extensions/dita/topic/table/cals/JoinRowCellsOperation.md)
This is the DITA CALS tables implementation of the operation used to join the content of two or more cells from the same table row.
  [JoinRowCellsOperation](ro/sync/ecss/extensions/dita/topic/table/simpletable/JoinRowCellsOperation.md)
This is the DITA simple tables implementation of the operation used to join the content of two or more cells from a table row.
  [JoinRowCellsOperation](ro/sync/ecss/extensions/tei/table/JoinRowCellsOperation.md)
This is the TEI tables implementation of the operation used to join the content of two or more cells from the same table row.
  [JoinRowCellsOperationBase](ro/sync/ecss/extensions/commons/table/operations/JoinRowCellsOperationBase.md)
Operation used to join the content of two or more cells from a table row.
  [JSONAndYAMLPropertiesRuleMatcherBase](ro/sync/json/JSONAndYAMLPropertiesRuleMatcherBase.md)
Matcher for schemas that have no versions, but have required properties.
  [JSONAndYAMLRuleMatcherBase](ro/sync/json/JSONAndYAMLRuleMatcherBase.md)
OpenAPI base matcher.
  [JSONNodeRendererCustomizer](ro/sync/ecss/extensions/json/JSONNodeRendererCustomizer.md)
Class used to customize the way an JSON node is rendered in the UI.
  [JSOperation](ro/sync/ecss/extensions/commons/operations/JSOperation.md)
An implementation of an operation that allows you to call the Java API from custom JavaScript content.
  [KeyDefinitionInfo](ro/sync/exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionInfo.md)
Information about a key definition.
  [KeyDefinitionManager](ro/sync/exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManager.md)
Provides information about all key definitions which are a context for all opened topics.
  [KeyDefinitionManagerProvider](ro/sync/exml/workspace/api/editor/page/ditamap/keys/KeyDefinitionManagerProvider.md)
Provides the keys manager for an opened document.
  [KeysController](ro/sync/ecss/extensions/commons/sort/KeysController.md)
Used for handling with a change of the keys selection.
  [KeysManagerBase](ro/sync/ecss/dita/KeysManagerBase.md)
Common keys manager methods
  [LabelContent](ro/sync/ecss/css/LabelContent.md)
The content correspondent to an oxy_label function.
  [LabelCSSConstants](ro/sync/ecss/css/functions/LabelCSSConstants.md)
Processed arguments of the oxy_label function.

[LazyValue](ro/sync/ecss/extensions/api/editor/LazyValue.md)<[T](ro/sync/ecss/extensions/api/editor/LazyValue.md)>

This class enables one to give a form control property that isn't constructed until the first time it's looked up with AuthorInplaceContext#getArguments().get(key) method.
  [LicenseEnforcerFilter](ro/sync/ecss/extensions/api/webapp/license/LicenseEnforcerFilter.md)
A servlet filter that MUST be used to license the WebApp.
  [LinkTextResolver](ro/sync/ecss/extensions/api/link/LinkTextResolver.md)
Resolves a link and obtains a text representation.
  [LinkTextResolverCustomizer](com/oxygenxml/editor/editors/dita/LinkTextResolverCustomizer.md)
Abstract class allowed as an extension point to customize the resolution of the text which appears on DITA xrefs.
  [ListContentProvider](ro/sync/ecss/extensions/commons/table/operations/ListContentProvider.md)
Empty implementation for the general purpose list (Collection) content provider.
  [LocalFileBrowseType](ro/sync/exml/workspace/api/standalone/ui/urlpanel/LocalFileBrowseType.md)
Allowed browse types for [InputUrlComponentProvider](ro/sync/exml/workspace/api/standalone/ui/urlpanel/InputUrlComponentProvider.md) choosers.
  [LockException](ro/sync/exml/plugin/lock/LockException.md)
Thrown when could not lock or unlock properly
  [LockHandler](ro/sync/exml/plugin/lock/LockHandler.md)
Manage locking and unlocking.
  [LockHandlerBase](ro/sync/exml/plugin/lock/LockHandlerBase.md)
Base for classes used for managing locking and unlocking.
  [LockHandlerFactoryPluginExtension](ro/sync/exml/plugin/urlstreamhandler/LockHandlerFactoryPluginExtension.md)
Extension used for locking resources from a specific protocol
  [LockHandlerWithContext](ro/sync/ecss/extensions/api/webapp/plugin/LockHandlerWithContext.md)
A base-class to be extended to implement lock/unlock functionality.
  [LWDITAExtensionsBundle](ro/sync/ecss/extensions/dita/LWDITAExtensionsBundle.md)
The Lightweight DITA framework extensions bundle.
  [MainFrameComponentsConstants](ro/sync/exml/MainFrameComponentsConstants.md)
Provides the components that enter the MainFrame; They are puzzled together by the MainFrameLayoutManager.
  [MarkdownValidator](ro/sync/exml/workspace/api/markdown/MarkdownValidator.md)
Implementations of this interface are used to validate markdown documents.
  [MarkdownValidatorFactory](ro/sync/exml/workspace/api/markdown/MarkdownValidatorFactory.md)
Factory class for creating MarkdownValidator objects.
  [MathFlowConfigurator](ro/sync/exml/workspace/api/math/MathFlowConfigurator.md)
Provide access to MathFlow specific methods.
  [MediaFileChooser](ro/sync/ecss/extensions/commons/MediaFileChooser.md)
Choose an media file.
  [MediaObjectsUtil](ro/sync/ecss/extensions/commons/MediaObjectsUtil.md)
Utility methods for media objects.
  [Menu](ro/sync/exml/workspace/api/standalone/ui/Menu.md)
A menu which looks like the ones in Oxygen.
  [MenuBarCustomizer](ro/sync/exml/workspace/api/standalone/MenuBarCustomizer.md)
Customizes components from the main menu bar.
  [MenusAndToolbarsContributorCustomizer](ro/sync/exml/workspace/api/standalone/actions/MenusAndToolbarsContributorCustomizer.md)
Abstract class allowed as an extension point to customize the menu and toolbar buttons added by our editors.
  [MergeConflictResolutionMethods](ro/sync/merge/MergeConflictResolutionMethods.md)
Possible methods of dealing with conflicts when auto-merging files.
  [MergedFileState](ro/sync/diff/merge/api/MergedFileState.md)
The state of a merged file contains information about the file location and the merge status (deleted, added, modified).
  [MergedFileState.MergeStatus](ro/sync/diff/merge/api/MergedFileState.MergeStatus.md)
The merge state
  [MergeFilesException](ro/sync/diff/merge/api/MergeFilesException.md)
An exception thrown when merge files fails.
  [MergeFilesOptionsConstants](ro/sync/diff/merge/api/MergeFilesOptionsConstants.md)
Constants used as keys in the **mergeOptions** map parameter from [DiffAndMergeTools.openMergeApplication(java.io.File, java.io.File, java.io.File, java.util.Map)](ro/sync/exml/workspace/api/standalone/DiffAndMergeTools.md#openMergeApplication(java.io.File,java.io.File,java.io.File,java.util.Map))
  [MergeFilesOptionsConstants.FilterModeValues](ro/sync/diff/merge/api/MergeFilesOptionsConstants.FilterModeValues.md)
The values for filter mode option.
  [MergeResult](ro/sync/merge/MergeResult.md)
Defines the result of a three way merge.
  [MergeResult.ResultType](ro/sync/merge/MergeResult.ResultType.md)
The way a merge has finalized.
  [MetaContentProvider](ro/sync/exml/workspace/api/editor/page/ditamap/keys/MetaContentProvider.md)
According to the: http://docs.oasis-open.org/dita/v1.2/os/spec/archSpec/processing_key_references.html and: http://dita.xml.org/resource/dita-tc-faq-about-keys#Q2 if a node of a certain type makes a keyref to a topic ref on which <topicmeta> is defined, the content of the key will be extracted from that particular <topicmeta>.
  [ModifiedStatusProvider](ro/sync/exml/workspace/api/base/ModifiedStatusProvider.md)
Provides access to the modified status of an object.
  [MoveBlockAuthorOperation](ro/sync/ecss/extensions/commons/operations/MoveBlockAuthorOperation.md)
Operation capable of moving the block element from the caret or the selected block elements by one position up or down.
  [MoveCaretOperation](ro/sync/ecss/extensions/commons/operations/MoveCaretOperation.md)
Author operation capable of moving the caret relative to an XML node identified by an XPath expression.
  [MoveCaretUtil](ro/sync/ecss/extensions/commons/operations/MoveCaretUtil.md)
Utility to detect an editor variable in the Author page and move the caret to that place.
  [MoveElementOperation](ro/sync/ecss/extensions/commons/operations/MoveElementOperation.md)
Flexible operation for moving an element to another location.
  [MoveRenameResult](ro/sync/exml/workspace/api/standalone/project/MoveRenameResult.md)
Result of a move rename operation
  [NamespaceContext](ro/sync/ecss/extensions/api/node/NamespaceContext.md)
Useful interface which can be used to obtain mappings from prefix to namespace and from namespace to prefix in the context of the current element.
  [NameValue](ro/sync/contentcompletion/xml/NameValue.md)
A pair class with name and value.
  [NewShapeDescriptor](ro/sync/ecss/extensions/commons/imagemap/operations/NewShapeDescriptor.md)
Descriptor for new shapes that were received from the JavaScript-base image map editor in Web Author.
  [NewWebappAreaView](ro/sync/ecss/extensions/api/webapp/imagemap/NewWebappAreaView.md)
Descriptor for a new area coming from the client-side editor.
  [NodeContext](ro/sync/exml/workspace/api/node/NodeContext.md)
Provide information like node name, node namespace, attributes (if available), that will be used for Author outline, Author bread crumb, Text page outline, content completion proposals window or DITA Map view rendering customization.
  [NodeDescription](ro/sync/contentcompletion/xml/NodeDescription.md)
Node description is in fact a collection of properties for a node.
  [NodeRendererCustomizerContext](ro/sync/exml/workspace/api/node/customizer/NodeRendererCustomizerContext.md)
Provide information like node name, node namespace, attributes (if available), that will be used for Author outline, Author bread crumb, Text page outline, content completion proposals window or DITA Map view rendering customization.
  [ObjectChooser](ro/sync/ecss/extensions/commons/ObjectChooser.md)
Base class for choosers dialogs.
  [OffsetInformation](ro/sync/ecss/extensions/api/content/OffsetInformation.md)
Information about the node which contains the offset.
  [OKCancelDialog](ro/sync/ecss/extensions/commons/ui/OKCancelDialog.md)
Dialog with OK and Cancel buttons.
  [OKCancelDialog](ro/sync/exml/workspace/api/standalone/ui/OKCancelDialog.md)
Dialog with OK and Cancel buttons.
  [OLinkInfo](ro/sync/ecss/docbook/olink/OLinkInfo.md)
OLink information.
  [OpenInSystemAppOperation](ro/sync/ecss/extensions/commons/operations/OpenInSystemAppOperation.md)
Detects the application that is associated with the given file in the OS and uses it to open the file.
  [OpenRedirectExtension](ro/sync/exml/plugin/openredirect/OpenRedirectExtension.md)
Plugin extension - open redirecting for URLs
  [OpenRedirectInformation](ro/sync/exml/plugin/openredirect/OpenRedirectInformation.md)
Information about redirecting an URL
  [OpenURLHandler](ro/sync/ecss/extensions/api/component/listeners/OpenURLHandler.md)
Listener for URLs the user is trying to open from the Author Component.
  [OperationInProgressException](ro/sync/exml/workspace/api/editor/validation/OperationInProgressException.md)
Indicates that the validation is impossible at this time.
  [OperationStatus](ro/sync/exml/workspace/api/OperationStatus.md)
The status of an operation/action.
  [OptionChangedEvent](ro/sync/ecss/extensions/api/OptionChangedEvent.md)
Represents an event which indicates that the value of an option has been changed.
  [OptionListener](ro/sync/ecss/extensions/api/OptionListener.md)
The listener which is notified about the value changes of an author extension level option.
  [OptionPagePluginExtension](ro/sync/exml/plugin/option/OptionPagePluginExtension.md)
Class used to create plugin option page extension.
  [OptionsPageGroupPluginExtension](ro/sync/exml/plugin/OptionsPageGroupPluginExtension.md)
Plugin extension for option pages group.
  [OptionsStorage](ro/sync/ecss/extensions/api/OptionsStorage.md)
This interface should be used if Author extension level options need to be stored and retrieved.
  [OxygenEclipseUIComponentsFactory](com/oxygenxml/workspace/api/eclipse/OxygenEclipseUIComponentsFactory.md)
Eclipse UI components factory.
  [OxygenUIComponentsFactory](ro/sync/exml/workspace/api/standalone/ui/OxygenUIComponentsFactory.md)
Create UI components that look and feel like the ones in oXygen.
  [OxygenURLStreamHandlerFactory](ro/sync/net/protocol/OxygenURLStreamHandlerFactory.md)
The URLStreamHandlerFactory that handles all the protocols supported by Oxygen.
  [ParserCreator](ro/sync/xml/parser/ParserCreator.md)
Creates all the parsers from the system.
  [Part](ro/sync/ecss/extensions/api/webapp/plugin/servlet/http/Part.md)
Part interface inspired from HTTP Servlet 5.0.
  [PasteAsContentKeyReferenceOperation](ro/sync/ecss/extensions/dita/conref/PasteAsContentKeyReferenceOperation.md)
Operation used to insert paste as a content key reference in DITA documents.
  [PasteAsContentReferenceOperation](ro/sync/ecss/extensions/dita/conref/PasteAsContentReferenceOperation.md)
Operation used to insert paste as a content reference in DITA documents.
  [PasteAsLinkKeyReferenceOperation](ro/sync/ecss/extensions/dita/keyref/PasteAsLinkKeyReferenceOperation.md)
Operation used to insert paste as a key reference in DITA documents.
  [PasteAsReferenceException](ro/sync/ecss/extensions/commons/PasteAsReferenceException.md)
Exception for when pasting as reference doesn't work properly.
  [PasteAsReferenceOperation](ro/sync/ecss/extensions/dita/link/PasteAsReferenceOperation.md)
Operation used to insert paste as a Link in DITA documents.
  [PeerContext](ro/sync/ecss/extensions/api/webapp/ce/PeerContext.md)
Context information about a document model that is part of a [Room](ro/sync/ecss/extensions/api/webapp/ce/Room.md).
  [PersistentHighlightRenderer](ro/sync/ecss/extensions/api/highlights/PersistentHighlightRenderer.md)
Customize the way that the author persistent highlights are displayed.
  [PersistentObject](ro/sync/options/PersistentObject.md)
Defines an object that can be stored in the options.
  [Platform](ro/sync/exml/workspace/api/Platform.md)
Represents the type of the oXygen platform.
  [Plugin](ro/sync/exml/plugin/Plugin.md)
Plugin main class class.
  [PluginConfigExtension](ro/sync/ecss/extensions/api/webapp/plugin/PluginConfigExtension.md)
Deprecated.
This API is deprecated because it's based on javax package that's no more supported starting with Servlet 5.0 specification and because this extension type isn't protected against CSRF attacks.

 [PluginContext](ro/sync/exml/plugin/PluginContext.md)
Annotation for plugin extension fields that should be populated from plugin context.
  [PluginDescriptor](ro/sync/exml/plugin/PluginDescriptor.md)
Descriptor of the plugin.
  [PluginDescriptor.PluginExtensionDescription](ro/sync/exml/plugin/PluginDescriptor.PluginExtensionDescription.md)
Contains a plugin description + plugin type + keyboard shortcuts
  [PluginExtension](ro/sync/exml/plugin/PluginExtension.md)
Any plugin extension must implement this interface.
  [PluginResourceBundle](ro/sync/exml/workspace/api/PluginResourceBundle.md)
Bundle used to translate specific messages in the language set in the editor's preferences.
  [PluginWorkspace](ro/sync/exml/workspace/api/PluginWorkspace.md)
Access the entire workspace of Oxygen.
  [PluginWorkspaceProvider](ro/sync/exml/workspace/api/PluginWorkspaceProvider.md)
Provides static access to the workspace API of the Oxygen editor.
  [PluginWorkspaceTCBase](ro/sync/exml/workspace/api/PluginWorkspaceTCBase.md)
Base class for testing plugins and frameworks.
  [Point](ro/sync/exml/view/graphics/Point.md)
A point with X and Y coordinates..
  [Polygon](ro/sync/exml/view/graphics/Polygon.md)
The Polygon class encapsulates a description of a closed, two-dimensional region within a coordinate space.
  [PopupCheckBoxEditor](ro/sync/ecss/component/editor/PopupCheckBoxEditor.md)
A panel with checkboxes that can be used to render boolean values but also lists of values.
  [PopupCheckBoxRenderer](ro/sync/ecss/component/editor/PopupCheckBoxRenderer.md)
Presents a simple or a composed value (multiple values separated by a separator) using a JLabel.
  [PopupListEditor](ro/sync/ecss/component/editor/PopupListEditor.md)
A panel that can be used to render lists of values.
  [PopupMenu](ro/sync/exml/workspace/api/standalone/ui/PopupMenu.md)
A popup menu which looks like the ones in Oxygen.
  [PopupMenuCustomizer](ro/sync/ecss/extensions/api/component/PopupMenuCustomizer.md)
Can be used to customize a JPopupMenu before showing it.
  [PrettyPrintException](ro/sync/exml/workspace/api/util/PrettyPrintException.md)
Exception thrown when an error occurs while pretty printing an XML document.
  [PrioritizableHighlightPainter](ro/sync/ecss/extensions/api/highlights/PrioritizableHighlightPainter.md)
A highlight painter that can be prioritized, by telling it to paint all its highlight on a specific layer.
  [PrioritizableHighlightPainter.ZLayer](ro/sync/ecss/extensions/api/highlights/PrioritizableHighlightPainter.ZLayer.md)
Layers where a painter can paint its highlights.
  [ProcessController](ro/sync/exml/workspace/api/process/ProcessController.md)
The process controller.
  [ProcessListener](ro/sync/exml/workspace/api/process/ProcessListener.md)
The process listener.
  [ProfileConditionGroupPO](ro/sync/ecss/conditions/ProfileConditionGroupPO.md)
Profile condition group representation.
  [ProfileConditionInfoPO](ro/sync/ecss/conditions/ProfileConditionInfoPO.md)
Contains information about a condition processing attribute name and possible values.
  [ProfileConditionsSetInfoPO](ro/sync/ecss/conditions/ProfileConditionsSetInfoPO.md)
Contains information about a condition processing attribute name and possible values.
  [ProfileConditionValuePO](ro/sync/ecss/conditions/ProfileConditionValuePO.md)
Profile condition attribute value representation.
  [ProfilingAttributesPresentingColorsPO](ro/sync/ecss/conditions/ProfilingAttributesPresentingColorsPO.md)
Persistent object containing information about the colors used when presenting the profiling attributes in the Author page.
  [ProfilingAttributeStylePO](ro/sync/ecss/conditions/ProfilingAttributeStylePO.md)
Contains information about a profiling attribute value and associated profiling styles.
  [ProfilingConditionalTextProvider](ro/sync/ecss/extensions/api/ProfilingConditionalTextProvider.md)
**Profiling/Conditional Text** is a way to mark elements meant to appear in some renditions of the document, but not in others.
  [ProfilingConditionAttributesManager](ro/sync/ecss/extensions/api/webapp/profiling/ProfilingConditionAttributesManager.md)
Gives access to profiling attributes.
  [ProgressUpdater](ro/sync/ecss/dita/mapeditor/actions/export/ProgressUpdater.md)
Interface used to update the export progress dialog.
  [ProjectChangeListener](ro/sync/exml/workspace/api/standalone/project/ProjectChangeListener.md)
Project change listener.
  [ProjectController](ro/sync/exml/workspace/api/standalone/project/ProjectController.md)
API to access the Project view.
  [ProjectIndexerException](ro/sync/exml/workspace/api/standalone/project/ProjectIndexerException.md)
Signals a problem in the project indexer (either search or index).
  [ProjectIndexerProgressMonitor](ro/sync/exml/workspace/api/standalone/project/ProjectIndexerProgressMonitor.md)
Listener for indexing progress events.
  [ProjectPopupMenuCustomizer](ro/sync/exml/workspace/api/standalone/project/ProjectPopupMenuCustomizer.md)
Can be used to customize a pop-up menu before showing it.
  [ProjectRendererCustomizer](ro/sync/exml/workspace/api/standalone/project/ProjectRendererCustomizer.md)
Base class which can be extended to customize the rendering of the files from the Project view in the stand-alone Oxygen installation.
  [PromoteDemoteItemOperation](ro/sync/ecss/extensions/commons/operations/PromoteDemoteItemOperation.md)
Operation that promotes or demotes a list item.
  [PromoteDemoteSectionOperation](ro/sync/ecss/extensions/docbook/PromoteDemoteSectionOperation.md)
Operation on Docbook for promoting/demoting section nodes.
  [PromoteDemoteSectionUtil](ro/sync/ecss/extensions/docbook/PromoteDemoteSectionUtil.md)
Utility class for promote/demote actions for Docbook.
  [PromoteDemoteSectionUtil.PromoteDemote](ro/sync/ecss/extensions/docbook/PromoteDemoteSectionUtil.PromoteDemote.md)
Promote/demote section action.
  [PromoteTopicrefOperation](ro/sync/ecss/extensions/dita/map/topicref/PromoteTopicrefOperation.md)
Implements a promote operation.
  [PropertySelectionController](ro/sync/ecss/extensions/commons/table/properties/PropertySelectionController.md)
Used for handling with a change of the properties values.
  [ProxyDetailsProvider](ro/sync/exml/workspace/api/standalone/proxy/ProxyDetailsProvider.md)
Provides the proxy details for connecting to a specific URL
  [ProxyNamespaceMapping](ro/sync/xml/ProxyNamespaceMapping.md)
Stores the mappings between the namespace prefixes and the URI's.
  [PseudoClassOperation](ro/sync/ecss/extensions/commons/operations/PseudoClassOperation.md)
A base class for the operations that changes a pseudo-class from an element.
  [PseudoElementDescriptor](ro/sync/exml/workspace/api/editor/page/author/PseudoElementDescriptor.md)
Describes a pseudo element.
  [PseudoElementDescriptor.PsuedoElementType](ro/sync/exml/workspace/api/editor/page/author/PseudoElementDescriptor.PsuedoElementType.md)
Pseudo-element type.
  [PushElementOperation](ro/sync/ecss/extensions/dita/conref/PushElementOperation.md)
Operation used to insert a push operation in DITA documents.
  [QuickAssistProposalGroup](ro/sync/exml/editor/quickassist/QuickAssistProposalGroup.md)
The group for a quick assist proposal.
  [QuickFixType](ro/sync/quickfix/QuickFixType.md)
The type IDs for the quick fixes.
  [RangeProcessor](ro/sync/ecss/extensions/api/content/RangeProcessor.md)
Used to receive call backs when processing a range from the document.
  [ReadOnlyReason](ro/sync/exml/workspace/api/editor/ReadOnlyReason.md)
An object describing the cause for which an editor is read-only.
  [Rectangle](ro/sync/exml/view/graphics/Rectangle.md)
Rectangle.
  [RectangleHighlightPainter](ro/sync/ecss/extensions/api/highlights/RectangleHighlightPainter.md)
Fill a rectangle for the given highlight.
  [RedirectFollowingURLConnection](ro/sync/ecss/extensions/api/webapp/plugin/RedirectFollowingURLConnection.md)
Marker interface that indicates that the URLConnection follows redirects.
  [Reference](ro/sync/ecss/dita/Reference.md)
Contains DITA content reference information.
  [Reference](ro/sync/exml/workspace/api/references/Reference.md)
Simple bean class used to contain references.
  [Reference.Type](ro/sync/exml/workspace/api/references/Reference.Type.md)
Constants enumerating the resource types.
  [ReferenceCollector](ro/sync/exml/workspace/api/references/ReferenceCollector.md)
Implementations of this interface are used to collect the references to external resources (images, audio, video, XInclude, etc.).
  [ReferenceCollectorFactory](ro/sync/exml/workspace/api/references/ReferenceCollectorFactory.md)
Factory that creates ReferenceCollector objects to collect references from an XML document at specified URL.
  [ReferenceErrorResolver](ro/sync/ecss/extensions/api/ReferenceErrorResolver.md)
Resolver for errors concerning references.
  [ReferenceErrorResolverExt](ro/sync/ecss/extensions/api/ReferenceErrorResolverExt.md)
Resolver for errors concerning references.
  [ReferenceExtractor](ro/sync/exml/workspace/api/references/ReferenceExtractor.md)
Interface used to extract a Reference from a node
  [ReferenceResolverException](ro/sync/ecss/extensions/api/ReferenceResolverException.md)
Exception thrown if the reference resolver could not resolve a target.
  [ReferenceResolverSAXParseException](ro/sync/ecss/extensions/api/ReferenceResolverSAXParseException.md)
Exception thrown if the reference resolver could not resolve a target.
  [ReferencesCustomizer](ro/sync/exml/workspace/api/standalone/ReferencesCustomizer.md)
Contains methods for customizing the Input URL Choosers and for computing relative paths from URLs in an implementation specific manner.
  [ReferenceType](ro/sync/ecss/extensions/api/ReferenceType.md)
The type of a resource denoted by an URL.
  [RelativeInsertPosition](ro/sync/exml/editor/xmleditor/operations/context/RelativeInsertPosition.md)
Defines an insert position relative to a node.
  [RelativeLength](ro/sync/ecss/css/RelativeLength.md)
A length that may be expressed as an absolute or relative value, or as an "auto" value, that is to be computed at later time, by the layout engine.
  [RelativeReferenceResolver](ro/sync/exml/workspace/api/util/RelativeReferenceResolver.md)
Control the way in which a relative reference is computed in Oxygen for a given protocol.
  [RelLink](ro/sync/ecss/dita/reference/reltable/RelLink.md)
Defines a relationship between two topic URLs.
  [ReloadContentOperation](ro/sync/ecss/extensions/commons/operations/ReloadContentOperation.md)
Reloads the content of the editor by reading again from the URL used to open it.
  [ReltableCellSpanProvider](ro/sync/ecss/extensions/dita/map/table/ReltableCellSpanProvider.md)
The DITA reltable cell span provider.
  [ReltableConstants](ro/sync/ecss/extensions/dita/map/table/ReltableConstants.md)
Interface containing the name of the elements and attributes used in the DITA map reltable model.
  [RelTablePropertiesHelper](ro/sync/ecss/extensions/dita/map/table/RelTablePropertiesHelper.md)
Table helper for "Table properties" action.
  [RelTableShowPropertiesOperation](ro/sync/ecss/extensions/dita/map/table/RelTableShowPropertiesOperation.md)
"Show table properties" operation for DITA Map rel table.
  [RemovableURLConnection](ro/sync/net/protocol/RemovableURLConnection.md)
Adds methods to delete a resource
  [RemoveConrefOperation](ro/sync/ecss/extensions/dita/conref/RemoveConrefOperation.md)
Operation used to remove a conref from an element in DITA documents.
  [RemovePseudoClassOperation](ro/sync/ecss/extensions/commons/operations/RemovePseudoClassOperation.md)
An operation that removes a pseudo-class from an element.
  [RenameElementOperation](ro/sync/ecss/extensions/commons/operations/RenameElementOperation.md)
An implementation of an operation that renames one or more elements identified by the given XPath expression.
  [RendererLayoutInfo](ro/sync/ecss/extensions/api/editor/RendererLayoutInfo.md)
Class which contains rendering information about a renderer, information like the baseline and the size.
  [RenderingInfoChangedListener](ro/sync/ecss/component/RenderingInfoChangedListener.md)
Listener that is notified when the rendering info for a node is changed.
  [RenderingInfoChangeType](ro/sync/ecss/component/RenderingInfoChangeType.md)
The type of the rendering info change.
  [RenderingInformation](ro/sync/ecss/extensions/api/structure/RenderingInformation.md)
The rendering information used to render a node in the outliner and bread crumb.
  [ReplaceAllKeyrefsAndConrefsOperation](ro/sync/ecss/extensions/dita/conref/ReplaceAllKeyrefsAndConrefsOperation.md)
Operation that replaces all conrefs, keyrefs and conkeyrefs in a DITA topic with the resolved content.
  [ReplaceConrefOperation](ro/sync/ecss/extensions/dita/conref/ReplaceConrefOperation.md)
Operation used to remove the conref and bring the referred content in the current document.
  [ReplaceContentOperation](ro/sync/ecss/extensions/commons/operations/ReplaceContentOperation.md)
An implementation of an operation to replace the content of the document.
  [ReplaceElementContentOperation](ro/sync/ecss/extensions/commons/operations/ReplaceElementContentOperation.md)
Replaces the content of the: - specified element (indicated by an XPath expression) or - fully selected element or - element at caret (if the selection is empty or a node is not entirely selected).
  [ReportableDocumentPositionedInfo](ro/sync/document/ReportableDocumentPositionedInfo.md)
Interface used to mark the [DocumentPositionedInfo](ro/sync/document/DocumentPositionedInfo.md) that can be reported as a problem by using the "Report Problem" oXygen dialog.
  [ResourceFilter](ro/sync/exml/workspace/api/standalone/ResourceFilter.md)
Resource filter returned by the InputURLCustomizer.
  [Response](ro/sync/exml/plugin/workspace/security/Response.md)
A response describing what this provider knows about this host.
  [ResponseType](ro/sync/ui/application/security/ResponseType.md)
The types of responses allowed when an external link wants to connect to the application.
  [ResultsManager](ro/sync/exml/workspace/api/results/ResultsManager.md)
Manages the results of various operations.
  [ResultsManager.ResultType](ro/sync/exml/workspace/api/results/ResultsManager.ResultType.md)
The type of the result.
  [ResultsTabEvent](ro/sync/exml/workspace/api/results/ResultsTabEvent.md)
An event triggered inside a results tab.
  [ResultsTabEvent.ResultsTabEventType](ro/sync/exml/workspace/api/results/ResultsTabEvent.ResultsTabEventType.md)
The type of the event from the results tab.
  [ResultsTabEventHandler](ro/sync/exml/workspace/api/results/ResultsTabEventHandler.md)
Handles the event triggered inside a results tab.
  [ResultsTabPopUpMenuCustomizer](ro/sync/exml/workspace/api/results/ResultsTabPopUpMenuCustomizer.md)
Customizes the contextual pop-up menu of a results tab.
  [ReviewActionsProvider](ro/sync/ecss/extensions/api/review/ReviewActionsProvider.md)
Provides a set of custom actions for a certain highlight.
  [ReviewController](ro/sync/ecss/extensions/api/webapp/review/ReviewController.md)
Provides support for marker related actions (accept/reject tracked changes, add/edit comments, edit author name etc.).
  [ReviewsRenderingInformationProvider](ro/sync/ecss/extensions/api/review/ReviewsRenderingInformationProvider.md)
Provider for data that will be rendered in the review view, in Author mode for highlights.
  [Room](ro/sync/ecss/extensions/api/webapp/ce/Room.md)
A room is an abstraction for a set of document models created for the same document.
  [RoomCreatedListener](ro/sync/ecss/extensions/api/webapp/ce/RoomCreatedListener.md)
Listener called when a room was created.
  [RoomFactory](ro/sync/ecss/extensions/api/webapp/ce/RoomFactory.md)
Factory for [Room](ro/sync/ecss/extensions/api/webapp/ce/Room.md) objects.
  [RoomObserver](ro/sync/ecss/extensions/api/webapp/ce/RoomObserver.md)
Observer for a [Room](ro/sync/ecss/extensions/api/webapp/ce/Room.md), whose state can be used as a source of truth for the current state of the edited document.
  [RoomObserver.EditListener](ro/sync/ecss/extensions/api/webapp/ce/RoomObserver.EditListener.md)
Listener called when an edit happened in the room.
  [RoomObserver.SyncListener](ro/sync/ecss/extensions/api/webapp/ce/RoomObserver.SyncListener.md)
Listener called when a batch of changes are synchronized.
  [RoomProxyCouldNotBeCreatedException](ro/sync/ecss/extensions/api/webapp/ce/RoomProxyCouldNotBeCreatedException.md)
Exception to be thrown when the creation of a proxy room failed.
  [RoomsManager](ro/sync/ecss/extensions/api/webapp/ce/RoomsManager.md)
Class that manages the creation of instances concurrent editing [Room](ro/sync/ecss/extensions/api/webapp/ce/Room.md).
  [SACustomTableColumnInsertionDialog](ro/sync/ecss/extensions/commons/table/operations/SACustomTableColumnInsertionDialog.md)
Dialog displayed when trying to customize column insertion (using "Insert Columns...").
  [SACustomTableRowInsertionDialog](ro/sync/ecss/extensions/commons/table/operations/SACustomTableRowInsertionDialog.md)
Dialog displayed when trying to customize row insertion (using "Insert Rows...").
  [SADITARelTableCustomizer](ro/sync/ecss/extensions/dita/map/table/SADITARelTableCustomizer.md)
Customize a DITA map reltable.
  [SADITARelTableCustomizerDialog](ro/sync/ecss/extensions/dita/map/table/SADITARelTableCustomizerDialog.md)
Dialog used to customize DITA map reltable creation.
  [SADITATableCustomizer](ro/sync/ecss/extensions/dita/topic/table/SADITATableCustomizer.md)
Customize a DITA table.
  [SADITATableCustomizerDialog](ro/sync/ecss/extensions/dita/topic/table/SADITATableCustomizerDialog.md)
Dialog used to customize DITA table creation.
  [SADocbook4TableCustomizerDialog](ro/sync/ecss/extensions/docbook/table/SADocbook4TableCustomizerDialog.md)
Dialog used to customize DocBook4 table creation.
  [SADocbook5TableCustomizerDialog](ro/sync/ecss/extensions/docbook/table/SADocbook5TableCustomizerDialog.md)
Dialog used to customize DocBook5 table creation.
  [SADocbookInnerTableCustomizer](ro/sync/ecss/extensions/docbook/table/SADocbookInnerTableCustomizer.md)
Customize a Docbook inner table (entrytbl).
  [SADocbookTableCustomizer](ro/sync/ecss/extensions/docbook/table/SADocbookTableCustomizer.md)
Customize a Docbook table.
  [SADocbookTableCustomizerDialog](ro/sync/ecss/extensions/docbook/table/SADocbookTableCustomizerDialog.md)
Dialog used to customize DocBook table creation.
  [SafeAuthorOperation](ro/sync/ecss/extensions/api/webapp/SafeAuthorOperation.md)
Deprecated.
This interface is not used anymore as marker interface for operations that can be invoked via REST API with user supplied arguments.

 [SAIDElementsCustomizer](ro/sync/ecss/extensions/commons/id/SAIDElementsCustomizer.md)
Customize the list of elements for auto ID generation.
  [SAIDElementsCustomizerDialog](ro/sync/ecss/extensions/commons/id/SAIDElementsCustomizerDialog.md)
Dialog used to customize DITA elements which have auto ID generation.
  [SAPropertyPanel](ro/sync/ecss/extensions/commons/table/properties/SAPropertyPanel.md)
This class will add to the given parent container a label with the property render string and a combobox containing all the possible values for the given property.
  [SAQuickAssistProposal](ro/sync/exml/editor/quickassist/sa/SAQuickAssistProposal.md)
The interface of completion proposals generated by content assist processors.
  [SASortCustomizerDialog](ro/sync/ecss/extensions/commons/sort/SASortCustomizerDialog.md)
Standalone implementation of the customizer used to select the criterion information used when sorting.
  [SATableColumnInsertionCustomizerInvoker](ro/sync/ecss/extensions/commons/table/operations/SATableColumnInsertionCustomizerInvoker.md)
Customize table column at insertion.
  [SATableCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/SATableCustomizerDialog.md)
Dialog used to customize the insertion of a table (number of rows, columns, table caption).
  [SATablePropertiesCustomizerDialog](ro/sync/ecss/extensions/commons/table/properties/SATablePropertiesCustomizerDialog.md)
Dialog that allows the user to edit the table properties.
  [SATableRowInsertionCustomizerInvoker](ro/sync/ecss/extensions/commons/table/operations/SATableRowInsertionCustomizerInvoker.md)
Customize table rows at insertion.
  [SATableSplitCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/SATableSplitCustomizerDialog.md)
Dialog that allows the user to choose the information necessary for the Split operation.
  [SATEIFigureEntityAttributeCustomizer](ro/sync/ecss/extensions/tei/SATEIFigureEntityAttributeCustomizer.md)
Customize the value of the attribute for a TEI figure.
  [SATEITableCustomizer](ro/sync/ecss/extensions/tei/table/SATEITableCustomizer.md)
Customize a TEI table.
  [SATEITableCustomizerDialog](ro/sync/ecss/extensions/tei/table/SATEITableCustomizerDialog.md)
Dialog used to customize a TEI table.
  [SaveStrategy](ro/sync/ecss/extensions/api/webapp/ce/SaveStrategy.md)
Details required when saving a concurrently edited document.
  [SAXHTMLTableCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/xhtml/SAXHTMLTableCustomizerDialog.md)
Dialog used to customize XHTML table creation.
  [SAXHTMLTableCustomizerInvoker](ro/sync/ecss/extensions/commons/table/operations/xhtml/SAXHTMLTableCustomizerInvoker.md)
Customize a XHTML table.
  [SaxonEdition](ro/sync/exml/plugin/transform/SaxonEdition.md)
Saxon XSLT and XQuery transformer edition.
  [SaxonXQueryTransformerPluginExtension](ro/sync/exml/plugin/transform/SaxonXQueryTransformerPluginExtension.md)
A plugin extension that contributes a Saxon XQuery transformer.
  [SaxonXSLTTransformerPluginExtension](ro/sync/exml/plugin/transform/SaxonXSLTTransformerPluginExtension.md)
A plugin extension that contributes a Saxon XSLT transformer.
  [ScenarioInvoker](ro/sync/exml/workspace/api/editor/ScenarioInvoker.md)
Convenience interface for a validation and transformation scenarios invoker.
  [SchemaAwareHandlerResult](ro/sync/ecss/extensions/api/schemaaware/SchemaAwareHandlerResult.md)
Contains information about the result of the last operation handled by [AuthorSchemaAwareEditingHandler](ro/sync/ecss/extensions/api/AuthorSchemaAwareEditingHandler.md).
  [SchemaAwareHandlerResultInsertConstants](ro/sync/ecss/extensions/api/schemaaware/SchemaAwareHandlerResultInsertConstants.md)
Result informations available for an schema aware insert operation (either typing or insert fragment).
  [SchemaAwareHandlerResultsImpl](ro/sync/ecss/extensions/api/schemaaware/SchemaAwareHandlerResultsImpl.md)
Default implementation for [SchemaAwareHandlerResult](ro/sync/ecss/extensions/api/schemaaware/SchemaAwareHandlerResult.md)}.
  [SchemaManagerFilter](ro/sync/contentcompletion/xml/SchemaManagerFilter.md)
Interface for objects used to filter the editor content completion schema manager proposals.
  [SchemaManagerFilterBase](ro/sync/contentcompletion/xml/SchemaManagerFilterBase.md)
Base class for objects used to filter the editor content completion schema manager proposals.
  [SchematronExtensionsBundle](ro/sync/ecss/extensions/schematron/SchematronExtensionsBundle.md)
The Schematron framework extensions bundle.
  [SchematronNodeRendererCustomizer](ro/sync/ecss/extensions/schematron/SchematronNodeRendererCustomizer.md)
Class used to customize the way a Schematron node is rendered in the UI.
  [SearchParams](ro/sync/exml/workspace/api/standalone/project/SearchParams.md)
Params for finding content in the project.
  [SearchReferencesDITAOperation](ro/sync/ecss/extensions/dita/search/SearchReferencesDITAOperation.md)
Operation to search references to the current DITA element.
  [SelectedTextOperation](ro/sync/ecss/extensions/commons/operations/text/SelectedTextOperation.md)
Provides upper case and lower case operations over a selected text.
  [SelectionInterpretationMode](ro/sync/ecss/extensions/api/SelectionInterpretationMode.md)
Impose how the selection is interpreted by the application.
  [SelectionPluginContext](ro/sync/exml/plugin/selection/SelectionPluginContext.md)
Plugin context interface.
  [SelectionPluginExtension](ro/sync/exml/plugin/selection/SelectionPluginExtension.md)
Plugin extension.
  [SelectionPluginResult](ro/sync/exml/plugin/selection/SelectionPluginResult.md)
Plugin result interface.
  [SelectionPluginResultImpl](ro/sync/exml/plugin/selection/SelectionPluginResultImpl.md)
Support implementation of the PluginResult interface.
  [ServletConfig](ro/sync/ecss/extensions/api/webapp/plugin/servlet/ServletConfig.md)
ServletConfig interface inspired from HTTP Servlet 5.0.
  [ServletContext](ro/sync/ecss/extensions/api/webapp/plugin/servlet/ServletContext.md)
ServletContext interface inspired from HTTP Servlet 5.0.
  [ServletException](ro/sync/ecss/extensions/api/webapp/plugin/servlet/ServletException.md)
ServletException interface inspired from HTTP Servlet 5.0.
  [ServletInputStream](ro/sync/ecss/extensions/api/webapp/plugin/servlet/ServletInputStream.md)
ServletInputStream interface inspired from HTTP Servlet 5.0.
  [ServletOutputStream](ro/sync/ecss/extensions/api/webapp/plugin/servlet/ServletOutputStream.md)
ServletOutputStream interface inspired from HTTP Servlet 5.0.
  [ServletPluginConfigExtension](ro/sync/ecss/extensions/api/webapp/plugin/ServletPluginConfigExtension.md)
This class should be extended to create a configuration page for a Web Author plugin.
  [ServletPluginExtension](ro/sync/ecss/extensions/api/webapp/plugin/ServletPluginExtension.md)
This abstract class should be extended in order to create a servlet.
  [ServletRequest](ro/sync/ecss/extensions/api/webapp/plugin/servlet/ServletRequest.md)
ServletRequest interface inspired from HTTP Servlet 5.0.
  [ServletResponse](ro/sync/ecss/extensions/api/webapp/plugin/servlet/ServletResponse.md)
ServletResponse interface inspired from HTTP Servlet 5.0.
  [SessionStore](ro/sync/ecss/extensions/api/webapp/SessionStore.md)
A per-session key value store (sessionId, key, value).
  [SetPseudoClassOperation](ro/sync/ecss/extensions/commons/operations/SetPseudoClassOperation.md)
An operation that sets a pseudo-class to an element.
  [SetReadOnlyStatusOperation](ro/sync/ecss/extensions/commons/operations/SetReadOnlyStatusOperation.md)
Operation that sets the read-only status of a document.
  [Severity](ro/sync/ecss/extensions/api/link/Severity.md)
A hint about the severity of the exception.
  [Shape](ro/sync/exml/view/graphics/Shape.md)
Common shape
  [ShowDITAElementDocumentationOperation](ro/sync/ecss/extensions/dita/ShowDITAElementDocumentationOperation.md)
Operation that opens the associated specification html page for the current DITA element.
  [ShowElementDocumentationOperation](ro/sync/ecss/extensions/commons/operations/ShowElementDocumentationOperation.md)
Operation that opens the associated specification html page for the current element.
  [ShowKeyDefinitionOperation](ro/sync/ecss/extensions/dita/search/ShowKeyDefinitionOperation.md)
Operation that shows the definition of the key used on the current element.
  [ShowKeysAndReusableComponentsOperation](ro/sync/ecss/extensions/dita/reuse/ShowKeysAndReusableComponentsOperation.md)
Operation used to show a list of reusable keys and/or components.
  [ShowTablePropertiesBaseOperation](ro/sync/ecss/extensions/commons/table/properties/ShowTablePropertiesBaseOperation.md)
Base class for operations that shows a dialog which allows the user to modify some properties for a table.
  [SimpleListOfStringsExternalPersistentObject](ro/sync/exml/workspace/api/options/SimpleListOfStringsExternalPersistentObject.md)
A persistent object which holds a list of strings.
  [SimpleQuickAssistProcessor](ro/sync/exml/editor/quickassist/SimpleQuickAssistProcessor.md)
Quick assist processor for quick fixes and quick assists.
  [SimpleTableConstants](ro/sync/ecss/extensions/dita/topic/table/simpletable/SimpleTableConstants.md)
Provides elements and attributes information used in DITA simple table model.
  [SimpleTableHelper](ro/sync/ecss/extensions/dita/topic/table/simpletable/properties/SimpleTableHelper.md)
Helper class for edit properties on DITA Simple tables.
  [SimpleTableShowPropertiesOperation](ro/sync/ecss/extensions/dita/topic/table/simpletable/properties/SimpleTableShowPropertiesOperation.md)
Class for edit properties on DITA CALS tables.
  [SimpleTableShowPropertiesOperationBase](ro/sync/ecss/extensions/dita/topic/table/simpletable/properties/SimpleTableShowPropertiesOperationBase.md)
Base operation for edit choice properties on DITA simple tables.
  [SimpleTableSortOperation](ro/sync/ecss/extensions/commons/sort/SimpleTableSortOperation.md)
Sort operation for simple tables
  [SimpleURLChooserEditor](ro/sync/ecss/extensions/commons/editor/SimpleURLChooserEditor.md)
Simple URL Chooser in-place editor.
  [Slugifier](ro/sync/ecss/extensions/dita/map/topicref/util/Slugifier.md)
Computes a slug from an arbitrary string.
  [SortCriteriaInformation](ro/sync/ecss/extensions/commons/sort/SortCriteriaInformation.md)
Holds information about the sort criteria and scope.
  [SortCustomizer](ro/sync/ecss/extensions/commons/sort/SortCustomizer.md)
Used for customizing the sorting information, typically through user interaction.
  [SortOperation](ro/sync/ecss/extensions/commons/sort/SortOperation.md)
Sort operations base class.
  [SortUtil](ro/sync/ecss/extensions/commons/sort/SortUtil.md)
Util class for table sort operations
  [SpellCheckerHelper](ro/sync/ecss/extensions/api/spell/SpellCheckerHelper.md)
Helper utilties for the spell checker.
  [SpellcheckingEngine](ro/sync/ecss/extensions/api/webapp/SpellcheckingEngine.md)

 [SpellCheckingProblemInfo](ro/sync/ecss/extensions/api/SpellCheckingProblemInfo.md)

 [SpellCheckingProblemInfoWithSuggestions](ro/sync/ecss/extensions/api/SpellCheckingProblemInfoWithSuggestions.md)

 [SpellSuggestionsInfo](ro/sync/ecss/extensions/api/SpellSuggestionsInfo.md)
Container for spellchecking suggestions information.
  [SplitCellAboveBelowOperation](ro/sync/ecss/extensions/commons/table/operations/cals/SplitCellAboveBelowOperation.md)
Operation for splitting a table cell above or below.
  [SplitCellAboveBelowOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/SplitCellAboveBelowOperation.md)
Operation for splitting a table cell above or below.
  [SplitCellAboveBelowOperation](ro/sync/ecss/extensions/dita/topic/table/cals/SplitCellAboveBelowOperation.md)
Operation for splitting a DITA table cell above or below.
  [SplitCellAboveBelowOperation](ro/sync/ecss/extensions/tei/table/SplitCellAboveBelowOperation.md)
Operation used to split a table cell above or below.
  [SplitCellAboveBelowOperationBase](ro/sync/ecss/extensions/commons/table/operations/SplitCellAboveBelowOperationBase.md)
Base operation for splitting a table cell.
  [SplitLeftRightOperation](ro/sync/ecss/extensions/commons/table/operations/cals/SplitLeftRightOperation.md)
Operation for splitting a table cell to the left or to the right.
  [SplitLeftRightOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/SplitLeftRightOperation.md)
Operation for splitting a table cell to the left or to the right.
  [SplitLeftRightOperation](ro/sync/ecss/extensions/dita/topic/table/cals/SplitLeftRightOperation.md)
Operation for splitting a DITA table cell to the left or to the right.
  [SplitLeftRightOperation](ro/sync/ecss/extensions/tei/table/SplitLeftRightOperation.md)
Operation used to split a table cell.
  [SplitLeftRightOperationBase](ro/sync/ecss/extensions/commons/table/operations/SplitLeftRightOperationBase.md)
Operation for splitting a table cell.
  [SplitMenuButton](ro/sync/exml/workspace/api/standalone/ui/SplitMenuButton.md)
A component representing a combination of a button and a menu.
  [SplitOperation](ro/sync/ecss/extensions/commons/table/operations/cals/SplitOperation.md)
Operation for splitting the selected table cell (or the cell at caret when there is no selection).
  [SplitOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/SplitOperation.md)
Operation for splitting the selected table cell (or the cell at caret when there is no selection).
  [SplitOperation](ro/sync/ecss/extensions/dita/topic/table/cals/SplitOperation.md)
Operation for splitting the selected table cell (or the cell at caret when there is no selection).
  [SplitOperation](ro/sync/ecss/extensions/tei/table/SplitOperation.md)
Operation for splitting the selected table cell (or the cell at caret when there is no selection).
  [SplitOperationBase](ro/sync/ecss/extensions/commons/table/operations/SplitOperationBase.md)
Operation for splitting the selected table cell (or the cell at caret when there is no selection), if it spans over multiple rows or columns
  [StandalonePluginWorkspace](ro/sync/exml/workspace/api/standalone/StandalonePluginWorkspace.md)
The **Plugin Workspace** offers the possibility to customize the Workspace toolbars, menu bars or views, to access utility methods or to access (and add listeners for) all opened editors from the Main editing area or from the DITA Maps editing area.
  [StaticContent](ro/sync/ecss/css/StaticContent.md)
Static content which should be generated for an element
  [StopCurrentTransformationScenarioOperation](ro/sync/ecss/extensions/commons/operations/StopCurrentTransformationScenarioOperation.md)
An implementation of an operation which stops the currently running transformation scenario.
  [StringContent](ro/sync/ecss/css/StringContent.md)
String content
  [StyleGuideSchemaManagerFilterBase](ro/sync/contentcompletion/xml/StyleGuideSchemaManagerFilterBase.md)
Style guide schema manager filter base.
  [Styles](ro/sync/ecss/css/Styles.md)
Represents the **computed** style properties for a particular element.
  [StylesFilter](ro/sync/ecss/extensions/api/StylesFilter.md)
Filter for the element styles.
  [StylesFilterContributor](com/oxygenxml/editor/editors/StylesFilterContributor.md)
Provider for an author styles filter.
  [SupportedFrameworks](ro/sync/ecss/imagemap/SupportedFrameworks.md)
The suported frameworks.
  [SurroundWithFragmentOperation](ro/sync/ecss/extensions/commons/operations/SurroundWithFragmentOperation.md)
Surround with fragment operation.
  [SurroundWithTextOperation](ro/sync/ecss/extensions/commons/operations/SurroundWithTextOperation.md)
Surround with text operation.
  [SWTExtension](ro/sync/ecss/extensions/api/SWTExtension.md)
The base interface for all SWT Oxygen extension classes.
  [TabInfo](ro/sync/ecss/extensions/commons/table/properties/TabInfo.md)
Information associated with a tab from the 'Table Properties' dialog.
  [Table](ro/sync/exml/workspace/api/standalone/ui/Table.md)
A table that looks like the ones in oXygen.
  [TableColumnInsertionCustomizer](ro/sync/ecss/extensions/commons/table/operations/TableColumnInsertionCustomizer.md)
Table column insertion customizer.
  [TableColumnsInfo](ro/sync/ecss/extensions/commons/table/operations/TableColumnsInfo.md)
Contains information about the columns to be inserted.
  [TableColumnSpecificationInformation](ro/sync/ecss/extensions/api/table/operations/TableColumnSpecificationInformation.md)
Contains information about column specification (like column specified width).
  [TableCustomizer](ro/sync/ecss/extensions/commons/table/operations/TableCustomizer.md)
Base for frameworks table customizers.
  [TableCustomizerConstants](ro/sync/ecss/extensions/commons/table/operations/TableCustomizerConstants.md)
Constants used to choose certain table attributes.
  [TableCustomizerConstants.ColumnWidthsType](ro/sync/ecss/extensions/commons/table/operations/TableCustomizerConstants.ColumnWidthsType.md)
Column widths specifications
  [TableHelper](ro/sync/ecss/extensions/commons/table/properties/TableHelper.md)

 [TableHelperConstants](ro/sync/ecss/extensions/commons/table/properties/TableHelperConstants.md)
Constants used in table operations
  [TableInfo](ro/sync/ecss/extensions/commons/table/operations/TableInfo.md)
Contains information about the table element (number of rows, columns, table title).

[TableLayoutErrorsListener](ro/sync/ecss/extensions/commons/table/support/errorscanner/TableLayoutErrorsListener.md)<[E](ro/sync/ecss/extensions/commons/table/support/errorscanner/TableLayoutErrorsListener.md)>

Listener to table layout problems
  [TableLayoutProblem](ro/sync/ecss/extensions/commons/table/support/errorscanner/TableLayoutProblem.md)
Table layout problem
  [TableLayoutProblem.Severity](ro/sync/ecss/extensions/commons/table/support/errorscanner/TableLayoutProblem.Severity.md)
Problem severity
  [TableMoveOrCopyColumnOperation](ro/sync/ecss/webapp/actions/TableMoveOrCopyColumnOperation.md)
Operation that can be used to move table column.
  [TableMoveOrCopyRowsOperation](ro/sync/ecss/webapp/actions/TableMoveOrCopyRowsOperation.md)
Operation that can be used to move table rows.
  [TableOperationsUtil](ro/sync/ecss/extensions/commons/table/operations/TableOperationsUtil.md)
Utility class for table operations.
  [TablePropertiesConstants](ro/sync/ecss/extensions/commons/table/properties/TablePropertiesConstants.md)
Interface that contains all constants used in the table properties operation.
  [TablePropertiesHelper](ro/sync/ecss/extensions/commons/table/properties/TablePropertiesHelper.md)
Table helper for 'Table Properties' dialog.
  [TablePropertiesHelperBase](ro/sync/ecss/extensions/commons/table/properties/TablePropertiesHelperBase.md)
Abstract class for table properties helper.
  [TableProperty](ro/sync/ecss/extensions/commons/table/properties/TableProperty.md)
Class representing a table property.
  [TableRowInsertionCustomizer](ro/sync/ecss/extensions/commons/table/operations/TableRowInsertionCustomizer.md)
Table row insertion customizer.
  [TableRowsInfo](ro/sync/ecss/extensions/commons/table/operations/TableRowsInfo.md)
Contains information about the rows to be inserted.
  [TableRowsSpecificationInformation](ro/sync/ecss/extensions/api/table/operations/TableRowsSpecificationInformation.md)
Contains information about rows (like the place where empty cells must be inserted to compensate the spanning cells).
  [TableSortOperation](ro/sync/ecss/extensions/commons/sort/TableSortOperation.md)
Base table sort operation.
  [TableSortUtil](ro/sync/ecss/extensions/commons/sort/TableSortUtil.md)
Util class for table sort operations.
  [TargetedURLStreamHandlerPluginExtension](ro/sync/exml/plugin/urlstreamhandler/TargetedURLStreamHandlerPluginExtension.md)
Usually oXygen has specific fixed URL stream handlers for http and https protocols.
  [TEI_jteiExtensionsBundle](ro/sync/ecss/extensions/tei/TEI_jteiExtensionsBundle.md)
The TEI P5 framework extensions bundle.
  [TEI_jteiExternalObjectInsertionHandler](ro/sync/ecss/extensions/tei/TEI_jteiExternalObjectInsertionHandler.md)
Dropped URLs handler
  [TEIAuthorActionEventHandler](ro/sync/ecss/extensions/api/TEIAuthorActionEventHandler.md)
Author action event handler for TEI.
  [TEIAuthorImageDecorator](ro/sync/ecss/extensions/tei/TEIAuthorImageDecorator.md)
Handles a TEI vocabulary image map (facsimile).
  [TEIAuthorTableOperationsHandler](ro/sync/ecss/extensions/tei/TEIAuthorTableOperationsHandler.md)
Author table operations handler for TEIP4 framework.
  [TEIConfigureAutoIDElementsOperation](ro/sync/ecss/extensions/tei/id/TEIConfigureAutoIDElementsOperation.md)
Operation used to insert a Link in TEI documents.
  [TEIConstants](ro/sync/ecss/extensions/tei/table/TEIConstants.md)
Interface containing the names of the elements and attributes used in TEI.
  [TEIDocumentTypeHelper](ro/sync/ecss/extensions/tei/TEIDocumentTypeHelper.md)
Implementation of the document type helper for TEI.
  [TEIEditImageMapCore](ro/sync/ecss/extensions/tei/TEIEditImageMapCore.md)
Edit Image Map Core for TEI.
  [TEIExtensionsBundleBase](ro/sync/ecss/extensions/tei/TEIExtensionsBundleBase.md)
The TEI framework extensions bundle.
  [TEIIDElementsConstants](ro/sync/ecss/extensions/tei/id/TEIIDElementsConstants.md)
Some constants for ID Generation.
  [TEIInsertListOperation](ro/sync/ecss/extensions/tei/TEIInsertListOperation.md)
Operation used to convert a selection to an ordered/itemized list for TEI.
  [TEIListSortOperation](ro/sync/ecss/extensions/commons/sort/TEIListSortOperation.md)
The implementation for TEI list sort operation.
  [TEINodeRendererCustomizer](ro/sync/ecss/extensions/tei/TEINodeRendererCustomizer.md)
Class used to customize the way an TEI node is rendered in the UI.
  [TEIP5ConfigureAutoIDElementsOperation](ro/sync/ecss/extensions/tei/id/TEIP5ConfigureAutoIDElementsOperation.md)
Operation specific for TEI P5
  [TEIP5ExtensionsBundle](ro/sync/ecss/extensions/tei/TEIP5ExtensionsBundle.md)
The TEI P5 framework extensions bundle.
  [TEIP5ExternalObjectInsertionHandler](ro/sync/ecss/extensions/tei/TEIP5ExternalObjectInsertionHandler.md)
Dropped URLs handler
  [TEIP5IDTypeRecognizer](ro/sync/ecss/extensions/tei/id/TEIP5IDTypeRecognizer.md)
Implementation of ID declarations and references recognizer for TEI P5 framework.
  [TEIP5UniqueAttributesRecognizer](ro/sync/ecss/extensions/tei/id/TEIP5UniqueAttributesRecognizer.md)
Unique attributes recognizer
  [TEISchemaAwareEditingHandler](ro/sync/ecss/extensions/tei/TEISchemaAwareEditingHandler.md)
Specific editing support for TEI documents.
  [TEITableCellSpanProvider](ro/sync/ecss/extensions/commons/table/spansupport/TEITableCellSpanProvider.md)
Provides cell spanning information about TEI tables.
  [TEITableSortOperation](ro/sync/ecss/extensions/tei/table/TEITableSortOperation.md)
TEI tables sort operation implementation.
  [TemplateContentInfo](ro/sync/template/TemplateContentInfo.md)
Template content information.
  [TemplateManager](ro/sync/exml/workspace/api/templates/TemplateManager.md)
Utilities related to providing new file templates...
  [TemplatesCategory](ro/sync/exml/workspace/api/templates/TemplatesCategory.md)
A template category...
  [TextActionsProvider](ro/sync/exml/workspace/api/editor/page/text/actions/TextActionsProvider.md)
Provides access to actions defined in the Text page.
  [TextAttribute](ro/sync/exml/view/graphics/TextAttribute.md)
Constants for the [AttributedString](ro/sync/exml/view/graphics/AttributedString.md) attributes.
  [TextChunkDescriptor](ro/sync/exml/workspace/api/util/TextChunkDescriptor.md)
Descriptor for a text chunk from a document.
  [TextContentIterator](ro/sync/ecss/extensions/api/content/TextContentIterator.md)
Iterate over the text content in the Author document between a start and an end offset.
  [TextContext](ro/sync/ecss/extensions/api/content/TextContext.md)
Current Text Context where the text content iterator is positioned.
  [TextDnDListener](com/oxygenxml/editor/editors/TextDnDListener.md)
Text Drag and Drop listener interface for the SWT implementation.
  [TextDocumentController](ro/sync/exml/workspace/api/editor/page/text/xml/TextDocumentController.md)
Contains API for inserting XML content in certain places in the Text editing mode.
  [TextField](ro/sync/exml/workspace/api/standalone/ui/TextField.md)
Text field with undo/redo support.
  [TextFieldEditor](ro/sync/ecss/component/editor/TextFieldEditor.md)
A text field with CC support.
  [TextForegroundHighlighterPainter](ro/sync/ecss/extensions/api/highlights/TextForegroundHighlighterPainter.md)
Can also draw the text foreground with a certain color.
  [TextOperationException](ro/sync/exml/workspace/api/editor/page/text/xml/TextOperationException.md)
An exception thrown by a text editing operation when it fails.
  [TextPageExternalObjectInsertionHandler](ro/sync/ecss/extensions/api/text/TextPageExternalObjectInsertionHandler.md)
This class is notified when URLs are dropped or pasted from a file explorer or from an Oxygen internal view to a Text Editor page.
  [TextPageOperationException](ro/sync/ecss/extensions/api/text/TextPageOperationException.md)
An exception thrown when something goes wrong.
  [TextPopupMenuCustomizer](ro/sync/exml/workspace/api/editor/page/text/TextPopupMenuCustomizer.md)
Can be used to customize a pop-up menu before showing it.
  [TextReferenceReader](ro/sync/ecss/extensions/dita/conref/TextReferenceReader.md)
A XMLReader implementation used to provide the content of a DITA reference as text.
  [ToggleCommentOperation](ro/sync/ecss/extensions/commons/operations/ToggleCommentOperation.md)
Provides an operation to toggle comment.
  [TogglePseudoClassOperation](ro/sync/ecss/extensions/commons/operations/TogglePseudoClassOperation.md)
An implementation of an operation to toggle on/off the pseudo-class of an element.
  [ToggleSurroundWithElementOperation](ro/sync/ecss/extensions/commons/operations/ToggleSurroundWithElementOperation.md)
Toggle "surround with element" operation.
  [TokenMarkerFactory](ro/sync/syntaxhighlight/marker/TokenMarkerFactory.md)
Factory for the TokenMarkers.
  [ToLowerCaseOperation](ro/sync/ecss/extensions/commons/operations/text/ToLowerCaseOperation.md)
Provides an operation to convert the text from a selection into lower case text.
  [ToolbarButton](ro/sync/exml/workspace/api/standalone/ui/ToolbarButton.md)
A toolbar button which looks like the ones in Oxygen
  [ToolbarComponentsCustomizer](ro/sync/exml/workspace/api/standalone/ToolbarComponentsCustomizer.md)
Customizes components for the toolbar
  [ToolbarInfo](ro/sync/exml/workspace/api/standalone/ToolbarInfo.md)
Information about a toolbar.
  [ToolbarToggleButton](ro/sync/exml/workspace/api/standalone/ui/ToolbarToggleButton.md)
A toolbar toggle button which looks like the ones in Oxygen
  [TooltipIconInfo](ro/sync/ecss/extensions/api/TooltipIconInfo.md)
The information(tooltip and icon) used to describe the editing of the value for an attribute.
  [TooltipInformation](ro/sync/exml/workspace/api/editor/page/author/tooltip/TooltipInformation.md)
Information about the tooltip.
  [TopicContentViewModeOperation](ro/sync/ecss/extensions/dita/map/topicref/TopicContentViewModeOperation.md)
Operation used to configure Topic Content view mode.This mode consists of: expanding topic references adding a pseudo-class on root to customize the document
  [TopicReferencesViewModeOperation](ro/sync/ecss/extensions/dita/map/topicref/TopicReferencesViewModeOperation.md)
Operation used to enable Topic References view mode.
  [TopicRefInfo](ro/sync/exml/workspace/api/standalone/ditamap/TopicRefInfo.md)
A map holding information about the topic reference in the DITA Map.
  [TopicrefMoveAction](ro/sync/ecss/extensions/dita/map/topicref/TopicrefMoveAction.md)
Promotes or demotes a topicref.
  [TopicrefMoveAction.Builder](ro/sync/ecss/extensions/dita/map/topicref/TopicrefMoveAction.Builder.md)
Builder for the TopicrefTransitionOperation.
  [TopicRefTargetInfo](ro/sync/exml/workspace/api/standalone/ditamap/TopicRefTargetInfo.md)
A map holding information about the target of a topic reference.
  [TopicRefTargetInfoProvider](ro/sync/exml/workspace/api/standalone/ditamap/TopicRefTargetInfoProvider.md)
Provides information about targets for each topic reference.
  [TopicTitlesViewModeOperation](ro/sync/ecss/extensions/dita/map/topicref/TopicTitlesViewModeOperation.md)
Operation used to configure Topic Titles view mode.
  [ToUpperCaseOperation](ro/sync/ecss/extensions/commons/operations/text/ToUpperCaseOperation.md)
Provides an operation to convert the text from a selection into upper case text.
  [TrackChangesMode](ro/sync/exml/workspace/api/util/diff/TrackChangesMode.md)
Decides whether the modifications performed by [CompareUtilAccess.mergeAuthorContent(ro.sync.ecss.extensions.api.AuthorAccess, java.lang.String, java.lang.String, ro.sync.exml.workspace.api.util.diff.TrackChangesMode)](ro/sync/exml/workspace/api/util/CompareUtilAccess.md#mergeAuthorContent(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.exml.workspace.api.util.diff.TrackChangesMode)) are recorded as tracked changes.
  [TransformationFeedback](ro/sync/exml/workspace/api/editor/transformation/TransformationFeedback.md)
Receives feedback from a transformation scenario which is running.
  [TransformationScenarioInvoker](ro/sync/exml/workspace/api/editor/transformation/TransformationScenarioInvoker.md)
Invokes a transformation scenario.
  [TransformationScenarioNotFoundException](ro/sync/exml/workspace/api/editor/transformation/TransformationScenarioNotFoundException.md)
Thrown when a transformation scenario cannot be found.
  [TransformOperation](ro/sync/ecss/extensions/commons/operations/TransformOperation.md)
An implementation of an operation to apply a script (XSLT or XQuery) on a element and replacing it with the result of the transformation or inserting the result in the document.
  [Tree](ro/sync/exml/workspace/api/standalone/ui/Tree.md)
A javax.swing.JTree extension which has a consistent look and feel with the ones used in Oxygen.
  [TreeCellRenderer](ro/sync/exml/workspace/api/standalone/ui/TreeCellRenderer.md)
A javax.swing.tree.DefaultTreeCellRenderer extension which has a consistent look and feel with the renderers used in Oxygen.
  [UIPerspectives](ro/sync/exml/UIPerspectives.md)
Defines constants for each UI perspective in oXygen.
  [UniqueAttributesProcessor](ro/sync/ecss/extensions/api/UniqueAttributesProcessor.md)
Identifies unique attributes like ID's.
  [UniqueAttributesRecognizer](ro/sync/ecss/extensions/api/UniqueAttributesRecognizer.md)
Identifies unique attributes like ID's.
  [UnsavedContentReferenceManager](ro/sync/ecss/extensions/api/access/UnsavedContentReferenceManager.md)
Manager that can be used to find (and save) the resources that have been modified during the editing of a document that contained the expanded references to these resources.
  [UnsavedReferenceNodeDescriptor](ro/sync/ecss/extensions/api/access/UnsavedReferenceNodeDescriptor.md)
Descriptor for an [AuthorReferenceNode](ro/sync/ecss/extensions/api/node/AuthorReferenceNode.md) that contains an unsaved reference.
  [UnwrapTagsOperation](ro/sync/ecss/extensions/commons/operations/UnwrapTagsOperation.md)
Unwrap tags operation.
  [UpdateImageMapOperationBase](ro/sync/ecss/extensions/commons/imagemap/operations/UpdateImageMapOperationBase.md)
Updates an image map with shape information from an SVG.
  [URIContent](ro/sync/ecss/css/URIContent.md)
URI content
  [URLChooserEditorSWT](ro/sync/ecss/extensions/commons/editor/URLChooserEditorSWT.md)
URL Chooser in-place editor on Eclipse.
  [URLChooserMenuExtension](ro/sync/exml/plugin/urlstreamhandler/URLChooserMenuExtension.md)
Get the name of the action which will be displayed in the File menu.
  [URLChooserPluginExtension](ro/sync/exml/plugin/urlstreamhandler/URLChooserPluginExtension.md)
Deprecated.
This approach will continue to work but it is recommanded to use the **ro.sync.exml.plugin.urlstreamhandler.URLChooserPluginExtension2** interface which also receives access to the Oxygen workspace.

 [URLChooserPluginExtension2](ro/sync/exml/plugin/urlstreamhandler/URLChooserPluginExtension2.md)
URL chooser plugin extension.
  [URLChooserToolbarExtension](ro/sync/exml/plugin/urlstreamhandler/URLChooserToolbarExtension.md)
URL chooser toolbar extension.
  [URLHandlerReadOnlyCheckerExtension](ro/sync/exml/plugin/urlstreamhandler/URLHandlerReadOnlyCheckerExtension.md)
This interface can be called to decide if an URL is read-only or not.
  [URLStreamHandlerPluginExtension](ro/sync/exml/plugin/urlstreamhandler/URLStreamHandlerPluginExtension.md)
This URL stream handler provides the possibility to impose the URL stream handlers for specific protocols.
  [URLStreamHandlerPluginExtensionConstants](ro/sync/exml/plugin/urlstreamhandler/URLStreamHandlerPluginExtensionConstants.md)
Constants used from URLStreamHandler provider plugin extensions.
  [URLStreamHandlerWithContext](ro/sync/ecss/extensions/api/webapp/plugin/URLStreamHandlerWithContext.md)
A base-class for URLStreamHandlers that need a context for the URL whose connection is to be opened.
  [URLStreamHandlerWithContextUtil](ro/sync/ecss/extensions/api/webapp/plugin/URLStreamHandlerWithContextUtil.md)
Utility class for adding/removing the user context id from the URLs.
  [URLStreamHandlerWithLockPluginExtension](ro/sync/exml/plugin/urlstreamhandler/URLStreamHandlerWithLockPluginExtension.md)
An URLStreamHandler with lock support plugin extension.
  [UserActionRequiredException](ro/sync/ecss/extensions/api/webapp/plugin/UserActionRequiredException.md)
Class that extends an IOException with an WebappMessage that should be sent to the client-side code.
  [UserActionRequiredMessage](ro/sync/ecss/extensions/api/webapp/plugin/UserActionRequiredMessage.md)
Contains details for the server message that is presented on client side when a user action required exception is thrown.
  [UserContext](ro/sync/ecss/extensions/api/webapp/plugin/UserContext.md)
The context of the user that opened the URL.
  [UserInfo](ro/sync/ecss/extensions/api/webapp/license/UserInfo.md)
Information about an user.
  [UserManagerSingleton](ro/sync/ecss/extensions/api/webapp/license/UserManagerSingleton.md)
Class that can be used to retrieve the user on behalf of which the current request is executed.
  [UserNotLicensedException](ro/sync/ecss/extensions/api/webapp/license/UserNotLicensedException.md)
Exception thrown when a user which is not licensed to use the app, performs some action.
  [UtilAccess](ro/sync/exml/workspace/api/util/UtilAccess.md)
Provides access to utility methods.
  [ValidatingAuthorReferenceResolver](ro/sync/ecss/extensions/api/ValidatingAuthorReferenceResolver.md)
This resolver also validates the target
  [ValidatingReferenceResolverException](ro/sync/ecss/extensions/api/ValidatingReferenceResolverException.md)
Exception thrown if the source does not accept the target as a resolved reference
  [ValidationMode](ro/sync/exml/plugin/validator/ValidationMode.md)
Validation modes supported by the validation plugin extension: automatic or manual.
  [ValidationProblems](ro/sync/exml/workspace/api/editor/validation/ValidationProblems.md)
Holds a set of problems which were reported during the validation process.
  [ValidationProblemsCodes](ro/sync/exml/workspace/api/util/validation/ValidationProblemsCodes.md)
Contains codes for various validation problems.
  [ValidationProblemsFilter](ro/sync/exml/workspace/api/editor/validation/ValidationProblemsFilter.md)
Filter which can be used by the user to ignore (or add) to the list of validation problems found by the validation process (manual or automatic) for a certain file.
  [ValidationScenarioInvoker](ro/sync/exml/workspace/api/editor/validation/ValidationScenarioInvoker.md)
Invokes a validation scenario.
  [ValidationScenarioNotFoundException](ro/sync/exml/workspace/api/editor/validation/ValidationScenarioNotFoundException.md)
Thrown when a transformation scenario cannot be found.
  [ValidationType](ro/sync/exml/plugin/validator/ValidationType.md)
Current validation types that can be performed over a document: strict validation, wellformed validation or both.
  [ValidationUtilAccess](ro/sync/exml/workspace/api/util/validation/ValidationUtilAccess.md)
Validation Utilities.
  [ValidatorPluginExtension](ro/sync/exml/plugin/validator/ValidatorPluginExtension.md)
Plug-in extension that allows custom validation engines.
  [ValidatorProblemCollector](ro/sync/exml/workspace/api/util/validation/ValidatorProblemCollector.md)
Validation Utilities Problems Collector.
  [ViewComponentCustomizer](ro/sync/exml/workspace/api/standalone/ViewComponentCustomizer.md)
Customizes components for the Oxygen views.
  [ViewInfo](ro/sync/exml/workspace/api/standalone/ViewInfo.md)
Information about a view.
  [WebappActionsManager](ro/sync/ecss/extensions/api/webapp/WebappActionsManager.md)
Helper object that provides access to extension actions, and provides support for invoking operations.
  [WebappAreaView](ro/sync/ecss/extensions/api/webapp/imagemap/WebappAreaView.md)
Interface that represents an area on an image map to be rendered in the browser.
  [WebappAreaViewFactory](ro/sync/ecss/extensions/api/webapp/imagemap/WebappAreaViewFactory.md)
Creates instances of WebappAreaView.
  [WebappAuthorDocumentFactory](ro/sync/ecss/extensions/api/webapp/WebappAuthorDocumentFactory.md)
Factory class that creates the document model to be used in the Web Reviewer.
  [WebappAuthorDocumentFactoryConstants](ro/sync/ecss/extensions/api/webapp/WebappAuthorDocumentFactoryConstants.md)
Constants for the webapp document factory.
  [WebappAuthorSchemaAwareActionsHandler](ro/sync/ecss/extensions/api/webapp/WebappAuthorSchemaAwareActionsHandler.md)
Handles schema aware actions like paste.
  [WebappCompatible](ro/sync/ecss/extensions/api/WebappCompatible.md)
Annotation that should be placed on AuthorOperations to indicate whether they are suitable to be invoked from the WebApp.
  [WebappDocumentValidator](ro/sync/ecss/extensions/api/webapp/WebappDocumentValidator.md)

 [WebappEditingSessionLifecycleListener](ro/sync/ecss/extensions/api/webapp/access/WebappEditingSessionLifecycleListener.md)
Listener for the main lifecycle events of an editing session.
  [WebappExtensionsProvider](ro/sync/ecss/extensions/api/WebappExtensionsProvider.md)
Web Author specific extensions for a document type.
  [WebappFindOptions](ro/sync/ecss/extensions/api/webapp/findreplace/WebappFindOptions.md)
Find/Replace options.
  [WebappFormControlRenderer](ro/sync/ecss/extensions/api/webapp/formcontrols/WebappFormControlRenderer.md)
Common interface for server-side form control renderers used in the Web Author.
  [WebappFormControlRendererRegistry](ro/sync/ecss/extensions/api/webapp/formcontrols/WebappFormControlRendererRegistry.md)
Registry for form control renderers used in the Author Reviewer Webapp.
  [WebappImageMapSupport](ro/sync/ecss/extensions/api/webapp/imagemap/WebappImageMapSupport.md)
Represents an instance of an image map embedded in a document.
  [WebappImageMapSupportFactory](ro/sync/ecss/extensions/api/webapp/imagemap/WebappImageMapSupportFactory.md)
Factory class to create image maps for a specific document element.
  [WebappLockManager](ro/sync/ecss/extensions/api/webapp/WebappLockManager.md)
The lock manager associated with a document.
  [WebappMarkAsSavedOperation](ro/sync/ecss/extensions/commons/operations/WebappMarkAsSavedOperation.md)
Operation that marks a webapp document as saved.
  [WebappMessage](ro/sync/ecss/extensions/api/webapp/WebappMessage.md)
Webapp server message that is presented on client side.
  [WebappMessagesProvider](ro/sync/ecss/extensions/api/webapp/WebappMessagesProvider.md)
Gets all the error messages reported by the application.
  [WebappPluginWorkspace](ro/sync/ecss/extensions/api/webapp/access/WebappPluginWorkspace.md)
Plugin workspace access API with webapp-specific features.
  [WebappReferenceCollectorFactory](ro/sync/ecss/extensions/api/webapp/references/WebappReferenceCollectorFactory.md)
Contains methods to create a reference collector for the webapp component
  [WebappRestSafe](ro/sync/ecss/extensions/api/webapp/WebappRestSafe.md)
Annotation that should be placed on AuthorOperations to indicate that they are safe to be invoked in Web Author via a REST API with user supplied arguments.
  [WebappSchematronPhaseChooser](ro/sync/ecss/extensions/api/webapp/WebappSchematronPhaseChooser.md)
Interface that is asked to provide the schematron phase to use.
  [WebappServletPluginExtension](ro/sync/ecss/extensions/api/webapp/plugin/WebappServletPluginExtension.md)
Deprecated.
This API is deprecated because it's based on javax package that's no more supported starting with Servlet 5.0 specification and because this extension type isn't protected against CSRF attacks.

 [WebappSpellchecker](ro/sync/ecss/extensions/api/webapp/WebappSpellchecker.md)

 [WebappTextModeState](ro/sync/ecss/common/WebappTextModeState.md)
The state of the document that can be input to a text editor.
  [WebAuthorPlatformCustomRuleMatcher](ro/sync/ecss/extensions/xhtml/WebAuthorPlatformCustomRuleMatcher.md)
Check if the document is loaded in the WebApp distribution of the oXygen.
  [WebAuthorSpellcheckErrorTypes](ro/sync/ecss/extensions/api/webapp/WebAuthorSpellcheckErrorTypes.md)
Spellcheck error types used for Web Author.
  [WebdavLockHelper](ro/sync/net/protocol/http/WebdavLockHelper.md)
Helper class that allows one to implement locking for a WebDAV server in a multi-user scenario.
  [WhatAttributesCanGoHereContext](ro/sync/contentcompletion/xml/WhatAttributesCanGoHereContext.md)
Used by the schema manager to find out the attributes that can be inserted in a given context.
  [WhatElementsCanGoHereContext](ro/sync/contentcompletion/xml/WhatElementsCanGoHereContext.md)
It is used to determine the elements that can be inserted in the current context.
  [WhatPossibleValuesHasAttributeContext](ro/sync/contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md)
It is used to determine the possible values of the current attribute.
  [WidthRepresentation](ro/sync/ecss/extensions/api/WidthRepresentation.md)
Specifies the fixed and relative width determined from the value of width/colwidth attribute of the col.
  [WidthRepresentation.Unit](ro/sync/ecss/extensions/api/WidthRepresentation.Unit.md)
The fixed width unit.
  [Workspace](ro/sync/exml/workspace/api/Workspace.md)
Provides access to workspace specific information and actions.
  [WorkspaceAccessPluginExtension](ro/sync/exml/plugin/workspace/WorkspaceAccessPluginExtension.md)
Workspace Access plugin extension.
  [WorkspaceUtilities](ro/sync/exml/workspace/api/WorkspaceUtilities.md)
Provides access to global utility methods.
  [WSAuthorComponentEditorPage](ro/sync/exml/workspace/api/editor/page/author/WSAuthorComponentEditorPage.md)
Provides enhanced access (with additional methods) to the author page from an Author Component editor.
  [WSAuthorEditorPage](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPage.md)
Author editor page.
  [WSAuthorEditorPageBase](ro/sync/exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md)
Provides access to methods related to the Author editor actions and information.
  [WSDesignEditorPage](ro/sync/exml/workspace/api/editor/page/design/WSDesignEditorPage.md)
API for the Design page, currently only editable status can be set here...
  [WSDITAMapEditorPage](ro/sync/exml/workspace/api/editor/page/ditamap/WSDITAMapEditorPage.md)
DITA Maps Manager editor page.
  [WSDLExtensionsBundle](ro/sync/ecss/extensions/wsdl/WSDLExtensionsBundle.md)
The WSDL framework extensions bundle.
  [WSDLNodeRendererCustomizer](ro/sync/ecss/extensions/wsdl/WSDLNodeRendererCustomizer.md)
Class used to customize the way an WSDL node is rendered in the UI.
  [WSEditor](ro/sync/exml/workspace/api/editor/WSEditor.md)
Provides access to methods related to the editor actions and information.
  [WSEditorBase](ro/sync/exml/workspace/api/editor/WSEditorBase.md)
Provides access to methods related to the editor actions and information.
  [WSEditorChangeListener](ro/sync/exml/workspace/api/listeners/WSEditorChangeListener.md)
Notified when an editor is added, removed or the editor page is changed
  [WSEditorListener](ro/sync/exml/workspace/api/listeners/WSEditorListener.md)
WS Editor listener.
  [WSEditorPage](ro/sync/exml/workspace/api/editor/page/WSEditorPage.md)
Access to an editor's page.
  [WSEditorPageChangedListener](ro/sync/exml/workspace/api/listeners/WSEditorPageChangedListener.md)
WS Editor page changed listener.
  [WSGridEditorPage](ro/sync/exml/workspace/api/editor/page/grid/WSGridEditorPage.md)
API for the grid page, currently only editable status can be set here...
  [WSOptionChangedEvent](ro/sync/exml/workspace/api/options/WSOptionChangedEvent.md)
Represents an event which indicates that the value of an option has been changed.
  [WSOptionListener](ro/sync/exml/workspace/api/options/WSOptionListener.md)
The listener which is notified about the value changes of an author extension level option.
  [WSOptionsStorage](ro/sync/exml/workspace/api/options/WSOptionsStorage.md)
Support for the user to save and retrieve custom options in the Oxygen common preferences.
  [WSOutline](ro/sync/exml/workspace/api/editor/page/WSOutline.md)
The Workspace Outline.
  [WSTextBasedEditorPage](ro/sync/exml/workspace/api/editor/page/WSTextBasedEditorPage.md)
Provides access to methods related to the editor actions and information for the Text and Author pages.
  [WSTextEditorPage](ro/sync/exml/workspace/api/editor/page/text/WSTextEditorPage.md)
Text editor page access.
  [WSTextXMLSchemaManager](ro/sync/exml/workspace/api/editor/page/text/WSTextXMLSchemaManager.md)
Text page XML schema manager.
  [WSXMLTextEditorPage](ro/sync/exml/workspace/api/editor/page/text/xml/WSXMLTextEditorPage.md)
Contains methods specific to XML editors.
  [WSXMLTextNodeRange](ro/sync/exml/workspace/api/editor/page/text/xml/WSXMLTextNodeRange.md)
The range of an XML node.
  [XHTMLAuthorActionEventHandler](ro/sync/ecss/extensions/api/XHTMLAuthorActionEventHandler.md)
Author action event handler for XHTML.
  [XHTMLAuthorImageDecorator](ro/sync/ecss/extensions/xhtml/XHTMLAuthorImageDecorator.md)
Handles an HTML vocabulary image map.
  [XHTMLAuthorTableOperationsHandler](ro/sync/ecss/extensions/xhtml/XHTMLAuthorTableOperationsHandler.md)
Author table operations handler for XHTML framework.
  [XHTMLConstants](ro/sync/ecss/extensions/commons/table/operations/xhtml/XHTMLConstants.md)
This interface contains the name of the elements and attributes used in XHTML.
  [XHTMLDocumentTypeHelper](ro/sync/ecss/extensions/commons/table/operations/xhtml/XHTMLDocumentTypeHelper.md)
Implementation of the document type helper for XHTML.
  [XHTMLEditImageMapCore](ro/sync/ecss/extensions/xhtml/imagemap/XHTMLEditImageMapCore.md)
Edit map core for XHTML.
  [XHTMLElementLocator](ro/sync/ecss/extensions/xhtml/XHTMLElementLocator.md)
Locator for a XHTML document.
  [XHTMLElementLocatorProvider](ro/sync/ecss/extensions/xhtml/XHTMLElementLocatorProvider.md)
In XHTML the reference can point to an ID type attribute and also to the name attribute of the a element.
  [XHTMLExtensionsBundle](ro/sync/ecss/extensions/xhtml/XHTMLExtensionsBundle.md)
The XHTML framework extensions bundle.
  [XHTMLExternalObjectInsertionHandler](ro/sync/ecss/extensions/xhtml/XHTMLExternalObjectInsertionHandler.md)
Dropped URLs handler
  [XHTMLInsertListOperation](ro/sync/ecss/extensions/xhtml/XHTMLInsertListOperation.md)
Operation used to convert selected paragraphs to ordered/unordered list.
  [XHTMLListSortOperation](ro/sync/ecss/extensions/commons/sort/XHTMLListSortOperation.md)
'Sort list' operation for XHTML.
  [XHTMLNodeRendererCustomizer](ro/sync/ecss/extensions/xhtml/XHTMLNodeRendererCustomizer.md)
Class used to customize the way an XHTML node is rendered in the UI.
  [XHTMLSchemaManagerFilter](ro/sync/ecss/extensions/xhtml/XHTMLSchemaManagerFilter.md)
XHTML implementation for schema manager filter for adding type attribute values for script and style elements in content completion proposals list.
  [XHTMLTableCustomizerConstants](ro/sync/ecss/extensions/commons/table/operations/xhtml/XHTMLTableCustomizerConstants.md)
Constants used to choose XHTML table attributes.
  [XHTMLTableSortOperation](ro/sync/ecss/extensions/commons/table/operations/xhtml/XHTMLTableSortOperation.md)
XHTML table sort operation implementation.
  [XHTMLUniqueAttributesRecognizer](ro/sync/ecss/extensions/xhtml/id/XHTMLUniqueAttributesRecognizer.md)
Unique attributes recognizer
  [XHTMLUpdateImageMapOperation](ro/sync/ecss/extensions/xhtml/imagemap/XHTMLUpdateImageMapOperation.md)
XHTML implementation of the operation that updates an image map with shape information from an SVG.
  [XHTMLUpdateImageMapOperation.XHTMLNewShapeDescriptor](ro/sync/ecss/extensions/xhtml/imagemap/XHTMLUpdateImageMapOperation.XHTMLNewShapeDescriptor.md)
Descriptor of a shape that was added client-side.
  [XHTMLWebappImageMapSupport](ro/sync/ecss/extensions/xhtml/imagemap/XHTMLWebappImageMapSupport.md)
Image map support for XHTML.
  [XHTMLWebappImageMapSupportFactory](ro/sync/ecss/extensions/xhtml/imagemap/XHTMLWebappImageMapSupportFactory.md)
Creates image map support objects for "map" elements.
  [XMLImageHandler](ro/sync/exml/workspace/api/images/handlers/XMLImageHandler.md)
Special handler for editing images defined as XML (SVG, MathML, etc).
  [XMLNodeRendererCustomizer](ro/sync/exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md)
Class used to customize the way an XML node is rendered in the UI.
  [XMLNodeRendererCustomizerAdapter](ro/sync/ecss/extensions/commons/XMLNodeRendererCustomizerAdapter.md)
Empty implementation for [XMLNodeRendererCustomizer](ro/sync/exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md).
  [XMLReaderWithGrammar](ro/sync/exml/workspace/api/util/XMLReaderWithGrammar.md)
XML Reader + grammar cache
  [XMLRefactorProblemCollector](ro/sync/exml/workspace/api/util/refactor/XMLRefactorProblemCollector.md)
Validation Utilities Problems Collector.
  [XMLRefactorUtilAccess](ro/sync/exml/workspace/api/util/refactor/XMLRefactorUtilAccess.md)
XML Refactoring Utilities.
  [XMLUtilAccess](ro/sync/exml/workspace/api/util/XMLUtilAccess.md)
XML Utilities
  [XPathException](ro/sync/exml/workspace/api/editor/page/text/xml/XPathException.md)
An exception thrown when performing an XPath.
  [XPathVersion](ro/sync/ecss/extensions/api/XPathVersion.md)
XPath version types.
  [XPointerElementLocator](ro/sync/ecss/extensions/commons/XPointerElementLocator.md)
Element locator for links that have the one of the following patterns: element(elementID) - locate the element with the same id element(/1/2/5) - A child sequence appearing alone identifies an element by means of stepwise navigation, which is directed by a sequence of integers separated by slashes (/); each integer n locates the nth child element of the previously located element.
  [XProcVersion](ro/sync/contentcompletion/xproc/XProcVersion.md)
Enumeration containing all XProc versions.
  [XQueryOperation](ro/sync/ecss/extensions/commons/operations/XQueryOperation.md)
An implementation of an operation to apply an XQuery script on a element and replacing it with the result of the XQuery transformation, or inserting the result in the document.
  [XQueryTransformerPluginExtension](ro/sync/exml/plugin/transform/XQueryTransformerPluginExtension.md)
A plugin extension that contributes an XQuery transformer.
  [XQueryUpdateOperation](ro/sync/ecss/extensions/commons/operations/XQueryUpdateOperation.md)
An implementation of an operation that applies an XQuery Update script.
  [XSDExtensionsBundle](ro/sync/ecss/extensions/xsd/XSDExtensionsBundle.md)
The XML Schema framework extensions bundle.
  [XSDNodeRendererCustomizer](ro/sync/ecss/extensions/xsd/XSDNodeRendererCustomizer.md)
Class used to customize the way an XML Schema node is rendered in the UI.
  [XSLMessageListener](ro/sync/exml/plugin/transform/XSLMessageListener.md)
Receives a callback generated by xsl:message and xsl:assert.
  [XSLTExtensionsBundle](ro/sync/ecss/extensions/xslt/XSLTExtensionsBundle.md)
The XSLT framework extensions bundle.
  [XSLTNodeRendererCustomizer](ro/sync/ecss/extensions/xslt/XSLTNodeRendererCustomizer.md)
Class used to customize the way an XSLT node is rendered in the UI.
  [XSLTOperation](ro/sync/ecss/extensions/commons/operations/XSLTOperation.md)
An implementation of an operation to apply an XSLT stylesheet on a element and replacing it with the result of the XSLT transformation or inserting the result in the document.
  [XSLTTransformerPluginExtension](ro/sync/exml/plugin/transform/XSLTTransformerPluginExtension.md)
A plugin extension that contributes an XSLT transformer.
  [XSLTTransformerPluginExtensionBase](ro/sync/exml/plugin/transform/XSLTTransformerPluginExtensionBase.md)
Base class for transformers.
  [XSLTVersion](ro/sync/contentcompletion/xsl/XSLTVersion.md)
Enumeration containing all XSLT versions.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
