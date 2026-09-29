Package [ro.sync.ecss.extensions.api.webapp.plugin](package-summary.md)

# Class WebappServletPluginExtension

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.plugin.WebappServletPluginExtension
   All Implemented Interfaces: [PluginExtension](../../../../../exml/plugin/PluginExtension.md)   Direct Known Subclasses: [PluginConfigExtension](PluginConfigExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) [@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public abstract class WebappServletPluginExtension extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [PluginExtension](../../../../../exml/plugin/PluginExtension.md) Deprecated.
This API is deprecated because it's based on javax package that's no more supported starting with Servlet 5.0 specification and because this extension type isn't protected against CSRF attacks. Use [ServletPluginExtension](ServletPluginExtension.md) instead.

This abstract should be extended in order to create a webapp plugin servlet extension.

To register the servlet you just have to declare an extension of type "WebappServlet" in the plugin's plugin.xml file.

For example: <extension type="WebappServlet" class="com.domain.example.WebappServletPluginExtensionImpl"/>

The webapp will register it automatically. The Servlet will map it to an URL which is computed from the path returned by the [getPath()](#getPath()) method.

For example, if the webapp is available at http://example.com/xml-editor/ and the [getPath()](#getPath()) method returns mypath, this servlet handles requests for the urls starting with: http://example.com/xml-editor/plugins-dispatcher/mypath/.
  Since: 17
## Field Summary
 Fields
Modifier and Type

Field

Description
 protected javax.servlet.ServletConfig [config](#config)  Deprecated.
The servlet configuration.

## Constructor Summary
 Constructors
Constructor

Description
 [WebappServletPluginExtension](#%3Cinit%3E())()
 Deprecated.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 void [doDelete](#doDelete(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse))(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)  Deprecated.
Servlet's doDelete method.
  void [doGet](#doGet(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse))(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)  Deprecated.
Servlet's doGet method.
  void [doPost](#doPost(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse))(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)  Deprecated.
Servlet's doPost method.
  void [doPut](#doPut(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse))(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)  Deprecated.
Servlet's doPut method.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPath](#getPath())()  Deprecated.
Should be implemented to return the relative path handled by this plugin.
  javax.servlet.ServletConfig [getServletConfig](#getServletConfig())()
 Deprecated.
 void [init](#init())()  Deprecated.
Servlet's init() method.
  void [init](#init(javax.servlet.ServletConfig))(javax.servlet.ServletConfig config)  Deprecated.
Init function that stores the config.
  boolean [requiresAuthorization](#requiresAuthorization())()
 Deprecated.
 void [service](#service(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse))(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)  Deprecated.
Servlet's service method.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### config

protected javax.servlet.ServletConfig config
 Deprecated.
The servlet configuration.

## Constructor Details

### WebappServletPluginExtension

public WebappServletPluginExtension()
 Deprecated.
## Method Details

### init

public void init(javax.servlet.ServletConfig config)throws javax.servlet.ServletException
 Deprecated.
Init function that stores the config. Consider overriding the [init()](#init()) method instead. If you decide to override this one, call the super implementation.
  Parameters: config - The configuration. Throws: javax.servlet.ServletException
### init

public void init() throws javax.servlet.ServletException
 Deprecated.
Servlet's init() method.
  Throws: javax.servlet.ServletException
### service

public void service(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)throws javax.servlet.ServletException, [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Deprecated.
Servlet's service method.
  Parameters: req - the request. resp - the response. Throws: javax.servlet.ServletException [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### doGet

public void doGet(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)throws javax.servlet.ServletException, [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Deprecated.
Servlet's doGet method.
  Parameters: req - the request. resp - the response. Throws: javax.servlet.ServletException [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### doPost

public void doPost(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)throws javax.servlet.ServletException, [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Deprecated.
Servlet's doPost method.
  Parameters: req - the request. resp - the response. Throws: javax.servlet.ServletException [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### doPut

public void doPut(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)throws javax.servlet.ServletException, [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Deprecated.
Servlet's doPut method.
  Parameters: req - the request. resp - the response. Throws: javax.servlet.ServletException [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### doDelete

public void doDelete(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)throws javax.servlet.ServletException, [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Deprecated.
Servlet's doDelete method.
  Parameters: req - the request. resp - the response. Throws: javax.servlet.ServletException [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### getPath

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPath()
 Deprecated.
Should be implemented to return the relative path handled by this plugin. The path should be unique among other webapp servlet plugins paths and should contain only lower case letters or the '-' sign. Example: "plugin-path"
  Returns: the path at which the servlet will be accessed.
### getServletConfig

public javax.servlet.ServletConfig getServletConfig()
 Deprecated.  Returns: Returns the servlet configuration.
### requiresAuthorization

public boolean requiresAuthorization()
 Deprecated.  Returns: True if this extension requires user to be authenticated as administrator.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
