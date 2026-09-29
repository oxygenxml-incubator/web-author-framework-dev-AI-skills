Package [ro.sync.exml.workspace.api.editor](package-summary.md)

# Interface ScenarioInvoker
    All Superinterfaces: [TransformationScenarioInvoker](transformation/TransformationScenarioInvoker.md), [ValidationScenarioInvoker](validation/ValidationScenarioInvoker.md)   All Known Subinterfaces: [AuthorEditorAccess](../../../../ecss/extensions/api/access/AuthorEditorAccess.md), [IWebappAuthorEditorAccess](../../../../ecss/extensions/api/webapp/access/IWebappAuthorEditorAccess.md), [WSEditor](WSEditor.md), [WSEditorBase](WSEditorBase.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ScenarioInvokerextends [TransformationScenarioInvoker](transformation/TransformationScenarioInvoker.md), [ValidationScenarioInvoker](validation/ValidationScenarioInvoker.md)
Convenience interface for a validation and transformation scenarios invoker.
  Since: 22.1
## Method Summary

### Methods inherited from interface ro.sync.exml.workspace.api.editor.transformation.[TransformationScenarioInvoker](transformation/TransformationScenarioInvoker.md)
 [runTransformationScenario](transformation/TransformationScenarioInvoker.md#runTransformationScenario(java.lang.String,java.util.Map,ro.sync.exml.workspace.api.editor.transformation.TransformationFeedback)), [runTransformationScenarios](transformation/TransformationScenarioInvoker.md#runTransformationScenarios(java.lang.String%5B%5D,ro.sync.exml.workspace.api.editor.transformation.TransformationFeedback)), [stopCurrentTransformationScenario](transformation/TransformationScenarioInvoker.md#stopCurrentTransformationScenario())
### Methods inherited from interface ro.sync.exml.workspace.api.editor.validation.[ValidationScenarioInvoker](validation/ValidationScenarioInvoker.md)
 [runValidationScenarios](validation/ValidationScenarioInvoker.md#runValidationScenarios(java.lang.String%5B%5D))
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
