Package [ro.sync.ecss.extensions.api.access](package-summary.md)

# Interface AuthorOutlineAccess
    All Superinterfaces: [WSOutline](../../../../exml/workspace/api/editor/page/WSOutline.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorOutlineAccessextends [WSOutline](../../../../exml/workspace/api/editor/page/WSOutline.md)
Author Outline access.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [refreshNodes](#refreshNodes(ro.sync.ecss.extensions.api.node.AuthorNode%5B%5D))([AuthorNode](../node/AuthorNode.md)[] nodes)
The Outline usually automatically updates the nodes based on the document changes.

### Methods inherited from interface ro.sync.exml.workspace.api.editor.page.[WSOutline](../../../../exml/workspace/api/editor/page/WSOutline.md)
 [getSelectedPaths](../../../../exml/workspace/api/editor/page/WSOutline.md#getSelectedPaths(boolean)), [setSelectionPaths](../../../../exml/workspace/api/editor/page/WSOutline.md#setSelectionPaths(javax.swing.tree.TreePath%5B%5D))
## Method Details

### refreshNodes

void refreshNodes([AuthorNode](../node/AuthorNode.md)[] nodes)

The Outline usually automatically updates the nodes based on the document changes. If the developer sets an AuthorOutlineCustomizer or an AuthorBreadCrumbCustomizer which uses as render text for a node the information available in another node, if the second node changes, the Outline/Bread Crumb components do not know what other nodes to update. Example: If the developer renders for a <chapter> the gathered text from the <title> child nodes then he will have to add a document listener and when a <title> node's text changes update the parent <chapter>.
  Parameters: nodes - The nodes to Refresh in the outline/bread crumb
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
