Package [ro.sync.exml.workspace.api.editor.documenttype](package-summary.md)

# Interface DocumentTypeInformation
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface DocumentTypeInformation
Provides information about the document type configuration which was loaded for the current editor ('Document Type Association' preferences page). Only available for XML-type editors.
  Since: 16
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFrameworkStoreLocation](#getFrameworkStoreLocation())()
Returns the location on disk of the framework configuration.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getID](#getID())()
Returns the unique ID of the document type.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Returns the name of the document type.

## Method Details

### getFrameworkStoreLocation

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFrameworkStoreLocation()

Returns the location on disk of the framework configuration.
  Returns: The location on disk of the framework configuration.
### getName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

Returns the name of the document type.
  Returns: the name of the document type.
### getID

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getID()

Returns the unique ID of the document type.
  Returns: the unique ID of the document type. Since: 20
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
