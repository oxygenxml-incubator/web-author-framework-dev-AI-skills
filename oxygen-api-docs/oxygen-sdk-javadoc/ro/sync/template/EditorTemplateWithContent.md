Package [ro.sync.template](package-summary.md)

# Interface EditorTemplateWithContent
    All Superinterfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), [EditorTemplate](../exml/editor/EditorTemplate.md), [PersistentObject](../options/PersistentObject.md), [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface EditorTemplateWithContentextends [EditorTemplate](../exml/editor/EditorTemplate.md)
Editor template with predefined string content.

## Field Summary

### Fields inherited from interface ro.sync.exml.editor.[EditorTemplate](../exml/editor/EditorTemplate.md)
 [ARCHIVE_TEMPLATE](../exml/editor/EditorTemplate.md#ARCHIVE_TEMPLATE), [EDITOR_TEMPLATE](../exml/editor/EditorTemplate.md#EDITOR_TEMPLATE), [FILE_TEMPLATE](../exml/editor/EditorTemplate.md#FILE_TEMPLATE), [PROJECT_ARCHIVE_TEMPLATE](../exml/editor/EditorTemplate.md#PROJECT_ARCHIVE_TEMPLATE)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [TemplateContentInfo](TemplateContentInfo.md) [getContentInfo](#getContentInfo(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) saveLocation)
Gets the template content.
  [TemplateContentInfo](TemplateContentInfo.md) [getContentInfo](#getContentInfo(java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) saveLocation, boolean interactive)
Returns the template content with editor variables expanded.
  [TemplateContentInfo](TemplateContentInfo.md) [getContentInfo](#getContentInfo(java.lang.String,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) saveLocation, boolean expandEditorVariables, boolean interactive)
Returns the template content with editor variables expanded.

### Methods inherited from interface ro.sync.exml.editor.[EditorTemplate](../exml/editor/EditorTemplate.md)
 [clone](../exml/editor/EditorTemplate.md#clone()), [getAdditionalInformation](../exml/editor/EditorTemplate.md#getAdditionalInformation()), [getCaretPosition](../exml/editor/EditorTemplate.md#getCaretPosition()), [getCustomizePageID](../exml/editor/EditorTemplate.md#getCustomizePageID()), [getDescription](../exml/editor/EditorTemplate.md#getDescription()), [getExtension](../exml/editor/EditorTemplate.md#getExtension()), [getFilenamePrefix](../exml/editor/EditorTemplate.md#getFilenamePrefix()), [getFilenameSuffix](../exml/editor/EditorTemplate.md#getFilenameSuffix()), [getLongDescription](../exml/editor/EditorTemplate.md#getLongDescription()), [getName](../exml/editor/EditorTemplate.md#getName()), [getSource](../exml/editor/EditorTemplate.md#getSource()), [getTemplateType](../exml/editor/EditorTemplate.md#getTemplateType()), [getTypeProperty](../exml/editor/EditorTemplate.md#getTypeProperty()), [isCustomizable](../exml/editor/EditorTemplate.md#isCustomizable())
### Methods inherited from interface ro.sync.options.[PersistentObject](../options/PersistentObject.md)
 [checkValid](../options/PersistentObject.md#checkValid()), [getNotPersistentFieldNames](../options/PersistentObject.md#getNotPersistentFieldNames())
## Method Details

### getContentInfo

[TemplateContentInfo](TemplateContentInfo.md) getContentInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) saveLocation)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), ro.sync.exml.editor.xmleditor.transform.CancelledException

Gets the template content.
  Parameters: saveLocation - The location where the new template will be saved. Returns: The template content. It can be null. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) ro.sync.exml.editor.xmleditor.transform.CancelledException
### getContentInfo

[TemplateContentInfo](TemplateContentInfo.md) getContentInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) saveLocation, boolean interactive)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), ro.sync.exml.editor.xmleditor.transform.CancelledException

Returns the template content with editor variables expanded.
  Parameters: saveLocation - The location where the content will be saved. interactive - true if we should expand interactive editor variables. Returns: The expanded content. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) ro.sync.exml.editor.xmleditor.transform.CancelledException
### getContentInfo

[TemplateContentInfo](TemplateContentInfo.md) getContentInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) saveLocation, boolean expandEditorVariables, boolean interactive)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), ro.sync.exml.editor.xmleditor.transform.CancelledException

Returns the template content with editor variables expanded.
  Parameters: saveLocation - The location where the content will be saved. expandEditorVariables - true to expand editor variables. interactive - true if we should expand interactive editor variables. Returns: The expanded content. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) ro.sync.exml.editor.xmleditor.transform.CancelledException
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
