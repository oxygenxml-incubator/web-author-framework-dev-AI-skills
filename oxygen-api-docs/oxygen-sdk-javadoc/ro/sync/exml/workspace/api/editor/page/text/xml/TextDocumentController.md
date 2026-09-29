Package [ro.sync.exml.workspace.api.editor.page.text.xml](package-summary.md)

# Interface TextDocumentController
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface TextDocumentController
Contains API for inserting XML content in certain places in the Text editing mode.
  Since: 16.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [indentSection](#indentSection(int,int))(int startOffset, int endOffset)
Indents the give section of the document.
  void [insertXMLFragment](#insertXMLFragment(java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int caretOffset)
Insert an XML fragment at the caret location with indent.
  void [insertXMLFragment](#insertXMLFragment(java.lang.String,java.lang.String,ro.sync.exml.editor.xmleditor.operations.context.RelativeInsertPosition))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [RelativeInsertPosition](../../../../../../editor/xmleditor/operations/context/RelativeInsertPosition.md) relativePosition)
Insert an XML fragment relative to the node identified by the xpathLocation and according with the relativePosition.

## Method Details

### insertXMLFragment

void insertXMLFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathLocation, [RelativeInsertPosition](../../../../../../editor/xmleditor/operations/context/RelativeInsertPosition.md) relativePosition)throws [TextOperationException](TextOperationException.md)

Insert an XML fragment relative to the node identified by the xpathLocation and according with the relativePosition. The inserted fragment is indented after being added to the document.
After the operation the caret will be positioned in the first leaf of the fragment.

  Parameters: xmlFragment - The XML fragment. xpathLocation - The XPath location. relativePosition - The position relative to the node identified by the XPath location. Can be one of the constants: [AuthorConstants.POSITION_BEFORE](../../../../../../../ecss/extensions/api/AuthorConstants.md#POSITION_BEFORE), [AuthorConstants.POSITION_AFTER](../../../../../../../ecss/extensions/api/AuthorConstants.md#POSITION_AFTER), [AuthorConstants.POSITION_INSIDE_FIRST](../../../../../../../ecss/extensions/api/AuthorConstants.md#POSITION_INSIDE_FIRST) or [AuthorConstants.POSITION_INSIDE_LAST](../../../../../../../ecss/extensions/api/AuthorConstants.md#POSITION_INSIDE_LAST). Throws: [TextOperationException](TextOperationException.md) - Unable to insert the fragment.
### insertXMLFragment

void insertXMLFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int caretOffset)throws [TextOperationException](TextOperationException.md)

Insert an XML fragment at the caret location with indent. When the caret offset is inside an element tag (start element, empty element or end element) tries to place the caret inside the element's contents. If the element is empty, it tries to expand the element (eg: from <a/> to <a></a>) placing the caret between the tags. After insertion is done, the caret is placed after the inserted element.
  Parameters: xmlFragment - The XML fragment. caretOffset - The caret offset Throws: [TextOperationException](TextOperationException.md) - Unable to insert the fragment. Since: 21.0
### indentSection

void indentSection(int startOffset, int endOffset)throws [TextOperationException](TextOperationException.md)

Indents the give section of the document. Indents each line from the section according to the XML structure.
  Parameters: startOffset - The start offset of the section. endOffset - The end offset of the section. Inclusive. Throws: [TextOperationException](TextOperationException.md) - Unable to indent the section. Since: 28.0  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
