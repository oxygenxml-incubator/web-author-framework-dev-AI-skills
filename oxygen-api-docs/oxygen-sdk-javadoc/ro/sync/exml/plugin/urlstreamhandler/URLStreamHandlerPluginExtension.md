Package [ro.sync.exml.plugin.urlstreamhandler](package-summary.md)

# Interface URLStreamHandlerPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md), [URLStreamHandlerPluginExtensionConstants](URLStreamHandlerPluginExtensionConstants.md)   All Known Subinterfaces: [URLStreamHandlerWithLockPluginExtension](URLStreamHandlerWithLockPluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface URLStreamHandlerPluginExtensionextends [PluginExtension](../PluginExtension.md), [URLStreamHandlerPluginExtensionConstants](URLStreamHandlerPluginExtensionConstants.md)
This URL stream handler provides the possibility to impose the URL stream handlers for specific protocols.  This plugin extension can provide URL stream handlers for multiple protocols, other than then ones handled by the application (like file, http, ftp, sftp or https).  If it is necessary to impose the application stream URL handlers for specific URLs with protocols like:http, https, ftp or sftp, the [TargetedURLStreamHandlerPluginExtension](TargetedURLStreamHandlerPluginExtension.md) can be used.

## Field Summary

### Fields inherited from interface ro.sync.exml.plugin.urlstreamhandler.[URLStreamHandlerPluginExtensionConstants](URLStreamHandlerPluginExtensionConstants.md)
 [ADVICE_CLOSE](URLStreamHandlerPluginExtensionConstants.md#ADVICE_CLOSE), [ADVICE_RELOAD](URLStreamHandlerPluginExtensionConstants.md#ADVICE_RELOAD), [LOCATION_HEADER](URLStreamHandlerPluginExtensionConstants.md#LOCATION_HEADER), [OXYGEN_ACTION_HEADER](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_ACTION_HEADER), [OXYGEN_READ_ONLY_HEADER](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_READ_ONLY_HEADER), [OXYGEN_READ_ONLY_REASON_CODE_HEADER](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_READ_ONLY_REASON_CODE_HEADER), [OXYGEN_READ_ONLY_REASON_HEADER](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_READ_ONLY_REASON_HEADER), [OXYGEN_SAVE_TYPE](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_SAVE_TYPE), [SAVE_AS](URLStreamHandlerPluginExtensionConstants.md#SAVE_AS), [SAVE_AUTO](URLStreamHandlerPluginExtensionConstants.md#SAVE_AUTO)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html) [getURLStreamHandler](#getURLStreamHandler(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol)
Get the URL handler for the specified protocol.

## Method Details

### getURLStreamHandler

[URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html) getURLStreamHandler([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol)

Get the URL handler for the specified protocol.
  Parameters: protocol - The name of the protocol. Returns: The handler for the protocol or null if it does not know it.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
