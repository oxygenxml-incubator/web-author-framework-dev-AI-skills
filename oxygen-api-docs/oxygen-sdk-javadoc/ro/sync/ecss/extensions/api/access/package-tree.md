# Hierarchy For Package ro.sync.ecss.extensions.api.access
 Package Hierarchies:
* [All Packages](../../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * ro.sync.ecss.extensions.api.access.[EditingSessionContext](EditingSessionContext.md) (implements ro.sync.ecss.dita.[ContextKeyManagerProvider](../../../dita/ContextKeyManagerProvider.md))

## Interface Hierarchy

* ro.sync.exml.workspace.api.application.[ApplicationInformationAccess](../../../../exml/workspace/api/application/ApplicationInformationAccess.md)
    * ro.sync.exml.workspace.api.[WorkspaceUtilities](../../../../exml/workspace/api/WorkspaceUtilities.md) (also extends ro.sync.exml.workspace.api.util.[ColorThemeUtilities](../../../../exml/workspace/api/util/ColorThemeUtilities.md))

        * ro.sync.exml.workspace.api.[Workspace](../../../../exml/workspace/api/Workspace.md)

            * ro.sync.ecss.extensions.api.access.[AuthorWorkspaceAccess](AuthorWorkspaceAccess.md)

* ro.sync.ecss.extensions.api.access.[AuthorTableAccess](AuthorTableAccess.md)
* ro.sync.exml.workspace.api.editor.page.author.tooltip.[AuthorTooltipCustomizerProvider](../../../../exml/workspace/api/editor/page/author/tooltip/AuthorTooltipCustomizerProvider.md)
    * ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPageBase](../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md) (also extends ro.sync.exml.workspace.api.editor.page.[WSTextBasedEditorPage](../../../../exml/workspace/api/editor/page/WSTextBasedEditorPage.md))

        * ro.sync.ecss.extensions.api.access.[AuthorEditorAccess](AuthorEditorAccess.md) (also extends ro.sync.exml.workspace.api.editor.[WSEditorBase](../../../../exml/workspace/api/editor/WSEditorBase.md))

* ro.sync.exml.workspace.api.util.[ColorThemeUtilities](../../../../exml/workspace/api/util/ColorThemeUtilities.md)
    * ro.sync.exml.workspace.api.[WorkspaceUtilities](../../../../exml/workspace/api/WorkspaceUtilities.md) (also extends ro.sync.exml.workspace.api.application.[ApplicationInformationAccess](../../../../exml/workspace/api/application/ApplicationInformationAccess.md))

        * ro.sync.exml.workspace.api.[Workspace](../../../../exml/workspace/api/Workspace.md)

            * ro.sync.ecss.extensions.api.access.[AuthorWorkspaceAccess](AuthorWorkspaceAccess.md)

* ro.sync.exml.workspace.api.base.[ModifiedStatusProvider](../../../../exml/workspace/api/base/ModifiedStatusProvider.md)
    * ro.sync.exml.workspace.api.editor.[WSEditorBase](../../../../exml/workspace/api/editor/WSEditorBase.md) (also extends ro.sync.exml.workspace.api.editor.[ScenarioInvoker](../../../../exml/workspace/api/editor/ScenarioInvoker.md))

        * ro.sync.ecss.extensions.api.access.[AuthorEditorAccess](AuthorEditorAccess.md) (also extends ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPageBase](../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md))

* ro.sync.exml.workspace.api.editor.transformation.[TransformationScenarioInvoker](../../../../exml/workspace/api/editor/transformation/TransformationScenarioInvoker.md)
    * ro.sync.exml.workspace.api.editor.[ScenarioInvoker](../../../../exml/workspace/api/editor/ScenarioInvoker.md) (also extends ro.sync.exml.workspace.api.editor.validation.[ValidationScenarioInvoker](../../../../exml/workspace/api/editor/validation/ValidationScenarioInvoker.md))

        * ro.sync.exml.workspace.api.editor.[WSEditorBase](../../../../exml/workspace/api/editor/WSEditorBase.md) (also extends ro.sync.exml.workspace.api.base.[ModifiedStatusProvider](../../../../exml/workspace/api/base/ModifiedStatusProvider.md))

            * ro.sync.ecss.extensions.api.access.[AuthorEditorAccess](AuthorEditorAccess.md) (also extends ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPageBase](../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md))

* ro.sync.ecss.extensions.api.access.[UnsavedContentReferenceManager](UnsavedContentReferenceManager.md)
* ro.sync.ecss.extensions.api.access.[UnsavedReferenceNodeDescriptor](UnsavedReferenceNodeDescriptor.md)
* ro.sync.exml.workspace.api.util.[UtilAccess](../../../../exml/workspace/api/util/UtilAccess.md)
    * ro.sync.ecss.extensions.api.access.[AuthorUtilAccess](AuthorUtilAccess.md)

* ro.sync.exml.workspace.api.editor.validation.[ValidationScenarioInvoker](../../../../exml/workspace/api/editor/validation/ValidationScenarioInvoker.md)
    * ro.sync.exml.workspace.api.editor.[ScenarioInvoker](../../../../exml/workspace/api/editor/ScenarioInvoker.md) (also extends ro.sync.exml.workspace.api.editor.transformation.[TransformationScenarioInvoker](../../../../exml/workspace/api/editor/transformation/TransformationScenarioInvoker.md))

        * ro.sync.exml.workspace.api.editor.[WSEditorBase](../../../../exml/workspace/api/editor/WSEditorBase.md) (also extends ro.sync.exml.workspace.api.base.[ModifiedStatusProvider](../../../../exml/workspace/api/base/ModifiedStatusProvider.md))

            * ro.sync.ecss.extensions.api.access.[AuthorEditorAccess](AuthorEditorAccess.md) (also extends ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPageBase](../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md))

* ro.sync.exml.workspace.api.editor.page.[WSEditorPage](../../../../exml/workspace/api/editor/page/WSEditorPage.md)
    * ro.sync.exml.workspace.api.editor.page.[WSTextBasedEditorPage](../../../../exml/workspace/api/editor/page/WSTextBasedEditorPage.md)

        * ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPageBase](../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md) (also extends ro.sync.exml.workspace.api.editor.page.author.tooltip.[AuthorTooltipCustomizerProvider](../../../../exml/workspace/api/editor/page/author/tooltip/AuthorTooltipCustomizerProvider.md))

            * ro.sync.ecss.extensions.api.access.[AuthorEditorAccess](AuthorEditorAccess.md) (also extends ro.sync.exml.workspace.api.editor.[WSEditorBase](../../../../exml/workspace/api/editor/WSEditorBase.md))

* ro.sync.exml.workspace.api.editor.page.[WSOutline](../../../../exml/workspace/api/editor/page/WSOutline.md)
    * ro.sync.ecss.extensions.api.access.[AuthorOutlineAccess](AuthorOutlineAccess.md)

* ro.sync.exml.workspace.api.util.[XMLUtilAccess](../../../../exml/workspace/api/util/XMLUtilAccess.md)

    * ro.sync.ecss.extensions.api.access.[AuthorXMLUtilAccess](AuthorXMLUtilAccess.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
