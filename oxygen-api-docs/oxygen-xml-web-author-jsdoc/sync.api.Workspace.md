# Class: Workspace

##   [sync](sync.md)[.api](sync.api.md). Workspace

#### new Workspace()

 Access to the Workspace in which the editor is opened.

### Extends

* [goog.events.EventTarget](goog.events.EventTarget.md)

### Classes
    [BeforeEditorOpenedEvent](sync.api.Workspace.BeforeEditorOpenedEvent.md)    [DashboardLifecycleEvent](sync.api.Workspace.DashboardLifecycleEvent.md)    [EditorLifecycleEvent](sync.api.Workspace.EditorLifecycleEvent.md)
### Members

#### &lt;static&gt; EventType :string

 The types of the sync.api.Workspace events.

##### Type:

*   string

##### Properties:

  | Name | Type | Default | Description |
  | -----------| -----------| -----------| -----------|
| `BEFORE_EDITOR_LOADED` |   string   |  before_editor_loaded  | Triggered before the editor content was loaded. Note that frameworks code cannot use this event since the framework is detected while the document is loaded.See [sync.api.Workspace.BeforeEditorOpenedEvent](sync.api.Workspace.BeforeEditorOpenedEvent.md) for more details. |
| `EDITOR_LOADED` |   string   |  editor_loaded  | Triggered after the editor was loaded.See [sync.api.Workspace.EditorLifecycleEvent](sync.api.Workspace.EditorLifecycleEvent.md) for more details. |
| `EDITOR_LOADING_FAILED` |   string   |  editor_loading_failed  | Triggered after the editor was loaded.See [sync.api.Workspace.EditorLifecycleEvent](sync.api.Workspace.EditorLifecycleEvent.md) for more details. |
| `EDITOR_DISPOSED` |   string   |  editor_disposed  | Triggered when the editor was disposed.See [sync.api.Workspace.EditorLifecycleEvent](sync.api.Workspace.EditorLifecycleEvent.md) for more details. |
| `BEFORE_EDITOR_DISPOSED` |   string   |  before_editor_disposed  | Triggered before the editor will be disposed.See [sync.api.Workspace.EditorLifecycleEvent](sync.api.Workspace.EditorLifecycleEvent.md) for more details. |
| `BEFORE_DASHBOARD_LOADED` |   string   |  before_dashboard_loaded  | Triggered before the dashboard is loaded.See [sync.api.Workspace.DashboardLifecycleEvent](sync.api.Workspace.DashboardLifecycleEvent.md) for more details. |
| `DASHBOARD_LOADED` |   string   |  dashboard_loaded  | Triggered after the dashboard was loaded.See [sync.api.Workspace.DashboardLifecycleEvent](sync.api.Workspace.DashboardLifecycleEvent.md) for more details. |

### Methods

#### &lt;static&gt; createEditorStripe(height [, first] [, below])

 Create and add a stripe above/below the editor.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `height` |   number   |    | The height of the stripe in pixels. |
| `first` |   boolean   |  &lt;optional&gt;   | Flag that causes the stripe to be added first (false by default). |
| `below` |   boolean   |  &lt;optional&gt;   | Flag that causes the stripe to be added below the editor (false by default). |
    Since:
* 26

##### Returns:

 The stripe element.
     Type     [Element](Element.md)
#### addOnDisposeCallback(callback [, opt_scope])

 Invokes a callback function when this object is disposed. Callbacks are invoked in the order in which they were added. If a callback is added to an already disposed Disposable, it will be called immediately.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `callback` |   function   |    | The callback function. |
| `opt_scope` |   T   |  &lt;optional&gt;   | An optional scope to call the callback in. |
    Inherited From:
*   [goog.Disposable#addOnDisposeCallback](goog.Disposable.md#addOnDisposeCallback)

#### addRelativeReferencesResolver(protocol, resolver)

 Web Author prefers to insert the external references as relative URLs. It has a default algorithm to make an URL relative to a given base. However, you for certain URL protocols you can provide your own algorithm.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `protocol` |   string   | The protocol handled by the resolver. |
| `resolver` |   function   | The relative references resolver. The first argument the URL used as a base for relativization and the second one is is the URL to make relative . |

#### createDialog( [opt_id])

 Creates a dialog that can have custom content and behavior. The advantage of using this method is that the dialog will have a consistent appearance with the rest of the application and that it will work on all devices supported by the WebApp.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `opt_id` |   string   |  &lt;optional&gt;   | The id that will be given to the dialog box. For example, you can use it for specifying the width of the dialog in CSS. |

##### Returns:

 The dialog.
     Type     [sync.api.Dialog](sync.api.Dialog.md)
#### dispatchEvent(e)

 Dispatches an event (or event like object) and calls all listeners listening for events of this type. The type of the event is decided by the type property on the event object. If any of the listeners returns false OR calls preventDefault then this function will return false. If one of the capture listeners calls stopPropagation, then the bubble listeners won't fire.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `e` |   Object  /  [goog.events.Event](goog.events.Event.md)   | Event object. |
    Inherited From:
*   [goog.events.EventTarget#dispatchEvent](goog.events.EventTarget.md#dispatchEvent)

##### Returns:

 If anyone called preventDefault on the event object (or if any of the listeners returns false) this will also return false.
     Type     boolean
#### dispose()

 Disposes of the object. If the object hasn't already been disposed of, calls #disposeInternal. Classes that extend `goog.Disposable` should override #disposeInternal in order to delete references to COM objects, DOM nodes, and other disposable objects. Reentrant.
    Inherited From:
*   [goog.Disposable#dispose](goog.Disposable.md#dispose)

##### Returns:

 Nothing.
     Type     void
#### getEditingContextManager()

 Return the editing context manager.

##### Returns:

 The editing context manager.
     Type     [sync.api.EditingContextManager](sync.api.EditingContextManager.md)
#### getEditingSupportManager()

 Returns the editing support manager that can be used to create a specific [sync.api.EditingSupport](sync.api.EditingSupport.md) to the current editor.
    Since:
* 21.1.1

##### Returns:

 The editing support manager.
     Type     [sync.api.EditingSupportManager](sync.api.EditingSupportManager.md)
#### getFileServersManager()

 Returns the file servers manager helper object that can be used to register a descriptor that provides rendering information and file browsing functionality for a specific file server.
    Since:
* 20.1.1

##### Returns:

 The file servers manager.
     Type     [sync.api.FileServersManager](sync.api.FileServersManager.md)
#### getNotificationManager()

 Returns an object that can be used to display notifications to the user.

##### Returns:

 the notifications manager.
     Type     [sync.api.NotificationsManager](sync.api.NotificationsManager.md)
#### getOption(optionKey, defaultValue)

 Client options getter function.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `optionKey` |   string   | {sync.api.Workspace.Options} property name. |
| `defaultValue` |   string   | the default value to be returned in case the option is not set. |

##### Returns:

 the set option. In case the option is not set it returns the defaultValue or null.
     Type     string
#### getParentEventTarget()

 Returns the parent of this event target to use for bubbling.
    Inherited From:
*   [goog.events.EventTarget#getParentEventTarget](goog.events.EventTarget.md#getParentEventTarget)

##### Returns:

 The parent EventTarget or null if there is no parent.
     Type     [goog.events.EventTarget](goog.events.EventTarget.md)
#### getUrlChooser()

 Returns the URL chooser used when the user is asked to provide an URL.

##### Returns:

 The currently registered URL chooser.
     Type     [sync.api.UrlChooser](sync.api.UrlChooser.md)
#### getViewManager()

 Returns the view manager helper object that can be used to customize Oxygen XML Web Author views.

##### Returns:

 The view manager.
     Type     [sync.view.ViewManager](sync.view.ViewManager.md)
#### isDisposed()
        Inherited From:
*   [goog.Disposable#isDisposed](goog.Disposable.md#isDisposed)

##### Returns:

 Whether the object has been disposed of.
     Type     boolean
#### listen(type, listener [, opt_useCapture] [, opt_listenerScope])

 Adds an event listener. A listener can only be added once to an object and if it is added again the key for the listener is returned. Note that if the existing listener is a one-off listener (registered via listenOnce), it will no longer be a one-off listener after a call to listen().

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `type` |   string   |    | The event type id. |
| `listener` |   function   |    | Callback method. |
| `opt_useCapture` |   boolean   |  &lt;optional&gt;   | Whether to fire in capture phase (defaults to false). |
| `opt_listenerScope` |   SCOPE   |  &lt;optional&gt;   | Object in whose scope to call the listener. |
    Inherited From:
*   [goog.events.EventTarget#listen](goog.events.EventTarget.md#listen)

#### listenOnce(type, listener [, opt_useCapture] [, opt_listenerScope])

 Adds an event listener that is removed automatically after the listener fired once. If an existing listener already exists, listenOnce will do nothing. In particular, if the listener was previously registered via listen(), listenOnce() will not turn the listener into a one-off listener. Similarly, if there is already an existing one-off listener, listenOnce does not modify the listeners (it is still a once listener).

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `type` |   string   |    | The event type id. |
| `listener` |   function   |    | Callback method. |
| `opt_useCapture` |   boolean   |  &lt;optional&gt;   | Whether to fire in capture phase (defaults to false). |
| `opt_listenerScope` |   SCOPE   |  &lt;optional&gt;   | Object in whose scope to call the listener. |
    Inherited From:
*   [goog.events.EventTarget#listenOnce](goog.events.EventTarget.md#listenOnce)

#### makeRelative(base, url)

 Makes an URL relative to the base.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `base` |   string   | The relativization base, needs to be an absolute URL. |
| `url` |   string   | The URL to make relative. |

##### Returns:

 The relative URL.
     Type     string
#### openLink(e)

 Open a link with the behavior determined by the provided event.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `e` |   [sync.api.Editor.LinkOpenedEvent](sync.api.Editor.LinkOpenedEvent.md)   | The link opened event. |
    Since:
* 25

#### registerDisposable(disposable)

 Associates a disposable object with this object so that they will be disposed together.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `disposable` |   goog.disposable.IDisposable   | that will be disposed when this object is disposed. |
    Inherited From:
*   [goog.Disposable#registerDisposable](goog.Disposable.md#registerDisposable)

#### removeAllListeners( [opt_type])

 Removes all listeners from this listenable. If type is specified, it will only remove listeners of the particular type. otherwise all registered listeners will be removed.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `opt_type` |   string   |  &lt;optional&gt;   | Type of event to remove, default is to remove all types. |
    Inherited From:
*   [goog.events.EventTarget#removeAllListeners](goog.events.EventTarget.md#removeAllListeners)

##### Returns:

 Number of listeners removed.
     Type     number
#### removeEditorStripe(stripe [, below])

 Removes an editor stripe.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `stripe` |   [Element](Element.md)   |    | The stripe element. |
| `below` |   boolean   |  &lt;optional&gt;   | Flag indicating if the stripe is placed below or above the editor (false by default). |
    Since:
* 26

#### setBaseFontFamily(fontFamily)

 Sets the base font family for all views and dialogs.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `fontFamily` |   string   | The font family to apply (e.g., 'Arial, sans-serif'). |

#### setOption(optionKey, newValue)

 Client options setter function.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `optionKey` |   string   | {sync.api.Workspace.Options} property name. |
| `newValue` |   string   | the option's new value. |

#### setStripesContainer(stripesContainer)

 Sets the stripes container.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `stripesContainer` |   [Element](Element.md)   | The stripes container. |

#### setUrlChooser(urlChooser)

 Sets the URL chooser used when the user is asked to provide an URL. When there is not chooser set, the user will usually have to enter the URLs in a text field.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `urlChooser` |   [sync.api.UrlChooser](sync.api.UrlChooser.md)   | The URL chooser to set. |

#### unlisten(type, listener [, opt_useCapture] [, opt_listenerScope])

 Removes an event listener which was added with listen() or listenOnce().

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `type` |   string   |    | The event type id. |
| `listener` |   function   |    | Callback method. |
| `opt_useCapture` |   boolean   |  &lt;optional&gt;   | Whether to fire in capture phase (defaults to false). |
| `opt_listenerScope` |   SCOPE   |  &lt;optional&gt;   | Object in whose scope to call the listener. |
    Inherited From:
*   [goog.events.EventTarget#unlisten](goog.events.EventTarget.md#unlisten)

##### Returns:

 Whether any listener was removed.
     Type     boolean
### Type Definitions

#### DashboardLoadingOptions

 The options used to open the dashboard.

##### Type:

*   Object

##### Properties:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `folderUrl` |   string   | The URL of the folder to be opened on the dashboard. |
| `fileServerName` |   string   | The name of the file server to be opened on the dashboard. |

#### LoadingOptions

 The object used to open the editor.

##### Type:

*   Object

##### Properties:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `url` |   string   |    | The URL of the document. |
| `title` |   string   |  &lt;optional&gt;   | The title of the document. If not specified, it is inferred from URL. |
| `userName` |   string   |  &lt;optional&gt;   | The name of the user which will edit the document. Used as the author for comments and displayed in the top-right corner. If not specified, it is inferred from the *userName* URL variable. |
| `content` |   string   |  &lt;optional&gt;   | The content of the document. If not specified, the server will load the content from the given URL. |
| `modes` |   string   |  &lt;optional&gt;   | The available editing modes, comma-separated. If multiple values are passed in, the first one will be active and the user can switch to another one using the GUI. Possible values: * review - only the review actions are enabled * edit - full editing support is enabled  |
| `trackChanges` |   [sync.api.change_tracking.ChangeTrackingInitialState](sync.api.change_tracking.md#.ChangeTrackingInitialState)   |  &lt;optional&gt;   | Controls the initial change-tracking state: If you use an option different than 'default', the server change tracking status (as configured in the Administration Page) should not be "Stored in the document". |
| `autoSaveInterval` |   number   |  &lt;optional&gt;   | the interval of time (in seconds) to wait until an auto-save is performed. If &lt;= 0 or falsy, auto-save is disabled. |
| `contentType` |   string   |  &lt;optional&gt;   | The content type of the edited document, "text/xml" for XML documents. The content encoding can be passed 'text/xml: charset=utf-8'. |
| `'show.caret.position.info'` |   boolean   |  &lt;optional&gt;   | Flag that controls whether to show caret tooltip or not. Have precedence over the server option. Default value is true. |
| `'validate.as.you.type'` |   string   |  &lt;optional&gt;   | Whether automatic validation should be enabled. Defaults to true. |
| `ccOnEnter` |   string   |  &lt;optional&gt;   | Flag that controls whether the content completion list is presented when the user press 'Enter'. Has precedence over the value of "Show content completion list on Enter" server option (controlled from "General" option page). |
| `elementNameEnhancer` |   [sync.api.ElementNameEnhancer](sync.api.md#.ElementNameEnhancer)   |  &lt;optional&gt;   | A function which can enhance the name of elements depending on their attributes. |
| `'stylesheet-titles'` |   string  /  Array.&lt;string&gt;   |    | A list of titles of CSS groups (defined in the framework) that will be used to render the document. The list can be passed either as a JS array or concatenated as a comma-separated string. |
| `expandTopicRefs` |   boolean   |  &lt;optional&gt;   | If set to true, when a DITA map is opened in Oxygen XML Web Author, the content of all topics referenced in the map will be presented. |
| `KeyscopeStack` |   string   |  &lt;optional&gt;   | (DITA-specific Parameter) Used for resolving keys when DITA 1.3 key scopes are defined in the DITA map. The value looks like this: `a b c,d e f` for a DITA map that has the key scope defined like this:  |
| `backupTimeout` |   number   |  &lt;optional&gt;   | The time to wait, after an edit, before making a backup. |
| `compactTagsMode` |   boolean   |  &lt;optional&gt;   | Flag that controls whether the consecutive block tags are displayed on the same line (when the value is true) or on separate lines (when the value is false). Default value is true. |
| `quickUpDownNavigation` |   boolean   |  &lt;optional&gt;   | This option is false by default and this means that when the user navigates using the up and down arrow keys, the cursor is placed within each of the underlying XML elements between two blocks of text (the cursor changes to a horizontal line when it is between blocks of text). This allows to easily insert elements and manage the structure of the XML content. However, if this option is true, the cursor ignores the XML structure and jumps from one line of text to another, similar to how the cursor behaves in a word processor. |
| `textModeReadOnly` |   boolean   |  &lt;optional&gt;   | Flag that controls whether the text mode will be read-only. Defaults to false. |
| `readOnlyState` |   string  /  Object   |    | Can be either the string `read-only` or an object with a `reason` field that contains a message to be displayed in the user interface and a `code` that can be used, for example, when rendering the read-only stripe of the editor {@see sync.api.Editor#setReadOnlyStripeRenderer}. The `code` is a way to encode the `reason` that does not change according the the UI locale. |
| `'schematron.imposed.phase'` |   string   |  &lt;optional&gt;   | Used to impose a phase with that name in any Schematron file used for validation. |
| `schematronUrl` |   string   |  &lt;optional&gt;   | (Markdown only) Used to specify a Schematron file to validate the Markdown file with. It will only work for Markdown files, if the Markdown editing plugin is installed. |
| `showDitaMapView` |   boolean   |  &lt;optional&gt;   | (DITA-specific Parameter) whether to show the DITA Map View on load. |
| `editReferencesInPlace` |   boolean   |  &lt;optional&gt;   | (DITA-specific Parameter) allow inplace editing for referred content. If the opened document is a DITA Map, the content of all topics referenced in the map will be presented in the editor and it will be possible to be edited. Defaults to false. |
| `outlinePlacement` |   string   |  &lt;optional&gt;   | Controls the side where the outline will be shown. Possible values: *  right *  left  |
| `showTopicTitles` |   boolean   |  &lt;optional&gt;   | (DITA Map-specific Parameter) whether to resolve the topic titles for DITA Maps. Defaults to false. |
| `multipleNonFoldedChildren` |   boolean   |  &lt;optional&gt;   | `true` to display all children whose names are listed in the `-oxy-not-foldable-child` CSS property. `false` to display only the first one. `true` by default. |
| `roomId` |   string   |  &lt;optional&gt;   | The ID of the concurrent editing room to join. This option should be added besides the usual `url` parameter that specifies the URL of the document. |
| `sharedSessionCompatible` |   boolean   |  &lt;optional&gt;   | Can be set by a CMS-connector plugin to declare that a it is compatible with the [Editing Session Sharing feature / https://www.oxygenxml.com/doc/help.php?product=webauthor&pageId=webauthor-concurrent-editing-api}. |
| `inplaceReferenceEditingSupported` |   boolean   |  &lt;optional&gt;   | option to be set to mark that the connector supports editing references in-place. |
| `search.find` |   String   |  &lt;optional&gt;   | Text to find |
| `search.replace` |   String   |  &lt;optional&gt;   | Replacement text that should be written in the find-replace dialog. |
| `search.matchCase` |   Boolean   |  &lt;optional&gt;   | Flag controlling the find-replace match-case option. |
| `search.wholeWords` |   Boolean   |  &lt;optional&gt;   | Flag controlling the find-replace whole-words option. |
| `searchMode` |   String   |    | controls in what UI component the find/replace form is rendered. Possible values: * dialog - the find/replace form is presented in a dialog. * view - the find/replace form is presented in a side-view.  |

#### Options

 The object used to open the editor.

##### Type:

*   Object

##### Properties:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `'selected.language'` |   string   |  &lt;optional&gt;   | The current language. |
| `'sentinels.display.mode'` |   string   |  &lt;optional&gt;   | Controls the sentinels display mode. Possible values: *  no-tags - no tags. *  partial-tags - partial tags. *  inline-tags - inline tags. *  block-tags - block tags. *  full-tags - full tags. *  full-tags-with-attributes - full tags with attributes.  |
| `'spellcheck.enabled'` |   string   |  &lt;optional&gt;   | controls whether the spellchecker is enabled or not. Possible values: *  true - The spellchecker is enabled. *  false - The spellchecker is disabled.  |

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
