Package [ro.sync.exml.workspace.api.editor](package-summary.md)

# Interface WSEditor
    All Superinterfaces: [EditorPageConstants](../../../editor/EditorPageConstants.md), [ModifiedStatusProvider](../base/ModifiedStatusProvider.md), [ScenarioInvoker](ScenarioInvoker.md), [TransformationScenarioInvoker](transformation/TransformationScenarioInvoker.md), [ValidationScenarioInvoker](validation/ValidationScenarioInvoker.md), [WSEditorBase](WSEditorBase.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WSEditorextends [WSEditorBase](WSEditorBase.md), [EditorPageConstants](../../../editor/EditorPageConstants.md)
Provides access to methods related to the editor actions and information.
  Since: 11.2
## Field Summary

### Fields inherited from interface ro.sync.exml.editor.[EditorPageConstants](../../../editor/EditorPageConstants.md)
 [HIGHLIGHT_CLASS_DEBUGGER_CONTEXT](../../../editor/EditorPageConstants.md#HIGHLIGHT_CLASS_DEBUGGER_CONTEXT), [PAGE_AUTHOR](../../../editor/EditorPageConstants.md#PAGE_AUTHOR), [PAGE_DESIGN](../../../editor/EditorPageConstants.md#PAGE_DESIGN), [PAGE_DITA_MAP](../../../editor/EditorPageConstants.md#PAGE_DITA_MAP), [PAGE_GRID](../../../editor/EditorPageConstants.md#PAGE_GRID), [PAGE_TEXT](../../../editor/EditorPageConstants.md#PAGE_TEXT), [PAGE_UNKNOWN](../../../editor/EditorPageConstants.md#PAGE_UNKNOWN)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addEditorListener](#addEditorListener(ro.sync.exml.workspace.api.listeners.WSEditorListener))([WSEditorListener](../listeners/WSEditorListener.md) editorListener)
Add a listener for editor related events.
  void [addPageChangedListener](#addPageChangedListener(ro.sync.exml.workspace.api.listeners.WSEditorPageChangedListener))([WSEditorPageChangedListener](../listeners/WSEditorPageChangedListener.md) pageChangedListener)
Add a listener for page changed events.
  void [addValidationProblemsFilter](#addValidationProblemsFilter(ro.sync.exml.workspace.api.editor.validation.ValidationProblemsFilter))([ValidationProblemsFilter](validation/ValidationProblemsFilter.md) validationProblemsFilter)
Add a filter for problems encountered during validation of the current editor.
  void [changePage](#changePage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pageID)
Change the current selected page in the editor.
  boolean [checkValid](#checkValid())()
Check if the current editor is valid, performs manual validation and returns trueif the last validation was finished without errors or warnings.
  boolean [checkValid](#checkValid(boolean))(boolean automatic)
Check if the current editor is valid, performs manual validation and returns trueif the last validation was finished without errors or warnings.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getComponent](#getComponent())()
Get the internal component (Swing or SWT based) which represents the editor (the editor in its turn has multiple pages, each with its subcomponent).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContentType](#getContentType())()
Get the content type of the editor ("text/xml" for XML, "text/css" for CSS, etc).
  [WSEditorPage](page/WSEditorPage.md) [getCurrentPage](#getCurrentPage())()
Get access to the current page.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCurrentPageID](#getCurrentPageID())()
Get the ID of the current page.
  [WSEditorListener](../listeners/WSEditorListener.md)[] [getEditorListeners](#getEditorListeners())()
Get a list with all editor listeners, never null.
  boolean [isEditable](#isEditable())()
Check if the document can be edited.
  void [reload](#reload())()
Reload this opened document from the resource from which it was originally opened.
  void [reloadIfChangeOnDiskDetected](#reloadIfChangeOnDiskDetected())()
If the opened file is local, this method compares the current file timestamp with the previous file timestamp from when the document was opened.
  void [removeEditorListener](#removeEditorListener(ro.sync.exml.workspace.api.listeners.WSEditorListener))([WSEditorListener](../listeners/WSEditorListener.md) editorListener)
Remove the listener for editor events.
  void [removePageChangedListener](#removePageChangedListener(ro.sync.exml.workspace.api.listeners.WSEditorPageChangedListener))([WSEditorPageChangedListener](../listeners/WSEditorPageChangedListener.md) pageChangedListener)
Remove the listener for page changed events.
  void [removeValidationProblemsFilter](#removeValidationProblemsFilter(ro.sync.exml.workspace.api.editor.validation.ValidationProblemsFilter))([ValidationProblemsFilter](validation/ValidationProblemsFilter.md) validationProblemsFilter)
Remove a filter for problems encountered during validation of the current editor.
  void [setEditable](#setEditable(boolean))(boolean editable)
Sets the specified flag to indicate whether or not this opened editor should be editable.

### Methods inherited from interface ro.sync.exml.workspace.api.base.[ModifiedStatusProvider](../base/ModifiedStatusProvider.md)
 [isModified](../base/ModifiedStatusProvider.md#isModified())
### Methods inherited from interface ro.sync.exml.workspace.api.editor.transformation.[TransformationScenarioInvoker](transformation/TransformationScenarioInvoker.md)
 [runTransformationScenario](transformation/TransformationScenarioInvoker.md#runTransformationScenario(java.lang.String,java.util.Map,ro.sync.exml.workspace.api.editor.transformation.TransformationFeedback)), [runTransformationScenarios](transformation/TransformationScenarioInvoker.md#runTransformationScenarios(java.lang.String%5B%5D,ro.sync.exml.workspace.api.editor.transformation.TransformationFeedback)), [stopCurrentTransformationScenario](transformation/TransformationScenarioInvoker.md#stopCurrentTransformationScenario())
### Methods inherited from interface ro.sync.exml.workspace.api.editor.validation.[ValidationScenarioInvoker](validation/ValidationScenarioInvoker.md)
 [runValidationScenarios](validation/ValidationScenarioInvoker.md#runValidationScenarios(java.lang.String%5B%5D))
### Methods inherited from interface ro.sync.exml.workspace.api.editor.[WSEditorBase](WSEditorBase.md)
 [close](WSEditorBase.md#close(boolean)), [createContentInputStream](WSEditorBase.md#createContentInputStream()), [createContentReader](WSEditorBase.md#createContentReader()), [getDocumentTypeInformation](WSEditorBase.md#getDocumentTypeInformation()), [getEditorLocation](WSEditorBase.md#getEditorLocation()), [getEncodingForSerialization](WSEditorBase.md#getEncodingForSerialization()), [isNewDocument](WSEditorBase.md#isNewDocument()), [reloadContent](WSEditorBase.md#reloadContent(java.io.Reader)), [reloadContent](WSEditorBase.md#reloadContent(java.io.Reader,boolean)), [save](WSEditorBase.md#save()), [saveAs](WSEditorBase.md#saveAs(java.net.URL)), [setEditorTabText](WSEditorBase.md#setEditorTabText(java.lang.String)), [setEditorTabTooltipText](WSEditorBase.md#setEditorTabTooltipText(java.lang.String)), [setModified](WSEditorBase.md#setModified(boolean))
## Method Details

### getCurrentPage

[WSEditorPage](page/WSEditorPage.md) getCurrentPage()

Get access to the current page.
  Returns: the current page access. Can be null for pages which do not have special access methods (for example Grid or Design). For the Text page this return an implementation of [WSTextEditorPage](page/text/WSTextEditorPage.md). If the Text page is for an XML Editor, this return an implementation of [WSXMLTextEditorPage](page/text/xml/WSXMLTextEditorPage.md). For the Author page this return an implementation of [WSAuthorEditorPage](page/author/WSAuthorEditorPage.md). Note that in Reviewer edition only the Author page is available.
### getCurrentPageID

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCurrentPageID()

Get the ID of the current page.
  Returns: The ID of the page, one of the constant fields: [EditorPageConstants.PAGE_TEXT](../../../editor/EditorPageConstants.md#PAGE_TEXT), [EditorPageConstants.PAGE_AUTHOR](../../../editor/EditorPageConstants.md#PAGE_AUTHOR), [EditorPageConstants.PAGE_GRID](../../../editor/EditorPageConstants.md#PAGE_GRID), [EditorPageConstants.PAGE_DESIGN](../../../editor/EditorPageConstants.md#PAGE_DESIGN), [EditorPageConstants.PAGE_DITA_MAP](../../../editor/EditorPageConstants.md#PAGE_DITA_MAP) Note that in Reviewer edition only the Author page is available.
### addPageChangedListener

void addPageChangedListener([WSEditorPageChangedListener](../listeners/WSEditorPageChangedListener.md) pageChangedListener)

Add a listener for page changed events.
  Parameters: pageChangedListener - The page changed listener. Note that in Reviewer edition only the Author page is available. Since: 12
### removePageChangedListener

void removePageChangedListener([WSEditorPageChangedListener](../listeners/WSEditorPageChangedListener.md) pageChangedListener)

Remove the listener for page changed events.
  Parameters: pageChangedListener - The page changed listener. Note that in Reviewer edition only the Author page is available. Since: 12
### addEditorListener

void addEditorListener([WSEditorListener](../listeners/WSEditorListener.md) editorListener)

Add a listener for editor related events.
  Parameters: editorListener - The editor listener. Since: 13
### getEditorListeners

[WSEditorListener](../listeners/WSEditorListener.md)[] getEditorListeners()

Get a list with all editor listeners, never null.
  Returns: a list with all registered editor listeners, never null. Since: 16
### removeEditorListener

void removeEditorListener([WSEditorListener](../listeners/WSEditorListener.md) editorListener)

Remove the listener for editor events.
  Parameters: editorListener - The editor listener. Since: 13
### changePage

void changePage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pageID)

Change the current selected page in the editor. This does not affect editors opened in the DITA Maps Manager. If problems occur during the page switch or the page ID is not recognized the page will be switched to Text and the operation is aborted. Note that in Reviewer edition only the Author page is available.
  Parameters: pageID - The ID of the page, one of the constant fields: [EditorPageConstants.PAGE_TEXT](../../../editor/EditorPageConstants.md#PAGE_TEXT), [EditorPageConstants.PAGE_AUTHOR](../../../editor/EditorPageConstants.md#PAGE_AUTHOR), [EditorPageConstants.PAGE_GRID](../../../editor/EditorPageConstants.md#PAGE_GRID), [EditorPageConstants.PAGE_DESIGN](../../../editor/EditorPageConstants.md#PAGE_DESIGN) Since: 13
### addValidationProblemsFilter

void addValidationProblemsFilter([ValidationProblemsFilter](validation/ValidationProblemsFilter.md) validationProblemsFilter)

Add a filter for problems encountered during validation of the current editor. Validation can be manual or automatic. Automatic validation is done when modifications occur in the XML file.
  Parameters: validationProblemsFilter - a filter for problems encountered during validation of the current editor. Since: 13
### removeValidationProblemsFilter

void removeValidationProblemsFilter([ValidationProblemsFilter](validation/ValidationProblemsFilter.md) validationProblemsFilter)

Remove a filter for problems encountered during validation of the current editor. Validation can be manual or automatic. Automatic validation is done when modifications occur in the XML file.
  Parameters: validationProblemsFilter - a filter for problems encountered during validation of the current editor. Since: 13
### checkValid

boolean checkValid()

Check if the current editor is valid, performs manual validation and returns trueif the last validation was finished without errors or warnings. For document types which do not support validation, this returns always true. If you want to see the problems reported by the validation process you can add a validation problems filter [addValidationProblemsFilter(ValidationProblemsFilter)](#addValidationProblemsFilter(ro.sync.exml.workspace.api.editor.validation.ValidationProblemsFilter)).
  Returns: true if right now no error is reported on the editor content. Since: 17.1
### checkValid

boolean checkValid(boolean automatic)

Check if the current editor is valid, performs manual validation and returns trueif the last validation was finished without errors or warnings. For document types which do not support validation, this returns always true. If you want to see the problems reported by the validation process you can add a validation problems filter [addValidationProblemsFilter(ValidationProblemsFilter)](#addValidationProblemsFilter(ro.sync.exml.workspace.api.editor.validation.ValidationProblemsFilter)).
  Parameters: automatic - true If Oxygen performs automatic validation (identical with the validation performed when the document is modified) or false if Oxygen should perform manual validation (identical to the validation made when you press the Validate toolbar action). Returns: true if right now no error is reported on the editor content. Since: 18
### getComponent

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getComponent()

Get the internal component (Swing or SWT based) which represents the editor (the editor in its turn has multiple pages, each with its subcomponent). Use of this method is discouraged but it may be useful in some cases like: This can be helpful when you want to set a busy cursor on the entire editor or when you want to get access to the swing JTabbedPane pane where the editor is located.
  Returns: for the stand alone version, a javax.swing.JPanel and for the eclipse implementation of org.eclipse.ui.part.EditorPart. Since: 17.1
### setEditable

void setEditable(boolean editable)

Sets the specified flag to indicate whether or not this opened editor should be editable. This method is not available in the Oxygen Eclipse plugin which relies on the IEditorInput for the information.
  Parameters: editable - true if the editor should be editable. Since: 18
### isEditable

boolean isEditable()

Check if the document can be edited. A document can be set as read-only from API, by using the [setEditable(boolean)](#setEditable(boolean)) method.
  Returns: true if the document is editable. Since: 18
### getContentType

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContentType()

Get the content type of the editor ("text/xml" for XML, "text/css" for CSS, etc).
  Returns: the content type. Never null. Since: 22
### reloadIfChangeOnDiskDetected

void reloadIfChangeOnDiskDetected()

If the opened file is local, this method compares the current file timestamp with the previous file timestamp from when the document was opened. If the timestamps differ the document will be reloaded or the user will be asked if the document contains unsaved modifications.This method is implemented only for the desktop version of the application.
  Since: 26.1
### reload

void reload()

Reload this opened document from the resource from which it was originally opened. If the document contains unsaved changes, the end user is asked if they want to continue the reload and lose the modifications.This method is implemented only for the desktop version of the application.
  Since: 26.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
