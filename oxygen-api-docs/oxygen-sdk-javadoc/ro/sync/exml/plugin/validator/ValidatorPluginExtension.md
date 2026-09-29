Package [ro.sync.exml.plugin.validator](package-summary.md)

# Interface ValidatorPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ValidatorPluginExtensionextends [PluginExtension](../PluginExtension.md)
Plug-in extension that allows custom validation engines.
  Since: 24
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 boolean [allowsAutomaticValidation](#allowsAutomaticValidation())()
Check if the custom validation engine allows as you type validation which occurs every time the end user types.
  boolean [allowsValidation](#allowsValidation(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
Checks if the current document is accepted for this validation.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getEngineName](#getEngineName())()
Get the name of the engine.
  default void [setSchemaSystemID](#setSchemaSystemID(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) schemaSystemID)
Set the schema system ID in the custom validation engine, in case the validation engine needs a schema for validation.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../document/DocumentPositionedInfo.md)> [validate](#validate(java.lang.String,java.io.Reader,ro.sync.exml.plugin.validator.ValidationType,ro.sync.exml.plugin.validator.ValidationMode))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) documentReader, [ValidationType](ValidationType.md) validationType, [ValidationMode](ValidationMode.md) mode)
Validate the document and provide a list of problems.

## Method Details

### getEngineName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getEngineName()

Get the name of the engine. The name of the engine is shown to the end user as a possible option when they configure a validation scenario's stage in Oxygen. It must be unique.
  Returns: The name of the current validation engine.
### allowsValidation

boolean allowsValidation([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)

Checks if the current document is accepted for this validation.
  Parameters: contentType - Current document content type: ro.sync.basic.contenttypes.ContentTypes Returns: true if the current document can be validated.
### allowsAutomaticValidation

boolean allowsAutomaticValidation()

Check if the custom validation engine allows as you type validation which occurs every time the end user types. If the validation engine is slow or it cannot validate content directly over the Reader provided on the "scan" method, the method should return false
  Returns: if the custom validation engine allows automatic validation.
### validate

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../document/DocumentPositionedInfo.md)> validate([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) documentReader, [ValidationType](ValidationType.md) validationType, [ValidationMode](ValidationMode.md) mode)

Validate the document and provide a list of problems.
  Parameters: systemID - The systemID of the document to be checked. documentReader - The reader of the document. validationType - Indicates the type of validation to be performed usually depending on what action was initiated by the end user from the application. mode - Current validation mode: automatic or manual. Returns: The result of the scanning. Can be null or an empty list to signify there are no validation problems.
### setSchemaSystemID

default void setSchemaSystemID([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) schemaSystemID)

Set the schema system ID in the custom validation engine, in case the validation engine needs a schema for validation.
  Parameters: schemaSystemID - The schema system ID
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
