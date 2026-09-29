Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Interface WebappAuthorSchemaAwareActionsHandler
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WebappAuthorSchemaAwareActionsHandler
Handles schema aware actions like paste.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [delete](#delete(boolean,boolean))(boolean del, boolean wordLevel)
Deletes the the current selection using information from the schema associated to the document such that document is left in a valid state.
  ro.sync.ecss.component.AuthorClipboardObject [handleCopy](#handleCopy())()
Copy from offset to offset inclusive.
  ro.sync.ecss.component.AuthorClipboardObject [handleCopyAsMarkdown](#handleCopyAsMarkdown())()
Copy from the current selection as markdown text only.
  ro.sync.ecss.component.AuthorClipboardObject [handleCut](#handleCut())()
Cuts from offset to offset inclusive.
  void [handleDragAndDrop](#handleDragAndDrop(int,boolean))(int targetOffset, boolean doCut)
Drag and drop selection to the given location.
  void [handleDragAndDrop](#handleDragAndDrop(int,int,int))(int start, int end, int target)
Drag and drop from offset to offset inclusive.
  void [handleHtmlPaste](#handleHtmlPaste(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) html)
Handles a paste with an HTML content from an external source.
  void [handlePaste](#handlePaste(ro.sync.ecss.component.AuthorClipboardObject,boolean,boolean))(ro.sync.ecss.component.AuthorClipboardObject toPaste, boolean removeSelection, boolean pasteAsXml)
Paste a fragment.
  void [handleTextPaste](#handleTextPaste(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text)
Handles a paste with a text content.
  void [handleXmlPaste](#handleXmlPaste(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xml)
Handles a paste with an XML content.
  void [insertCharAtCurrentOffset](#insertCharAtCurrentOffset(char))(char ch)
Inserts the given character at the current caret position.
  void [insertCodePointAtCurrentOffset](#insertCodePointAtCurrentOffset(int))(int codePoint)
Inserts the given Unicode code point at the current caret position.

## Method Details

### handleHtmlPaste

void handleHtmlPaste([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) html)throws [InvalidEditException](../InvalidEditException.md)

Handles a paste with an HTML content from an external source.
  Parameters: html - The HTML content. Throws: [InvalidEditException](../InvalidEditException.md) - If the paste could not be performed.
### handleXmlPaste

void handleXmlPaste([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xml)throws [InvalidEditException](../InvalidEditException.md)

Handles a paste with an XML content.
  Parameters: xml - the XML content. Throws: [InvalidEditException](../InvalidEditException.md) - If the paste could not be performed.
### handleTextPaste

void handleTextPaste([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text)throws [InvalidEditException](../InvalidEditException.md)

Handles a paste with a text content.
  Parameters: text - the text content. Throws: [InvalidEditException](../InvalidEditException.md) - If the paste could not be performed.
### handlePaste

void handlePaste(ro.sync.ecss.component.AuthorClipboardObject toPaste, boolean removeSelection, boolean pasteAsXml)throws [InvalidEditException](../InvalidEditException.md)

Paste a fragment.
  Parameters: toPaste - The fragment to paste removeSelection - Remove the selection pasteAsXml - If true treat the pasted text as an xml fragment. Else escape it and insert it. Throws: [InvalidEditException](../InvalidEditException.md) - When paste was rejected.
### handleCopy

ro.sync.ecss.component.AuthorClipboardObject handleCopy() throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Copy from offset to offset inclusive.
  Returns: The doc fragment with the copy text. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### handleCut

ro.sync.ecss.component.AuthorClipboardObject handleCut() throws [InvalidEditException](../InvalidEditException.md)

Cuts from offset to offset inclusive.
  Returns: The doc fragment with the cut text. Throws: [InvalidEditException](../InvalidEditException.md)
### handleCopyAsMarkdown

ro.sync.ecss.component.AuthorClipboardObject handleCopyAsMarkdown() throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Copy from the current selection as markdown text only.
  Returns: The markdown text representation of the copied selection content. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) Since: 28
### insertCharAtCurrentOffset

void insertCharAtCurrentOffset(char ch)

Inserts the given character at the current caret position. Any selected content is first deleted.
  Parameters: ch - The character to insert.
### insertCodePointAtCurrentOffset

void insertCodePointAtCurrentOffset(int codePoint)

Inserts the given Unicode code point at the current caret position. Any selected content is first deleted.
  Parameters: codePoint - The code point to insert. Since: 26.1
### delete

void delete(boolean del, boolean wordLevel)throws [InvalidEditException](../InvalidEditException.md)

Deletes the the current selection using information from the schema associated to the document such that document is left in a valid state.
  Parameters: del - true if the deletion was triggered by a DEL. wordLevel - Whether we should delete an entire word. Throws: [InvalidEditException](../InvalidEditException.md) - If the edit fails.
### handleDragAndDrop

void handleDragAndDrop(int start, int end, int target)throws [InvalidEditException](../InvalidEditException.md), [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Drag and drop from offset to offset inclusive.
  Parameters: start - The start offset of the dragged fragment. end - The end offset of the dragged fragment. target - The location where the fragment is dropped. Throws: [InvalidEditException](../InvalidEditException.md) - If the edit fails. [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If the target is in a bad location. Since: 21.1.1
### handleDragAndDrop

void handleDragAndDrop(int targetOffset, boolean doCut)throws [InvalidEditException](../InvalidEditException.md), [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Drag and drop selection to the given location.
  Parameters: targetOffset - The location where the fragment is dropped. doCut - True to cut, otherwise copy. Throws: [InvalidEditException](../InvalidEditException.md) - If the edit fails. [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If the target is in a bad location. Since: 26.1.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
