Package [ro.sync.exml.workspace.api.editor.page.text](package-summary.md)

# Interface IExternalContentCompletionContext
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface IExternalContentCompletionContext
Contains context information about the position where the content completion is invoked.
  Since: 22.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 int [getPosition](#getPosition())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSkippedText](#getSkippedText())()

## Method Details

### getPosition

int getPosition()
  Returns: The position to start the content completion, represents an offset in the document.
### getSkippedText

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSkippedText()
  Returns: The text to be skipped/overwritten by the content completion item insertion. Can be null in case no text should be overwritten.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
