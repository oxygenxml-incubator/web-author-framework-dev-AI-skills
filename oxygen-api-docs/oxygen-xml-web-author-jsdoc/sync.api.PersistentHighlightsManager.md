# Class: PersistentHighlightsManager

##   [sync](sync.md)[.api](sync.api.md). PersistentHighlightsManager

#### new PersistentHighlightsManager()

 Manages custom persistent highlights. To get access to this manager use[sync.api.AuthorEditingSupport#getPersistentHighlightsManager](sync.api.AuthorEditingSupport.md#getPersistentHighlightsManager). The custom persistent highlights are serialized in the XML as processing instructions with the following form:`&lt;?oxy_custom_start prop1="val1"....?&gt; xml content &lt;?oxy_custom_end?&gt;`This manager allows you to add a single highlight at a time, by using the async[sync.api.PersistentHighlightsManager#addHighlight](sync.api.PersistentHighlightsManager.md#addHighlight) operation. If multiples highlights needs to be added in a single step, you can [create an AuthorOperation](tutorial-modifydoc.md)that uses the server side ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlighter JAVA API.To listen for highlights updates register a listener on this manager:
```
highlightsManager.listen(sync.api.PersistentHighlightUpdateEvent.EventType.HIGHLIGHT_ADDED, function(e) {});highlightsManager.listen(sync.api.PersistentHighlightUpdateEvent.EventType.HIGHLIGHT_REMOVED, function(e) {});

```

    Since:
* 22.1

### Extends

* [goog.events.EventTarget](goog.events.EventTarget.md)

### Methods

#### addHighlight( [attributes], callback)

 Adds a custom highlight over the current selection.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `attributes` |   Map.&lt;String, String&gt;   |  &lt;optional&gt;   | The attributes of the highlight to be added on the HTML element generated for this highlight. The value of the "className" attribute will also be added to the class name list of the generated element. |
| `callback` |   function   |    | The callback when the highlight is added. The callback's first argument is the error object or null; the second one is the id of the added highlight. |

#### addOnDisposeCallback(callback [, opt_scope])

 Invokes a callback function when this object is disposed. Callbacks are invoked in the order in which they were added. If a callback is added to an already disposed Disposable, it will be called immediately.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `callback` |   function   |    | The callback function. |
| `opt_scope` |   T   |  &lt;optional&gt;   | An optional scope to call the callback in. |
    Inherited From:
*   [goog.Disposable#addOnDisposeCallback](goog.Disposable.md#addOnDisposeCallback)

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
#### getAllHighlights()

 Get all highlights.

##### Returns:

 The ids of all highlights.
     Type     Array.&lt;string&gt;
#### getHighlightAttributes(id)

 Get the attributes of a highlight.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `id` |   String   | The id of the highlight. |

##### Returns:

 The object representing the highlights attributes
     Type     object
#### getHighlightsAtCaret( [matchStartEnd])

 Get all the custom persistent highlights at caret.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `matchStartEnd` |   boolean   |  &lt;optional&gt;   | If true, the results match markers that start / end at the given position (by default it's false). |

##### Returns:

 The ids of the highlights at caret.
     Type     Array.&lt;string&gt;
#### getHighlightSelection(highlightId)

 Ge the selection corresponding to a highlight

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `highlightId` |   string   | The highlight id. |

##### Returns:

 The selection.
     Type     [sync.api.Selection](sync.api.Selection.md) | null
#### getParentEventTarget()

 Returns the parent of this event target to use for bubbling.
    Inherited From:
*   [goog.events.EventTarget#getParentEventTarget](goog.events.EventTarget.md#getParentEventTarget)

##### Returns:

 The parent EventTarget or null if there is no parent.
     Type     [goog.events.EventTarget](goog.events.EventTarget.md)
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
#### removeHighlights(ids, callback)

 Removes highlights.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `ids` |   Array.&lt;String&gt;   | The ids of the highlights to be removed. |
| `callback` |   function   | The callback when the highlights are removed. The callback's argument is the error object or null. |

#### scrollToHighlight(highlightId)

 Scroll to a specific highlight.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `highlightId` |   String   | The id of the highlight to be selected. |

#### selectHighlight(highlightId)

 Select a specific highlight.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `highlightId` |   String   | The id of the highlight to be selected. |

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
#### updateHighlight(id [, attributes], callback)

 Updates a highlight.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `id` |   String   |    | The id of the highlight to update. |
| `attributes` |   Map.&lt;String, String&gt;   |  &lt;optional&gt;   | The attributes to be updated. If the map is null, the attributes remain unchanged. To remove an attribute, add it to the map with a null value. |
| `callback` |   function   |    | The callback when the highlight update is done. The callback's first argument is the error object or null; the second one is the new id of the highlight. |

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
