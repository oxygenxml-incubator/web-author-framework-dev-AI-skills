Package [ro.sync.exml.workspace.api.standalone](package-summary.md)

# Interface ViewComponentCustomizer
    @API(type=EXTENDABLE, src=PUBLIC) public interface ViewComponentCustomizer
Customizes components for the Oxygen views.
  Since: 11.2
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CUSTOM](#CUSTOM)  Deprecated.
since Oxygen 12.2.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [customizeView](#customizeView(ro.sync.exml.workspace.api.standalone.ViewInfo))([ViewInfo](ViewInfo.md) viewInfo)
Customize the component which gets displayed on a certain view.

## Field Details

### CUSTOM

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CUSTOM
 Deprecated.
since Oxygen 12.2. Please define a view id for the extension in the "plugin.xml".

The CUSTOM view.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.ViewComponentCustomizer.CUSTOM)

## Method Details

### customizeView

void customizeView([ViewInfo](ViewInfo.md) viewInfo)

Customize the component which gets displayed on a certain view. This callback may be called multiple times if the application views layout (perspective) changes or is reloaded so you should strive to create your Swing components for a certain view ID only once.
  Parameters: viewInfo - Information about a view. The view ID is either the ID of an existing Oxygen view or the reserved **CUSTOM** view.
You can set a new component to display for the view, new title or icon.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
