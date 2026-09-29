Package [ro.sync.exml.workspace.api.editor.transformation](package-summary.md)

# Interface TransformationScenarioInvoker
    All Known Subinterfaces: [AuthorEditorAccess](../../../../../ecss/extensions/api/access/AuthorEditorAccess.md), [IWebappAuthorEditorAccess](../../../../../ecss/extensions/api/webapp/access/IWebappAuthorEditorAccess.md), [ScenarioInvoker](../ScenarioInvoker.md), [WSEditor](../WSEditor.md), [WSEditorBase](../WSEditorBase.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface TransformationScenarioInvoker
Invokes a transformation scenario.
  Since: 15
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [runTransformationScenario](#runTransformationScenario(java.lang.String,java.util.Map,ro.sync.exml.workspace.api.editor.transformation.TransformationFeedback))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scenarioName, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> scenarioParameters, [TransformationFeedback](TransformationFeedback.md) transformationFeedback)
Run specific already defined transformation scenario with custom values for parameters.
  void [runTransformationScenarios](#runTransformationScenarios(java.lang.String%5B%5D,ro.sync.exml.workspace.api.editor.transformation.TransformationFeedback))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] scenarioNames, [TransformationFeedback](TransformationFeedback.md) transformationFeedback)
Run specific already defined transformation scenarios.
  void [stopCurrentTransformationScenario](#stopCurrentTransformationScenario())()
Stops the current transformation scenario.

## Method Details

### runTransformationScenarios

void runTransformationScenarios([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] scenarioNames, [TransformationFeedback](TransformationFeedback.md) transformationFeedback)throws [TransformationScenarioNotFoundException](TransformationScenarioNotFoundException.md)

Run specific already defined transformation scenarios. A separate thread is started and runs each scenario sequentially. The method returns immediately.
  Parameters: scenarioNames - An array of scenario names defined in the document type associated to the current editor. transformationFeedback - An interface through which the user receives feedback from the started transformation process. Throws: [TransformationScenarioNotFoundException](TransformationScenarioNotFoundException.md) - If one of the scenarios is not found.
### runTransformationScenario

void runTransformationScenario([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scenarioName, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> scenarioParameters, [TransformationFeedback](TransformationFeedback.md) transformationFeedback)throws [TransformationScenarioNotFoundException](TransformationScenarioNotFoundException.md)

Run specific already defined transformation scenario with custom values for parameters. A separate thread is started and runs each scenario sequentially. The method returns immediately.
  Parameters: scenarioName - The scenario name defined in the document type associated to the current editor. scenarioParameters - Pairs of transformation scenario names and values that will be used when running this transformation. transformationFeedback - An interface through which the user receives feedback from the started transformation process. Throws: [TransformationScenarioNotFoundException](TransformationScenarioNotFoundException.md) - If the transformation scenario is not found. Since: 25.0
### stopCurrentTransformationScenario

void stopCurrentTransformationScenario()

Stops the current transformation scenario.
  Since: 25.0
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
