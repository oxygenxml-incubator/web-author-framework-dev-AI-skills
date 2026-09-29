Package [ro.sync.ecss.extensions.api.webapp.plugin](package-summary.md)

# Class ServletPluginConfigExtension

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.webapp.plugin.ServletPluginExtension](ServletPluginExtension.md)
        * ro.sync.ecss.extensions.api.webapp.plugin.ServletPluginConfigExtension
   All Implemented Interfaces: [PluginExtension](../../../../../exml/plugin/PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ServletPluginConfigExtension extends [ServletPluginExtension](ServletPluginExtension.md)
This class should be extended to create a configuration page for a Web Author plugin. For common use-cases, only the abstract methods should be implemented/overridden.

This class creates an HTML form that will be presented in the Administration Page to the user to configure some options. The options will be applied for all the users.

These options can be read from the server-side code like in the code snippet below: PluginWorkspaceProvider.getPluginWorkspace().getOptionsStorage().getOption("option_name", "default_value");

The options can be read from client-side like in the code snippet below: sync.options.PluginsOptions.getClientOption('option_name');

 Make sure to call super.init() in the extended class otherwise you won't be able to manipulate the options.
  Since: 26
## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.api.webapp.plugin.[ServletPluginExtension](ServletPluginExtension.md)
 [config](ServletPluginExtension.md#config)
## Constructor Summary
 Constructors
Constructor

Description
 [ServletPluginConfigExtension](#%3Cinit%3E())()
In the derived class make sure to set the default options.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 void [doDelete](#doDelete(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse))([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)
This method should return a plugin to its default options.
  void [doGet](#doGet(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse))([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)
This method responds with the plugin configuration page (html/css/js).
  void [doPut](#doPut(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse))([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)
The request body of this request should contain a JSON object of the options to set, containing only key-value pairs with value being a string and not an object.
  [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getDefaultOptions](#getDefaultOptions())()

 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOption](#getOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)
Returns the option for the given key or the default value if the key doesn't exist.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOptionsForm](#getOptionsForm())()
Implement this method to return an HTML form containing the options which should be modified using the administration page.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOptionsJson](#getOptionsJson())()
Returns the options available of the client-side in JSON format.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOrMigrateSecretOption](#getOrMigrateSecretOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)
Retrieves a secret option with migration support.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPath](#getPath())()
Should be implemented to return the relative path handled by this plugin.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSecretOption](#getSecretOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)
Returns the secret option for the given key or the default value if the key doesn't exist.
  void [init](#init())()
Derived classes should make sure to call this method.
  final boolean [requiresAuthorization](#requiresAuthorization())()
PluginConfigExtensions will only serve content if the user is authenticated.
  protected void [saveOptions](#saveOptions())()
Saves the set options to disk.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [serializeMapToJSON](#serializeMapToJSON(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> map)
Serializes a map to a JSON string.
  void [setDefaultOptions](#setDefaultOptions(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> defaultOptions)
Sets the default options for this plugin configuration extension.
  protected void [setOption](#setOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Sets the value of an option referenced by its key.
  protected void [setSecretOption](#setSecretOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Sets the value of a secret option referenced by its key.

### Methods inherited from class ro.sync.ecss.extensions.api.webapp.plugin.[ServletPluginExtension](ServletPluginExtension.md)
 [doPost](ServletPluginExtension.md#doPost(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse)), [getServletConfig](ServletPluginExtension.md#getServletConfig()), [init](ServletPluginExtension.md#init(ro.sync.ecss.extensions.api.webapp.plugin.servlet.ServletConfig)), [service](ServletPluginExtension.md#service(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ServletPluginConfigExtension

public ServletPluginConfigExtension()

In the derived class make sure to set the default options.

## Method Details

### getPath

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPath()

Should be implemented to return the relative path handled by this plugin. The path should be unique among other webapp servlet plugins paths and not an empty String. and should contain only lower case letters or the '-' sign. Example: "plugin-path".
  Specified by: [getPath](ServletPluginExtension.md#getPath()) in class [ServletPluginExtension](ServletPluginExtension.md) Returns: The path at which the servlet will be accessed.
### init

public void init() throws [ServletException](servlet/ServletException.md)

Derived classes should make sure to call this method.
  Overrides: [init](ServletPluginExtension.md#init()) in class [ServletPluginExtension](ServletPluginExtension.md) Throws: [ServletException](servlet/ServletException.md) - Thrown to respect the interface
### doGet

public void doGet([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)throws [ServletException](servlet/ServletException.md), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

This method responds with the plugin configuration page (html/css/js).
  Overrides: [doGet](ServletPluginExtension.md#doGet(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse)) in class [ServletPluginExtension](ServletPluginExtension.md) Parameters: req - The HTTP request resp - The HTTP response Throws: [ServletException](servlet/ServletException.md) - To respect the interface [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - Thrown by getWriter
### doPut

public void doPut([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)throws [ServletException](servlet/ServletException.md), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

The request body of this request should contain a JSON object of the options to set, containing only key-value pairs with value being a string and not an object. Derived methods should use setOption in this method. And afterwards call saveOptions().
  Overrides: [doPut](ServletPluginExtension.md#doPut(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse)) in class [ServletPluginExtension](ServletPluginExtension.md) Parameters: req - The HTTP request object resp - The HTTP response object Throws: [ServletException](servlet/ServletException.md) - To respect the interface [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the options file is not found or storing the options encounters an error
### doDelete

public void doDelete([HttpServletRequest](servlet/http/HttpServletRequest.md) req, [HttpServletResponse](servlet/http/HttpServletResponse.md) resp)throws [ServletException](servlet/ServletException.md), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

This method should return a plugin to its default options.

It sets the options back to their defaults and saves them on disk.

In derived classes return your plugin to the default options and call the super method to set the options to the default values and save them on disk.
  Overrides: [doDelete](ServletPluginExtension.md#doDelete(ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletRequest,ro.sync.ecss.extensions.api.webapp.plugin.servlet.http.HttpServletResponse)) in class [ServletPluginExtension](ServletPluginExtension.md) Parameters: req - The HTTP request object resp - The HTTP response object Throws: [ServletException](servlet/ServletException.md) - To respect the interface [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - When the options file is not found or storing options encounters an error
### getOption

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)

Returns the option for the given key or the default value if the key doesn't exist.
  Parameters: key - The key for the option to return defaultValue - The value to return if the key doesn't exist Returns: The option for the given key or the default value if the key doesn't exist
### getSecretOption

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSecretOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)

Returns the secret option for the given key or the default value if the key doesn't exist.
  Parameters: key -  defaultValue -  Returns: The secret option for the given key or the default value if the key doesn't exist
### getOrMigrateSecretOption

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOrMigrateSecretOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)

Retrieves a secret option with migration support. If no encrypted option is found, it falls back to a non-encrypted value, encrypts it, saves it securely, and removes the non-encrypted version.
  Parameters: key - The key for the option. defaultValue - The default value to return if no option is found. Returns: The decrypted value, or the default value if neither is found.
### setOption

protected void setOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Sets the value of an option referenced by its key.
  Parameters: key - The key of the option to set value - The value of the option to set
### setSecretOption

protected void setSecretOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Sets the value of a secret option referenced by its key.
  Parameters: key - The key of the option to set value - The value of the secret option to set
### saveOptions

protected void saveOptions() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Saves the set options to disk.
  Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - Couldn't save options.
### getDefaultOptions

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getDefaultOptions()
  Returns: the defaultOptions
### setDefaultOptions

public void setDefaultOptions([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> defaultOptions)

Sets the default options for this plugin configuration extension.
If you want the default values for your options to be empty/null make sure to set them as empty/null, don't leave them out of the defaultOptions map.

  Parameters: defaultOptions - the defaultOptions to set
### getOptionsForm

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOptionsForm()

Implement this method to return an HTML form containing the options which should be modified using the administration page. The form inputs name attribute should be the option name.
  Returns: The options form representing an html form with inputs where every input's name attribute represents the name of the option which we want to set.
### getOptionsJson

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOptionsJson()

Returns the options available of the client-side in JSON format. These options will be available for all type of users so you should not include sensitive options that should require authorization.
  Returns: the options available on client formated as JSON.
### requiresAuthorization

public final boolean requiresAuthorization()

PluginConfigExtensions will only serve content if the user is authenticated.
  Overrides: [requiresAuthorization](ServletPluginExtension.md#requiresAuthorization()) in class [ServletPluginExtension](ServletPluginExtension.md) Returns: True to require authorization
### serializeMapToJSON

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) serializeMapToJSON([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> map)

Serializes a map to a JSON string.
  Parameters: map - the map to serialize to JSON string. Returns: the map serialized as a JSON.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
