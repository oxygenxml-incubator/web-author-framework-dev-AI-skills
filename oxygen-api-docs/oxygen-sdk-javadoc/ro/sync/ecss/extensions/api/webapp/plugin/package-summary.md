# Package ro.sync.ecss.extensions.api.webapp.plugin

package ro.sync.ecss.extensions.api.webapp.plugin
    Related Packages
Package

Description
 [ro.sync.ecss.extensions.api.webapp](../package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.plugin.servlet](servlet/package-summary.md)

     All Classes and InterfacesInterfacesClassesExceptions
Class

Description
 [FilterURLConnection](FilterURLConnection.md)
URLConnection that delegates all methods to the connection given as a parameter.
  [LockHandlerWithContext](LockHandlerWithContext.md)
A base-class to be extended to implement lock/unlock functionality.
  [PluginConfigExtension](PluginConfigExtension.md)
Deprecated.
This API is deprecated because it's based on javax package that's no more supported starting with Servlet 5.0 specification and because this extension type isn't protected against CSRF attacks.

 [RedirectFollowingURLConnection](RedirectFollowingURLConnection.md)
Marker interface that indicates that the URLConnection follows redirects.
  [ServletPluginConfigExtension](ServletPluginConfigExtension.md)
This class should be extended to create a configuration page for a Web Author plugin.
  [ServletPluginExtension](ServletPluginExtension.md)
This abstract class should be extended in order to create a servlet.
  [URLStreamHandlerWithContext](URLStreamHandlerWithContext.md)
A base-class for URLStreamHandlers that need a context for the URL whose connection is to be opened.
  [URLStreamHandlerWithContextUtil](URLStreamHandlerWithContextUtil.md)
Utility class for adding/removing the user context id from the URLs.
  [UserActionRequiredException](UserActionRequiredException.md)
Class that extends an IOException with an WebappMessage that should be sent to the client-side code.
  [UserActionRequiredMessage](UserActionRequiredMessage.md)
Contains details for the server message that is presented on client side when a user action required exception is thrown.
  [UserContext](UserContext.md)
The context of the user that opened the URL.
  [WebappServletPluginExtension](WebappServletPluginExtension.md)
Deprecated.
This API is deprecated because it's based on javax package that's no more supported starting with Servlet 5.0 specification and because this extension type isn't protected against CSRF attacks.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
