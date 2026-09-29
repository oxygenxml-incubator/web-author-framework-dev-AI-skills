# Class: exports

##  exports

#### new exports(options)

 Instance of [sync.api.EditingSupport](sync.api.EditingSupport.md) used when the current document is an XML document opened in "Author" mode.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `options` |   [sync.api.Workspace.LoadingOptions](sync.api.Workspace.md#.LoadingOptions)   | The options to be used by the editing support. |

### Members

#### ditamapUrl :string

 The URL of the context DITA Map - used for resolving keys and to display.

##### Type:

*   string

#### ditaProjectContextId :string

 The id of the DITA context.

##### Type:

*   string

#### ditaProjectUrl :string

 The URL of the DITA Project

##### Type:

*   string

#### filterUrl :string

 The URL of the DITAVAL filter used to conditionally include and exclude content from both the DITA Map and the editor.

##### Type:

*   string

#### guessed :boolean

 true if the DITA map URL is guessed from the history.

##### Type:

*   boolean

#### isProjectActive :boolean

 True if DITA project is active.

##### Type:

*   boolean

# Class: exports

##  exports

Renders the DITA Map view.

#### new exports()

 Constructor.
    Since:
* 26.1

### Members

#### ditamapUrl :string

 The URL of the context DITA Map - used for resolving keys and to display.

##### Type:

*   string

#### ditaProjectContextId :string

 The id of the DITA context.

##### Type:

*   string

#### ditaProjectUrl :string

 The URL of the DITA Project

##### Type:

*   string

#### filterUrl :string

 The URL of the DITAVAL filter used to conditionally include and exclude content from both the DITA Map and the editor.

##### Type:

*   string

#### guessed :boolean

 true if the DITA map URL is guessed from the history.

##### Type:

*   boolean

#### isProjectActive :boolean

 True if DITA project is active.

##### Type:

*   boolean

# Class: exports

##  exports

Editing context for a DITA file.

#### new exports(ditamapUrl, filterUrl [, opt_guessed] [, opt_ditaProjectUrl] [, opt_contextId] [, opt_isProjectActive])

##### Parameters:

  | Name | Type | Argument | Description |
  | -----------| -----------| -----------| -----------|
| `ditamapUrl` |   string   |    | The URL of the context DITA Map - used for resolving keys and to display. |
| `filterUrl` |   string   |    | The URL of the DITAVAL filter used to conditionally include and exclude content from both the DITA Map and the editor. |
| `opt_guessed` |   boolean   |  &lt;optional&gt;   | true if the DITA map or project URL is guessed from the history rather that provided by the user explicitly. |
| `opt_ditaProjectUrl` |   string   |  &lt;optional&gt;   | The URL of the context DITA Project (@since 26.1). See more details about DITA Project XML files here: https://www.dita-ot.org/dev/topics/using-project-files.html |
| `opt_contextId` |   string   |  &lt;optional&gt;   | The id of the DITA project context (@since 26.1) |
| `opt_isProjectActive` |   boolean   |  &lt;optional&gt;   | If DITA project is currently active (@since 26.1) |
    Since:
* 22

### Members

#### ditamapUrl :string

 The URL of the context DITA Map - used for resolving keys and to display.

##### Type:

*   string

#### ditaProjectContextId :string

 The id of the DITA context.

##### Type:

*   string

#### ditaProjectUrl :string

 The URL of the DITA Project

##### Type:

*   string

#### filterUrl :string

 The URL of the DITAVAL filter used to conditionally include and exclude content from both the DITA Map and the editor.

##### Type:

*   string

#### guessed :boolean

 true if the DITA map URL is guessed from the history.

##### Type:

*   boolean

#### isProjectActive :boolean

 True if DITA project is active.

##### Type:

*   boolean

# Class: exports

##  exports

A review comment.

#### new exports(commentText, mentionedUserNames, authorName, timestampRaw)

 Constructor.

##### Parameters:

  | Name | Type | Description |
  | -----------| -----------| -----------|
| `commentText` |   string   | The comment text. |
| `mentionedUserNames` |   Array.&lt;string&gt;   | The mentioned user names within the comment. |
| `authorName` |   string   | The comment author name as it can be found in document. |
| `timestampRaw` |   string   | The raw timestamp value as it can be found in document. |
    Since:
* 28.1

### Members

#### ditamapUrl :string

 The URL of the context DITA Map - used for resolving keys and to display.

##### Type:

*   string

#### ditaProjectContextId :string

 The id of the DITA context.

##### Type:

*   string

#### ditaProjectUrl :string

 The URL of the DITA Project

##### Type:

*   string

#### filterUrl :string

 The URL of the DITAVAL filter used to conditionally include and exclude content from both the DITA Map and the editor.

##### Type:

*   string

#### guessed :boolean

 true if the DITA map URL is guessed from the history.

##### Type:

*   boolean

#### isProjectActive :boolean

 True if DITA project is active.

##### Type:

*   boolean

# Class: exports

##  exports

Hook that is called when a review comment is explicitly added or edited in the document by the user Note that this hook is called when the user explicitly adds a comment in the document using the Add Comment dialog, but there are also other ways to add a comment in the document, for example when the user adds a fragment with copy-paste, from XML Source (text page), etc.

#### new exports()
        Since:
* 28.1

### Members

#### ditamapUrl :string

 The URL of the context DITA Map - used for resolving keys and to display.

##### Type:

*   string

#### ditaProjectContextId :string

 The id of the DITA context.

##### Type:

*   string

#### ditaProjectUrl :string

 The URL of the DITA Project

##### Type:

*   string

#### filterUrl :string

 The URL of the DITAVAL filter used to conditionally include and exclude content from both the DITA Map and the editor.

##### Type:

*   string

#### guessed :boolean

 true if the DITA map URL is guessed from the history.

##### Type:

*   boolean

#### isProjectActive :boolean

 True if DITA project is active.

##### Type:

*   boolean

# Class: exports

##  exports

The manager for review comments inside an author editing session.

#### new exports()
        Since:
* 28.1

### Members

#### ditamapUrl :string

 The URL of the context DITA Map - used for resolving keys and to display.

##### Type:

*   string

#### ditaProjectContextId :string

 The id of the DITA context.

##### Type:

*   string

#### ditaProjectUrl :string

 The URL of the DITA Project

##### Type:

*   string

#### filterUrl :string

 The URL of the DITAVAL filter used to conditionally include and exclude content from both the DITA Map and the editor.

##### Type:

*   string

#### guessed :boolean

 true if the DITA map URL is guessed from the history.

##### Type:

*   boolean

#### isProjectActive :boolean

 True if DITA project is active.

##### Type:

*   boolean

# Class: exports

##  exports

Text-based selection manager.

#### new exports()

### Members

#### ditamapUrl :string

 The URL of the context DITA Map - used for resolving keys and to display.

##### Type:

*   string

#### ditaProjectContextId :string

 The id of the DITA context.

##### Type:

*   string

#### ditaProjectUrl :string

 The URL of the DITA Project

##### Type:

*   string

#### filterUrl :string

 The URL of the DITAVAL filter used to conditionally include and exclude content from both the DITA Map and the editor.

##### Type:

*   string

#### guessed :boolean

 true if the DITA map URL is guessed from the history.

##### Type:

*   boolean

#### isProjectActive :boolean

 True if DITA project is active.

##### Type:

*   boolean

# Class: exports

##  exports

A provider that returns user names that will be presented as proposals when user types "@" in the Add Comment dialog.

#### new exports()
        Since:
* 28.1

### Members

#### ditamapUrl :string

 The URL of the context DITA Map - used for resolving keys and to display.

##### Type:

*   string

#### ditaProjectContextId :string

 The id of the DITA context.

##### Type:

*   string

#### ditaProjectUrl :string

 The URL of the DITA Project

##### Type:

*   string

#### filterUrl :string

 The URL of the DITAVAL filter used to conditionally include and exclude content from both the DITA Map and the editor.

##### Type:

*   string

#### guessed :boolean

 true if the DITA map URL is guessed from the history.

##### Type:

*   boolean

#### isProjectActive :boolean

 True if DITA project is active.

##### Type:

*   boolean

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
