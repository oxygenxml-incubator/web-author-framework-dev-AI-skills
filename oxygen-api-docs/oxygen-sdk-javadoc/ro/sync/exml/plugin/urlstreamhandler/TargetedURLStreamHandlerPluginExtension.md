Package [ro.sync.exml.plugin.urlstreamhandler](package-summary.md)

# Interface TargetedURLStreamHandlerPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md), [URLStreamHandlerPluginExtensionConstants](URLStreamHandlerPluginExtensionConstants.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface TargetedURLStreamHandlerPluginExtensionextends [PluginExtension](../PluginExtension.md), [URLStreamHandlerPluginExtensionConstants](URLStreamHandlerPluginExtensionConstants.md)
Usually oXygen has specific fixed URL stream handlers for http and https protocols. This URL stream handler plugin extension provides the possibility to impose custom stream handlers for specific URLs.  If the plugin decides that it could handle connections for a particular protocol ([canHandleProtocol(String)](#canHandleProtocol(java.lang.String))), it will be asked to provide the handler for each opened connection of an URL having that protocol([getURLStreamHandler(URL)](#getURLStreamHandler(java.net.URL))).  This extension can be useful in situations when opened connections from a specific host must be handled in a particular way. For example, the Oxygen HTTP URLStreamHandler may not be compatible for sending and receiving SOAP using the SUN Webservices implementation. In this case you can override the stream handler set by Oxygen for HTTP to use the default SUN URLStreamHandler which is more compatible with sending and receiving SOAP requests.  This extension can handle the following protocols: http, https, ftp or sftp.  If it is necessary to impose the application stream URL handlers for protocols different than the one handled by the application, the [URLStreamHandlerPluginExtension](URLStreamHandlerPluginExtension.md) can be used.
  Since: 13.2
## Field Summary

### Fields inherited from interface ro.sync.exml.plugin.urlstreamhandler.[URLStreamHandlerPluginExtensionConstants](URLStreamHandlerPluginExtensionConstants.md)
 [ADVICE_CLOSE](URLStreamHandlerPluginExtensionConstants.md#ADVICE_CLOSE), [ADVICE_RELOAD](URLStreamHandlerPluginExtensionConstants.md#ADVICE_RELOAD), [LOCATION_HEADER](URLStreamHandlerPluginExtensionConstants.md#LOCATION_HEADER), [OXYGEN_ACTION_HEADER](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_ACTION_HEADER), [OXYGEN_READ_ONLY_HEADER](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_READ_ONLY_HEADER), [OXYGEN_READ_ONLY_REASON_CODE_HEADER](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_READ_ONLY_REASON_CODE_HEADER), [OXYGEN_READ_ONLY_REASON_HEADER](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_READ_ONLY_REASON_HEADER), [OXYGEN_SAVE_TYPE](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_SAVE_TYPE), [SAVE_AS](URLStreamHandlerPluginExtensionConstants.md#SAVE_AS), [SAVE_AUTO](URLStreamHandlerPluginExtensionConstants.md#SAVE_AUTO)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [canHandleProtocol](#canHandleProtocol(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol)
Check if the plugin can handle a specific protocol.
  [URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html) [getURLStreamHandler](#getURLStreamHandler(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Get the URL handler for the specified URL.

## Method Details

### canHandleProtocol

boolean canHandleProtocol([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol)

Check if the plugin can handle a specific protocol. If this method returns true for a specific protocol, the [getURLStreamHandler(URL)](#getURLStreamHandler(java.net.URL)) method will be called for each opened connection of an URL having this protocol. The plugin can handle multiple protocols like: http, https, ftp, sftp.
  Parameters: protocol - The protocol. Returns: true if this plugin extension can handle this protocol type.
### getURLStreamHandler

[URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html) getURLStreamHandler([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Get the URL handler for the specified URL. This method is called for each opened connection of an URL with a protocol for which the [canHandleProtocol(String)](#canHandleProtocol(java.lang.String)) method returns true. If this method returns null, the Oxygen [URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html) is used.
  Parameters: url - The URL to provide a handler for. Returns: The URL stream handler.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
