# Class: ActionsLoadedEvent

##   [sync](sync.md)[.api](sync.api.md)[.Editor](sync.api.Editor.md). ActionsLoadedEvent

#### new ActionsLoadedEvent(actionsConfiguration)

Configuration of the actions that are going to be enabled for the current editor was loaded. This configuration may specify some of the:

* the action together with their shortcuts
* the configuration of one of the toolbars
* the configuration of the context menu
* configuration for the content completion menu

This event is triggered before the action are used, so changes to the configuration will take effect in the UI.

The toolbar and contextmenu configurations contain only action ids. In order to change the actual actions or to add more actions one can use the [sync.api.ActionsManager](sync.api.ActionsManager.md).

Example of listening for this event:

```
editor.listen(sync.api.Editor.EventTypes.ACTIONS_LOADED, function(e) {  // e is of type sync.api.Editor.ActionsLoadedEvent});
```

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `actionsConfiguration` |   [sync.api.Editor.ActionsLoadedEvent.ActionsConfiguration](sync.api.Editor.ActionsLoadedEvent.md#.ActionsConfiguration)   | A object that represents the actions configuration. |

### Members

#### actionsConfiguration :[sync.api.Editor.ActionsLoadedEvent.ActionsConfiguration](sync.api.Editor.ActionsLoadedEvent.md#.ActionsConfiguration)

##### Type:

*   [sync.api.Editor.ActionsLoadedEvent.ActionsConfiguration](sync.api.Editor.ActionsLoadedEvent.md#.ActionsConfiguration)

#### type :string

##### Type:

*   string

### Type Definitions

#### ActionDescriptor

 The action descriptor.

##### Type:

*   Object

##### Properties:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `compatible` |   boolean   |    | Whether the action is compatible with webapp. If not, it will not be used in the UI. |
| `icon16` |   string   |  &lt;optional&gt;   | The URL for a 16x16 icon to be used for the action. |
| `icon20` |   string   |  &lt;optional&gt;   | The URL for a 24x24 icon to be used for the action. Yes, 24x24, it's called icon20 for backwards compatibility reasons. |
| `id` |   string   |    | The unique ID of the action. |
| `name` |   string   |  &lt;optional&gt;   | The display name of the action. |
| `tooltip` |   string   |  &lt;optional&gt;   | The tooltip description of the action. |
| `shortcut` |   string   |  &lt;optional&gt;   | The shortcut of the action. Can use platform-generic modifiers: * M1 - Ctrl or Cmd on Mac * M2 - Shift * M3 - Alt * M4 - Ctrl on Mac, or nothing on other platforms  |

#### ActionEntry

 The descriptor for an action entry on the toolbar or in the context menu.

##### Type:

*   Object

##### Properties:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `id` |   string   | The ID of the action to render on the toolbar. |
| `type` |   string   | Equal to "action". |

#### ActionsConfiguration

 The object used to open the editor.

##### Type:

*   Object

##### Properties:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `actions` |   Array.&lt;[sync.api.Editor.ActionsLoadedEvent.ActionDescriptor](sync.api.Editor.ActionsLoadedEvent.md#.ActionDescriptor)&gt;   |    | An array of actions descriptors. |
| `toolbars` |   Array.&lt;[sync.api.Editor.ActionsLoadedEvent.ActionsListDescriptor](sync.api.Editor.ActionsLoadedEvent.md#.ActionsListDescriptor)&gt;   |    | An array of descriptors for actions lists that will be rendered as toolbars. |
| `contextualItems` |   Array.&lt;[sync.api.Editor.ActionsLoadedEvent.ContextMenuEntry](sync.api.Editor.ActionsLoadedEvent.md#.ContextMenuEntry)&gt;   |    | An array of descriptors for entries in the context menu. |
| `filterCCItems` |   Array.&lt;string&gt;   |  &lt;nullable&gt;   | A list of names to filter from the Content Completion menu. This property is not always defined when the [sync.api.Editor.ActionsLoadedEvent](sync.api.Editor.ActionsLoadedEvent.md) event is dispatched. Changes to this list are reflected in the UI only when this field is defined, not when you define it yourself. There are several types of entries * Raw names of elements, for example `p` instead of the display name which is **Paragraph**. * Entries that contain the `&lt;SPLIT&gt;` token to filter entries like "Split Paragraph" in all the supported languages. * An entry equal `&lt;ENTER&gt;` to remove the "Enter" entry that appears for code-blocks.  |

#### ActionsListDescriptor

 The descriptor for a toolbar, a drop-down menu on the toolbar, or context sub-menu.

##### Type:

*   Object

##### Properties:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `icon16` |   string   |  &lt;optional&gt;   | The URL for a 16x16 icon to be used to render the actions list. |
| `icon20` |   string   |  &lt;optional&gt;   | The URL for a 24x24 icon to be used to render the actions list. Yes, 24x24, it's called icon20 for backwards compatibility reasons. If the image is placed inside framework the absolute URL of the icon can be obtain by concatenating [sync.ext.Registry.extensionURL](sync.ext.Registry.md#.extensionURL). |
| `iconDom` |   HTMLElement   |  &lt;optional&gt;   | A DOM element that will be used to render the actions list. |
| `name` |   string   |  &lt;optional&gt;   | The name of the toolbar, used as an HTML attribute. It is used also a fallback for displayName. |
| `displayName` |   string   |  &lt;optional&gt;   | The display name of the toolbar. |
| `type` |   string   |    | Equal to "list". |
| `small` |   boolean   |    | true to render a small toolbar (with no padding). |
| `toBottom` |   boolean   |    | true if the toolbar is placed at the bottom of the editor (in this case the drop-down arrow points to top). |
| `children` |   Array.&lt;[sync.api.Editor.ActionsLoadedEvent.ListEntry](sync.api.Editor.ActionsLoadedEvent.md#.ListEntry)&gt;   |    | the list entries. |

#### ContextMenuEntry

 The context menu entry descriptor.

##### Type:

*   Object

##### Properties:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `icon` |   string   |  &lt;optional&gt;   | The URL for a 16x16 icon to be used for the toolbar. |
| `name` |   string   |  &lt;optional&gt;   | The display name of the toolbar. |
| `type` |   string   |    | Equal to "list". |
| `children` |   Array.&lt;[sync.api.Editor.ActionsLoadedEvent.ListEntry](sync.api.Editor.ActionsLoadedEvent.md#.ListEntry)&gt;   |    | the context menu entries entries. |

#### ListEntry

 An entry that can appear in the toolbar, toolbar dropdown menu, context menu or context sub-menu. Can be an action, a sub-menu, or a separator.

##### Type:

*   [sync.api.Editor.ActionsLoadedEvent.ActionsListDescriptor](sync.api.Editor.ActionsLoadedEvent.md#.ActionsListDescriptor) | [sync.api.Editor.ActionsLoadedEvent.ActionEntry](sync.api.Editor.ActionsLoadedEvent.md#.ActionEntry) | [sync.api.Editor.ActionsLoadedEvent.Sep](sync.api.Editor.ActionsLoadedEvent.md#.Sep)

#### Sep

 A separator.

##### Type:

*   Object

##### Properties:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `type` |   string   | Equal to "sep". |

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
