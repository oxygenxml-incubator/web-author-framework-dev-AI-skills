# Class: EventTarget

##  EventTarget

#### new EventTarget()

 An implementation of `goog.events.Listenable` with full W3C EventTarget-like support (capture/bubble mechanism, stopping event propagation, preventing default actions). You may subclass this class to turn your class into a Listenable. Unless propagation is stopped, an event dispatched by an EventTarget will bubble to the parent returned by `getParentEventTarget`. To set the parent, call `setParentEventTarget`. Subclasses that don't support changing the parent can override the setter to throw an error. Example usage:
```

  var source = new goog.events.EventTarget();
  function handleEvent(e) {
    alert('Type: ' + e.type + '; Target: ' + e.target);
  }
  source.listen('foo', handleEvent);
  ...
  source.dispatchEvent('foo');  // will call handleEvent
  ...
  source.unlisten('foo', handleEvent);

```

### Extends

* [goog.Disposable](goog.Disposable.md)

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

#### dispatchEvent(e)

 Dispatches an event (or event like object) and calls all listeners listening for events of this type. The type of the event is decided by the type property on the event object. If any of the listeners returns false OR calls preventDefault then this function will return false. If one of the capture listeners calls stopPropagation, then the bubble listeners won't fire.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `e` |   Object  /  [goog.events.Event](goog.events.Event.md)   | Event object. |

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
#### &lt;protected&gt; disposeInternal()

 Removes listeners from this object. Classes that extend EventTarget may need to override this method in order to remove references to DOM Elements and additional listeners.
    Inherited From:
*   [goog.events.EventTarget#disposeInternal](goog.events.EventTarget.md#disposeInternal)
    Overrides:
*   [goog.Disposable#disposeInternal](goog.Disposable.md#disposeInternal)

#### getParentEventTarget()

 Returns the parent of this event target to use for bubbling.

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

#### listenOnce(type, listener [, opt_useCapture] [, opt_listenerScope])

 Adds an event listener that is removed automatically after the listener fired once. If an existing listener already exists, listenOnce will do nothing. In particular, if the listener was previously registered via listen(), listenOnce() will not turn the listener into a one-off listener. Similarly, if there is already an existing one-off listener, listenOnce does not modify the listeners (it is still a once listener).

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `type` |   string   |    | The event type id. |
| `listener` |   function   |    | Callback method. |
| `opt_useCapture` |   boolean   |  &lt;optional&gt;   | Whether to fire in capture phase (defaults to false). |
| `opt_listenerScope` |   SCOPE   |  &lt;optional&gt;   | Object in whose scope to call the listener. |

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

##### Returns:

 Number of listeners removed.
     Type     number
#### unlisten(type, listener [, opt_useCapture] [, opt_listenerScope])

 Removes an event listener which was added with listen() or listenOnce().

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `type` |   string   |    | The event type id. |
| `listener` |   function   |    | Callback method. |
| `opt_useCapture` |   boolean   |  &lt;optional&gt;   | Whether to fire in capture phase (defaults to false). |
| `opt_listenerScope` |   SCOPE   |  &lt;optional&gt;   | Object in whose scope to call the listener. |

##### Returns:

 Whether any listener was removed.
     Type     boolean

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
