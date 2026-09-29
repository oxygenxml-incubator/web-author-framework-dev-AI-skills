# Class: AbstractAction

##   [sync](sync.md)[.actions](sync.actions.md). AbstractAction

#### new AbstractAction( [keystrokeStr])

 The base class for the editor actions. Besides the action behavior, this class also specifies how the buttons that trigger the action should be rendered. This rendering is represented by an action display name, a description (usually presented on a tooltip), and some icons to be rendered depending on the button size.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `keystrokeStr` |   string   |  &lt;optional&gt;   | the string representation of the shortcut of the action. |

### Methods

#### actionPerformed(callback)

 Abstract method that executes the action.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `callback` |   function   | A function to call after the action was performed to notify the editor that the action was finished. It must be called even when the action finished with an error. |

#### dispose()

 Should dispose all the resources required by the action.

#### getDescription()

 Returns the description for the action - usually displayed on a tooltip.

##### Returns:

 The description.
     Type     string
#### getDisplayName()

 Returns the display name for the action.

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

##### Returns:

 The icon URL.
     Type     string
#### getShortcut()

 Returns the shortcut, represented as a string. E.g. - "Ctrl B" - "Alt Shift T" - "Ctrl Alt equals" - "Ctrl period" - "Ctrl comma" - "Ctrl back_quote" - "Ctrl open_bracket" - "Ctrl back_slash" - "Ctrl num_lock" - "Ctrl divide" The shortcut may use platform-independent modifiers M1 to M4.

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

##### Returns:

 The icon URL.
     Type     string
#### isEnabled()

 Tells whether the action is enabled. Note: The action is not permanently polled for its "enabled-ness". If you want the GUI to reflect the current status you will have to call sync.api.ActionsManager#refreshActionsStatus. In the implementation you can use [sync.api.SelectionManager](sync.api.SelectionManager.md) to determine the selection.

##### Returns:

 Whether the action is enabled.
     Type     boolean
#### renderLargeIcon()

 This method renders the large icon of the action in a 24px by 24px div with the action's large icon as its background. This allows the getLargeIcon() method to return different sized icons depending on the device pixel ration, the size constraints being imposed by the enclosing DIV. It should be overridden only for custom rendering strategies, otherwise consider using the getLargeIcon method.

##### Returns:

 the rendering of the large icon image.
     Type     [Element](Element.md)
#### renderSmallIcon()

 This method renders the small icon of the action in a 16px by 16px DIV with the action's small icon as its background. This allows the getSmallIcon() method to return different sized icons depending on the device pixel ration, the size constraints being imposed by the enclosing DIV. It should be overridden only for custom rendering strategies, otherwise consider using the getSmallIcon method.

##### Returns:

 the rendering of the small icon image.
     Type     HTMLElement

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
