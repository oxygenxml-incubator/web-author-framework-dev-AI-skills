# Namespace: api

##   [sync](sync.md). api

### Classes
    [ActionsManager](sync.api.ActionsManager.md)    [ActionsManagerCore](sync.api.ActionsManagerCore.md)    [AuthorWidgetsFactory](sync.api.AuthorWidgetsFactory.md)    [ChangeTrackingManager](sync.api.ChangeTrackingManager.md)    [ConcurrentEditingManager](sync.api.ConcurrentEditingManager.md)    [CreateDocumentAction](sync.api.CreateDocumentAction.md)    [Dialog](sync.api.Dialog.md)    [EditImageMapAction](sync.api.EditImageMapAction.md)    [EditingContextManager](sync.api.EditingContextManager.md)    [EditingSupport](sync.api.EditingSupport.md)    [EditingSupportManager](sync.api.EditingSupportManager.md)    [Editor](sync.api.Editor.md)    [FileBrowsingDialog](sync.api.FileBrowsingDialog.md)    [FileServersManager](sync.api.FileServersManager.md)    [HighlightUpdateEvent](sync.api.HighlightUpdateEvent.md)    [NotificationsManager](sync.api.NotificationsManager.md)    [PersistentHighlightsManager](sync.api.PersistentHighlightsManager.md)    [PersistentHighlightUpdateEvent](sync.api.PersistentHighlightUpdateEvent.md)    [PositionInformation](sync.api.PositionInformation.md)    [Selection](sync.api.Selection.md)    [SelectionCore](sync.api.SelectionCore.md)    [SelectionManager](sync.api.SelectionManager.md)    [SelectionManagerCore](sync.api.SelectionManagerCore.md)    [SpellChecker](sync.api.SpellChecker.md)    [UrlChooser](sync.api.UrlChooser.md)    [WebappMessage](sync.api.WebappMessage.md)    [Workspace](sync.api.Workspace.md)    [WorkspaceActionsManager](sync.api.WorkspaceActionsManager.md)    [WrapperAuthorEditingSupport](sync.api.WrapperAuthorEditingSupport.md)    [WrapperEditingSupport](sync.api.WrapperEditingSupport.md)
### Namespaces
    [change_tracking](sync.api.change_tracking.md)    [dom](sync.api.dom.md)    [math](sync.api.math.md)    [Translation](sync.api.Translation.md)
### Members

#### &lt;static&gt; SelectionModel
        Deprecated:
* Use [sync.api.SelectionManager](sync.api.SelectionManager.md) instead.

#### &lt;static&gt; SelectionModel
        Deprecated:
* Use [sync.api.SelectionManager](sync.api.SelectionManager.md) instead.

### Methods

#### &lt;static&gt; EditingSupportProvider()

 Provides the possibility to impose a specific [sync.api.EditingSupport](sync.api.EditingSupport.md) to be used instead of the built-in one to render the content of the current editor, to set the actions, toolbars and views associated with it.

### Type Definitions

#### ElementNameEnhancer(elementName, elementAttrs)

 A function callback used to enhance the name of elements, as shown in the UI (breadcrumbs and tags), depending on their attributes.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `elementName` |   string   | The name of the XML element. |
| `elementAttrs` |   Object   | The attributes stored in an object with the attribute names as keys and with a descriptor object as value. The descriptor contains: * the value of the object (attributeValue). * whether it's value comes from DTD or not (isDefaultValue). * whether the attribute is hidden (isHidden).  |

##### Returns:

 A new name for the given XML element.
     Type     string
#### FileBrowserDescriptor

 File browser descriptor that provides complete filtering configuration for all URL chooser types.

##### Type:

*   Object

##### Properties:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `types` |   Object.&lt;string, [sync.api.FileBrowserDescriptor.TypeConfiguration](sync.api.md#.FileBrowserDescriptor#.TypeConfiguration)&gt;   | A map of URL chooser type names to their filtering configurations. The keys are type names (e.g., "IMAGE", "DITA", "DOCUMENT") and the values are type configurations. |

#### FileServerDescriptor

 File server descriptor that provides rendering information and browsing functionality for a specific file server.

##### Type:

*   Object

##### Properties:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `id` |   string   | The id of the server. It will be used as a namespace to save the following server-specific information in the local storage: * server_id.latestRootUrl - The latest root URL used in the file servers Dashboard tab * server_id.latestUrl - The latest URL for which the content files are listed in the file servers Dashboard tab  |
| `name` |   string   | The name of the file server (it will be displayed in the Dashboard, on the file server tab). |
| `icon` |   string   | The URL of the file server icon (it will be displayed in the Dashboard, on the file server tab). |
| `matches` |   function   | Returns true if the URL given as parameter points to a file or folder from this file server. |
| `fileServer` |   [sync.api.FileServer](sync.api.FileServer.md)   | It provides login, logout and file browsing functionality for a specific server. |

#### ReadOnlyState

 The descriptor for the read-only or editable state of the editor.

##### Type:

*   Object

##### Properties:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `readOnly` |   boolean   | A flag that indicated whether the document is read-only. |
| `message` |   string   | The message to display to the user if the editor is read-only. |
| `code` |   string   | A code for the reason which will be the same across UI languages. |

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
