# Hierarchy For Package ro.sync.ecss.extensions.api.webapp.access
 Package Hierarchies:
* [All Packages](../../../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * java.lang.[Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html) (implements java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))
        * java.lang.[Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

            * ro.sync.ecss.extensions.api.webapp.access.[EditingSessionOpenVetoException](EditingSessionOpenVetoException.md)

    * ro.sync.ecss.extensions.api.webapp.access.[WebappEditingSessionLifecycleListener](WebappEditingSessionLifecycleListener.md)

## Interface Hierarchy

* ro.sync.exml.workspace.api.application.[ApplicationInformationAccess](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md)
    * ro.sync.exml.workspace.api.[WorkspaceUtilities](../../../../../exml/workspace/api/WorkspaceUtilities.md) (also extends ro.sync.exml.workspace.api.util.[ColorThemeUtilities](../../../../../exml/workspace/api/util/ColorThemeUtilities.md))

        * ro.sync.exml.workspace.api.[Workspace](../../../../../exml/workspace/api/Workspace.md)

            * ro.sync.exml.workspace.api.[PluginWorkspace](../../../../../exml/workspace/api/PluginWorkspace.md) (also extends ro.sync.exml.workspace.api.options.[GlobalOptionsStorage](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md), ro.sync.exml.workspace.api.standalone.[ReferencesCustomizer](../../../../../exml/workspace/api/standalone/ReferencesCustomizer.md))

                * ro.sync.exml.workspace.api.standalone.[StandalonePluginWorkspace](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md) (also extends ro.sync.exml.workspace.api.standalone.[DiffAndMergeTools](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md), ro.sync.exml.workspace.api.math.[MathFlowConfigurator](../../../../../exml/workspace/api/math/MathFlowConfigurator.md))

                    * ro.sync.ecss.extensions.api.webapp.access.[WebappPluginWorkspace](WebappPluginWorkspace.md)

* ro.sync.exml.workspace.api.editor.page.author.tooltip.[AuthorTooltipCustomizerProvider](../../../../../exml/workspace/api/editor/page/author/tooltip/AuthorTooltipCustomizerProvider.md)
    * ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPageBase](../../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md) (also extends ro.sync.exml.workspace.api.editor.page.[WSTextBasedEditorPage](../../../../../exml/workspace/api/editor/page/WSTextBasedEditorPage.md))

        * ro.sync.ecss.extensions.api.access.[AuthorEditorAccess](../../access/AuthorEditorAccess.md) (also extends ro.sync.exml.workspace.api.editor.[WSEditorBase](../../../../../exml/workspace/api/editor/WSEditorBase.md))

            * ro.sync.ecss.extensions.api.webapp.access.[IWebappAuthorEditorAccess](IWebappAuthorEditorAccess.md)

* ro.sync.exml.workspace.api.util.[ColorThemeUtilities](../../../../../exml/workspace/api/util/ColorThemeUtilities.md)
    * ro.sync.exml.workspace.api.[WorkspaceUtilities](../../../../../exml/workspace/api/WorkspaceUtilities.md) (also extends ro.sync.exml.workspace.api.application.[ApplicationInformationAccess](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md))

        * ro.sync.exml.workspace.api.[Workspace](../../../../../exml/workspace/api/Workspace.md)

            * ro.sync.exml.workspace.api.[PluginWorkspace](../../../../../exml/workspace/api/PluginWorkspace.md) (also extends ro.sync.exml.workspace.api.options.[GlobalOptionsStorage](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md), ro.sync.exml.workspace.api.standalone.[ReferencesCustomizer](../../../../../exml/workspace/api/standalone/ReferencesCustomizer.md))

                * ro.sync.exml.workspace.api.standalone.[StandalonePluginWorkspace](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md) (also extends ro.sync.exml.workspace.api.standalone.[DiffAndMergeTools](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md), ro.sync.exml.workspace.api.math.[MathFlowConfigurator](../../../../../exml/workspace/api/math/MathFlowConfigurator.md))

                    * ro.sync.ecss.extensions.api.webapp.access.[WebappPluginWorkspace](WebappPluginWorkspace.md)

* ro.sync.exml.workspace.api.standalone.[DiffAndMergeTools](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md)
    * ro.sync.exml.workspace.api.standalone.[StandalonePluginWorkspace](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md) (also extends ro.sync.exml.workspace.api.math.[MathFlowConfigurator](../../../../../exml/workspace/api/math/MathFlowConfigurator.md), ro.sync.exml.workspace.api.[PluginWorkspace](../../../../../exml/workspace/api/PluginWorkspace.md))

        * ro.sync.ecss.extensions.api.webapp.access.[WebappPluginWorkspace](WebappPluginWorkspace.md)

* ro.sync.exml.workspace.api.options.[GlobalOptionsStorage](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md)
    * ro.sync.exml.workspace.api.[PluginWorkspace](../../../../../exml/workspace/api/PluginWorkspace.md) (also extends ro.sync.exml.workspace.api.standalone.[ReferencesCustomizer](../../../../../exml/workspace/api/standalone/ReferencesCustomizer.md), ro.sync.exml.workspace.api.[Workspace](../../../../../exml/workspace/api/Workspace.md))

        * ro.sync.exml.workspace.api.standalone.[StandalonePluginWorkspace](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md) (also extends ro.sync.exml.workspace.api.standalone.[DiffAndMergeTools](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md), ro.sync.exml.workspace.api.math.[MathFlowConfigurator](../../../../../exml/workspace/api/math/MathFlowConfigurator.md))

            * ro.sync.ecss.extensions.api.webapp.access.[WebappPluginWorkspace](WebappPluginWorkspace.md)

* ro.sync.exml.workspace.api.math.[MathFlowConfigurator](../../../../../exml/workspace/api/math/MathFlowConfigurator.md)
    * ro.sync.exml.workspace.api.standalone.[StandalonePluginWorkspace](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md) (also extends ro.sync.exml.workspace.api.standalone.[DiffAndMergeTools](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md), ro.sync.exml.workspace.api.[PluginWorkspace](../../../../../exml/workspace/api/PluginWorkspace.md))

        * ro.sync.ecss.extensions.api.webapp.access.[WebappPluginWorkspace](WebappPluginWorkspace.md)

* ro.sync.exml.workspace.api.base.[ModifiedStatusProvider](../../../../../exml/workspace/api/base/ModifiedStatusProvider.md)
    * ro.sync.exml.workspace.api.editor.[WSEditorBase](../../../../../exml/workspace/api/editor/WSEditorBase.md) (also extends ro.sync.exml.workspace.api.editor.[ScenarioInvoker](../../../../../exml/workspace/api/editor/ScenarioInvoker.md))

        * ro.sync.ecss.extensions.api.access.[AuthorEditorAccess](../../access/AuthorEditorAccess.md) (also extends ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPageBase](../../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md))

            * ro.sync.ecss.extensions.api.webapp.access.[IWebappAuthorEditorAccess](IWebappAuthorEditorAccess.md)

* ro.sync.exml.workspace.api.standalone.[ReferencesCustomizer](../../../../../exml/workspace/api/standalone/ReferencesCustomizer.md)
    * ro.sync.exml.workspace.api.[PluginWorkspace](../../../../../exml/workspace/api/PluginWorkspace.md) (also extends ro.sync.exml.workspace.api.options.[GlobalOptionsStorage](../../../../../exml/workspace/api/options/GlobalOptionsStorage.md), ro.sync.exml.workspace.api.[Workspace](../../../../../exml/workspace/api/Workspace.md))

        * ro.sync.exml.workspace.api.standalone.[StandalonePluginWorkspace](../../../../../exml/workspace/api/standalone/StandalonePluginWorkspace.md) (also extends ro.sync.exml.workspace.api.standalone.[DiffAndMergeTools](../../../../../exml/workspace/api/standalone/DiffAndMergeTools.md), ro.sync.exml.workspace.api.math.[MathFlowConfigurator](../../../../../exml/workspace/api/math/MathFlowConfigurator.md))

            * ro.sync.ecss.extensions.api.webapp.access.[WebappPluginWorkspace](WebappPluginWorkspace.md)

* ro.sync.exml.workspace.api.editor.transformation.[TransformationScenarioInvoker](../../../../../exml/workspace/api/editor/transformation/TransformationScenarioInvoker.md)
    * ro.sync.exml.workspace.api.editor.[ScenarioInvoker](../../../../../exml/workspace/api/editor/ScenarioInvoker.md) (also extends ro.sync.exml.workspace.api.editor.validation.[ValidationScenarioInvoker](../../../../../exml/workspace/api/editor/validation/ValidationScenarioInvoker.md))

        * ro.sync.exml.workspace.api.editor.[WSEditorBase](../../../../../exml/workspace/api/editor/WSEditorBase.md) (also extends ro.sync.exml.workspace.api.base.[ModifiedStatusProvider](../../../../../exml/workspace/api/base/ModifiedStatusProvider.md))

            * ro.sync.ecss.extensions.api.access.[AuthorEditorAccess](../../access/AuthorEditorAccess.md) (also extends ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPageBase](../../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md))

                * ro.sync.ecss.extensions.api.webapp.access.[IWebappAuthorEditorAccess](IWebappAuthorEditorAccess.md)

* ro.sync.exml.workspace.api.editor.validation.[ValidationScenarioInvoker](../../../../../exml/workspace/api/editor/validation/ValidationScenarioInvoker.md)
    * ro.sync.exml.workspace.api.editor.[ScenarioInvoker](../../../../../exml/workspace/api/editor/ScenarioInvoker.md) (also extends ro.sync.exml.workspace.api.editor.transformation.[TransformationScenarioInvoker](../../../../../exml/workspace/api/editor/transformation/TransformationScenarioInvoker.md))

        * ro.sync.exml.workspace.api.editor.[WSEditorBase](../../../../../exml/workspace/api/editor/WSEditorBase.md) (also extends ro.sync.exml.workspace.api.base.[ModifiedStatusProvider](../../../../../exml/workspace/api/base/ModifiedStatusProvider.md))

            * ro.sync.ecss.extensions.api.access.[AuthorEditorAccess](../../access/AuthorEditorAccess.md) (also extends ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPageBase](../../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md))

                * ro.sync.ecss.extensions.api.webapp.access.[IWebappAuthorEditorAccess](IWebappAuthorEditorAccess.md)

* ro.sync.exml.workspace.api.editor.page.[WSEditorPage](../../../../../exml/workspace/api/editor/page/WSEditorPage.md)

    * ro.sync.exml.workspace.api.editor.page.[WSTextBasedEditorPage](../../../../../exml/workspace/api/editor/page/WSTextBasedEditorPage.md)

        * ro.sync.exml.workspace.api.editor.page.author.[WSAuthorEditorPageBase](../../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md) (also extends ro.sync.exml.workspace.api.editor.page.author.tooltip.[AuthorTooltipCustomizerProvider](../../../../../exml/workspace/api/editor/page/author/tooltip/AuthorTooltipCustomizerProvider.md))

            * ro.sync.ecss.extensions.api.access.[AuthorEditorAccess](../../access/AuthorEditorAccess.md) (also extends ro.sync.exml.workspace.api.editor.[WSEditorBase](../../../../../exml/workspace/api/editor/WSEditorBase.md))

                * ro.sync.ecss.extensions.api.webapp.access.[IWebappAuthorEditorAccess](IWebappAuthorEditorAccess.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
