# Interface: FileServer

##   [sync](sync.md)[.api](sync.api.md). FileServer

Provides browsing functionality and server address rendering for a file server.

### Type Definitions

#### listFilesSuccessCallback(folderEntries)

 Callback that receives the folder entries.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `folderEntries` |   Array.&lt;[sync.api.FileServer.EntryDescriptor](sync.api.FileServer.EntryDescriptor.md)&gt;   | The list of the folder entries descriptors entries. |

#### createRootUrlComponent(rootUrl, rootURLChangedCallback, readOnly)

 This method can be used to create the element that renders the root URL address (it may contain for example some branches information or it may render some server specific images) on the top part of the server browser component.It can also be used to render the editing components for the root URL.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `rootUrl` |   string   | The server root URL to render details for. |
| `rootURLChangedCallback` |   [sync.api.FileServer~serverURLsInfoCallback](sync.api.FileServer.md#~serverURLsInfoCallback)   | The function to call when the root URL is changed. |
| `readOnly` |   boolean   | True if the root URL should not be editable by using this component. |

##### Returns:

 The HTML element that represents UI component.
     Type     HTMLElement
#### getDefaultRootUrl()

 Impose a default server to be browsed in the file server specific Dashboard tab.

##### Returns:

 The default root URL.
     Type     string
#### getUrlInfo(url, urlInfoCallback, showErrorMessageCallback)

 Request the URL info from the file server.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `url` |   string   | The URL about which we ask for information. |
| `urlInfoCallback` |   [sync.api.FileServer~serverURLsInfoCallback](sync.api.FileServer.md#~serverURLsInfoCallback)   | The function to call when the URL info is available. |
| `showErrorMessageCallback` |   [sync.api.FileServer~showErrorMessageCallback](sync.api.FileServer.md#~showErrorMessageCallback)   | The function to call when an error message must be presented to the user. |

#### getUserName()

 Get current user name.

##### Returns:

 The current user name.
     Type     string
#### listFiles(folderUrl, successCallback, failureCallback)

 Get the contents of the given folder. By default the server-side *ro.sync.net.protocol.FileBrowsingConnection.listFiles()* method is called to retrieve files so this method should be used only if a custom implementation is needed.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `folderUrl` |   string   | The URL of the folder to list. |
| `successCallback` |   [sync.api.FileServer.listFilesSuccessCallback](sync.api.FileServer.md#.listFilesSuccessCallback)   | The function to call when the folder listing is available. |
| `failureCallback` |   function   | The function to call when there was a failure retrieving folder content, passing in the exception. |

#### login(message, loginSuccessCallback, url)

 Login to the server. This method should implement both the UI used by the user to provide the login credentials and the login functionality.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `message` |   String   | The message received from the server, from the ro.sync.ecss.extensions.api.webapp.plugin.UserActionRequiredException that triggers the login action. |
| `loginSuccessCallback` |   function   | The function to call after the log in process is finished successful. |
| `url` |   String   | The url of the resource that requires the login action. |

#### logout(logoutCallback)

 Disconnect from server. This method should only implement the file server disconnect functionality, since it is called when a disconnect action is called (and after the user confirmation).

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `logoutCallback` |   function   | The function to call when the file server logout process is completed. |

#### serverURLsInfoCallback(rootUrl, browseUrl)

 Callback that receives the server URLs information.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `rootUrl` |   string   | The server root URL |
| `browseUrl` |   string   | The URL of the current folder whose content will be presented in the file browser. |

#### setUserChangedCallback(The)

 Set the callback to be called when the user name is changed.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `The` |   function   | callback function to be called when the user is changed (the name is send as parameter). |

#### showErrorMessageCallback(The)

 Callback that receives an error message that must be presented to the user

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `The` |   string   | error message to be presented to the user. |

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
