Package [ro.sync.exml.plugin.startup](package-summary.md)

# Interface ComponentsValidatorPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface ComponentsValidatorPluginExtensionextends [PluginExtension](../PluginExtension.md)
Startup plugin. It is invoked before the main frame of the editor is displayed.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [ComponentsValidator](../../ComponentsValidator.md) [getComponentsValidator](#getComponentsValidator())()
Gets the componet validator.

## Method Details

### getComponentsValidator

[ComponentsValidator](../../ComponentsValidator.md) getComponentsValidator()

Gets the componet validator. It acts like a filter, removing buttons/toolbars, views, menu items from the main interface.
  Returns: The componentsValidator.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
