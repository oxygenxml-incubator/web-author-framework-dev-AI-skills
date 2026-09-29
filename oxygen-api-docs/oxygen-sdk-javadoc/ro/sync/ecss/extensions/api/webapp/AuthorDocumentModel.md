Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Interface AuthorDocumentModel
    All Superinterfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)   All Known Subinterfaces: [DITAMapDocumentModel](../../../webapp/ditamap/DITAMapDocumentModel.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorDocumentModelextends [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)
The model of an XML document to be edited. It has the following components:
1. some associated CSS files
2. a schema used to validate the document and to propose elements to be inserted in a specific context.
3. a set of markers added by reviewers
4. a selection model
5. an undo manager that supports undoable edits
This class is a facade over all these components.
  Since: 15.1
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) [createReader](#createReader())()
Returns a reader over the document.
  ro.sync.ecss.extensions.api.webapp.AuthorNodesRenderer [createRenderer](#createRenderer(java.io.Writer))([Writer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Writer.html) writer)
Returns a renderer of the document to the specified writer.
  ro.sync.ecss.extensions.api.webapp.AuthorNodesRenderer [createRenderer](#createRenderer(java.io.Writer,ro.sync.ecss.extensions.api.highlights.AuthorHighlighter))([Writer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Writer.html) writer, [AuthorHighlighter](../highlights/AuthorHighlighter.md) highlighter)
Returns a renderer of the document to the specified writer.
  void [dispose](#dispose())()
Dispose the current document.
  [WebappActionsManager](WebappActionsManager.md) [getActionsManager](#getActionsManager())()

 [WebappAuthorSchemaAwareActionsHandler](WebappAuthorSchemaAwareActionsHandler.md) [getActionsSupport](#getActionsSupport())()
Returns the schema aware actions handler.
  [AttributesManager](attributes/AttributesManager.md) [getAttributesManager](#getAttributesManager())()
Returns the attribute manager offering attributes support.
  [AuthorAccess](../AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()
Returns the Autor access object.
  [AuthorDocumentController](../AuthorDocumentController.md) [getAuthorDocumentController](#getAuthorDocumentController())()
Getter for the document controller.
  [ContentCompletionManager](cc/ContentCompletionManager.md) [getContentCompletionManager](#getContentCompletionManager())()
Returns the content completion manager that can be used to insert XML tags in the document such that the document remains valid according to its schema.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCssContent](#getCssContent())()
TODO (EXM-27739): split it into document-specific and doctype specific CSS in order to allow separate caching.
  ro.sync.exml.editor.xmleditor.DocumentTypeProvider [getDocTypeProvider](#getDocTypeProvider())()
Get document type provider.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentTypeId](#getDocumentTypeId())()
Returns the id of the document type of the document.
  [WebappDocumentValidator](WebappDocumentValidator.md) [getDocumentValidator](#getDocumentValidator())()

 [DPILocation](DPILocation.md) [getDPILocation](#getDPILocation(ro.sync.document.DocumentPositionedInfo))([DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md) dpInfo)  Deprecated.
use {[getDocumentValidator()](#getDocumentValidator()).
   [FormControlEditingHelper](formcontrols/FormControlEditingHelper.md) [getEditingHelper](#getEditingHelper())()
Returns the form control editing helper.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getEncoding](#getEncoding())()

 [FindReplaceSupport](findreplace/FindReplaceSupport.md) [getFindReplaceSupport](#getFindReplaceSupport())()
The support object for find and replace actions.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFloatingToolbarsJsonContent](#getFloatingToolbarsJsonContent())()
Returns the CSS that describes floating tool-bars as JSON.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLicenseeId](#getLicenseeId())()

 [WebappLockManager](WebappLockManager.md) [getLockManager](#getLockManager())()

 [AuthorIdIndex](AuthorIdIndex.md)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> [getMarkersIndexer](#getMarkersIndexer())()
Return an indexer that assigned IDs to all markers in the document.
  [WebappMessagesProvider](WebappMessagesProvider.md) [getMessageProvider](#getMessageProvider())()
Returns the message reporter.
  [AuthorIdIndex](AuthorIdIndex.md)<[AuthorNode](../node/AuthorNode.md)> [getNodeIndexer](#getNodeIndexer())()
Returns an indexer that assigned IDs to the nodes in the document.
  [ProfilingConditionAttributesManager](profiling/ProfilingConditionAttributesManager.md) [getProfilingConditionAttributesManager](#getProfilingConditionAttributesManager())()
Get the profiling condition attributes manager.
  ro.sync.quickfix.QuickFixExecutor [getQuickFixExecutor](#getQuickFixExecutor())()

 [ReviewController](review/ReviewController.md) [getReviewController](#getReviewController())()
Returns a review controller that can be used to perform actions on the markers present in the document.
  [AuthorSelectionAndCaretModel](../AuthorSelectionAndCaretModel.md) [getSelectionModel](#getSelectionModel())()
Returns the selection model of the document.
  [WebappSpellchecker](WebappSpellchecker.md) [getSpellchecker](#getSpellchecker())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getUserId](#getUserId())()
The ID that uniquely identifies the user that opened the document.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.exml.editor.scenario.BaseScenario> [getValidationScenarios](#getValidationScenarios())()  Deprecated.
use {[getDocumentValidator()](#getDocumentValidator()).
   [Callable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/concurrent/Callable.html)<[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)>> [getValidationTask](#getValidationTask())()  Deprecated.
use {[getDocumentValidator()](#getDocumentValidator()).
   [WSEditor](../../../../exml/workspace/api/editor/WSEditor.md) [getWSEditor](#getWSEditor())()
Exposes some of the WSEditor functionality for the current document.
  void [setUserId](#setUserId(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) userId)
Sets the user id.

## Method Details

### getAuthorDocumentController

[AuthorDocumentController](../AuthorDocumentController.md) getAuthorDocumentController()

Getter for the document controller. The controller is used to perform undoable edits on the document content.
  Returns: the document controller.
### createRenderer

ro.sync.ecss.extensions.api.webapp.AuthorNodesRenderer createRenderer([Writer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Writer.html) writer)

Returns a renderer of the document to the specified writer.
  Parameters: writer - The writer Returns: The renderer Since: 26.1
### createRenderer

ro.sync.ecss.extensions.api.webapp.AuthorNodesRenderer createRenderer([Writer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Writer.html) writer, [AuthorHighlighter](../highlights/AuthorHighlighter.md) highlighter)

Returns a renderer of the document to the specified writer.
  Parameters: writer - The writer highlighter - The author highligher Returns: The renderer Since: 26.1
### createReader

[Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) createReader()

Returns a reader over the document. The reader serializes the current content of the document trying to match the indentation and line-width that were used in the document before the editing started.
  Returns: a reader over the document.
### getNodeIndexer

[AuthorIdIndex](AuthorIdIndex.md)<[AuthorNode](../node/AuthorNode.md)> getNodeIndexer()

Returns an indexer that assigned IDs to the nodes in the document. Note that only the rendered node have an ID assigned.
  Returns: The node indexer.
### getMarkersIndexer

[AuthorIdIndex](AuthorIdIndex.md)<[AuthorPersistentHighlight](../highlights/AuthorPersistentHighlight.md)> getMarkersIndexer()

Return an indexer that assigned IDs to all markers in the document.
  Returns: The marker indexer.
### getCssContent

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCssContent()

TODO (EXM-27739): split it into document-specific and doctype specific CSS in order to allow separate caching. Returns the CSS to be applied to the HTML document.
  Returns: The CSS to be applied to the HTML document.
### getFloatingToolbarsJsonContent

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFloatingToolbarsJsonContent()

Returns the CSS that describes floating tool-bars as JSON.
  Returns: the CSS that describes floating tool-bars as JSON.
### getProfilingConditionAttributesManager

[ProfilingConditionAttributesManager](profiling/ProfilingConditionAttributesManager.md) getProfilingConditionAttributesManager()

Get the profiling condition attributes manager.
  Returns: the profiling condition attributes manager. Since: 26
### getReviewController

[ReviewController](review/ReviewController.md) getReviewController()

Returns a review controller that can be used to perform actions on the markers present in the document.
  Returns: The review controller.
### getAttributesManager

[AttributesManager](attributes/AttributesManager.md) getAttributesManager()

Returns the attribute manager offering attributes support.
  Returns: The attribute manager.
### getContentCompletionManager

[ContentCompletionManager](cc/ContentCompletionManager.md) getContentCompletionManager()

Returns the content completion manager that can be used to insert XML tags in the document such that the document remains valid according to its schema.
  Returns: The content completion manager.
### getSelectionModel

[AuthorSelectionAndCaretModel](../AuthorSelectionAndCaretModel.md) getSelectionModel()

Returns the selection model of the document.
  Returns: The selection model.
### getValidationTask

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [Callable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/concurrent/Callable.html)<[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)>> getValidationTask()
 Deprecated.
use {[getDocumentValidator()](#getDocumentValidator()).

A task that tries to validate the document according to its schema and returns the list of found errors.
  Returns: The validation task for the current document.
### getEncoding

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getEncoding()
  Returns: The encoding of the document in Java format.
### getActionsManager

[WebappActionsManager](WebappActionsManager.md) getActionsManager()
  Returns: Actions support.
### getEditingHelper

[FormControlEditingHelper](formcontrols/FormControlEditingHelper.md) getEditingHelper()

Returns the form control editing helper.
  Returns: the form control editing helper.
### getActionsSupport

[WebappAuthorSchemaAwareActionsHandler](WebappAuthorSchemaAwareActionsHandler.md) getActionsSupport()

Returns the schema aware actions handler.
  Returns: The schema aware actions handler.
### getAuthorAccess

[AuthorAccess](../AuthorAccess.md) getAuthorAccess()

Returns the Autor access object.
  Returns: Returns the author access object.
### getMessageProvider

[WebappMessagesProvider](WebappMessagesProvider.md) getMessageProvider()

Returns the message reporter. It collects error/warning/info messages.
  Returns: The message reporter.
### getDocumentTypeId

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentTypeId()

Returns the id of the document type of the document.
  Returns: The id of the document type of the document.
### getValidationScenarios

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.exml.editor.scenario.BaseScenario> getValidationScenarios()
 Deprecated.
use {[getDocumentValidator()](#getDocumentValidator()).

Get validation scenarios associated with the document.
  Returns: Validation scenarios associated with the document.
### getDocTypeProvider

ro.sync.exml.editor.xmleditor.DocumentTypeProvider getDocTypeProvider()

Get document type provider.
  Returns: The document type provider.
### getDPILocation

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [DPILocation](DPILocation.md) getDPILocation([DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md) dpInfo)
 Deprecated.
use {[getDocumentValidator()](#getDocumentValidator()).

Compute for the given document position info the content offsets.
  Parameters: dpInfo - The document position info. Returns: The DPI location info.
### dispose

void dispose()

Dispose the current document. Its use after disposal produce undefined behavior.

### getFindReplaceSupport

[FindReplaceSupport](findreplace/FindReplaceSupport.md) getFindReplaceSupport()

The support object for find and replace actions.
  Returns: The support object for find and replace actions.
### getWSEditor

[WSEditor](../../../../exml/workspace/api/editor/WSEditor.md) getWSEditor()

Exposes some of the WSEditor functionality for the current document.
  Returns: An WSEditor adapter.
### getUserId

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getUserId()

The ID that uniquely identifies the user that opened the document.
  Returns: The ID of the user. By default we use the license ID.
### setUserId

void setUserId([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) userId)

Sets the user id.
  Parameters: userId - Sets the unique ID of the user that opened the document.
### getLicenseeId

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLicenseeId()
  Returns: The licensee ID which is unique for each browser connected to the webapp, even if the same person uses multiple browsers.
### getLockManager

[WebappLockManager](WebappLockManager.md) getLockManager()
  Returns: The lock manager for this document.
### getSpellchecker

[WebappSpellchecker](WebappSpellchecker.md) getSpellchecker()
  Returns: The spellchecker for this document.
### getQuickFixExecutor

ro.sync.quickfix.QuickFixExecutor getQuickFixExecutor()
  Returns: The quick fix executor for the current document.
### getDocumentValidator

[WebappDocumentValidator](WebappDocumentValidator.md) getDocumentValidator()
  Returns: An object that can be used to validate the content of the document. Since: 20.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
