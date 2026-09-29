Package [ro.sync.ecss.extensions.api.webapp.plugin](package-summary.md)

# Class PluginConfigExtension

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.webapp.plugin.WebappServletPluginExtension](WebappServletPluginExtension.md)
        * ro.sync.ecss.extensions.api.webapp.plugin.PluginConfigExtension
   All Implemented Interfaces: [PluginExtension](../../../../../exml/plugin/PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) [@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public abstract class PluginConfigExtension extends [WebappServletPluginExtension](WebappServletPluginExtension.md) Deprecated.
This API is deprecated because it's based on javax package that's no more supported starting with Servlet 5.0 specification and because this extension type isn't protected against CSRF attacks. Use [ServletPluginConfigExtension](ServletPluginConfigExtension.md) instead.

This class should be extended to create a configuration page for a Web Author plugin. For common use-cases, only the abstract methods should be implemented/overridden.

This class creates an HTML form that will be presented in the Administration Page to the user to configure some options. The options will be applied for all the users.

These options can be read from the server-side code like in the code snippet below: PluginWorkspaceProvider.getPluginWorkspace().getOptionsStorage().getOption("option_name", "default_value");

The options can be read from client-side like in the code snippet below: sync.options.PluginsOptions.getClientOption('option_name');

 Make sure to call super.init() in the extended class otherwise you won't be able to manipulate the options.
  Since: 17.1
## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.api.webapp.plugin.[WebappServletPluginExtension](WebappServletPluginExtension.md)
 [config](WebappServletPluginExtension.md#config)
## Constructor Summary
 Constructors
Constructor

Description
 [PluginConfigExtension](#%3Cinit%3E())()  Deprecated.
In the derived class make sure to set the default options.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 void [doDelete](#doDelete(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse))(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)  Deprecated.
This method should return a plugin to its default options.
  void [doGet](#doGet(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse))(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)  Deprecated.
This method responds with the plugin configuration page (html/css/js).
  void [doPut](#doPut(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse))(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)  Deprecated.
The request body of this request should contain a JSON object of the options to set, containing only key-value pairs with value being a string and not an object.
  [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getDefaultOptions](#getDefaultOptions())()
 Deprecated.
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOption](#getOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)  Deprecated.
Returns the option for the given key or the default value if the key doesn't exist.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOptionsForm](#getOptionsForm())()  Deprecated.
Implement this method to return an HTML form containing the options which should be modified using the administration page.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOptionsJson](#getOptionsJson())()  Deprecated.
Returns the options available of the client-side in JSON format.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPath](#getPath())()  Deprecated.
Should be implemented to return the relative path handled by this plugin.
  void [init](#init())()  Deprecated.
Derived classes should make sure to call this method.
  final boolean [requiresAuthorization](#requiresAuthorization())()  Deprecated.
PluginConfigExtensions will only serve content if the user is authenticated.
  protected void [saveOptions](#saveOptions())()  Deprecated.
Saves the set options to disk.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [serializeMapToJSON](#serializeMapToJSON(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> map)  Deprecated.
Serializes a map to a JSON string.
  void [setDefaultOptions](#setDefaultOptions(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> defaultOptions)  Deprecated.
Sets the default options for this plugin configuration extension.
  protected void [setOption](#setOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)  Deprecated.
Sets the value of an option referenced by its key.

### Methods inherited from class ro.sync.ecss.extensions.api.webapp.plugin.[WebappServletPluginExtension](WebappServletPluginExtension.md)
 [doPost](WebappServletPluginExtension.md#doPost(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse)), [getServletConfig](WebappServletPluginExtension.md#getServletConfig()), [init](WebappServletPluginExtension.md#init(javax.servlet.ServletConfig)), [service](WebappServletPluginExtension.md#service(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### PluginConfigExtension

public PluginConfigExtension()
 Deprecated.
In the derived class make sure to set the default options.

## Method Details

### getPath

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPath()
 Deprecated.
Should be implemented to return the relative path handled by this plugin. The path should be unique among other webapp servlet plugins paths and not an empty String. and should contain only lower case letters or the '-' sign. Example: "plugin-path".
  Specified by: [getPath](WebappServletPluginExtension.md#getPath()) in class [WebappServletPluginExtension](WebappServletPluginExtension.md) Returns: The path at which the servlet will be accessed.
### init

public void init() throws javax.servlet.ServletException
 Deprecated.
Derived classes should make sure to call this method.
  Overrides: [init](WebappServletPluginExtension.md#init()) in class [WebappServletPluginExtension](WebappServletPluginExtension.md) Throws: javax.servlet.ServletException - Thrown to respect the interface
### doGet

public void doGet(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)throws javax.servlet.ServletException, [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Deprecated.
This method responds with the plugin configuration page (html/css/js).
  Overrides: [doGet](WebappServletPluginExtension.md#doGet(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse)) in class [WebappServletPluginExtension](WebappServletPluginExtension.md) Parameters: req - The HTTP request resp - The HTTP response Throws: javax.servlet.ServletException - To respect the interface [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - Thrown by getWriter
### doPut

public void doPut(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)throws javax.servlet.ServletException, [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Deprecated.
The request body of this request should contain a JSON object of the options to set, containing only key-value pairs with value being a string and not an object. Derived methods should use setOption in this method. And afterwards call saveOptions().
  Overrides: [doPut](WebappServletPluginExtension.md#doPut(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse)) in class [WebappServletPluginExtension](WebappServletPluginExtension.md) Parameters: req - The HTTP request object resp - The HTTP response object Throws: javax.servlet.ServletException - To respect the interface [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the options file is not found or storing the options encounters an error
### doDelete

public void doDelete(javax.servlet.http.HttpServletRequest req, javax.servlet.http.HttpServletResponse resp)throws javax.servlet.ServletException, [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Deprecated.
This method should return a plugin to its default options.

It sets the options back to their defaults and saves them on disk.

In derived classes return your plugin to the default options and call the super method to set the options to the default values and save them on disk.
  Overrides: [doDelete](WebappServletPluginExtension.md#doDelete(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse)) in class [WebappServletPluginExtension](WebappServletPluginExtension.md) Parameters: req - The HTTP request object resp - The HTTP response object Throws: javax.servlet.ServletException - To respect the interface [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - When the options file is not found or storing options encounters an error
### getOption

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)
 Deprecated.
Returns the option for the given key or the default value if the key doesn't exist.
  Parameters: key - The key for the option to return defaultValue - The value to return if the key doesn't exist Returns: The option for the given key or the default value if the key doesn't exist
### setOption

protected void setOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
 Deprecated.
Sets the value of an option referenced by its key.
  Parameters: key - The key of the option to set value - The value of the option to set
### saveOptions

protected void saveOptions() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Deprecated.
Saves the set options to disk.
  Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - Couldn't save options.
### getDefaultOptions

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getDefaultOptions()
 Deprecated.  Returns: the defaultOptions
### setDefaultOptions

public void setDefaultOptions([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> defaultOptions)
 Deprecated.
Sets the default options for this plugin configuration extension.
If you want the default values for your options to be empty/null make sure to set them as empty/null, don't leave them out of the defaultOptions map.

  Parameters: defaultOptions - the defaultOptions to set
### getOptionsForm

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOptionsForm()
 Deprecated.
Implement this method to return an HTML form containing the options which should be modified using the administration page. The form inputs name attribute should be the option name.
  Returns: The options form representing an html form with inputs where every input's name attribute represents the name of the option which we want to set.
### getOptionsJson

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOptionsJson()
 Deprecated.
Returns the options available of the client-side in JSON format. These options will be available for all type of users so you should not include sensitive options that should require authorization.
  Returns: the options available on client formated as JSON.
### requiresAuthorization

public final boolean requiresAuthorization()
 Deprecated.
PluginConfigExtensions will only serve content if the user is authenticated.
  Overrides: [requiresAuthorization](WebappServletPluginExtension.md#requiresAuthorization()) in class [WebappServletPluginExtension](WebappServletPluginExtension.md) Returns: True to require authorization
### serializeMapToJSON

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) serializeMapToJSON([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> map)
 Deprecated.
Serializes a map to a JSON string.
  Parameters: map - the map to serialize to JSON string. Returns: the map serialized as a JSON.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
