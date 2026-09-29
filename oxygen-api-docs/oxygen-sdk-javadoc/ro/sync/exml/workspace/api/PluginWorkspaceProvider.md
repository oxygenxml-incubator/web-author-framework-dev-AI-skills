Package [ro.sync.exml.workspace.api](package-summary.md)

# Class PluginWorkspaceProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.PluginWorkspaceProvider
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public final class PluginWorkspaceProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Provides static access to the workspace API of the Oxygen editor.
  Since: 14
## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [PluginWorkspace](PluginWorkspace.md) [getPluginWorkspace](#getPluginWorkspace())()
Get access to API used to control the Oxygen editors.
  static void [setPluginWorkspace](#setPluginWorkspace(ro.sync.exml.workspace.api.PluginWorkspace))([PluginWorkspace](PluginWorkspace.md) pluginWorkspace)
Set the workspace.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### getPluginWorkspace

public static [PluginWorkspace](PluginWorkspace.md) getPluginWorkspace()

Get access to API used to control the Oxygen editors. This static access can be used when running the standalone or the Eclipse version of Oxygen from any part of the developer's code.
  Returns: Returns the pluginWorkspace.
### setPluginWorkspace

public static void setPluginWorkspace([PluginWorkspace](PluginWorkspace.md) pluginWorkspace)

Set the workspace. FOR INTERNAL USE ONLY.
  Parameters: pluginWorkspace - The plugin Workspace to set.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
