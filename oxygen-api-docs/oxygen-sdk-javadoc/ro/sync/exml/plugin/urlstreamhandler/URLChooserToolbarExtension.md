Package [ro.sync.exml.plugin.urlstreamhandler](package-summary.md)

# Interface URLChooserToolbarExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface URLChooserToolbarExtensionextends [PluginExtension](../PluginExtension.md)
URL chooser toolbar extension. Provides toolbar icon and toolbar tooltip for the button to be inserted in the "File" toolbar. When pressing the button, the URLChooserPluginExtension's chooseURL()will be invoked.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Icon](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Icon.html) [getToolbarIcon](#getToolbarIcon())()
Get the toolbar icon.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getToolbarTooltip](#getToolbarTooltip())()
Get the tooltip to be placed on the toolbar button.

## Method Details

### getToolbarIcon

[Icon](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Icon.html) getToolbarIcon()

Get the toolbar icon. The action will be placed in the "File" toolbar. Return nullif the action should not be included in the toolbar.
  Returns: The toolbar icon or null.
### getToolbarTooltip

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getToolbarTooltip()

Get the tooltip to be placed on the toolbar button. If the tooltip is null but there is an icon provided, the URLChooserPluginExtension.getMenuName() will be used instead.
  Returns: The toolbar tooltip or null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
