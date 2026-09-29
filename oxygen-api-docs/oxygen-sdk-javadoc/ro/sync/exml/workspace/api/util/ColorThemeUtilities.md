Package [ro.sync.exml.workspace.api.util](package-summary.md)

# Interface ColorThemeUtilities
    All Known Subinterfaces: [AuthorWorkspaceAccess](../../../../ecss/extensions/api/access/AuthorWorkspaceAccess.md), [EclipsePluginWorkspace](../../../../../../com/oxygenxml/workspace/api/eclipse/EclipsePluginWorkspace.md), [PluginWorkspace](../PluginWorkspace.md), [StandalonePluginWorkspace](../standalone/StandalonePluginWorkspace.md), [WebappPluginWorkspace](../../../../ecss/extensions/api/webapp/access/WebappPluginWorkspace.md), [Workspace](../Workspace.md), [WorkspaceUtilities](../WorkspaceUtilities.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ColorThemeUtilities
A theme manager is an object that is able to provide information about the color theme used by oXygen. The color theme is used to style all the views and controls used by oxygen as well as the editors.
  Since: 16.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [ColorTheme](ColorTheme.md) [getColorTheme](#getColorTheme())()
Get the color theme used by Oxygen to render its views, controls and all the editors.
  [ImageInverter](ImageInverter.md) [getImageInverter](#getImageInverter())()
Get the image inverter used to invert images for certain color themes.

## Method Details

### getColorTheme

[ColorTheme](ColorTheme.md) getColorTheme()

Get the color theme used by Oxygen to render its views, controls and all the editors. The returned object changes according to the currently active color theme.
  Returns: The color theme. Since: 16.1
### getImageInverter

[ImageInverter](ImageInverter.md) getImageInverter()

Get the image inverter used to invert images for certain color themes.
  Returns: The image inverter. Since: 16.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
