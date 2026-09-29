Package [ro.sync.exml.editor](package-summary.md)

# Interface EditorTemplate
    All Superinterfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), [PersistentObject](../../options/PersistentObject.md), [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)   All Known Subinterfaces: [EditorTemplateWithContent](../../template/EditorTemplateWithContent.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface EditorTemplateextends [PersistentObject](../../options/PersistentObject.md)
Used to create a new editor for a given extension. It also has a description

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [ARCHIVE_TEMPLATE](#ARCHIVE_TEMPLATE)
The archive template type.
  static final int [EDITOR_TEMPLATE](#EDITOR_TEMPLATE)
The new editor template type.
  static final int [FILE_TEMPLATE](#FILE_TEMPLATE)
The classic type of template represented by a file on HDD.
  static final int [PROJECT_ARCHIVE_TEMPLATE](#PROJECT_ARCHIVE_TEMPLATE)
The archived project template type.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()
Clone this editor template.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAdditionalInformation](#getAdditionalInformation())()
Return additional information about this template (e.g.
  int [getCaretPosition](#getCaretPosition())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCustomizePageID](#getCustomizePageID())()
Get the ID representing the page used for customizing the template.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()
Return the template description.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getExtension](#getExtension())()
Return the template extension.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFilenamePrefix](#getFilenamePrefix())()
A template can have the "filenamePrefix" property specified in its ".properties" file, whose value will be used as the prefix of the names of all the documents to be created.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFilenameSuffix](#getFilenameSuffix())()
A template can have the "filenameSuffix" property specified in its ".properties" file, whose value will be used as the suffix of the names of all the documents to be created.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLongDescription](#getLongDescription())()
Return the template's description which will be shown as a tooltip.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Return the template name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSource](#getSource())()

 int [getTemplateType](#getTemplateType())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTypeProperty](#getTypeProperty())()

 boolean [isCustomizable](#isCustomizable())()

### Methods inherited from interface ro.sync.options.[PersistentObject](../../options/PersistentObject.md)
 [checkValid](../../options/PersistentObject.md#checkValid()), [getNotPersistentFieldNames](../../options/PersistentObject.md#getNotPersistentFieldNames())
## Field Details

### EDITOR_TEMPLATE

static final int EDITOR_TEMPLATE

The new editor template type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.editor.EditorTemplate.EDITOR_TEMPLATE)

### FILE_TEMPLATE

static final int FILE_TEMPLATE

The classic type of template represented by a file on HDD.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.editor.EditorTemplate.FILE_TEMPLATE)

### ARCHIVE_TEMPLATE

static final int ARCHIVE_TEMPLATE

The archive template type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.editor.EditorTemplate.ARCHIVE_TEMPLATE)

### PROJECT_ARCHIVE_TEMPLATE

static final int PROJECT_ARCHIVE_TEMPLATE

The archived project template type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.editor.EditorTemplate.PROJECT_ARCHIVE_TEMPLATE)

## Method Details

### getDescription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()

Return the template description.
  Returns: The template description.
### getExtension

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getExtension()

Return the template extension.
  Returns: The template extension.
### getSource

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSource()
  Returns: A description from where this template was loaded.
### getTemplateType

int getTemplateType()
  Returns: The template type. Currently one of: EDITOR_TEMPLATE, FILE_TEMPLATE or ARCHIVE_TEMPLATE.
### clone

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone()

Clone this editor template.
  Specified by: [clone](../../options/PersistentObject.md#clone()) in interface [PersistentObject](../../options/PersistentObject.md) Returns: The clone or null if unsuccessful.
### getName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

Return the template name.
  Returns: The template name.
### getAdditionalInformation

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAdditionalInformation()

Return additional information about this template (e.g. Framework, Path etc).
  Returns: Additional information.
### isCustomizable

boolean isCustomizable()
  Returns: true if the template can be customized.
### getCustomizePageID

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCustomizePageID()

Get the ID representing the page used for customizing the template.
  Returns: The ID representing the page used for customizing the template.
### getCaretPosition

int getCaretPosition()
  Returns: The caret position to be set after loading the template.
### getLongDescription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLongDescription()

Return the template's description which will be shown as a tooltip.
  Returns: The template long description.
### getTypeProperty

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTypeProperty()
  Returns: The type property (from the .properties file) for the current template. Can be: 'dita', 'general' or possibly others.
### getFilenamePrefix

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFilenamePrefix()

A template can have the "filenamePrefix" property specified in its ".properties" file, whose value will be used as the prefix of the names of all the documents to be created. This method returns the value of the "filenamePrefix" property or null if the property is not set.
  Returns: the value of the "filenamePrefix" property, which is used as the prefix of a new file created from this template. Since: 18
### getFilenameSuffix

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFilenameSuffix()

A template can have the "filenameSuffix" property specified in its ".properties" file, whose value will be used as the suffix of the names of all the documents to be created. This method returns the value of the "filenameSuffix" property or null if the property is not set.
  Returns: the value of the "filenameSuffix" property, which is used as the prefix of a new file created from this template. Since: 18
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
