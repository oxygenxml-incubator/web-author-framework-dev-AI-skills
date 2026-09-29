Package [ro.sync.exml.workspace.api.editor.validation](package-summary.md)

# Interface ValidationScenarioInvoker
    All Known Subinterfaces: [AuthorEditorAccess](../../../../../ecss/extensions/api/access/AuthorEditorAccess.md), [IWebappAuthorEditorAccess](../../../../../ecss/extensions/api/webapp/access/IWebappAuthorEditorAccess.md), [ScenarioInvoker](../ScenarioInvoker.md), [WSEditor](../WSEditor.md), [WSEditorBase](../WSEditorBase.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ValidationScenarioInvoker
Invokes a validation scenario.
  Since: 22.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Thread](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Thread.html) [runValidationScenarios](#runValidationScenarios(java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] scenarioNames)
Run specific, already-defined validation scenarios.

## Method Details

### runValidationScenarios

[Thread](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Thread.html) runValidationScenarios([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] scenarioNames)throws [ValidationScenarioNotFoundException](ValidationScenarioNotFoundException.md), [OperationInProgressException](OperationInProgressException.md)

Run specific, already-defined validation scenarios. A separate thread is started and runs each scenario sequentially. The method returns immediately.
  Parameters: scenarioNames - An array of scenario names defined in the document type associated to the current editor. Returns: The thread that runs the validation. Throws: [ValidationScenarioNotFoundException](ValidationScenarioNotFoundException.md) - If one of the scenarios is not found. [OperationInProgressException](OperationInProgressException.md) - Another validation task is currently running.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
