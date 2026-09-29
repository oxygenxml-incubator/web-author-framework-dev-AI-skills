# Class: CreateDocumentAction

##   [sync](sync.md)[.api](sync.api.md). CreateDocumentAction

#### new CreateDocumentAction(urlChooser)

 Create action.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `urlChooser` |   [sync.api.UrlChooser](sync.api.UrlChooser.md)   | the urlChooser the create action will use. |
    Deprecated:
* since version 20.1.1. Use [sync.api.FileServersManager#registerFileServerConnector](sync.api.FileServersManager.md#registerFileServerConnector) to register a file server for which inline browsing and create files features are provided.

### Extends

* [sync.actions.AbstractAction](sync.actions.AbstractAction.md)

### Members

#### selectedTemplate_ :sync.model.FrameworkTemplate

##### Type:

*   sync.model.FrameworkTemplate

### Methods

#### dispose()

 Should dispose all the resources required by the action.
    Inherited From:
*   [sync.api.CreateDocumentAction#dispose](sync.api.CreateDocumentAction.md#dispose)
    Overrides:
*   [sync.actions.AbstractAction#dispose](sync.actions.AbstractAction.md#dispose)

#### getActionId()

 Get the action id.

##### Returns:

 the action id or null if none was provided.
     Type     string
#### getDescription()

 Returns the description for the action - usually displayed on a tooltip.
    Inherited From:
*   [sync.api.CreateDocumentAction#getDescription](sync.api.CreateDocumentAction.md#getDescription)
    Overrides:
*   [sync.actions.AbstractAction#getDescription](sync.actions.AbstractAction.md#getDescription)

##### Returns:

 The description.
     Type     string
#### getDisplayName()

 Returns the display name for the action.
    Inherited From:
*   [sync.api.CreateDocumentAction#getDisplayName](sync.api.CreateDocumentAction.md#getDisplayName)
    Overrides:
*   [sync.actions.AbstractAction#getDisplayName](sync.actions.AbstractAction.md#getDisplayName)

##### Returns:

 The display name.
     Type     string
#### &lt;protected&gt; getLargeIcon( [devicePixelRation])

One should override this method to provide the absolute URL of the action's large icon.

If you want to distribute the icon in a framework, you need to place it in the "web/" sub-folder of the framework. In this case the absolute URL of the icon can be obtain by concatenating [sync.ext.Registry.extensionURL](sync.ext.Registry.md#.extensionURL)with the relative path of the icon to the "web/" sub-folder.

If you want to distribute the icon in a plugin, you can place it in a directory with static resources using a[WebappStaticResourcesFolder](https://oxygenxml.com/doc/ug-waCustom/topics/customizing_plugins.html) extension.

The large icon should have a minimum size of 24 by 24 px for non-hidpi displays and can vary depending on the device pixel ration, the icon being used as the background of a 24 by 24 px DIV.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `devicePixelRation` |   number   |  &lt;optional&gt;   | the device pixel ratio. |
    Inherited From:
*   [sync.api.CreateDocumentAction#getLargeIcon](sync.api.CreateDocumentAction.md#getLargeIcon)
    Overrides:
*   [sync.actions.AbstractAction#getLargeIcon](sync.actions.AbstractAction.md#getLargeIcon)

##### Returns:

 The icon URL.
     Type     string
#### getShortcut()

 Returns the shortcut, represented as a string. E.g. - "Ctrl B" - "Alt Shift T" - "Ctrl Alt equals" - "Ctrl period" - "Ctrl comma" - "Ctrl back_quote" - "Ctrl open_bracket" - "Ctrl back_slash" - "Ctrl num_lock" - "Ctrl divide" The shortcut may use platform-independent modifiers M1 to M4.
    Inherited From:
*   [sync.actions.AbstractAction#getShortcut](sync.actions.AbstractAction.md#getShortcut)

##### Returns:

 the string representation of the shortcut. If there is no shortcut, returns an empty string.
     Type     string
#### &lt;protected&gt; getSmallIcon( [devicePixelRation])

One should override this method to provide the absolute URL of the action's small icon.

If you want to distribute the icon in a framework, you need to place it in the "web/" sub-folder of the framework. In this case the absolute URL of the icon can be obtain by concatenating [sync.ext.Registry.extensionURL](sync.ext.Registry.md#.extensionURL)with the relative path of the icon to the "web/" sub-folder.

If you want to distribute the icon in a plugin, you can place it in a directory with static resources using a[WebappStaticResourcesFolder](https://oxygenxml.com/doc/ug-waCustom/topics/customizing_plugins.html) extension.

The small icon should have a minimum size of 16 by 16 px for non-hidpi displays and can vary depending on the device pixel ration, the small icon being used as the background of a 16px by 16px div.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `devicePixelRation` |   number   |  &lt;optional&gt;   | the device pixel ratio. |
    Inherited From:
*   [sync.api.CreateDocumentAction#getSmallIcon](sync.api.CreateDocumentAction.md#getSmallIcon)
    Overrides:
*   [sync.actions.AbstractAction#getSmallIcon](sync.actions.AbstractAction.md#getSmallIcon)

##### Returns:

 The icon URL.
     Type     string
#### isEnabled()

 Tells whether the action is enabled. Note: The action is not permanently polled for its "enabled-ness". If you want the GUI to reflect the current status you will have to call sync.api.ActionsManager#refreshActionsStatus. In the implementation you can use [sync.api.SelectionManager](sync.api.SelectionManager.md) to determine the selection.
    Inherited From:
*   [sync.api.CreateDocumentAction#isEnabled](sync.api.CreateDocumentAction.md#isEnabled)
    Overrides:
*   [sync.actions.AbstractAction#isEnabled](sync.actions.AbstractAction.md#isEnabled)

##### Returns:

 Whether the action is enabled.
     Type     boolean
#### renderLargeIcon()

 Handles the rendering of the action's large icon.
    Overrides:
*   [sync.actions.AbstractAction#renderLargeIcon](sync.actions.AbstractAction.md#renderLargeIcon)

##### Returns:

 the rendered large icon.
     Type     HTMLElement
#### renderSmallIcon()

 This method renders the small icon of the action in a 16px by 16px DIV with the action's small icon as its background. This allows the getSmallIcon() method to return different sized icons depending on the device pixel ration, the size constraints being imposed by the enclosing DIV. It should be overridden only for custom rendering strategies, otherwise consider using the getSmallIcon method.
    Inherited From:
*   [sync.actions.AbstractAction#renderSmallIcon](sync.actions.AbstractAction.md#renderSmallIcon)

##### Returns:

 the rendering of the small icon image.
     Type     HTMLElement
#### setActionId(newActionId)

 Set the action id.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `newActionId` |    | the new action id. |

#### setActionName(newName)

 Sets the action name. The action name is displayed under the action large icon.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `newName` |    | the new name. |

#### setDescription(newDescription)

 Sets the action's description.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `newDescription` |    | the new action description. |

#### setLargeIcon(newLargeIcon)

 Sets the action's large icon.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `newLargeIcon` |    | the new icon source. |

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
