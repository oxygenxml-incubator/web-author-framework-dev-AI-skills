# Class: ViewManager

##   [sync](sync.md)[.view](sync.view.md). ViewManager

#### new ViewManager()

Helper object used to control the lateral views.

The view manager can be obtained by using [workspace.getViewManager()](sync.api.Workspace.md#getViewManager).

Each view is identified by an ID and is registered on one of the two sides of the editor: left or right.

A view is not visible before a [sync.view.ViewRenderer](sync.view.ViewRenderer.md) is installed for it. Each view is enabled by default, and it can be disabled if it does not support the current editor. When the view is disabled, it will not be presented to the user, but it will still be present in the page's DOM.

Once visible, the view may be focused or not. There is only one focused view on each side of the editor.

### Methods

#### addView(viewId)

 Adds a new view with the given ID. The view is not rendered until a [sync.view.ViewRenderer](sync.view.ViewRenderer.md) is installed for it. Should be called before any view is installed.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `viewId` |   string   | The id of the view to be added. |

#### disableView(viewId)

Disables a view, which means the view is hidden from the user and can be enabled later.

To enable or disable a view based on the current editor, one should use the[sync.view.ViewRenderer#supportsEditor](sync.view.ViewRenderer.md#supportsEditor) method. This method should only be used for more complex cases.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `viewId` |   string   | The id of the view to be disable. |
    Since:
* 21.1.1

#### enableView(viewId)

Enables a view, which means the view is displayed and can be interacted with by the user.

To enable or disable a view based on the current editor, one should use the[sync.view.ViewRenderer#supportsEditor](sync.view.ViewRenderer.md#supportsEditor) method. This method should only be used for more complex cases.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `viewId` |   string   | The id of the view to be enabled. |
    Since:
* 21.1.1

#### focusView(viewId)

 Focuses the view with the given ID. Has no effect if the view is disabled.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `viewId` |   string   | The ID of the view to focus. |

#### getActionsManager(viewId)

 Get the actions manager used for a specified view.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `viewId` |   String   | The id of the view. |
    Since:
* 26.1

##### Returns:

 The action manager
     Type     [sync.api.ActionsManagerCore](sync.api.ActionsManagerCore.md)
#### getViewIds()

##### Returns:

 The list of IDs of all views defined in the layout.
     Type     Array.&lt;string&gt;
#### hideAppBar()

 Hides the application header bar that contains: - the application logo - some basic actions - when the header is hidden they migrate to the main toolbar. - the file name - the user name

#### installView(viewId, view, opt_viewProperties)

 Install the view renderer for the view with the given ID. It takes care of rendering the view content.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `viewId` |   String   | The ID of the view to focus. |
| `view` |   [sync.view.ViewRenderer](sync.view.ViewRenderer.md)   | The view handler. |
| `opt_viewProperties` |   [sync.view.ViewProperties](sync.view.md#.ViewProperties)  /  String   | The view properties. If this parameter value is a String, then it refers to the "side" property. |

#### isViewEnabled(viewId)

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `viewId` |   string   | The id of the view whose status we are interested in. |
    Since:
* 21.1.1

##### Returns:

 true if the view is enabled.
     Type     boolean
#### isViewOpen(viewId)

 Checks whether the view with the given ID is open.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `viewId` |   string   | The ID of the view. |
    Since:
* 22.1

##### Returns:

 true if the view with the given ID is open to the user.
     Type     boolean
#### removeView(viewId)

 Removes the given view from the layout. Should be called before any view is installed.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `viewId` |   string   | The id of the view to be removed. |

#### setSize(width, height)

 Sets the size of the entire Web Author view. Once this method is called automatic resizing based on window dimensions will be disabled.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `width` |   number   | The new width of the Web Author view element. |
| `height` |   number   | The new height of the Web Author view element. |

#### uninstallView(viewId)

 Uninstall the renderer associated with a given view.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `viewId` |   string   | The view whose renderer to uninstall. |
    Since:
* 21.1.1

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
