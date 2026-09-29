# Hierarchy For Package ro.sync.ecss.extensions.api.webapp.plugin
 Package Hierarchies:
* [All Packages](../../../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * ro.sync.exml.plugin.lock.[LockHandlerBase](../../../../../exml/plugin/lock/LockHandlerBase.md) (implements ro.sync.exml.plugin.lock.[LockHandler](../../../../../exml/plugin/lock/LockHandler.md))
        * ro.sync.ecss.extensions.api.webapp.plugin.[LockHandlerWithContext](LockHandlerWithContext.md)

    * ro.sync.ecss.extensions.api.webapp.plugin.[ServletPluginExtension](ServletPluginExtension.md) (implements ro.sync.exml.plugin.[PluginExtension](../../../../../exml/plugin/PluginExtension.md))
        * ro.sync.ecss.extensions.api.webapp.plugin.[ServletPluginConfigExtension](ServletPluginConfigExtension.md)

    * java.lang.[Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html) (implements java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))
        * java.lang.[Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

            * java.io.[IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

                * ro.sync.ecss.extensions.api.webapp.plugin.[UserActionRequiredException](UserActionRequiredException.md)

    * java.net.[URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html)
        * ro.sync.ecss.extensions.api.webapp.plugin.[FilterURLConnection](FilterURLConnection.md) (implements ro.sync.net.protocol.[FileBrowsingConnection](../../../../../net/protocol/FileBrowsingConnection.md))

    * java.net.[URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html)
        * ro.sync.ecss.extensions.api.webapp.plugin.[URLStreamHandlerWithContext](URLStreamHandlerWithContext.md)

    * ro.sync.ecss.extensions.api.webapp.plugin.[URLStreamHandlerWithContextUtil](URLStreamHandlerWithContextUtil.md)
    * ro.sync.ecss.extensions.api.webapp.plugin.[UserContext](UserContext.md)
    * ro.sync.ecss.extensions.api.webapp.[WebappMessage](../WebappMessage.md)
        * ro.sync.ecss.extensions.api.webapp.plugin.[UserActionRequiredMessage](UserActionRequiredMessage.md)

    * ro.sync.ecss.extensions.api.webapp.plugin.[WebappServletPluginExtension](WebappServletPluginExtension.md) (implements ro.sync.exml.plugin.[PluginExtension](../../../../../exml/plugin/PluginExtension.md))

        * ro.sync.ecss.extensions.api.webapp.plugin.[PluginConfigExtension](PluginConfigExtension.md)

## Interface Hierarchy

* ro.sync.ecss.extensions.api.webapp.plugin.[RedirectFollowingURLConnection](RedirectFollowingURLConnection.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
