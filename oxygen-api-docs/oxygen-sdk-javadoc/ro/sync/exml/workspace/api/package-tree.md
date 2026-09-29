# Hierarchy For Package ro.sync.exml.workspace.api
 Package Hierarchies:
* [All Packages](../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * junit.framework.Assert
        * junit.framework.TestCase (implements junit.framework.Test)

            * junit.extensions.jfcunit.JFCTestCase

                * ro.sync.exml.workspace.api.[PluginWorkspaceTCBase](PluginWorkspaceTCBase.md)

    * ro.sync.exml.workspace.api.[PluginWorkspaceProvider](PluginWorkspaceProvider.md)

## Interface Hierarchy

* ro.sync.exml.workspace.api.application.[ApplicationInformationAccess](application/ApplicationInformationAccess.md)
    * ro.sync.exml.workspace.api.[WorkspaceUtilities](WorkspaceUtilities.md) (also extends ro.sync.exml.workspace.api.util.[ColorThemeUtilities](util/ColorThemeUtilities.md))

        * ro.sync.exml.workspace.api.[Workspace](Workspace.md)

            * ro.sync.exml.workspace.api.[PluginWorkspace](PluginWorkspace.md) (also extends ro.sync.exml.workspace.api.options.[GlobalOptionsStorage](options/GlobalOptionsStorage.md), ro.sync.exml.workspace.api.standalone.[ReferencesCustomizer](standalone/ReferencesCustomizer.md))

* ro.sync.exml.workspace.api.util.[ColorThemeUtilities](util/ColorThemeUtilities.md)
    * ro.sync.exml.workspace.api.[WorkspaceUtilities](WorkspaceUtilities.md) (also extends ro.sync.exml.workspace.api.application.[ApplicationInformationAccess](application/ApplicationInformationAccess.md))

        * ro.sync.exml.workspace.api.[Workspace](Workspace.md)

            * ro.sync.exml.workspace.api.[PluginWorkspace](PluginWorkspace.md) (also extends ro.sync.exml.workspace.api.options.[GlobalOptionsStorage](options/GlobalOptionsStorage.md), ro.sync.exml.workspace.api.standalone.[ReferencesCustomizer](standalone/ReferencesCustomizer.md))

* ro.sync.exml.workspace.api.options.[GlobalOptionsStorage](options/GlobalOptionsStorage.md)
    * ro.sync.exml.workspace.api.[PluginWorkspace](PluginWorkspace.md) (also extends ro.sync.exml.workspace.api.standalone.[ReferencesCustomizer](standalone/ReferencesCustomizer.md), ro.sync.exml.workspace.api.[Workspace](Workspace.md))

* ro.sync.exml.workspace.api.[PluginResourceBundle](PluginResourceBundle.md)
* ro.sync.exml.workspace.api.standalone.[ReferencesCustomizer](standalone/ReferencesCustomizer.md)

    * ro.sync.exml.workspace.api.[PluginWorkspace](PluginWorkspace.md) (also extends ro.sync.exml.workspace.api.options.[GlobalOptionsStorage](options/GlobalOptionsStorage.md), ro.sync.exml.workspace.api.[Workspace](Workspace.md))

## Enum Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<E> (implements java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<T>, java.lang.constant.[Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))

        * ro.sync.exml.workspace.api.[OperationStatus](OperationStatus.md)
        * ro.sync.exml.workspace.api.[Platform](Platform.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
