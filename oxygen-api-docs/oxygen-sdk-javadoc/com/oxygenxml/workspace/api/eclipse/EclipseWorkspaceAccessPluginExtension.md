Package [com.oxygenxml.workspace.api.eclipse](package-summary.md)

# Interface EclipseWorkspaceAccessPluginExtension
    @API(type=EXTENDABLE, src=PUBLIC) public interface EclipseWorkspaceAccessPluginExtension
Workspace Access plugin extension for Eclipse. An Eclipse plugin which depends on our plugin can implement this extension and that Eclipse plugin will be called when our plugin is started and when it is stopped...
  Since: 18
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [pluginStarted](#pluginStarted(com.oxygenxml.workspace.api.eclipse.EclipsePluginWorkspace))([EclipsePluginWorkspace](EclipsePluginWorkspace.md) pluginWorkspaceAccess)
Notified when the Oxygen Eclipse plugin is starting.
  void [pluginStopping](#pluginStopping())()
Notified before the Oxygen Eclipse plugin will be stopped.

## Method Details

### pluginStarted

void pluginStarted([EclipsePluginWorkspace](EclipsePluginWorkspace.md) pluginWorkspaceAccess)

Notified when the Oxygen Eclipse plugin is starting.  **IMPORTANT**: This method must not block, the plug-in can add its listeners and then return.
  Parameters: pluginWorkspaceAccess - The workspace access context - The context the plugin was invoked in.
### pluginStopping

void pluginStopping()

Notified before the Oxygen Eclipse plugin will be stopped.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
