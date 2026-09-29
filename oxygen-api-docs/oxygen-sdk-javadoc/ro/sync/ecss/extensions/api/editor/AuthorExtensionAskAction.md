Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Interface AuthorExtensionAskAction
    All Superinterfaces: [IAuthorExtensionAction](IAuthorExtensionAction.md)   @API(type=INTERNAL, src=PUBLIC) public interface AuthorExtensionAskActionextends [IAuthorExtensionAction](IAuthorExtensionAction.md)
An author action created over an author operation who does not handle the ask variables expansion. Instead it receives the ask variables expansion.
  Since: 20.1
## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.editor.[IAuthorExtensionAction](IAuthorExtensionAction.md)
 [ACTION_ID](IAuthorExtensionAction.md#ACTION_ID), [ACTION_NAME](IAuthorExtensionAction.md#ACTION_NAME), [DESCRIPTION](IAuthorExtensionAction.md#DESCRIPTION), [LARGE_ICON_PATH](IAuthorExtensionAction.md#LARGE_ICON_PATH), [SMALL_ICON_PATH](IAuthorExtensionAction.md#SMALL_ICON_PATH)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 int [countAsksVariables](#countAsksVariables())()
Get the number of asks variables.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AskDescriptor](../../AskDescriptor.md)> [performActionWithValues](#performActionWithValues(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> askValues)
Performs the action using the values to expand the askValues.

### Methods inherited from interface ro.sync.ecss.extensions.api.editor.[IAuthorExtensionAction](IAuthorExtensionAction.md)
 [getValue](IAuthorExtensionAction.md#getValue(java.lang.String)), [performAction](IAuthorExtensionAction.md#performAction()), [performAction](IAuthorExtensionAction.md#performAction(int))
## Method Details

### performActionWithValues

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AskDescriptor](../../AskDescriptor.md)> performActionWithValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> askValues)

Performs the action using the values to expand the askValues.
  Parameters: askValues - the expanded ask values. Returns: list of descriptors for the ask variables that were not expanded.
### countAsksVariables

int countAsksVariables()

Get the number of asks variables.
  Returns: the number of asks variables that must be expanded.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
