Package [ro.sync.exml.workspace.api.options](package-summary.md)

# Interface GlobalOptionsStorage
    All Known Subinterfaces: [EclipsePluginWorkspace](../../../../../../com/oxygenxml/workspace/api/eclipse/EclipsePluginWorkspace.md), [PluginWorkspace](../PluginWorkspace.md), [StandalonePluginWorkspace](../standalone/StandalonePluginWorkspace.md), [WebappPluginWorkspace](../../../../ecss/extensions/api/webapp/access/WebappPluginWorkspace.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface GlobalOptionsStorage
This interface should be used to access global application options.
  Since: 18
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addGlobalOptionListener](#addGlobalOptionListener(ro.sync.ecss.extensions.api.OptionListener))([OptionListener](../../../../ecss/extensions/api/OptionListener.md) listener)
Adds an [OptionListener](../../../../ecss/extensions/api/OptionListener.md) to the current set of options.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [deserializePersistentObject](#deserializePersistentObject(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) persistentObjectStringRepresentation)
De-serialize a persistent object which has previously been serialized as XML using the "serializePersistentObject" method.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getGlobalObjectProperty](#getGlobalObjectProperty(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
Provides the value of the option associated with the specified key.
  void [importGlobalOptions](#importGlobalOptions(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) optionsFile)
Sets global properties in the Oxygen common preferences.
  void [importGlobalOptions](#importGlobalOptions(java.io.File,boolean))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) optionsFile, boolean preserveExistingOptionKeys)
Sets global properties in the Oxygen common preferences.
  void [removeGlobalOptionListener](#removeGlobalOptionListener(ro.sync.ecss.extensions.api.OptionListener))([OptionListener](../../../../ecss/extensions/api/OptionListener.md) listener)
Removes an option listener from the current set of option listeners.
  void [saveGlobalOptions](#saveGlobalOptions())()
Save the global application options to their default persistence location.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [serializePersistentObject](#serializePersistentObject(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) persistentObject)
Serialize a persistent object to an XML string.
  void [setGlobalObjectProperty](#setGlobalObjectProperty(java.lang.String,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)
Sets a global property in the Oxygen common preferences.
  void [showPreferencesPages](#showPreferencesPages(java.lang.String%5B%5D,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] pagesToShowKeys, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pageToSelectKey, boolean showChildrenOfPages)
Show the preferences dialog, with only the desired pages displayed in the table of contents, and select a specific options page. The pages to be shown or selected in the dialog are provided using their keys.

## Method Details

### addGlobalOptionListener

void addGlobalOptionListener([OptionListener](../../../../ecss/extensions/api/OptionListener.md) listener)

Adds an [OptionListener](../../../../ecss/extensions/api/OptionListener.md) to the current set of options. The listener is notified when the value of its associated option changes.
  Parameters: listener - The [OptionListener](../../../../ecss/extensions/api/OptionListener.md) to be added.
### removeGlobalOptionListener

void removeGlobalOptionListener([OptionListener](../../../../ecss/extensions/api/OptionListener.md) listener)

Removes an option listener from the current set of option listeners.
  Parameters: listener - The [OptionListener](../../../../ecss/extensions/api/OptionListener.md) to be removed.
### getGlobalObjectProperty

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getGlobalObjectProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

Provides the value of the option associated with the specified key. You can only get values for keys defined in the [APIAccessibleOptionTags](../../../options/APIAccessibleOptionTags.md) interface.
  Parameters: key - The key that uniquely identifies an option. Returns: The value corresponding to the key or null. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - If the given key is not accessible via the API.
### setGlobalObjectProperty

void setGlobalObjectProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)

Sets a global property in the Oxygen common preferences. You can use such methods to overwrite some global preferences in Oxygen with your own values. To find the key and value types which needs to be overwritten you can export the application preferences to XML (Options -> Export Global Options).
  Parameters: key - The key of the option whose value is to be modified. value - The new value of the option. Since: 15
### importGlobalOptions

void importGlobalOptions([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) optionsFile)

Sets global properties in the Oxygen common preferences. You can use such methods to overwrite some global preferences in Oxygen with your own values. Existing options with keys which are not present in the imported options file will be preserved.
  Parameters: optionsFile - The file containing the XML options exported from an Oxygen installation. Since: 16
### importGlobalOptions

void importGlobalOptions([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) optionsFile, boolean preserveExistingOptionKeys)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Sets global properties in the Oxygen common preferences. You can use such methods to overwrite some global preferences in Oxygen with your own values.
  Parameters: optionsFile - The file containing the XML options exported from an Oxygen installation. preserveExistingOptionKeys - If true existing options with keys which are not present in the imported options file will be preserved. Otherwise the existing options with keys which are not present in the imported options file are reset to default. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If some type of problem arises during the import or if the file cannot be accessed. Since: 18.1
### saveGlobalOptions

void saveGlobalOptions() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Save the global application options to their default persistence location.
  Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the save operation fails. Since: 15.2
### showPreferencesPages

void showPreferencesPages([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] pagesToShowKeys, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pageToSelectKey, boolean showChildrenOfPages)

Show the preferences dialog, with only the desired pages displayed in the table of contents, and select a specific options page. The pages to be shown or selected in the dialog are provided using their keys. For the stand-alone application each key corresponds to a OptionPagePluginExtension key (returned via the *ro.sync.exml.plugin.option.OptionPagePluginExtension.getKey()* method). For Eclipse the keys are actually the IDs of the corresponding <page> elements from plugin.xml.
  Parameters: pagesToShowKeys - The keys of the option pages to be shown in the table of contents. pageToSelectKey - The key of the page to be selected in the table of contents. showChildrenOfPages - True to also show the children of the option pages in the table of contents, false not to show them. Since: 17.1
### serializePersistentObject

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) serializePersistentObject([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) persistentObject)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Serialize a persistent object to an XML string.
  Parameters: persistentObject - The persistent object. It must be an instance of ro.sync.options.PersistentObject Returns: A string representation of the object in XML format. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - Thrown if something goes wrong during the serialization. Since: 21
### deserializePersistentObject

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) deserializePersistentObject([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) persistentObjectStringRepresentation)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

De-serialize a persistent object which has previously been serialized as XML using the "serializePersistentObject" method.
  Parameters: persistentObjectStringRepresentation - The XML representation of the object. Returns: The persistent object or null. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - Thrown if something goes wrong during the de-serialization. Since: 21
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
