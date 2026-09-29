Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorClipboardAccess
    All Known Subinterfaces: [AuthorAccess](AuthorAccess.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorClipboardAccess
Access to various content data in the system clipboard.
  Since: 25.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 ro.sync.ecss.component.AuthorClipboardObject [getAuthorObjectFromClipboard](#getAuthorObjectFromClipboard())()
Get the author object previously copied in the clipboard.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTextFromClipboard](#getTextFromClipboard())()
Gets the text from the clipboard.

## Method Details

### getAuthorObjectFromClipboard

ro.sync.ecss.component.AuthorClipboardObject getAuthorObjectFromClipboard()

Get the author object previously copied in the clipboard.  Not implemented for the *WebAuthor* distribution.
  Returns: The author object from the clipboard or null if no such object exists. Since: 17.1
### getTextFromClipboard

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTextFromClipboard()

Gets the text from the clipboard.  Not implemented for the *WebAuthor* distribution.
  Returns: The text from the clipboard or null if no such object exists. Since: 25.0
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
