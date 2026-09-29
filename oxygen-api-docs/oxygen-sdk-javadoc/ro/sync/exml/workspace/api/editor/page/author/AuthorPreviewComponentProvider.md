Package [ro.sync.exml.workspace.api.editor.page.author](package-summary.md)

# Interface AuthorPreviewComponentProvider
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorPreviewComponentProvider
A simple read only Author preview component.
  Since: 27
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorAccess](../../../../../../ecss/extensions/api/AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()
Get the AuthorAccess.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getComponent](#getComponent())()
Get the Swing JPanel to add to the custom application.
  void [load](#load(java.net.URL,java.io.Reader))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)
Load content from an URL or a reader or both.

## Method Details

### load

void load([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Load content from an URL or a reader or both.
  Parameters: url - The system id of the resource. If null, the reader must be provided and relative DTD entity references will not be properly resolved. reader - The document reader. If null, the reader will be created internally. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If any exception occurs during the loading, for example IO exception due to incorrect system id, unsupported encodings, etc.
### getAuthorAccess

[AuthorAccess](../../../../../../ecss/extensions/api/AuthorAccess.md) getAuthorAccess()

Get the AuthorAccess.
  Returns: The AuthorAccess.
### getComponent

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getComponent()

Get the Swing JPanel to add to the custom application.
  Returns: the Swing JPanel to add to the custom application.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
