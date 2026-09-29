Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Interface WebappActionsManager
    All Superinterfaces: [AuthorExtensionActionProvider](../AuthorExtensionActionProvider.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WebappActionsManagerextends [AuthorExtensionActionProvider](../AuthorExtensionActionProvider.md)
Helper object that provides access to extension actions, and provides support for invoking operations.
  Since: 17
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> [getExtensionActionsConfiguration](#getExtensionActionsConfiguration())()
Returns a representation of the extension actions configuration including the actions list and the toolbar configuration.
  void [invokeOperation](#invokeOperation(java.lang.String,java.util.Map,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) operationClassName, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> args, int imposedOffset)
Invokes an operation.

### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorExtensionActionProvider](../AuthorExtensionActionProvider.md)
 [getExtensionAction](../AuthorExtensionActionProvider.md#getExtensionAction(java.lang.String)), [getExtensionAction](../AuthorExtensionActionProvider.md#getExtensionAction(ro.sync.ecss.css.functions.ActionLexicalUnit))
## Method Details

### invokeOperation

void invokeOperation([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) operationClassName, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> args, int imposedOffset)throws [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html), [AuthorOperationException](../AuthorOperationException.md)

Invokes an operation.
  Parameters: operationClassName - The name of the class that implements the operation. args - The arguments in a representation that mimics JSON: JSON string maps to Java String, and JSON object maps to Java Map. imposedOffset - The offset where the action is to be executed. -1 if the action is to be executed for the current selection. Throws: [AuthorOperationException](../AuthorOperationException.md) - If the action invocation throws. [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - If the action invocation throws.
### getExtensionActionsConfiguration

[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> getExtensionActionsConfiguration()

Returns a representation of the extension actions configuration including the actions list and the toolbar configuration.
  Returns: The actions configuration.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
