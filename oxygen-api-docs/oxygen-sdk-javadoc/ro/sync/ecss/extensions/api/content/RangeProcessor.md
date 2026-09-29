Package [ro.sync.ecss.extensions.api.content](package-summary.md)

# Interface RangeProcessor
    @API(type=EXTENDABLE, src=PUBLIC) public interface RangeProcessor
Used to receive call backs when processing a range from the document.
  Since: 12.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [processRange](#processRange(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment))([AuthorDocumentFragment](../node/AuthorDocumentFragment.md) fragment)
Called from the AuthorDocumentController to process a fragment which was created from a specific range.

## Method Details

### processRange

void processRange([AuthorDocumentFragment](../node/AuthorDocumentFragment.md) fragment)throws [AuthorOperationException](../AuthorOperationException.md), [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Called from the AuthorDocumentController to process a fragment which was created from a specific range.
  Parameters: fragment - The fragment which was created from a specific range. It will be merged back in the document. Throws: [AuthorOperationException](../AuthorOperationException.md) [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
