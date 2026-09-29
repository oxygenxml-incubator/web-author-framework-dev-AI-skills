## Implementing a Custom Action

To provide custom functionality to the editor, you can implement a custom action and add it to one of the toolbars, in the contextual menu, or on an oxy_button form control.

## Implementing the action

Suppose you want an action that converts a piece of XML content to a web link in DITA. The action will have to extend the [sync.actions.AbstractAction](sync.actions.AbstractAction.md) class. Here is a sample implementation:

```
  /**
   * The action that shows a popup and then inserts the text in the pop-up.
   */
  class WebLinkAction extends sync.actions.AbstractAction {
    /**
     * @type {sync.api.Editor} editor The editor object.
     * */
    constructor(editor) {
      // shortcut is Meta+L on Mac and Ctrl+L on other platforms.
      super(editor, 'M1 L');
      this.editor = editor;
    }

    /** @override */
    getDisplayName() {
      return 'Convert to Web Link';
    }

    /** @override */
    isEnabled() {
      // The action is enabled only if there is some content selected.
      return !this.editor.getSelectionManager().getSelection().isEmpty();
    }

    /** @override */
    actionPerformed(callback) {
      var text = window.prompt("Please enter the link attribute");
      if (text) {
        this.editor.getActionsManager().invokeOperation(
          'ro.sync.ecss.extensions.commons.operations.SurroundWithFragmentOperation', {
            fragment: '&lt;' + 'xref href="' + text + '"/&gt;'
          }, callback);
      } else {
        callback && callback();
      }
    }
  }

```

The action needs to be registered with the editor. This should be done before the editor is loaded so that the shortcut starts working immediately:

```
    workspace.listen(sync.api.Workspace.EventType.BEFORE_EDITOR_LOADED, function(e) {
      var editor = e.editor;
      // Register the newly created action.
      editor.getActionsManager().registerAction('insert.link', new WebLinkAction(editor));

      addToDitaToolbar(editor, 'insert.link');
      // or
      addToDitaToolbarDropdown(editor, 'insert.link');

      addToContextMenu(editor, 'insert.link');
    });

    workspace.listen(sync.api.Workspace.EventType.EDITOR_LOADED, function(e) {
      var editor = e.editor;

      // Refresh the action enabled/disabled status when the selection changes.
      editor.getSelectionManager().listen(
          sync.api.SelectionManager.EventType.SELECTION_CHANGED, function() {
        editor.getActionsManager().refreshActionsStatus('insert.link')
      });
    });

```

## Adding the Action in the Editor User Interface

Suppose that you want to add the action on the DITA toolbar. To this end, you need to wait for the toolbar to be loaded and append the action to it:

```
    function addToDitaToolbar(editor, actionId) {
      editor.listen(sync.api.Editor.EventTypes.ACTIONS_LOADED, function(e) {
        var actionsConfig = e.actionsConfiguration;

        var ditaToolbar = null;
        if (actionsConfig.toolbars) {
          for (var i = 0; i &lt; actionsConfig.toolbars.length; i++) {
            var toolbar = actionsConfig.toolbars[i];
            if (toolbar.name === "DITA") {
              ditaToolbar = toolbar;
            }
          }
        }

        if (ditaToolbar) {
          ditaToolbar.children.push({
            id: actionId,
            type: "action"
          });
        }
      });
    }

```

If you want to add the action on the DITA toolbar, in a dropdown, you can create a toolbar dropdown list descriptor like this:

```
    function addToDitaToolbarDropdown(editor, actionId) {
      editor.listen(sync.api.Editor.EventTypes.ACTIONS_LOADED, function(e) {
        var actionsConfig = e.actionsConfiguration;

        var ditaToolbar = null;
        if (actionsConfig.toolbars) {
          for (var i = 0; i &lt; actionsConfig.toolbars.length; i++) {
            var toolbar = actionsConfig.toolbars[i];
            if (toolbar.name === "DITA") {
              ditaToolbar = toolbar;
            }
          }
        }

        if (ditaToolbar) {
          ditaToolbar.children.push({
            type: 'list', // type: list means this is a dropdown, all of its children will be shown when it is expanded
            name: 'Dropdown', // If no iconDom is provided the dropdown will display this name.
            iconDom: document.createElement('div'), // A DOM element that can be styled as needed.
            children: [{id: actionId, type: "action" }] // a list of action descriptors
          });
        }
      });
    }

```

To also add the action in the contextual menu, a similar procedure is used:

```
    function addToContextMenu(editor, actionId) {
      editor.listen(sync.api.Editor.EventTypes.ACTIONS_LOADED, function(e) {
        var contextualItems = e.actionsConfiguration.contextualItems;
        if (contextualItems) {
          contextualItems.push({
            id: actionId,
            type: "action"
          });
        }
      });
    }

```

To add the action on an `oxy_button` form control, one needs to make sure that the action is registered before te form controls are rendered. Otherwise, the button label is set to **Unknown** There are two approaches:

1. Register the action on the [sync.api.Workspace.EventType.BEFORE_EDITOR_LOADED](sync.api.Workspace.md#.EventType#.BEFORE_EDITOR_LOADED) event.
2. Define an action stub in the framework configuration with the same ID that defines the name and the icon and overwrite it in JavaScript on the [sync.api.Editor.EventTypes.ACTIONS_LOADED](sync.api.Editor.md#.EventTypes#.ACTIONS_LOADED) event.

The action should now appear in the user interface. To use it:

1. select some text
2. click the action button on the toolbar
3. enter the link target address
4. confirm the prompt

The text should now be converted to a web link.

## More Advanced Use-cases

For a better UX, instead of a native browser `prompt`, you can use a custom JavaScript dialog box. You can find more details in the [Presenting a Dialog to the User](tutorial-dialog.md) tutorial.

If the dialog requires the user to provide a reference to a file, you can invoke `workspace.getUrlChooser()` to obtain a reference to the CMS-specific file chooser.

For the actual document edit usually the `InsertFragmentOperation` or ` SurroundWithFragmentOperation` is enough. If not, you can also have a look at other builtin operations [in the JavaDoc](https://www.oxygenxml.com/InstData/Editor/SDK/javadoc/ro/sync/ecss/extensions/api/AuthorOperation.html) or even implement your own subclass of `AuthorOperation`.

---

Documentation generated by [JSDoc 3.6.11](https://github.com/jsdoc3/jsdoc) using the [DocStrap template](https://github.com/docstrap/docstrap).
