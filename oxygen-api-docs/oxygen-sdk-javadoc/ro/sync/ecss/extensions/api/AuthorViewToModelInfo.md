Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorViewToModelInfo
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorViewToModelInfo
An implementation of this interface is returned by the [WSAuthorEditorPageBase.viewToModel(int, int)](../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#viewToModel(int,int))method. Used to obtain the node whose graphic representation contains a certain point in the Author viewport.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorNode](node/AuthorNode.md) [getAuthorNode](#getAuthorNode())()
Return the [AuthorNode](node/AuthorNode.md) located at a specified position.
  int [getOffset](#getOffset())()
The offset of the specified position.

## Method Details

### getOffset

int getOffset()

The offset of the specified position. It is located within the bounds of the determined [AuthorNode](node/AuthorNode.md)which also contains the given position.
  Returns: The offset of the specified position.
### getAuthorNode

[AuthorNode](node/AuthorNode.md) getAuthorNode()

Return the [AuthorNode](node/AuthorNode.md) located at a specified position.
  Returns: The author node.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
