Package [ro.sync.exml.workspace.api.base](package-summary.md)

# Interface ModifiedStatusProvider
    All Known Subinterfaces: [AuthorEditorAccess](../../../../ecss/extensions/api/access/AuthorEditorAccess.md), [IWebappAuthorEditorAccess](../../../../ecss/extensions/api/webapp/access/IWebappAuthorEditorAccess.md), [WSEditor](../editor/WSEditor.md), [WSEditorBase](../editor/WSEditorBase.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ModifiedStatusProvider
Provides access to the modified status of an object.
  Since: 18.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [isModified](#isModified())()
Call this method to determine the status of this object.

## Method Details

### isModified

boolean isModified()

Call this method to determine the status of this object.
  Returns: true if this object contains modifications.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
