Package [ro.sync.exml.plugin.general](package-summary.md)

# Interface GeneralPluginContext
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface GeneralPluginContext
Plugin context interface. Provides information for the plugin about the context it was invoked in.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) [getFrame](#getFrame())()
Get the editing frame.
  [StandalonePluginWorkspace](../../workspace/api/standalone/StandalonePluginWorkspace.md) [getPluginWorkspace](#getPluginWorkspace())()
Get access to the entire workspace of Oxygen.

## Method Details

### getFrame

[Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) getFrame()

Get the editing frame.
  Returns: the frame in which is done the editing.
### getPluginWorkspace

[StandalonePluginWorkspace](../../workspace/api/standalone/StandalonePluginWorkspace.md) getPluginWorkspace()

Get access to the entire workspace of Oxygen.
  Returns: The access to the entire workspace of Oxygen Since: 12.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
