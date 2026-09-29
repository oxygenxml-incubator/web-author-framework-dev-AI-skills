# Class: ViewRenderer

##   [sync](sync.md)[.view](sync.view.md). ViewRenderer

#### new ViewRenderer()

 Base class for Oxygen XML Web Author views.

### Extends

* [goog.events.EventTarget](goog.events.EventTarget.md)

### Methods

#### addOnDisposeCallback(callback [, opt_scope])

 Invokes a callback function when this object is disposed. Callbacks are invoked in the order in which they were added. If a callback is added to an already disposed Disposable, it will be called immediately.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `callback` |   function   |    | The callback function. |
| `opt_scope` |   T   |  &lt;optional&gt;   | An optional scope to call the callback in. |
    Inherited From:
*   [goog.Disposable#addOnDisposeCallback](goog.Disposable.md#addOnDisposeCallback)

#### closed()

 Callback when the view is hidden from the user. This may include collapsing it, switching to another another view in a tabbed view container, etc.

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
#### editorChanged(editor)

Callback received when the focused editor was changed.

When the view renderer is installed, there might be no editor loaded. However, if the editor is already loaded when install is called, this method is called immediately after install. The view is not notified when the editor is disposed, but it can listen for the[sync.api.Editor.EventTypes.DISPOSE](sync.api.Editor.md#.EventTypes#.DISPOSE) event.

This method is not called if the given editor is not supported, i.e.[sync.view.ViewRenderer#supportsEditor](sync.view.ViewRenderer.md#supportsEditor) returns false.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `editor` |   [sync.api.Editor](sync.api.Editor.md)   | The new editor. |

#### focus()

 Method called to focus the current view.

#### &lt;protected&gt; getIcon( [devicePixelRatio])

One should override this method to provide the absolute URL of the action's large icon.

If you want to distribute the icon in a framework, you need to place it in the "web/" sub-folder of the framework. In this case the absolute URL of the icon can be obtained by concatenating [sync.ext.Registry.extensionURL](sync.ext.Registry.md#.extensionURL)with the relative path of the icon to the "web/" sub-folder.

If you want to distribute the icon in a plugin, you can place it in a directory with static resources using a[WebappStaticResourcesFolder](https://oxygenxml.com/doc/ug-waCustom/topics/customizing_plugins.html) extension.

The icon should have a minimum size of 24 by 24 px for non-hidpi displays and can vary depending on the device pixel ration, the icon being used as the background of a 24 by 24 px DIV.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `devicePixelRatio` |   number   |  &lt;optional&gt;   | the device pixel ratio. |

##### Returns:

 The icon URL.
     Type     string | null
#### getParentEventTarget()

 Returns the parent of this event target to use for bubbling.
    Inherited From:
*   [goog.events.EventTarget#getParentEventTarget](goog.events.EventTarget.md#getParentEventTarget)

##### Returns:

 The parent EventTarget or null if there is no parent.
     Type     [goog.events.EventTarget](goog.events.EventTarget.md)
#### getTitle()

 Returns the title of the view.

##### Returns:

 The title of the view.
     Type     string
#### getToolbarActionsMap()

 Returns a map of actions used to create an action manager for the view's toolbar. If it is not provided, the editor's action manager will be used.\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\***EXPERIMENTAL** - Subject to change\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

##### Returns:

 Map from action id to actions
     Type     Object.&lt;string, [sync.actions.AbstractAction](sync.actions.AbstractAction.md)&gt;
#### getToolbarDescriptor()

 Returns the toolbar descriptor for the view. This toolbar will be shown in the view's header.\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\***EXPERIMENTAL** - Subject to change\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

##### Returns:

 The toolbar's descriptor
     Type     [sync.api.Editor.ActionsLoadedEvent.ActionsListDescriptor](sync.api.Editor.ActionsLoadedEvent.md#.ActionsListDescriptor)
#### install(element)

 This method is called when the view renderer is linked to the actual place where the view will be rendered.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `element` |   HTMLElement   | The element. |

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

#### opened()

 Callback when the view is shown to the user. This may include expanding it, switching the tab of this view in a tabbed view container, etc.
To check the initial state of the view, when it is installed, use sync.view.ViewManager.isViewOpen.

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
#### renderIcon()

 This method renders the icon of the view in a 24px by 24px div. This allows the getIcon() method to return different sized icons depending on the device pixel ration, the size constraints being imposed by the enclosing DIV. It should be overridden only for custom rendering strategies, otherwise consider using the getIcon method.

##### Returns:

 the rendering of the view icon.
     Type     [Element](Element.md)
#### supportsEditor(editor)

Method used to determine if a given editor is supported. If supported, [sync.view.ViewRenderer#editorChanged](sync.view.ViewRenderer.md#editorChanged)will be called for that editor.

The default implementation of this method returns `true` only for Author editors.

If a view does not support an editor, it will be disabled. To enable it later one can use[sync.view.ViewManager#enableView](sync.view.ViewManager.md#enableView).

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `editor` |   [sync.api.Editor](sync.api.Editor.md)   | The editor to check support for. |
    Since:
* 21.1.1

##### Returns:

 returns true if the given editor is supported.
     Type     boolean
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

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
