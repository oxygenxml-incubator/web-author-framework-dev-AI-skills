# Package ro.sync.exml.workspace.api.standalone

package ro.sync.exml.workspace.api.standalone

Customizers which can be set by implementing a WorkspaceAccess-type plugin.
     Related Packages
Package

Description
 [ro.sync.exml.workspace.api](../package-summary.md)
API for accessing the application workspace.
  [ro.sync.exml.workspace.api.standalone.actions](actions/package-summary.md)

 [ro.sync.exml.workspace.api.standalone.ditamap](ditamap/package-summary.md)
Provide custom resolve capabilities for the topic titles and other information displayed in the DITA Maps Manager
  [ro.sync.exml.workspace.api.standalone.project](project/package-summary.md)

 [ro.sync.exml.workspace.api.standalone.proxy](proxy/package-summary.md)

 [ro.sync.exml.workspace.api.standalone.ui](ui/package-summary.md)
Simple components which can be extended by the customizer in order to make new buttons/dialogs look like the ones in the application.
      All Classes and InterfacesInterfacesClasses
Class

Description
 [AttributeEditingContextDescription](AttributeEditingContextDescription.md)
Provides language-independent information about the element and attribute name for which the value is edited.
  [ContextDescriptionProvider](ContextDescriptionProvider.md)
Provides language-independent information about a certain context.
  [DiffAndMergeTools](DiffAndMergeTools.md)
Tools used for executing operations like finding differences between files and folders, or merging different files.
  [InputURLChooser](InputURLChooser.md)
Interface through which the CMS can set a custom URL to any Input URL Panel from Oxygen.
  [InputURLChooserCustomizer](InputURLChooserCustomizer.md)
Customize the actions which appear in any Input URL chooser from Oxygen.
  [MenuBarCustomizer](MenuBarCustomizer.md)
Customizes components from the main menu bar.
  [ReferencesCustomizer](ReferencesCustomizer.md)
Contains methods for customizing the Input URL Choosers and for computing relative paths from URLs in an implementation specific manner.
  [ResourceFilter](ResourceFilter.md)
Resource filter returned by the InputURLCustomizer.
  [StandalonePluginWorkspace](StandalonePluginWorkspace.md)
The **Plugin Workspace** offers the possibility to customize the Workspace toolbars, menu bars or views, to access utility methods or to access (and add listeners for) all opened editors from the Main editing area or from the DITA Maps editing area.
  [ToolbarComponentsCustomizer](ToolbarComponentsCustomizer.md)
Customizes components for the toolbar
  [ToolbarInfo](ToolbarInfo.md)
Information about a toolbar.
  [ViewComponentCustomizer](ViewComponentCustomizer.md)
Customizes components for the Oxygen views.
  [ViewInfo](ViewInfo.md)
Information about a view.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
