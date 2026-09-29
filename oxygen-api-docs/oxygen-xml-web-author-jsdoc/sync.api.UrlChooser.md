# Class: UrlChooser

##   [sync](sync.md)[.api](sync.api.md). UrlChooser

#### new UrlChooser()

 A base class for URL choosers.

### Classes
    [Context](sync.api.UrlChooser.Context.md)
### Members

#### &lt;static&gt; Purpose :string

 The type of the URL to be chosen.

##### Type:

*   string

##### Properties:

  | Name | Type | Default | Description |
  | -----------| -----------| -----------| -----------|
| `SAVE` |   string   |  save  | The purpose of the chooser is to help the user save the specified resource. |
| `CHOOSE_SAVE_LOCATION` |   string   |  choose_save_location  | The purpose of the chooser is to choose a location where to save the given file. |
| `CHOOSE` |   string   |  choose  | The purpose of the chooser is to choose the location of a resource. |

#### &lt;static&gt; SaveResult :string

 Information about the save operation result.

##### Type:

*   string

##### Properties:

  | Name | Type | Default | Description |
  | -----------| -----------| -----------| -----------|
| `SAVED_AVAILABLE_URL` |   string   |  saved-and-available  | The save operation was successful and the file url is available. |
| `SAVED_UNAVAILABLE_URL` |   string   |  saved-unavailable  | The save operation was successful but the file url is not available, or cannot be determined by the urlChoser. |
| `FAILED` |   string   |  save-failed  | The save operation failed for some reason. |
| `CANCELED` |   string   |  save-canceled  |  |

#### &lt;static&gt; Type :string

 The type of the URL to be chosen.

##### Type:

*   string

##### Properties:

  | Name | Type | Default | Description |
  | -----------| -----------| -----------| -----------|
| `IMAGE` |   string   |  image  | The URL corresponds to an image resource. |
| `EXTERNAL_REF` |   string   |  xref  | The URL corresponds to an XML file that is referred from the currently edited one. |
| `DITA` |   string   |  dita  | The URL corresponds to a DITA topic or map resource. |
| `DITAMAP` |   string   |  ditamap  | The URL corresponds to a DITA map resource. |
| `DITAVAL` |   string   |  ditaval  | The URL corresponds to a DITA filter (ditaval) resource. |
| `DITAPROJECT` |   string   |  ditaproject  | The URL corresponds to a DITA project resource. |
| `GENERIC` |   string   |  generic  | The URL corresponds to another type of resource. |

### Methods

#### &lt;static&gt; getFileBrowserDescriptor()

 Gets the current file browser descriptor containing all filtering configuration.
    Since:
* 28.1

##### Returns:

 The current file browser descriptor containing all URL chooser type filtering configurations.
     Type     [sync.api.FileBrowserDescriptor](sync.api.md#.FileBrowserDescriptor)
#### &lt;static&gt; setFileBrowserDescriptor(descriptor)

 Sets the complete file browser descriptor, replacing all existing filtering configuration.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `descriptor` |   [sync.api.FileBrowserDescriptor](sync.api.md#.FileBrowserDescriptor)   | The file browser descriptor containing all URL chooser type filtering configurations. |
    Since:
* 28.1

#### chooseUrl(context, chosen, purpose)

 Invokes the URL chooser.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `context` |   [sync.api.UrlChooser.Context](sync.api.UrlChooser.Context.md)   | The context in which the chooser is invoked - it contains information like the type of the resource that we want the user to choose: image, external xml file, etc. |
| `chosen` |   [sync.api.UrlChooser~urlChosen](sync.api.UrlChooser.md#~urlChosen)   | The function to be called with the result of the choice. |
| `purpose` |   [sync.api.UrlChooser.Purpose](sync.api.UrlChooser.md#.Purpose)   | The purpose the chooser is invoked with. |

#### saveFile(fileURL, suggestedFileName, callback)

 Saves the file given file. IMPORTANT: Please consider overriding [sync.api.UrlChooser#chooseUrl](sync.api.UrlChooser.md#chooseUrl) instead of this one. The default implementation for this method uses [sync.api.UrlChooser#chooseUrl](sync.api.UrlChooser.md#chooseUrl) to determine the save location. An use-case for this method is to re-use a 'saver' widget which already takes care of the saving itself.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `fileURL` |   string   | the URL of the file to be saved. |
| `suggestedFileName` |   string   | the proposed name for the new file. |
| `callback` |   [sync.api.UrlChooser~fileSaved](sync.api.UrlChooser.md#~fileSaved)   | the callback to be called with the saved file url. |

#### supports(type)

 Checks whether the URL chooser supports choosing a given type of resource [sync.api.UrlChooser.Type](sync.api.UrlChooser.md#.Type). If not supported, the default UI (which is usually a text-field) will be presented to the user.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `type` |   [sync.api.UrlChooser.Type](sync.api.UrlChooser.md#.Type)   | The type of the URL to be chosen. |

##### Returns:

 true if the chooser supports the given type.
     Type     boolean
#### supportsOperation(purpose)

 Needs to be implemented to reflect whether the chooser suports the given operation: save or choose.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `purpose` |   [sync.api.UrlChooser.Purpose](sync.api.UrlChooser.md#.Purpose)   | The operation. |

##### Returns:

 true if the given operation is supported.
     Type     boolean
### Type Definitions

#### fileSaved( [url], resultInfo [, errorMessage])

 A callback invoked when the file is saved.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `url` |   string   |  &lt;optional&gt;   | The URL where the file was saved, or null if the location is not available. |
| `resultInfo` |   [sync.api.UrlChooser.SaveResult](sync.api.UrlChooser.md#.SaveResult)   |    | information about the save operation result. |
| `errorMessage` |   string   |  &lt;optional&gt;   | The error message in case the resultInfo is [sync.api.UrlChooser.SaveResult.FAILED](sync.api.UrlChooser.md#.SaveResult#.FAILED). |

#### urlChosen( [url])

 A callback invoked when the user choice is available.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `url` |   string   |  &lt;optional&gt;   | The URL chosen by the user, or null if the user failed to choose anything. |

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
