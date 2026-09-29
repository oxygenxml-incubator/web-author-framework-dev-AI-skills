Package [ro.sync.exml.workspace.api.editor.page](package-summary.md)

# Interface WSEditorPage
    All Known Subinterfaces: [AuthorEditorAccess](../../../../../ecss/extensions/api/access/AuthorEditorAccess.md), [IWebappAuthorEditorAccess](../../../../../ecss/extensions/api/webapp/access/IWebappAuthorEditorAccess.md), [WSAuthorComponentEditorPage](author/WSAuthorComponentEditorPage.md), [WSAuthorEditorPage](author/WSAuthorEditorPage.md), [WSAuthorEditorPageBase](author/WSAuthorEditorPageBase.md), [WSDesignEditorPage](design/WSDesignEditorPage.md), [WSDITAMapEditorPage](ditamap/WSDITAMapEditorPage.md), [WSGridEditorPage](grid/WSGridEditorPage.md), [WSTextBasedEditorPage](WSTextBasedEditorPage.md), [WSTextEditorPage](text/WSTextEditorPage.md), [WSXMLTextEditorPage](text/xml/WSXMLTextEditorPage.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WSEditorPage
Access to an editor's page.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [WSEditor](../WSEditor.md) [getParentEditor](#getParentEditor())()
Get the parent editor access.
  boolean [hasFocus](#hasFocus())()
Check if the page has focus
  boolean [isEditable](#isEditable())()
Check if the document can be edited.
  void [requestFocus](#requestFocus())()
Request focus in the current page.
  void [setEditable](#setEditable(boolean))(boolean editable)
Sets the specified flag to indicate whether or not this page should be editable.
  void [setReadOnly](#setReadOnly(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reason)
Sets the document as read-only.
  void [setReadOnly](#setReadOnly(ro.sync.exml.workspace.api.editor.ReadOnlyReason))([ReadOnlyReason](../ReadOnlyReason.md) reason)
Sets the document as read-only.

## Method Details

### setReadOnly

void setReadOnly([ReadOnlyReason](../ReadOnlyReason.md) reason)

Sets the document as read-only.
  Parameters: reason - The reason for making the document read-only. If null is passed, a default message will be displayed. Since: 19.1
### setReadOnly

void setReadOnly([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) reason)

Sets the document as read-only.
  Parameters: reason - The reason for making the document read-only. It will be displayed to the user. If null is passed, a default message will be displayed. Since: 18.0
### setEditable

void setEditable(boolean editable)

Sets the specified flag to indicate whether or not this page should be editable. It is recommended to use [setReadOnly(String)](#setReadOnly(java.lang.String)) if you plan to make the page read-only.
  Parameters: editable - true if the page should be editable. Since: 12.2
### isEditable

boolean isEditable()

Check if the document can be edited. A document can be set as read-only from API, by using the [setEditable(boolean)](#setEditable(boolean)) method.
  Returns: true if the document is editable. Since: 14.1
### getParentEditor

[WSEditor](../WSEditor.md) getParentEditor()

Get the parent editor access.
  Returns: The parent editor access. Since: 18
### requestFocus

void requestFocus()

Request focus in the current page. Works for all editing modes (Text/Grid/Author) in the standalone and Eclipse-based Oxygen and Author Component distributions. Does not do anything in the WebAuthor online editor.
  Since: 21
### hasFocus

boolean hasFocus()

Check if the page has focus
  Returns: true if focus is inside the page's main editing component. Since: 23
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
