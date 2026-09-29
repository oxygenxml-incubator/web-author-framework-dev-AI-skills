Package [ro.sync.exml.workspace.api.standalone](package-summary.md)

# Interface ToolbarComponentsCustomizer
    @API(type=EXTENDABLE, src=PUBLIC) public interface ToolbarComponentsCustomizer
Customizes components for the toolbar
  Since: 11.2
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CUSTOM](#CUSTOM)  Deprecated.
Since Oxygen 12.2 toolbar IDs are defined in the "plugin.xml".

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [customizeToolbar](#customizeToolbar(ro.sync.exml.workspace.api.standalone.ToolbarInfo))([ToolbarInfo](ToolbarInfo.md) toolbarInfo)
Customize the components which get displayed on a certain toolbar.

## Field Details

### CUSTOM

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CUSTOM
 Deprecated.
Since Oxygen 12.2 toolbar IDs are defined in the "plugin.xml".

The reserved plugins toolbar ID
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.ToolbarComponentsCustomizer.CUSTOM)

## Method Details

### customizeToolbar

void customizeToolbar([ToolbarInfo](ToolbarInfo.md) toolbarInfo)

Customize the components which get displayed on a certain toolbar.  **NOTICE** You will also receive notification for the Author extension toolbars (which are dynamically constructed based on the document type of the current selected XML file). The notifications will be received before the toolbars are constructed after an XML editor which is opened in the Author page was selected. Such toolbar IDs have the prefix "Author_custom_actions" and the suffix is a number depending on how many toolbars were created for that specific document type. In this way you can dynamically filter or add to toolbar buttons already declared in the document type associated to the XML editor.  **NOTICE** Notifications will arrive for the Dita Map Manager toolbars too. These toolbars have the IDs:
        * [MainFrameComponentsConstants.TOOLBAR_DITA_MAP_GLOBAL](../../../MainFrameComponentsConstants.md#TOOLBAR_DITA_MAP_GLOBAL)
        * [MainFrameComponentsConstants.TOOLBAR_DITA_MAP_EXTEND](../../../MainFrameComponentsConstants.md#TOOLBAR_DITA_MAP_EXTEND)
        * [MainFrameComponentsConstants.TOOLBAR_DITA_MAP_CUSTOM](../../../MainFrameComponentsConstants.md#TOOLBAR_DITA_MAP_CUSTOM)

  Parameters: toolbarInfo - Information about the toolbar (id, default components to add, title). The toolbar ID is either the ID of an existing Oxygen toolbar or the reserved **CUSTOM** toolbar. All Oxygen toolbars IDs are found in [MainFrameComponentsConstants](../../../MainFrameComponentsConstants.md) and begin with TOOLBAR_ prefix. You can set new components in the toolbar and change its title.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
