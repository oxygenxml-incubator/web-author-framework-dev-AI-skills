Package [ro.sync.exml.workspace.api.editor](package-summary.md)

# Interface WSEditorBase
    All Superinterfaces: [ModifiedStatusProvider](../base/ModifiedStatusProvider.md), [ScenarioInvoker](ScenarioInvoker.md), [TransformationScenarioInvoker](transformation/TransformationScenarioInvoker.md), [ValidationScenarioInvoker](validation/ValidationScenarioInvoker.md)   All Known Subinterfaces: [AuthorEditorAccess](../../../../ecss/extensions/api/access/AuthorEditorAccess.md), [IWebappAuthorEditorAccess](../../../../ecss/extensions/api/webapp/access/IWebappAuthorEditorAccess.md), [WSEditor](WSEditor.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WSEditorBaseextends [ModifiedStatusProvider](../base/ModifiedStatusProvider.md), [ScenarioInvoker](ScenarioInvoker.md)
Provides access to methods related to the editor actions and information.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [close](#close(boolean))(boolean askForSave)
Closes the current editor.
  [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) [createContentInputStream](#createContentInputStream())()
Create a properly encoded input stream reader over the whole editor's content (exactly the XML content which gets saved on disk).
  [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) [createContentReader](#createContentReader())()
Create a reader over the whole editor's content (exactly the XML content which gets saved on disk).
  [DocumentTypeInformation](documenttype/DocumentTypeInformation.md) [getDocumentTypeInformation](#getDocumentTypeInformation())()
Get information about the current document type configuration used to edit the XML document.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getEditorLocation](#getEditorLocation())()
Get the [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) representing the editor location.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getEncodingForSerialization](#getEncodingForSerialization())()
Get the Java character encoding of this editor's content.In Eclipse, this method will return the encoding detected when opening the editor, and it will not be aware of encoding changes until the editor is re-opened.
  boolean [isNewDocument](#isNewDocument())()
This method can be used to determine if the document from the editor was ever saved.
  void [reloadContent](#reloadContent(java.io.Reader))([Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)
Update the whole content of the editor with the one taken from the reader.
  void [reloadContent](#reloadContent(java.io.Reader,boolean))([Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader, boolean discardUndoableEdits)
Update the whole content of the editor with the one taken from the reader.
  void [save](#save())()
Saves the editor content.
  void [saveAs](#saveAs(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) location)
Saves the editor content to a new location.
  void [setEditorTabText](#setEditorTabText(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabText)
Set the text which appears on the editor's tab, by default it is the loaded file name.
  void [setEditorTabTooltipText](#setEditorTabTooltipText(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabTooltip)
Set the tooltip text for the editor's tab, by default it is the loaded file path.
  void [setModified](#setModified(boolean))(boolean modified)
Set the modified status of the editor document.

### Methods inherited from interface ro.sync.exml.workspace.api.base.[ModifiedStatusProvider](../base/ModifiedStatusProvider.md)
 [isModified](../base/ModifiedStatusProvider.md#isModified())
### Methods inherited from interface ro.sync.exml.workspace.api.editor.transformation.[TransformationScenarioInvoker](transformation/TransformationScenarioInvoker.md)
 [runTransformationScenario](transformation/TransformationScenarioInvoker.md#runTransformationScenario(java.lang.String,java.util.Map,ro.sync.exml.workspace.api.editor.transformation.TransformationFeedback)), [runTransformationScenarios](transformation/TransformationScenarioInvoker.md#runTransformationScenarios(java.lang.String%5B%5D,ro.sync.exml.workspace.api.editor.transformation.TransformationFeedback)), [stopCurrentTransformationScenario](transformation/TransformationScenarioInvoker.md#stopCurrentTransformationScenario())
### Methods inherited from interface ro.sync.exml.workspace.api.editor.validation.[ValidationScenarioInvoker](validation/ValidationScenarioInvoker.md)
 [runValidationScenarios](validation/ValidationScenarioInvoker.md#runValidationScenarios(java.lang.String%5B%5D))
## Method Details

### getEncodingForSerialization

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getEncodingForSerialization()

Get the Java character encoding of this editor's content.In Eclipse, this method will return the encoding detected when opening the editor, and it will not be aware of encoding changes until the editor is re-opened.
  Returns: the Java encoding of the content. May be null if couldn't be detected. Since: 19.1
### getEditorLocation

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getEditorLocation()

Get the [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) representing the editor location.
  Returns: The editor location. It cannot be null.
### save

void save()

Saves the editor content.

### saveAs

void saveAs([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) location)

Saves the editor content to a new location. This method is not implemented in the Oxygen Eclipse plugin.
  Parameters: location - The new editor location. Since: 13
### close

boolean close(boolean askForSave)

Closes the current editor.
If the editor has unsaved content and askForSave is true, the user will be given the opportunity to save it.

  Parameters: askForSave - true to save the editor contents if required, and false to discard any unsaved changes. Returns: true if the editor was successfully closed, and false if the editor is still open
### setModified

void setModified(boolean modified)

Set the modified status of the editor document.
For SWT the result of this method is guaranteed only when working exclusively with the author page. If the text page contains modifications (and is marked as dirty) this method is unable to change its state to unmodified.

For Web Author, can be used to mark the document as clean and to make sure that the clean state is properly identified after a series of undo/redo operations. This method has some limitations:

        *  It does not automatically update the client-side editor dirty status.
        *  It does nothing if invoked during a "compound edit" (see AuthorDocumentController.beginCompoundEdit()). Note that a "compound edit" is created automatically when invoking an AuthorOperation that does not extend AuthorOperationWithCustomUndoBehavior.
        * it does nothing if invoked with false.

  Parameters: modified - true if the document in the current editor contains unsaved modifications.
### isNewDocument

boolean isNewDocument()

This method can be used to determine if the document from the editor was ever saved.
  Returns: true if the document in the current editor is new.
### createContentReader

[Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) createContentReader()

Create a reader over the whole editor's content (exactly the XML content which gets saved on disk). The unsaved changes are included. If for the Author page change tracking highlights are present, they are also included as processing instructions.
  Returns: The content reader.In normal circumstances the reader should not be null. See Also:
        * for the processing instruction names

### createContentInputStream

[InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) createContentInputStream() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Create a properly encoded input stream reader over the whole editor's content (exactly the XML content which gets saved on disk). The unsaved changes are included. If for the Author page change tracking highlights are present, they are also included as processing instructions.
  Returns: An input stream over the XML contents.In normal circumstances the input stream should not be null. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If an I/O exception occurs. Since: 15.2 See Also:
        * for the processing instruction names

### reloadContent

void reloadContent([Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)

Update the whole content of the editor with the one taken from the reader. This will lose undo history and any modifications the editor may have.
  Parameters: reader - The reader provided by the extension.
### reloadContent

void reloadContent([Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader, boolean discardUndoableEdits)

Update the whole content of the editor with the one taken from the reader. This will lose any modifications the editor may have unless discardUndoableEdits is false in which case you will be able to UNDO the editor to the content prior to the reload.
  Parameters: reader - The reader provided by the extension. discardUndoableEdits - true to lose undo history. Since: 13.2
### setEditorTabText

void setEditorTabText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabText)

Set the text which appears on the editor's tab, by default it is the loaded file name. Set it with the value NULL to reset the tab title to the default value (the loaded file name).
  Parameters: tabText - the text which appears on the editor's tab, by default it is the loaded file name. NULL to reset the tab title to the default value (the loaded file name). Since: 12.1
### setEditorTabTooltipText

void setEditorTabTooltipText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabTooltip)

Set the tooltip text for the editor's tab, by default it is the loaded file path. Set it with the value NULL to reset the tab title to the default value (the loaded file path).
  Parameters: tabTooltip - the tooltip for the editor's tab, by default it is the loaded file path. NULL to reset the tab tooltip to the default value (the loaded file path). Since: 12.1
### getDocumentTypeInformation

[DocumentTypeInformation](documenttype/DocumentTypeInformation.md) getDocumentTypeInformation()

Get information about the current document type configuration used to edit the XML document.
  Returns: information about the current document type configuration used to edit the XML document or null if no document type configuration is matched or the editor does not have an XML content type. Since: 16.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
