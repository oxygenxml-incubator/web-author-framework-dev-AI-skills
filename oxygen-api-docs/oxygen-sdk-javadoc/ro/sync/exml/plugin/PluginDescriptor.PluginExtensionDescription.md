Package [ro.sync.exml.plugin](package-summary.md)

# Class PluginDescriptor.PluginExtensionDescription

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.plugin.PluginDescriptor.PluginExtensionDescription
   Enclosing class: [PluginDescriptor](PluginDescriptor.md)   public static class PluginDescriptor.PluginExtensionDescription extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Contains a plugin description + plugin type + keyboard shortcuts

## Field Summary
 Fields
Modifier and Type

Field

Description
 final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [aditionaFrameworkDir](#aditionaFrameworkDir)
The directory of the framework contributed by the plugin.
  final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [cssFile](#cssFile)
The CSS file specified by an extension.
  final [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)> [folders](#folders)
The folder paths provided by the plugin descriptor.
  final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [name](#name)
Name of plugin action
  final [PluginExtension](PluginExtension.md) [pluginExtension](#pluginExtension)
The plugin extension
  final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [pluginType](#pluginType)
The plugin type
  final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [resourcesContentSecurityPolicy](#resourcesContentSecurityPolicy)
The csp policy to use for the resources.
  final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [resourcesFolderPath](#resourcesFolderPath)
The path of the static resources folder relative to the plugin base dir.
  final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [resourcesHref](#resourcesHref)
The href at which the resources from the static folder will be accessed.
  final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [role](#role)
The role of this extension.
  final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [shortcut](#shortcut)
The plugin shortcut

## Constructor Summary
 Constructors
Constructor

Description
 [PluginExtensionDescription](#%3Cinit%3E(java.lang.String,ro.sync.exml.plugin.PluginExtension,java.lang.String,java.lang.String,java.lang.String,java.util.List,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pluginType, [PluginExtension](PluginExtension.md) pluginExtension, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) actionName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) shortcut, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cssFile, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)> folders, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourcesHref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourcesFolderPath, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourcesContentSecurityPolicy, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) role, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalFrameworkDir)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [PluginExtension](PluginExtension.md) [getPluginExtension](#getPluginExtension())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getResourcesHref](#getResourcesHref())()
Getter for the resource href.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### pluginExtension

public final [PluginExtension](PluginExtension.md) pluginExtension

The plugin extension

### pluginType

public final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pluginType

The plugin type

### name

public final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name

Name of plugin action

### shortcut

public final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) shortcut

The plugin shortcut

### folders

public final [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)> folders

The folder paths provided by the plugin descriptor.

### cssFile

public final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cssFile

The CSS file specified by an extension.

### resourcesHref

public final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourcesHref

The href at which the resources from the static folder will be accessed.

### resourcesFolderPath

public final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourcesFolderPath

The path of the static resources folder relative to the plugin base dir.

### resourcesContentSecurityPolicy

public final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourcesContentSecurityPolicy

The csp policy to use for the resources.

### role

public final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) role

The role of this extension. If the role is "config" this extension should have a class attribute with the class representing the class of a PluginConfigExtension which manages the configuration of a WebApp plugin.

### aditionaFrameworkDir

public final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) aditionaFrameworkDir

The directory of the framework contributed by the plugin.

## Constructor Details

### PluginExtensionDescription

public PluginExtensionDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pluginType, [PluginExtension](PluginExtension.md) pluginExtension, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) actionName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) shortcut, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) cssFile, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)> folders, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourcesHref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourcesFolderPath, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourcesContentSecurityPolicy, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) role, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) additionalFrameworkDir)

Constructor.
  Parameters: pluginType - The plugin type pluginExtension - The plugin extension actionName - Name of plugin action if any. shortcut - The plugin shortcut cssFile - The CSS file specified by an AuthorCSS extension. folders - The folder paths provided by the plugin descriptor. resourcesHref - The Href at which to request the plugin's static resources. resourcesFolderPath - The path to the static resources folder relative to the plugin base directory. resourcesContentSecurityPolicy - The csp policy to use for the resource. role - The role of this extension additionalFrameworkDir - Additional framework directory referenced by the plugin.
## Method Details

### getResourcesHref

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getResourcesHref()

Getter for the resource href.
  Returns: the resource href.
### getPluginExtension

public [PluginExtension](PluginExtension.md) getPluginExtension()
  Returns: The plugin extension instance.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
