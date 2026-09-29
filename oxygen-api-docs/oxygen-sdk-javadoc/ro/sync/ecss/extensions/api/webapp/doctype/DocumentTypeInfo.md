Package [ro.sync.ecss.extensions.api.webapp.doctype](package-summary.md)

# Interface DocumentTypeInfo
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface DocumentTypeInfo
Information about a document type.
  Since: 15.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorResourceBundle](../../AuthorResourceBundle.md) [getAuthorResourceBundle](#getAuthorResourceBundle())()
A message bundle that holds all the internationalized messages contrbuted by the current document type.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSGroup](../../../../../exml/workspace/api/editor/page/author/css/CSSGroup.md)> [getAvailableCssGroups](#getAvailableCssGroups())()
Returns the list of CSS groups defined in the framework.
  [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [getBaseFrameworkFolder](#getBaseFrameworkFolder())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()
Returns a description of the framework.
  [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [getFrameworkFile](#getFrameworkFile())()
Returns the location on disk of the framework file.
  [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [getFrameworkFolder](#getFrameworkFolder())()
Returns the location on disk of the framework folder.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getId](#getId())()
Returns the id of the document type.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Returns the name of the framework.
  int [getPriority](#getPriority())()
Getter for the document type priority.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)> [getWebResources](#getWebResources())()

 boolean [isEnabled](#isEnabled())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [validate](#validate())()
Checks if the framework contains invalid references.

## Method Details

### getFrameworkFolder

[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) getFrameworkFolder()

Returns the location on disk of the framework folder.
  Returns: The location on disk of the framework folder.
### getBaseFrameworkFolder

[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) getBaseFrameworkFolder()
  Returns: The location on disk of the base framework folder or null if this document type is not an extension. Since: 18.1.1
### getFrameworkFile

[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) getFrameworkFile()

Returns the location on disk of the framework file.
  Returns: The location on disk of the framework file.
### getId

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getId()

Returns the id of the document type.
  Returns: the id of the document type.
### getDescription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()

Returns a description of the framework.
  Returns: a description of the framework.
### getName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

Returns the name of the framework.
  Returns: the name of the framework.
### isEnabled

boolean isEnabled()
  Returns: true if the framework is enabled.
### getAvailableCssGroups

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSGroup](../../../../../exml/workspace/api/editor/page/author/css/CSSGroup.md)> getAvailableCssGroups()

Returns the list of CSS groups defined in the framework.
  Returns: The list of CSS groups defined in the framework. Since: 20.1
### getWebResources

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)> getWebResources()
  Returns: a list of JS files or folders containing js files that will be loaded client-side by the Web Author. Since: 23.1
### getAuthorResourceBundle

[AuthorResourceBundle](../../AuthorResourceBundle.md) getAuthorResourceBundle()

A message bundle that holds all the internationalized messages contrbuted by the current document type.
  Returns: The message bundle. Since: 24
### getPriority

int getPriority()

Getter for the document type priority.
  Returns: the document type priority (value between 1 and 5) used when matching to a document. Since: 24.1
### validate

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> validate()

Checks if the framework contains invalid references.
  Returns: A list of validation error messages or an empty list if the framework is valid.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
