Package [ro.sync.exml.plugin.workspace](package-summary.md)

# Interface WorkspaceAccessPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface WorkspaceAccessPluginExtensionextends [PluginExtension](../PluginExtension.md)
Workspace Access plugin extension.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [applicationClosing](#applicationClosing())()
Notified before the editors are closed and the application exits.
  void [applicationStarted](#applicationStarted(ro.sync.exml.workspace.api.standalone.StandalonePluginWorkspace))([StandalonePluginWorkspace](../../workspace/api/standalone/StandalonePluginWorkspace.md) pluginWorkspaceAccess)
Main plugin method.

## Method Details

### applicationStarted

void applicationStarted([StandalonePluginWorkspace](../../workspace/api/standalone/StandalonePluginWorkspace.md) pluginWorkspaceAccess)

Main plugin method. Notified when the application is started.  **IMPORTANT**: This method must not block, the plug-in can add its listeners or customize the main menu and then return.
  Parameters: pluginWorkspaceAccess - The workspace access
### applicationClosing

boolean applicationClosing()

Notified before the editors are closed and the application exits. You can reject the close.
  Returns: True application can close, false, if vetoed.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
