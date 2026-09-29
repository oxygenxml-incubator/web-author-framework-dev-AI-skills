# Package ro.sync.exml.plugin.urlstreamhandler

package ro.sync.exml.plugin.urlstreamhandler
    Related Packages
Package

Description
 [ro.sync.exml.plugin](../package-summary.md)

     Interfaces
Class

Description
 [CacheableUrlConnection](CacheableUrlConnection.md)
Marker interface that should be implemented by a URL connection and which instructs oXygen that it makes sense to cache data read from such a connection.
  [LockHandlerFactoryPluginExtension](LockHandlerFactoryPluginExtension.md)
Extension used for locking resources from a specific protocol
  [TargetedURLStreamHandlerPluginExtension](TargetedURLStreamHandlerPluginExtension.md)
Usually oXygen has specific fixed URL stream handlers for http and https protocols.
  [URLChooserMenuExtension](URLChooserMenuExtension.md)
Get the name of the action which will be displayed in the File menu.
  [URLChooserPluginExtension](URLChooserPluginExtension.md)
Deprecated.
This approach will continue to work but it is recommanded to use the **ro.sync.exml.plugin.urlstreamhandler.URLChooserPluginExtension2** interface which also receives access to the Oxygen workspace.

 [URLChooserPluginExtension2](URLChooserPluginExtension2.md)
URL chooser plugin extension.
  [URLChooserToolbarExtension](URLChooserToolbarExtension.md)
URL chooser toolbar extension.
  [URLHandlerReadOnlyCheckerExtension](URLHandlerReadOnlyCheckerExtension.md)
This interface can be called to decide if an URL is read-only or not.
  [URLStreamHandlerPluginExtension](URLStreamHandlerPluginExtension.md)
This URL stream handler provides the possibility to impose the URL stream handlers for specific protocols.
  [URLStreamHandlerPluginExtensionConstants](URLStreamHandlerPluginExtensionConstants.md)
Constants used from URLStreamHandler provider plugin extensions.
  [URLStreamHandlerWithLockPluginExtension](URLStreamHandlerWithLockPluginExtension.md)
An URLStreamHandler with lock support plugin extension.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
