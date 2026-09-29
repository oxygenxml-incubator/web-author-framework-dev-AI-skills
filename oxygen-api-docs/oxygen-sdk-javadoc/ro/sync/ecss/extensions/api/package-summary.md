# Package ro.sync.ecss.extensions.api

package ro.sync.ecss.extensions.api

Main API package used for controlling the Author page (making modifications, adding listeners).
     Related Packages
Package

Description
 [ro.sync.ecss.extensions](../package-summary.md)

 [ro.sync.ecss.extensions.api.access](access/package-summary.md)
API Access to different parts of the Author editor and of the entire application workspace.
  [ro.sync.ecss.extensions.api.attributes](attributes/package-summary.md)
Filter certain attributes from being displayed in certain parts of the Author editor (the Attributes view, the Attributes editor, the Outline).
  [ro.sync.ecss.extensions.api.callouts](callouts/package-summary.md)

 [ro.sync.ecss.extensions.api.component](component/package-summary.md)
API for interacting with the Author Component SDK.
  [ro.sync.ecss.extensions.api.content](content/package-summary.md)
API used to process the Author content.
  [ro.sync.ecss.extensions.api.editor](editor/package-summary.md)

 [ro.sync.ecss.extensions.api.filter](filter/package-summary.md)
API used to filter the Author content.
  [ro.sync.ecss.extensions.api.highlights](highlights/package-summary.md)
API used to interact with persistent (change tracking, comments, user persistent highlights) and non persistent highlights in the Author page
  [ro.sync.ecss.extensions.api.link](link/package-summary.md)
Used for implementing navigation between links and their targets.
  [ro.sync.ecss.extensions.api.node](node/package-summary.md)
API which allows access to the internal Author hierarchical structure.
  [ro.sync.ecss.extensions.api.review](review/package-summary.md)

 [ro.sync.ecss.extensions.api.schemaaware](schemaaware/package-summary.md)
Schema aware processing (smart typing, smart delete, smart paste).
  [ro.sync.ecss.extensions.api.spell](spell/package-summary.md)
Spell checker helper utilities.
  [ro.sync.ecss.extensions.api.structure](structure/package-summary.md)
API which allows access to the internal Author hierarchical structure.
  [ro.sync.ecss.extensions.api.text](text/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp](webapp/package-summary.md)

     All Classes and InterfacesInterfacesClassesEnum ClassesExceptionsAnnotation Interfaces
Class

Description
 [ArgumentDescriptor](ArgumentDescriptor.md)
Descriptor class for an author operation argument.
  [ArgumentsMap](ArgumentsMap.md)
Map between argument names and values.
  [AttributeChangedEvent](AttributeChangedEvent.md)
Event received by the [AuthorListener](AuthorListener.md) when an Author attribute has been changed.
  [AttributesValueEditor](AttributesValueEditor.md)
Deprecated.
Starting with version 15 the [CustomAttributeValueEditor](CustomAttributeValueEditor.md) can be used instead to edit only specific attributes using a custom editor.

 [AuthorAccess](AuthorAccess.md)
Access class to the author functions.
  [AuthorAccessDeprecated](AuthorAccessDeprecated.md)
Contains methods that are deprecated in the [AuthorAccess](AuthorAccess.md) and should no longer be used.
  [AuthorActionEventDetails](AuthorActionEventDetails.md)
Class offering details about an author action event.
  [AuthorActionEventHandler](AuthorActionEventHandler.md)
Intercepts action events in the Author mode and can handle them in a special manner.
  [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md)
Events that are delegated to this handler.
  [AuthorActionEventHandlerBase](AuthorActionEventHandlerBase.md)
Adds various API methods, for example it adds a method which intercepts action events in the Author mode and can handle them in a special manner.
  [AuthorAttributesController](AuthorAttributesController.md)
Helper used to set attributes
  [AuthorCaretEvent](AuthorCaretEvent.md)
AuthorCaretEvent is used to notify interested [AuthorCaretListener](AuthorCaretListener.md) that the position of the caret has changed in the Author editor page.
  [AuthorCaretListener](AuthorCaretListener.md)
Listener for changes in the caret position of the Author editor page.
  [AuthorChangeTrackingController](AuthorChangeTrackingController.md)
Controls the change tracking mode.
  [AuthorClipboardAccess](AuthorClipboardAccess.md)
Access to various content data in the system clipboard.
  [AuthorConstants](AuthorConstants.md)
Interface containing the constants used in Author API.
  [AuthorDocumentController](AuthorDocumentController.md)
Provides methods for modifying the Author document.
  [AuthorDocumentEvent](AuthorDocumentEvent.md)
Marker interface for all document change related events.
  [AuthorDocumentFilter](AuthorDocumentFilter.md)
AuthorDocumentFilter, is a filter for the methods which modify the AuthorDocument.
  [AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md)
Used as a way to circumvent calling back into the AuthorDocumentController to change the AuthorDocument.
  [AuthorDocumentType](AuthorDocumentType.md)
Author structure representing DOCTYPE information as present in the Author document.
  [AuthorElementBaseInterface](AuthorElementBaseInterface.md)
Element represents a tag in an XML document.
  [AuthorExtensionActionProvider](AuthorExtensionActionProvider.md)
Provides an author extension action for a given action ID.
  [AuthorExtensionStateAdapter](AuthorExtensionStateAdapter.md)
Adapter class for [AuthorExtensionStateListener](AuthorExtensionStateListener.md).
  [AuthorExtensionStateListener](AuthorExtensionStateListener.md)
Notified when the Author extension, where the listener is defined, was activated or deactivated in the detection process.
  [AuthorExtensionStateListenerDelegator](AuthorExtensionStateListenerDelegator.md)
A single Author extension state listeners which delegates to other registered listeners.
  [AuthorExternalObjectInsertionHandler](AuthorExternalObjectInsertionHandler.md)
This class is notified when URLs are dropped or pasted to an Author Editor page or when XHTML fragments are pasted or dropped from external applications (like web browsers or office applications) to the Author page.If you want to use a stylesheet to convert the pasted XHTML to your own XML vocabulary you can just overwrite the method: "ro.sync.ecss.extensions.api.AuthorExternalObjectInsertionHandler.getImporterStylesheetFileName(AuthorAccess)" and return the file name of the stylesheet which will be applied.
  [AuthorImageDecorator](AuthorImageDecorator.md)
Permits decoration of the images that are displayed in the Author view.
  [AuthorInputEvent](AuthorInputEvent.md)
Base class for Author input events.
  [AuthorListener](AuthorListener.md)
Listener notified about Author document changes, document structure changes and document content changes. **DANGER:** You must avoid making live document changes on the received call backs.
  [AuthorListenerAdapter](AuthorListenerAdapter.md)
Convenience implementation of the [AuthorListener](AuthorListener.md).
  [AuthorMouseAdapter](AuthorMouseAdapter.md)
Empty implementation of the [AuthorMouseListener](AuthorMouseListener.md).
  [AuthorMouseEvent](AuthorMouseEvent.md)
Mouse event received by the [AuthorMouseListener](AuthorMouseListener.md).
  [AuthorMouseListener](AuthorMouseListener.md)
Interface for the author mouse listeners.
  [AuthorOperation](AuthorOperation.md)
Interface defining an author extension operation.
  [AuthorOperationException](AuthorOperationException.md)
An exception thrown by an [AuthorOperation](AuthorOperation.md) when it fails.
  [AuthorOperationStoppedByUserException](AuthorOperationStoppedByUserException.md)
An exception thrown by an [AuthorOperation](AuthorOperation.md) when it interacts with the user and the user cancels it.
  [AuthorOperationWithCustomUndoBehavior](AuthorOperationWithCustomUndoBehavior.md)
Marker interface that specifies that a particular operation should not be wrapped in a compound undoable edit.
  [AuthorPreloadProcessor](AuthorPreloadProcessor.md)
This processor is notified before the Author document is loaded and renderer.
  [AuthorPseudoClassController](AuthorPseudoClassController.md)
Controls setting and resetting pseudo classes.
  [AuthorReferenceResolver](AuthorReferenceResolver.md)
Interface for the custom handlers used to expand content references.
  [AuthorResourceBundle](AuthorResourceBundle.md)
Gives access to translate keys.
  [AuthorReviewController](AuthorReviewController.md)
Controller that can be used to toggle the change tracking state, modify the review highlight author name, the highlight painting or to obtain information about the properties used in the serialization and representation of the review highlight (author name, reviewer auto color or the current time stamp in a format identical to the one used by Oxygen for insert, delete and comment review highlights).
  [AuthorReviewerNameController](AuthorReviewerNameController.md)
Provides access to reviewer author name, used in the processing instruction that results when a tracked change or a comment is serialized.
  [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md)
If Schema Aware mode is active in Oxygen, all actions that can generate invalid content will be redirected toward this handler.
  [AuthorSchemaAwareEditingHandlerAdapter](AuthorSchemaAwareEditingHandlerAdapter.md)
Adapter class.
  [AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions](AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions.md)
One of the default smart paste strategies involves detecting an path o ancestors from the context element to the inserted one.
  [AuthorSchemaManager](AuthorSchemaManager.md)
Author schema manager.
  [AuthorSelectionAndCaretModel](AuthorSelectionAndCaretModel.md)
Interface to the author selection and caret model providing methods to query and modify the selection intervals and caret position.
  [AuthorSelectionModel](AuthorSelectionModel.md)
Get the Author selection model containing access to all Author selection intervals and methods for adding simple and multiple selections.
  [AuthorTableCellSepProvider](AuthorTableCellSepProvider.md)
This is an interface for classes which are responsible for providing information about the cell separators: "rowsep" and "colsep".
  [AuthorTableCellSpanProvider](AuthorTableCellSpanProvider.md)
This is an interface for classes which are responsible for providing information about the cell spanning.
  [AuthorTableColumnWidthProvider](AuthorTableColumnWidthProvider.md)
This is an interface for classes which are responsible for providing information and handling modifications regarding table and column widths.
  [AuthorTableColumnWidthProviderBase](AuthorTableColumnWidthProviderBase.md)
This is an interface for classes which are responsible for providing information and handling modifications regarding table and column widths.
  [AuthorUndoManager](AuthorUndoManager.md)
Undo manager for Author edits.
  [AuthorViewToModelInfo](AuthorViewToModelInfo.md)
An implementation of this interface is returned by the [WSAuthorEditorPageBase.viewToModel(int, int)](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#viewToModel(int,int))method.
  [AuthorXPathExpressionBuilder](AuthorXPathExpressionBuilder.md)
Generates an XPath expression for an XML node.
  [AWTExtension](AWTExtension.md)
The base interface for all AWT Oxygen extension classes.
  [CacheableAuthorReferencesResolver](CacheableAuthorReferencesResolver.md)
Marker for cachable references resolvers.
  [CancelledByUserException](CancelledByUserException.md)
A custom class used for the exceptions generated by an operation canceled by user.
  [ChangeTrackingController](ChangeTrackingController.md)
Controls the change tracking mode.
  [ClassPathResourcesAccess](ClassPathResourcesAccess.md)
Provides access to all URLs which were added in the classpath for the specific framework when the document type was edited from the Oxygen preferences.
  [CompoundEditListener](CompoundEditListener.md)
Listener notified when compound edits are started and ended.
  [Content](Content.md)
Interface to describe a sequence of character content that can be edited.
  [ContentInterval](ContentInterval.md)
A content interval containing the **inclusive** start offset and **exclusive** end offset.
  [CursorType](CursorType.md)
Supported cursor types for author.
  [CustomAttributeValueContext](CustomAttributeValueContext.md)
Context for a custom attribute.
  [CustomAttributeValueEditingContext](CustomAttributeValueEditingContext.md)
Provides the contexts for the custom attribute value editing.
  [CustomAttributeValueEditor](CustomAttributeValueEditor.md)
A custom editor which gets invoked to edit the value for an attribute.
  [CustomResolverException](CustomResolverException.md)
Signals an custom reference that wasn't resolved.
  [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md)
Intercepts TAB and SHIFT+TAB events inside a list item and promotes or demotes it.
  [DefaultAuthorActionEventHandler.CiElementAndOffset](DefaultAuthorActionEventHandler.CiElementAndOffset.md)
A simple structure to return from the method getInsertableFormForElement both the CIElement that can be inserted for a given element and the offset that should be applied to the insertion position in order to insert it.
  [DITAAuthorActionEventHandler](DITAAuthorActionEventHandler.md)
Author action event handler for DITA.
  [DITAConrefsResolverBase](DITAConrefsResolverBase.md)
Resolve references when showing DITA content in the editor
  [DITAMapReferencesResolver](DITAMapReferencesResolver.md)
Resolve references when showing a DITA Map in the editor
  [DocbookAuthorActionEventHandler](DocbookAuthorActionEventHandler.md)
Author action event handler for DocBook.
  [DocumentContentChangedEvent](DocumentContentChangedEvent.md)
Event received by an [AuthorListener](AuthorListener.md) when changes have been made in the content of the [AuthorDocument](node/AuthorDocument.md).
  [DocumentContentDeletedEvent](DocumentContentDeletedEvent.md)
Event received by an [AuthorListener](AuthorListener.md) when a deletion has been made in the content of the [AuthorDocument](node/AuthorDocument.md).
  [DocumentContentInsertedEvent](DocumentContentInsertedEvent.md)
Event received by an [AuthorListener](AuthorListener.md) when insertion have been made in the content of the [AuthorDocument](node/AuthorDocument.md).
  [DocumentTypeAdvancedCustomRuleMatcher](DocumentTypeAdvancedCustomRuleMatcher.md)
Abstract class which can be implemented to provide custom matching to the document type it belongs to.
  [DocumentTypeCustomRuleMatcher](DocumentTypeCustomRuleMatcher.md)
Interface which can be implemented to provide custom matching to the document type it belongs to.
  [EditedAttribute](EditedAttribute.md)
Edited attribute information, like QName, element's QName and the proxy namespace mapping.
  [EditPropertiesHandler](EditPropertiesHandler.md)
A custom implementation to handle editing properties for an author node.
  [EditPropertiesHandlerAdapter](EditPropertiesHandlerAdapter.md)
Adapter class.
  [ErrorResolverContextInfo](ErrorResolverContextInfo.md)
Class that contains some information about the current error.
  [Extension](Extension.md)
The base interface for all Oxygen extensions classes.
  [ExtensionsBundle](ExtensionsBundle.md)
Abstract class representing a bundle for all extensions handlers.
  [ExternalObjectInsertionSources](ExternalObjectInsertionSources.md)
Drop and paste sources
  [InvalidEditException](InvalidEditException.md)
Exception thrown by [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) methods when an edit is considered invalid and must be rejected.
  [OptionChangedEvent](OptionChangedEvent.md)
Represents an event which indicates that the value of an option has been changed.
  [OptionListener](OptionListener.md)
The listener which is notified about the value changes of an author extension level option.
  [OptionsStorage](OptionsStorage.md)
This interface should be used if Author extension level options need to be stored and retrieved.
  [ProfilingConditionalTextProvider](ProfilingConditionalTextProvider.md)
**Profiling/Conditional Text** is a way to mark elements meant to appear in some renditions of the document, but not in others.
  [ReferenceErrorResolver](ReferenceErrorResolver.md)
Resolver for errors concerning references.
  [ReferenceErrorResolverExt](ReferenceErrorResolverExt.md)
Resolver for errors concerning references.
  [ReferenceResolverException](ReferenceResolverException.md)
Exception thrown if the reference resolver could not resolve a target.
  [ReferenceResolverSAXParseException](ReferenceResolverSAXParseException.md)
Exception thrown if the reference resolver could not resolve a target.
  [ReferenceType](ReferenceType.md)
The type of a resource denoted by an URL.
  [SelectionInterpretationMode](SelectionInterpretationMode.md)
Impose how the selection is interpreted by the application.
  [SpellCheckingProblemInfo](SpellCheckingProblemInfo.md)

 [SpellCheckingProblemInfoWithSuggestions](SpellCheckingProblemInfoWithSuggestions.md)

 [SpellSuggestionsInfo](SpellSuggestionsInfo.md)
Container for spellchecking suggestions information.
  [StylesFilter](StylesFilter.md)
Filter for the element styles.
  [SWTExtension](SWTExtension.md)
The base interface for all SWT Oxygen extension classes.
  [TEIAuthorActionEventHandler](TEIAuthorActionEventHandler.md)
Author action event handler for TEI.
  [TooltipIconInfo](TooltipIconInfo.md)
The information(tooltip and icon) used to describe the editing of the value for an attribute.
  [UniqueAttributesProcessor](UniqueAttributesProcessor.md)
Identifies unique attributes like ID's.
  [UniqueAttributesRecognizer](UniqueAttributesRecognizer.md)
Identifies unique attributes like ID's.
  [ValidatingAuthorReferenceResolver](ValidatingAuthorReferenceResolver.md)
This resolver also validates the target
  [ValidatingReferenceResolverException](ValidatingReferenceResolverException.md)
Exception thrown if the source does not accept the target as a resolved reference
  [WebappCompatible](WebappCompatible.md)
Annotation that should be placed on AuthorOperations to indicate whether they are suitable to be invoked from the WebApp.
  [WebappExtensionsProvider](WebappExtensionsProvider.md)
Web Author specific extensions for a document type.
  [WidthRepresentation](WidthRepresentation.md)
Specifies the fixed and relative width determined from the value of width/colwidth attribute of the col.
  [WidthRepresentation.Unit](WidthRepresentation.Unit.md)
The fixed width unit.
  [XHTMLAuthorActionEventHandler](XHTMLAuthorActionEventHandler.md)
Author action event handler for XHTML.
  [XPathVersion](XPathVersion.md)
XPath version types.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
