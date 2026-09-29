Package [ro.sync.exml.plugin](package-summary.md)

# Class PluginDescriptor

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.plugin.PluginDescriptor
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class PluginDescriptor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Descriptor of the plugin.
A plugin is characterised by:

- name The plugin name as it will appear in the oXygen menus.

- description A short description of what the plugin does.

- vendor The name of the vendor.

- version The current version.

- baseDir The base dir used for file crreation.

- extensions A set of extensions.

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static class  [PluginDescriptor.PluginExtensionDescription](PluginDescriptor.PluginExtensionDescription.md)
Contains a plugin description + plugin type + keyboard shortcuts

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ADDITIONAL_DITA_OT](#ADDITIONAL_DITA_OT)
Additional DITA OT plugin type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ADDITIONAL_FRAMEWORKS](#ADDITIONAL_FRAMEWORKS)
Additional frameworks location plugin type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ADDITIONAL_UI_TRANSLATIONS](#ADDITIONAL_UI_TRANSLATIONS)
Additional translations plugin type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ADDITIONAL_XPROC_ENGINE](#ADDITIONAL_XPROC_ENGINE)
Additional XProc Engine type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AI_CONNECTORS](#AI_CONNECTORS)
Extension point for external AI connectors that allow connection to an AI service
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AI_FUNCTIONS](#AI_FUNCTIONS)
Extension point for external AI functions
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AI_HOOKS_HANDLER](#AI_HOOKS_HANDLER)
Extension point for AI hooks handler
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AUTHOR_STYLESHEET](#AUTHOR_STYLESHEET)
Extension that provide an Author CSS.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [COMPONENTS_VALIDATOR_EXTENSION](#COMPONENTS_VALIDATOR_EXTENSION)
The startup extension.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CONFIGURATION_OPTIONS_PROVIDER](#CONFIGURATION_OPTIONS_PROVIDER)
Configuration options provider
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CSP](#CSP)
Extension point to provide additional CSP.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DOCUMENT_PROCESSOR](#DOCUMENT_PROCESSOR)
Document processor extension type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DOCUMENT_VALIDATOR](#DOCUMENT_VALIDATOR)
Extension point for external document validator
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [GENERAL_EXTENSION](#GENERAL_EXTENSION)
General extension type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [GENERAL_STYLES_FILTER](#GENERAL_STYLES_FILTER)
CSS Styles filter plugin type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LOCK_HANDLER_FACTORY](#LOCK_HANDLER_FACTORY)
A lock handler factory.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OPEN_REDIRECTOR](#OPEN_REDIRECTOR)
Open redirector plugin type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OPTION_PAGE](#OPTION_PAGE)
Option page extension plugin type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OPTION_PAGE_GROUP](#OPTION_PAGE_GROUP)
Option page group extension plugin type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [REFACTORING_OPERATIONS_PROVIDER](#REFACTORING_OPERATIONS_PROVIDER)
Refactoring operations provider plugin type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SELECTION_PROCESSOR](#SELECTION_PROCESSOR)
Selection processor extension type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TARGETED_URL_HANDLER](#TARGETED_URL_HANDLER)
Targeted URL stream handler extension type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TRANSFORMER](#TRANSFORMER)
An XSLT transformer extension.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TRUSTED_HOSTS](#TRUSTED_HOSTS)
Extension point to provide trusted hosts.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [URL_CHOOSER](#URL_CHOOSER)
URL stream handler extension type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [URL_CHOOSER_TOOLBAR](#URL_CHOOSER_TOOLBAR)
URL stream handler extension type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [URL_HANDLER](#URL_HANDLER)
URL stream handler extension type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [URL_STREAM_HANDLER](#URL_STREAM_HANDLER)
Deprecated.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [WEBAPP_CSS_RESOURCE](#WEBAPP_CSS_RESOURCE)
WebappStaticResourcesFolder
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [WEBAPP_SERVLET](#WEBAPP_SERVLET)
WebApp plugin servlet.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [WEBAPP_SERVLET_FILTER](#WEBAPP_SERVLET_FILTER)
WebApp plugin servlet filter.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [WEBAPP_STATIC_RESOURCE_FOL](#WEBAPP_STATIC_RESOURCE_FOL)
WebappStaticResourcesFolder
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [WORKSPACE_ACCESS](#WORKSPACE_ACCESS)
Workspace access plugin type.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [WORKSPACE_ACCESS_JS](#WORKSPACE_ACCESS_JS)
Workspace access plugin type implemented in JavaScript.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [WORKSPACE_ACCESS_JS_MODULE](#WORKSPACE_ACCESS_JS_MODULE)
A JavaScript module of the Workspace access plugin.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [XQUERY_TRANSFORMER](#XQUERY_TRANSFORMER)
An XQuery transformer extension.

## Constructor Summary
 Constructors
Constructor

Description
 [PluginDescriptor](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addContextInstance](#addContextInstance(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) contextInstance)
Add a context instance.
  void [addExtension](#addExtension(ro.sync.exml.plugin.PluginDescriptor.PluginExtensionDescription))([PluginDescriptor.PluginExtensionDescription](PluginDescriptor.PluginExtensionDescription.md) descr)
Put an extension corresponding to the specified key.
  void [addPluginContributedToolbar](#addPluginContributedToolbar(ro.sync.exml.plugin.PluginContributedToolbar))(ro.sync.exml.plugin.PluginContributedToolbar toolbarInfo)
Add a toolbar.
  void [addPluginContributedView](#addPluginContributedView(ro.sync.exml.plugin.PluginContributedView))(ro.sync.exml.plugin.PluginContributedView viewInfo)
Add a contributed view
  [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [getBaseDir](#getBaseDir())()
Get the base directory of the plugin.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getConfigUrlPath](#getConfigUrlPath())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> [getContextInstances](#getContextInstances())()
Getter for all context instances.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.exml.plugin.PluginContributedToolbar> [getContributedToolbars](#getContributedToolbars())()
Gets the toolbars contributed by this plugin.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.exml.plugin.PluginContributedView> [getContributedViews](#getContributedViews())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()
Get the description of the plugin.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[PluginDescriptor.PluginExtensionDescription](PluginDescriptor.PluginExtensionDescription.md)> [getExtensions](#getExtensions())()
Get all the extensions of a plugin.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[PluginDescriptor.PluginExtensionDescription](PluginDescriptor.PluginExtensionDescription.md)> [getExtensions](#getExtensions(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
Get the extension corresponding to the specified key.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getID](#getID())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLicense](#getLicense())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Gets the name of the plugin.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getVendor](#getVendor())()
Get the vendor of the plugin.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getVersion](#getVersion())()
Get the version of the plugin.
  boolean [isDisabledFromFile](#isDisabledFromFile())()

 boolean [isEnabledStatus](#isEnabledStatus())()
Get the enabled status.
  void [setBaseDir](#setBaseDir(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) baseDir)
Set the base dir of the plugin.
  void [setConfigUrlPath](#setConfigUrlPath(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) configUrlPath)

 void [setDescription](#setDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description)
Set the description of the plugin.
  void [setDisabledFromFile](#setDisabledFromFile(boolean))(boolean isDisabledFromFile)
Sets the disabled status from 'plugin.disable' file.
  void [setEnabledStatus](#setEnabledStatus(boolean))(boolean enabledStatus)
Set the plugin enabled status.
  void [setID](#setID(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) id)
Sets the ID of the plugin.
  void [setLicense](#setLicense(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) license)

 void [setName](#setName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Set the name of the plugin.
  void [setShouldAcceptLicense](#setShouldAcceptLicense(boolean))(boolean shouldAcceptLicense)

 void [setVendor](#setVendor(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) vendor)
Set the vendor of the plugin.
  void [setVersion](#setVersion(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) version)
Set the version of the plugin.
  boolean [shouldAcceptLicense](#shouldAcceptLicense())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()
The string representation of the plugin descriptor.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### WEBAPP_CSS_RESOURCE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) WEBAPP_CSS_RESOURCE

WebappStaticResourcesFolder
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.WEBAPP_CSS_RESOURCE)

### SELECTION_PROCESSOR

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SELECTION_PROCESSOR

Selection processor extension type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.SELECTION_PROCESSOR)

### WEBAPP_SERVLET_FILTER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) WEBAPP_SERVLET_FILTER

WebApp plugin servlet filter.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.WEBAPP_SERVLET_FILTER)

### WEBAPP_SERVLET

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) WEBAPP_SERVLET

WebApp plugin servlet.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.WEBAPP_SERVLET)

### WEBAPP_STATIC_RESOURCE_FOL

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) WEBAPP_STATIC_RESOURCE_FOL

WebappStaticResourcesFolder
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.WEBAPP_STATIC_RESOURCE_FOL)

### GENERAL_EXTENSION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) GENERAL_EXTENSION

General extension type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.GENERAL_EXTENSION)

### DOCUMENT_PROCESSOR

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DOCUMENT_PROCESSOR

Document processor extension type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.DOCUMENT_PROCESSOR)

### URL_STREAM_HANDLER

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) URL_STREAM_HANDLER
 Deprecated.
URL stream handler extension type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.URL_STREAM_HANDLER)

### URL_HANDLER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) URL_HANDLER

URL stream handler extension type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.URL_HANDLER)

### TARGETED_URL_HANDLER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TARGETED_URL_HANDLER

Targeted URL stream handler extension type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.TARGETED_URL_HANDLER)

### TRANSFORMER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TRANSFORMER

An XSLT transformer extension.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.TRANSFORMER)

### XQUERY_TRANSFORMER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) XQUERY_TRANSFORMER

An XQuery transformer extension.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.XQUERY_TRANSFORMER)

### URL_CHOOSER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) URL_CHOOSER

URL stream handler extension type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.URL_CHOOSER)

### URL_CHOOSER_TOOLBAR

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) URL_CHOOSER_TOOLBAR

URL stream handler extension type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.URL_CHOOSER_TOOLBAR)

### COMPONENTS_VALIDATOR_EXTENSION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) COMPONENTS_VALIDATOR_EXTENSION

The startup extension.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.COMPONENTS_VALIDATOR_EXTENSION)

### OPEN_REDIRECTOR

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OPEN_REDIRECTOR

Open redirector plugin type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.OPEN_REDIRECTOR)

### WORKSPACE_ACCESS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) WORKSPACE_ACCESS

Workspace access plugin type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.WORKSPACE_ACCESS)

### WORKSPACE_ACCESS_JS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) WORKSPACE_ACCESS_JS

Workspace access plugin type implemented in JavaScript.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.WORKSPACE_ACCESS_JS)

### WORKSPACE_ACCESS_JS_MODULE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) WORKSPACE_ACCESS_JS_MODULE

A JavaScript module of the Workspace access plugin.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.WORKSPACE_ACCESS_JS_MODULE)

### OPTION_PAGE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OPTION_PAGE

Option page extension plugin type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.OPTION_PAGE)

### OPTION_PAGE_GROUP

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OPTION_PAGE_GROUP

Option page group extension plugin type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.OPTION_PAGE_GROUP)

### GENERAL_STYLES_FILTER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) GENERAL_STYLES_FILTER

CSS Styles filter plugin type. This filter will be used to filter CSS styles for any document presented in author mode.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.GENERAL_STYLES_FILTER)

### LOCK_HANDLER_FACTORY

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LOCK_HANDLER_FACTORY

A lock handler factory.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.LOCK_HANDLER_FACTORY)

### REFACTORING_OPERATIONS_PROVIDER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) REFACTORING_OPERATIONS_PROVIDER

Refactoring operations provider plugin type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.REFACTORING_OPERATIONS_PROVIDER)

### ADDITIONAL_DITA_OT

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ADDITIONAL_DITA_OT

Additional DITA OT plugin type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.ADDITIONAL_DITA_OT)

### ADDITIONAL_XPROC_ENGINE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ADDITIONAL_XPROC_ENGINE

Additional XProc Engine type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.ADDITIONAL_XPROC_ENGINE)

### AUTHOR_STYLESHEET

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AUTHOR_STYLESHEET

Extension that provide an Author CSS.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.AUTHOR_STYLESHEET)

### ADDITIONAL_FRAMEWORKS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ADDITIONAL_FRAMEWORKS

Additional frameworks location plugin type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.ADDITIONAL_FRAMEWORKS)

### ADDITIONAL_UI_TRANSLATIONS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ADDITIONAL_UI_TRANSLATIONS

Additional translations plugin type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.ADDITIONAL_UI_TRANSLATIONS)

### TRUSTED_HOSTS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TRUSTED_HOSTS

Extension point to provide trusted hosts.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.TRUSTED_HOSTS)

### CSP

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CSP

Extension point to provide additional CSP.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.CSP)

### DOCUMENT_VALIDATOR

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DOCUMENT_VALIDATOR

Extension point for external document validator
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.DOCUMENT_VALIDATOR)

### AI_FUNCTIONS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AI_FUNCTIONS

Extension point for external AI functions
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.AI_FUNCTIONS)

### AI_CONNECTORS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AI_CONNECTORS

Extension point for external AI connectors that allow connection to an AI service
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.AI_CONNECTORS)

### AI_HOOKS_HANDLER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AI_HOOKS_HANDLER

Extension point for AI hooks handler
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.AI_HOOKS_HANDLER)

### CONFIGURATION_OPTIONS_PROVIDER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CONFIGURATION_OPTIONS_PROVIDER

Configuration options provider
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.plugin.PluginDescriptor.CONFIGURATION_OPTIONS_PROVIDER)

## Constructor Details

### PluginDescriptor

public PluginDescriptor()

## Method Details

### getExtensions

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[PluginDescriptor.PluginExtensionDescription](PluginDescriptor.PluginExtensionDescription.md)> getExtensions([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

Get the extension corresponding to the specified key.
Available extensions for the moment are: SELECTION_PROCESSOR & GENERAL_EXTENSION.

  Parameters: key - The extension key. Returns: The extension corresponding to the specified key.
### getExtensions

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[PluginDescriptor.PluginExtensionDescription](PluginDescriptor.PluginExtensionDescription.md)> getExtensions()

Get all the extensions of a plugin.
  Returns: an immutable list of all the extensions of a plugin.
### addExtension

public void addExtension([PluginDescriptor.PluginExtensionDescription](PluginDescriptor.PluginExtensionDescription.md) descr)

Put an extension corresponding to the specified key. Available extensions for the moment are: SELECTION_PROCESSOR & GENERAL_EXTENSION.
  Parameters: descr - The plugin extension description.
### addContextInstance

public void addContextInstance([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) contextInstance)

Add a context instance.
  Parameters: contextInstance - a context instance.
### getContextInstances

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> getContextInstances()

Getter for all context instances.
  Returns: the context instances.
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()

Get the description of the plugin.
  Returns: The description of the plugin.
### setDescription

public void setDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description)

Set the description of the plugin.
  Parameters: description - The description of the plugin.
### getName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

Gets the name of the plugin.
  Returns: The name of the plugin.
### setName

public void setName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Set the name of the plugin.
  Parameters: name - The name of the plugin.
### setID

public void setID([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) id)

Sets the ID of the plugin. Empty string is treated as no ID.
  Parameters: id - ID of the plugin.
### getID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getID()
  Returns: Returns the id of the plugin or null if the plugin doesn't have an ID.
### getVendor

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getVendor()

Get the vendor of the plugin.
  Returns: The vendor name.
### setVendor

public void setVendor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) vendor)

Set the vendor of the plugin.
  Parameters: vendor - The vendor of the plugin.
### getVersion

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getVersion()

Get the version of the plugin.
  Returns: The plugin version.
### setVersion

public void setVersion([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) version)

Set the version of the plugin.
  Parameters: version - The version of the plugin.
### isEnabledStatus

public boolean isEnabledStatus()

Get the enabled status.
  Returns: Returns true if the plugin is enabled.
### setEnabledStatus

public void setEnabledStatus(boolean enabledStatus)

Set the plugin enabled status.
  Parameters: enabledStatus - true if the plugin is enabled. false if the plugin is disabled.
### isDisabledFromFile

public boolean isDisabledFromFile()
  Returns: Returns true if the plugin is disabled using 'plugin.disable' file.
### setDisabledFromFile

public void setDisabledFromFile(boolean isDisabledFromFile)

Sets the disabled status from 'plugin.disable' file.
  Parameters: isDisabledFromFile - The true if the plugin is disabled using 'plugin.disable' file.
### getBaseDir

public [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) getBaseDir()

Get the base directory of the plugin.
  Returns: The plugin base directory.
### setBaseDir

public void setBaseDir([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) baseDir)

Set the base dir of the plugin.
  Parameters: baseDir - The base dir of the plugin.
### getConfigUrlPath

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getConfigUrlPath()
  Returns: Returns the configUrl.
### setConfigUrlPath

public void setConfigUrlPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) configUrlPath)
  Parameters: configUrlPath - The configUrl to set.
### addPluginContributedView

public void addPluginContributedView(ro.sync.exml.plugin.PluginContributedView viewInfo)

Add a contributed view
  Parameters: viewInfo - Information about the view
### getContributedViews

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.exml.plugin.PluginContributedView> getContributedViews()
  Returns: Returns the contributedViews.
### addPluginContributedToolbar

public void addPluginContributedToolbar(ro.sync.exml.plugin.PluginContributedToolbar toolbarInfo)

Add a toolbar.
  Parameters: toolbarInfo - Information about the new toolbar.
### getContributedToolbars

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.exml.plugin.PluginContributedToolbar> getContributedToolbars()

Gets the toolbars contributed by this plugin.
  Returns: The list of contributed toolbars.
### shouldAcceptLicense

public boolean shouldAcceptLicense()
  Returns: Returns the shouldAcceptLicense.
### setShouldAcceptLicense

public void setShouldAcceptLicense(boolean shouldAcceptLicense)
  Parameters: shouldAcceptLicense - The shouldAcceptLicense to set.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()

The string representation of the plugin descriptor.
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Returns: The string representation.
### getLicense

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLicense()
  Returns: Returns the license.
### setLicense

public void setLicense([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) license)
  Parameters: license - The license to set.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
