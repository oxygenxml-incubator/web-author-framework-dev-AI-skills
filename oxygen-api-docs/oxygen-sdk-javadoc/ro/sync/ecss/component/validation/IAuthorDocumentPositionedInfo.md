Package [ro.sync.ecss.component.validation](package-summary.md)

# Interface IAuthorDocumentPositionedInfo
    All Known Implementing Classes: [AuthorDocumentPositionedInfo](AuthorDocumentPositionedInfo.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface IAuthorDocumentPositionedInfo
Interface defining the Author Mode document positioned info: allows you to specify the problem AuthorNode.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final ro.sync.document.DPIData [CONTENT_DATA](#CONTENT_DATA)
Marks in the DPI that the offset is from the Author content

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorNode](../../extensions/api/node/AuthorNode.md) [getNode](#getNode())()

 boolean [isSelectEntireNode](#isSelectEntireNode())()
Checks if the entire node should be selected.

## Field Details

### CONTENT_DATA

static final ro.sync.document.DPIData CONTENT_DATA

Marks in the DPI that the offset is from the Author content

## Method Details

### getNode

[AuthorNode](../../extensions/api/node/AuthorNode.md) getNode()
  Returns: The node to locate the message.
### isSelectEntireNode

boolean isSelectEntireNode()

Checks if the entire node should be selected.
  Returns: true if the entire node should be selected.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
