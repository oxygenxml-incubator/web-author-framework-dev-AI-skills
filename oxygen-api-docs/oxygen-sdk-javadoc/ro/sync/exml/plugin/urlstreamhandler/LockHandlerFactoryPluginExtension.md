Package [ro.sync.exml.plugin.urlstreamhandler](package-summary.md)

# Interface LockHandlerFactoryPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   All Known Subinterfaces: [URLStreamHandlerWithLockPluginExtension](URLStreamHandlerWithLockPluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface LockHandlerFactoryPluginExtensionextends [PluginExtension](../PluginExtension.md)
Extension used for locking resources from a specific protocol
  Since: 13.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [LockHandler](../lock/LockHandler.md) [getLockHandler](#getLockHandler())()
Get the lock handler for the current handled protocol.
  boolean [isLockingSupported](#isLockingSupported(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol)
Check if a lock handler can be provided for a specific protocol.

## Method Details

### getLockHandler

[LockHandler](../lock/LockHandler.md) getLockHandler()

Get the lock handler for the current handled protocol. Might be null if not supported.
  Returns: The lock handler for this extension, or null if not supported.
### isLockingSupported

boolean isLockingSupported([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol)

Check if a lock handler can be provided for a specific protocol.
  Parameters: protocol - The URL protocol (like "http" or "file") Returns: true if this extension can return a lock handler for the protocol.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
