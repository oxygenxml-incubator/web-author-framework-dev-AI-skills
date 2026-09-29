# Class: EditingSupport

##   [sync](sync.md)[.api](sync.api.md). EditingSupport

#### new EditingSupport(options)

Support for rendering the content of the current editor and for setting the actions, toolbars and views associated with it.

Can be obtained by using [sync.api.Editor#getEditingSupport](sync.api.Editor.md#getEditingSupport).

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `options` |   [sync.api.Workspace.LoadingOptions](sync.api.Workspace.md#.LoadingOptions)   | The options to be used by the editing support. |

### Classes
    [DirtyStatusChangedEvent](sync.api.EditingSupport.DirtyStatusChangedEvent.md)
### Members

#### &lt;static&gt; EventType :String

 Event types.

##### Type:

*   String

##### Properties:

  | Name | Type | Default | Description |
  | -----------| -----------| -----------| -----------|
| `DIRTY_STATUS_CHANGED` |   String   |  AES_dirty_status_changed  |  |
| `MODEL_CHANGED` |   String   |  AES_model_changed  |  |

#### options :[sync.api.Workspace.LoadingOptions](sync.api.Workspace.md#.LoadingOptions)

 The options used to load the editing support.

##### Type:

*   [sync.api.Workspace.LoadingOptions](sync.api.Workspace.md#.LoadingOptions)

### Methods

#### disposeInternal()

 Method that disposes the editing support. Sub-classes must call the super implementation of this method. Use it to do things like: - dispose dialogs - stop timers - unregister listeners on global objects, etc.

#### focus()

 Focus the editing support.

#### getActionsManager()

 Returns the actions manager for the current document.

##### Returns:

 The actions manager.
     Type     [sync.api.ActionsManagerCore](sync.api.ActionsManagerCore.md)
#### getApplicationToolbar()

 Get the configuration of the application toolbar. By default the application toolbar is displayed on the left side of the file name, next to the application icon (on small screns it is the first toolbar from the toolbars bar).

##### Returns:

 The toolbars actions list descriptor.
     Type     Array.&lt;[sync.api.Editor.ActionsLoadedEvent.ActionsListDescriptor](sync.api.Editor.ActionsLoadedEvent.md#.ActionsListDescriptor)&gt;
#### getConcurrentEditingManager()

##### Returns:

 The concurrent editing manager for the current document, or null if concurrent editing is not supported for the current type of document.
     Type     [sync.api.ConcurrentEditingManager](sync.api.ConcurrentEditingManager.md) | null
#### getContent(callback)

 Retrieves the content of the document asynchronously.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `callback` |   [sync.api.EditingSupport~onContentReceived](sync.api.EditingSupport.md#~onContentReceived)   | The callback that will be called once the XML content is retrieved. |

#### getContentType()

 Get the content type of the document as detected by the server. See also: - editor, options) - sync.api.EditingSupport.getType - sync.api.Editor.getEditorType
    Since:
* 28.1.

##### Returns:

 The document content type (for example, "text/xml", "text/plain", "text/markdown", etc.).
     Type     string
#### getFirstToolbar()

 Get the configuration of the first toolbar.

##### Returns:

 The toolbars actions list descriptor.
     Type     Array.&lt;[sync.api.Editor.ActionsLoadedEvent.ActionsListDescriptor](sync.api.Editor.ActionsLoadedEvent.md#.ActionsListDescriptor)&gt;
#### getHighlightsManager()

 Returns the handler for non persistent highlights.

##### Returns:

 The highlights manager.
     Type     sync.api.HighlightsManager | null
#### getOtherToolbars(done)

 Get the configuration of other toolbars.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `done` |   function   | Callback when the toolbars actions list descriptor is ready to be used. |

#### getResourceDragHandler()

 Get the handler for dragging resources inside the editor area.

##### Returns:

 Resource drag handler.
     Type     [sync.view.ResourceDragHandler](sync.view.ResourceDragHandler.md)
#### getSelectionManager()

 Returns the selection manager of the document.

##### Returns:

 The selection manager.
     Type     [sync.api.SelectionManagerCore](sync.api.SelectionManagerCore.md)
#### getSpellChecker()

 Get the editor spellchecker.

##### Returns:

 The spellchecker.
     Type     [sync.api.SpellChecker](sync.api.SpellChecker.md)
#### getType()

 Get the type of the editor.

##### Returns:

 the type of the editor.
     Type     [sync.api.Editor.EditorTypes](sync.api.Editor.md#.EditorTypes)
#### getUrl()

 Get the URL of the document.

##### Returns:

 The URL.
     Type     string
#### load(newDoc, docContainer, problemReporter)

 Initializes the editing support.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `newDoc` |   [LoadedDocument](global.md#LoadedDocument)   | The document created by the server. |
| `docContainer` |   HTMLElement   | The element in which we add our editor. |
| `problemReporter` |   NotificationsManager   | The problem reporter. |

##### Returns:

 An object with a 'then' method that fulfills when the editing support is loaded.
     Type     Thenable
#### &lt;abstract&gt; performFind(termToFind)

 Performs a find query with the specified term.

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `termToFind` |   String   |  &lt;nullable&gt;   |  |

#### scheduleDocumentTransaction(transaction)

 Schedules a transaction to modify the document.
The transaction can read information from the document DOM, manipulate the selection and invoke AuthorOperations. Other concurrent user actions or synchronizations from peers do not affect the execution of this transaction.

The transaction may not run if an action with Scheduler.ActionType.HANDLES_BLOCKING type is in progress.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `transaction` |   function   | The transaction to schedule. |

#### scrollToAnchor(url)

 Scrolls the document to the anchor of the url, if any.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `url` |   string   | The url. |

##### Returns:

 True if the scroll is possible.
     Type     boolean
### Type Definitions

#### onContentReceived(error, content)

 A callback invoked when the asynchronous request for the content finishes. If the operation is successful, the first parameter is `null` and the second one is a string that represents the content. In case of an error, the first parameter is an object describing the error.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `error` |   object   | The error object, or null if the request was successful. |
| `content` |   string   | The serialized XML content. |

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
