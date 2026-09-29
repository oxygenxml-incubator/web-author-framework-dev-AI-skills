# Hierarchy For Package ro.sync.exml.workspace.api.editor
 Package Hierarchies:
* [All Packages](../../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * ro.sync.exml.workspace.api.editor.[ReadOnlyReason](ReadOnlyReason.md)

## Interface Hierarchy

* ro.sync.exml.editor.[EditorPageConstants](../../../editor/EditorPageConstants.md)
    * ro.sync.exml.workspace.api.editor.[WSEditor](WSEditor.md) (also extends ro.sync.exml.workspace.api.editor.[WSEditorBase](WSEditorBase.md))

* ro.sync.exml.workspace.api.base.[ModifiedStatusProvider](../base/ModifiedStatusProvider.md)
    * ro.sync.exml.workspace.api.editor.[WSEditorBase](WSEditorBase.md) (also extends ro.sync.exml.workspace.api.editor.[ScenarioInvoker](ScenarioInvoker.md))

        * ro.sync.exml.workspace.api.editor.[WSEditor](WSEditor.md) (also extends ro.sync.exml.editor.[EditorPageConstants](../../../editor/EditorPageConstants.md))

* ro.sync.exml.workspace.api.editor.transformation.[TransformationScenarioInvoker](transformation/TransformationScenarioInvoker.md)
    * ro.sync.exml.workspace.api.editor.[ScenarioInvoker](ScenarioInvoker.md) (also extends ro.sync.exml.workspace.api.editor.validation.[ValidationScenarioInvoker](validation/ValidationScenarioInvoker.md))

        * ro.sync.exml.workspace.api.editor.[WSEditorBase](WSEditorBase.md) (also extends ro.sync.exml.workspace.api.base.[ModifiedStatusProvider](../base/ModifiedStatusProvider.md))

            * ro.sync.exml.workspace.api.editor.[WSEditor](WSEditor.md) (also extends ro.sync.exml.editor.[EditorPageConstants](../../../editor/EditorPageConstants.md))

* ro.sync.exml.workspace.api.editor.validation.[ValidationScenarioInvoker](validation/ValidationScenarioInvoker.md)

    * ro.sync.exml.workspace.api.editor.[ScenarioInvoker](ScenarioInvoker.md) (also extends ro.sync.exml.workspace.api.editor.transformation.[TransformationScenarioInvoker](transformation/TransformationScenarioInvoker.md))

        * ro.sync.exml.workspace.api.editor.[WSEditorBase](WSEditorBase.md) (also extends ro.sync.exml.workspace.api.base.[ModifiedStatusProvider](../base/ModifiedStatusProvider.md))

            * ro.sync.exml.workspace.api.editor.[WSEditor](WSEditor.md) (also extends ro.sync.exml.editor.[EditorPageConstants](../../../editor/EditorPageConstants.md))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
