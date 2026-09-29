Package [ro.sync.exml.workspace.api.options](package-summary.md)

# Interface WSOptionsStorage
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WSOptionsStorage
Support for the user to save and retrieve custom options in the Oxygen common preferences.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 void [addOptionListener](#addOptionListener(ro.sync.exml.workspace.api.options.WSOptionListener))([WSOptionListener](WSOptionListener.md) listener)
Adds an [OptionListener](../../../../ecss/extensions/api/OptionListener.md) to the current set of options.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOption](#getOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)
Provides the value of the option associated with the specified key.
  [ExternalPersistentObject](ExternalPersistentObject.md) [getPersistentObjectOption](#getPersistentObjectOption(java.lang.String,ro.sync.exml.workspace.api.options.ExternalPersistentObject))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [ExternalPersistentObject](ExternalPersistentObject.md) defaultValue)
Get a persistent object.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSecretOption](#getSecretOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)
Provides the value of the option associated with the specified key.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getStringArrayOption](#getStringArrayOption(java.lang.String,java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] defaultValues)
Provides the values set for the option identified by the given key.
  void [removeOptionListener](#removeOptionListener(ro.sync.exml.workspace.api.options.WSOptionListener))([WSOptionListener](WSOptionListener.md) listener)
Removes an option listener from the current set of option listeners.
  void [setOption](#setOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Modifies the value of an option.
  void [setOptionsDoctypePrefix](#setOptionsDoctypePrefix(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionsDoctypePrefix)  Deprecated.
WARNING: THE USE OF THIS METHOD IS DISCOURAGED AND DEPRECATED
   void [setPersistentObjectOption](#setPersistentObjectOption(java.lang.String,ro.sync.exml.workspace.api.options.ExternalPersistentObject))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [ExternalPersistentObject](ExternalPersistentObject.md) persistentObject)
Set a persistent object.
  void [setSecretOption](#setSecretOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Modifies the value of an option.
  void [setStringArrayOption](#setStringArrayOption(java.lang.String,java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] values)
Modifies the values set for the option identified by the given key.

## Method Details

### setOptionsDoctypePrefix

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void setOptionsDoctypePrefix([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionsDoctypePrefix)
 Deprecated.
WARNING: THE USE OF THIS METHOD IS DISCOURAGED AND DEPRECATED

All plugins initially share a common settings namespace. So that would mean that a plugin could read values set by other plugins or it could register to receive value changed events for certain option keys set by other plugins (which may sometimes be useful). But this also means that accidentally a plugin could also overwrite the value for a certain key if more than one plugin use the same key. So ideally your plugin's persisted keys would all be manually prefixed with some unique ID when they are defined. This would be the recommended way of doing things. If you still want to use the method:

Using this method when working with the singleton access to the workspace "PluginWorkspaceProvider.getPluginWorkspace().getOptionsStorage()" will set it for all plugins. So a plugin will globally influence the global prefixes for keys loaded and saved also by other plugins. Which is never a good thing.

But using this method on the WorkspaceAccessPluginExtension.applicationStarted will only set the prefix for your plugin. So as long as your plugin will keep using the "WSOptionsStorage" received on the applicationStarted callback you will not influence other plugins.

Sets the options doctype prefix which is used to prefix options like a namespace.
  Parameters: optionsDoctypePrefix - The document type prefix used to build the options keys. This should not be null.
### addOptionListener

void addOptionListener([WSOptionListener](WSOptionListener.md) listener)

Adds an [OptionListener](../../../../ecss/extensions/api/OptionListener.md) to the current set of options. The listener is notified when the value of its associated option changes.
  Parameters: listener - The [OptionListener](../../../../ecss/extensions/api/OptionListener.md) to be added.
### removeOptionListener

void removeOptionListener([WSOptionListener](WSOptionListener.md) listener)

Removes an option listener from the current set of option listeners.
  Parameters: listener - The [OptionListener](../../../../ecss/extensions/api/OptionListener.md) to be removed.
### getOption

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)

Provides the value of the option associated with the specified key.
  Parameters: key - The key that uniquely identifies an option. defaultValue - The default value for the specified option. Returns: The value of the specified option or the default value if the option has not been set yet.
### setOption

void setOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Modifies the value of an option. If the supplied value is nullThe option will be removed from storage.
  Parameters: key - The key of the option whose value is to be modified. value - The new value of the option. If nullthe option will be removed from the storage.
### getSecretOption

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSecretOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)

Provides the value of the option associated with the specified key.
  Parameters: key - The key that uniquely identifies an option. defaultValue - The default value for the specified option. Returns: The value of the specified option or the default value if the option has not been set yet. Since: 27.1
### setSecretOption

void setSecretOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Modifies the value of an option. If the supplied value is nullThe option will be removed from storage.
  Parameters: key - The key of the option whose value is to be modified. value - The new value of the option. If nullthe option will be removed from the storage. Since: 27.1
### setPersistentObjectOption

void setPersistentObjectOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [ExternalPersistentObject](ExternalPersistentObject.md) persistentObject)

Set a persistent object.
  Parameters: key - The key. persistentObject - The persistent object. Since: 22
### getPersistentObjectOption

[ExternalPersistentObject](ExternalPersistentObject.md) getPersistentObjectOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [ExternalPersistentObject](ExternalPersistentObject.md) defaultValue)

Get a persistent object.
  Parameters: key - The key. defaultValue - Default value Returns: The external persistent object or the default provided value. Since: 22
### getStringArrayOption

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getStringArrayOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] defaultValues)

Provides the values set for the option identified by the given key.
  Parameters: key - The key that uniquely identifies the option. defaultValues - The default values for the specified option. Returns: the values set for the option identified by the given key or the default values if other values have not been set yet.
### setStringArrayOption

void setStringArrayOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] values)

Modifies the values set for the option identified by the given key. If the provided value is null, the option will be removed from storage.
  Parameters: key - The key that uniquely identifies the option. values - The new values to set. If null, the option will be removed from the storage.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
