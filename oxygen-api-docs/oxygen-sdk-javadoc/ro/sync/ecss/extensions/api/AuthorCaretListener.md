Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorCaretListener
    @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorCaretListener
Listener for changes in the caret position of the Author editor page. Adding a caret listener starting from an [AuthorAccess](AuthorAccess.md) :
```

 authorAccess.getEditorAccess().addAuthorCaretListener(caretListener);

```
Adding a caret listener starting from a [PluginWorkspace](../../../exml/workspace/api/PluginWorkspace.md) :
```

 WSEditor editorAccess = pluginWorkspaceAccess.getCurrentEditorAccess(StandalonePluginWorkspace.MAIN_EDITING_AREA);
 if (editorAccess != null && EditorPageConstants.PAGE_AUTHOR.equals(editorAccess.getCurrentPageID())) {
     WSAuthorEditorPage authorPageAccess = (WSAuthorEditorPage) editorAccess.getCurrentPage();
     authorPageAccess.addAuthorCaretListener(caretListener);
  }

```

  See Also:
* [WSAuthorEditorPageBase](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md)
* [AuthorAccess](AuthorAccess.md)
* [PluginWorkspace](../../../exml/workspace/api/PluginWorkspace.md)

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [caretMoved](#caretMoved(ro.sync.ecss.extensions.api.AuthorCaretEvent))([AuthorCaretEvent](AuthorCaretEvent.md) caretEvent)
Called when the caret position is updated.

## Method Details

### caretMoved

void caretMoved([AuthorCaretEvent](AuthorCaretEvent.md) caretEvent)

Called when the caret position is updated.
  Parameters: caretEvent - The [AuthorCaretEvent](AuthorCaretEvent.md) containing information about the offset and the author node holding the offset.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
