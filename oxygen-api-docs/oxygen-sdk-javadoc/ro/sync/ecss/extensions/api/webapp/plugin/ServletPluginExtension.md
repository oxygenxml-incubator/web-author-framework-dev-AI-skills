Package [ro.sync.ecss.extensions.api.webapp.plugin](package-summary.md)

# Class ServletPluginExtension

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.plugin.ServletPluginExtension
   All Implemented Interfaces: [PluginExtension](../../../../../exml/plugin/PluginExtension.md)   Direct Known Subclasses: [ServletPluginConfigExtension](ServletPluginConfigExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ServletPluginExtension extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [PluginExtension](../../../../../exml/plugin/PluginExtension.md)
This abstract class should be extended in order to create a servlet.

To register the servlet you just have to declare an extension of type "WebappServlet" in the plugin's plugin.xml file. For example: <extension type="WebappServlet" class="com.domain.example.ServletPluginExtensionImpl"/>

Web Author installs servlet extensions automatically, each one receiving requests from specific URLs based on the path returned by the [getPath()](#getPath()) method.

For example, if the Web Author is available at https://example.com/oxygen-xml-web-author/ and the [getPath()](#getPath()) method returns custom-path, the servlet handles requests for the URLs starting with: https://example.com/oxygen-xml-web-author/plugins-dispatcher/custom-path/.
  Since: 26
## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [ServletConfig](servlet/ServletConfig.md) [config](#config)
The servlet configuration.

## Constructor Summary
 Constructors
Constructor

Description
 [ServletPluginExtension](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 void [doDelete](#doDelete(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse))([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)
Servlet's doDelete method.
  void [doGet](#doGet(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse))([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)
Servlet's doGet method.
  void [doPost](#doPost(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse))([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)
Servlet's doPost method.
  void [doPut](#doPut(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse))([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)
Servlet's doPut method.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPath](#getPath())()
Should be implemented to return the relative path handled by this plugin.
  [ServletConfig](servlet/ServletConfig.md) [getServletConfig](#getServletConfig())()

 void [init](#init())()
Servlet's init() method.
  void [init](#init(ro.sync.ecss.extensions.api.webapp.plugin.servlet.ServletConfig))([ServletConfig](servlet/ServletConfig.md) config)
Init function that stores the config.
  boolean [requiresAuthorization](#requiresAuthorization())()

 void [service](#service(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse))([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)
Servlet's service method.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### config

protected [ServletConfig](servlet/ServletConfig.md) config

The servlet configuration.

## Constructor Details

### ServletPluginExtension

public ServletPluginExtension()

## Method Details

### getPath

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPath()

Should be implemented to return the relative path handled by this plugin. The path should be unique among other webapp servlet plugins paths and should contain only lower case letters or the '-' sign. Example: "plugin-path"
  Returns: the path at which the servlet will be accessed.
### init

public void init([ServletConfig](servlet/ServletConfig.md) config)throws [ServletException](servlet/ServletException.md)

Init function that stores the config. Consider overriding the [init()](#init()) method instead. If you decide to override this one, call the super implementation.
  Parameters: config - The configuration. Throws: [ServletException](servlet/ServletException.md)
### init

public void init() throws [ServletException](servlet/ServletException.md)

Servlet's init() method.
  Throws: [ServletException](servlet/ServletException.md)
### service

public void service([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)throws [ServletException](servlet/ServletException.md), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Servlet's service method.
  Parameters: req - the request. resp - the response. Throws: [ServletException](servlet/ServletException.md) [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### doGet

public void doGet([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)throws [ServletException](servlet/ServletException.md), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Servlet's doGet method.
  Parameters: req - the request. resp - the response. Throws: [ServletException](servlet/ServletException.md) [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### doPost

public void doPost([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)throws [ServletException](servlet/ServletException.md), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Servlet's doPost method.
  Parameters: req - the request. resp - the response. Throws: [ServletException](servlet/ServletException.md) [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### doPut

public void doPut([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)throws [ServletException](servlet/ServletException.md), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Servlet's doPut method.
  Parameters: req - the request. resp - the response. Throws: [ServletException](servlet/ServletException.md) [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### doDelete

public void doDelete([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)throws [ServletException](servlet/ServletException.md), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Servlet's doDelete method.
  Parameters: req - the request. resp - the response. Throws: [ServletException](servlet/ServletException.md) [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### getServletConfig

public [ServletConfig](servlet/ServletConfig.md) getServletConfig()
  Returns: Returns the servlet configuration.
### requiresAuthorization

public boolean requiresAuthorization()
  Returns: True if this extension requires user to be authenticated as administrator.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
