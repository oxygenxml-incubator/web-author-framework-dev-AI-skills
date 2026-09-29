Package [ro.sync.exml.workspace.api.markdown](package-summary.md)

# Interface MarkdownValidator
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface MarkdownValidator
Implementations of this interface are used to validate markdown documents.
  Since: 22
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)> [validate](#validate(java.lang.String,java.io.Reader))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) documentReader)
Validates the passed in markdown content and returns a list of errors or an empty list if the document is valid.

## Method Details

### validate

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)> validate([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) documentReader)

Validates the passed in markdown content and returns a list of errors or an empty list if the document is valid. Note: The validator may check the existence of external resources (e.g. images) referred in the document with relative URLs. The given system ID in this case can be used to resolve those URLs.
  Parameters: systemID - the system ID of the document to be validated. Can be null. Passing a null value for systemID may result in incorrect position (line, column) for the reported errors. documentReader - the reader of the markdown document Returns: list of validation errors or empty list if the document is valid
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
