Package [ro.sync.exml.workspace.api.standalone.proxy](package-summary.md)

# Interface ProxyDetailsProvider
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ProxyDetailsProvider
Provides the proxy details for connecting to a specific URL
  Since: 19.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 ro.sync.exml.workspace.api.standalone.proxy.ProxyConnectionInfo [getProxyConnectionInfo](#getProxyConnectionInfo(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Get information about proxy configuration in order to access a certain URL.

## Method Details

### getProxyConnectionInfo

ro.sync.exml.workspace.api.standalone.proxy.ProxyConnectionInfo getProxyConnectionInfo([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Get information about proxy configuration in order to access a certain URL. If the URL is null you might not get accurate information, for example the "no proxy for..." host names information will not be used.
  Parameters: url - The URL to access. Returns: information about network proxy configuration in order to access a certain URL. Can be null if there is no network proxy configured on the system.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
