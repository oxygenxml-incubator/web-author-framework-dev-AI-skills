Package [ro.sync.exml.workspace.api.editor.page](package-summary.md)

# Interface WSOutline
    All Known Subinterfaces: [AuthorOutlineAccess](../../../../../ecss/extensions/api/access/AuthorOutlineAccess.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WSOutline
The Workspace Outline.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [TreePath](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/tree/TreePath.html)[] [getSelectedPaths](#getSelectedPaths(boolean))(boolean minimizeSelectedPaths)
Get the tree paths selected in the Outline tree.
  void [setSelectionPaths](#setSelectionPaths(javax.swing.tree.TreePath%5B%5D))([TreePath](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/tree/TreePath.html)[] treePath)
Select and scroll the given tree paths.

## Method Details

### getSelectedPaths

[TreePath](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/tree/TreePath.html)[] getSelectedPaths(boolean minimizeSelectedPaths)

Get the tree paths selected in the Outline tree. The tree path contain arrays of AuthorNodes starting from the AuthorDocument and ending in the selected leaf node. The bread crumb displays the path to the last node selected in the Outline.
  Parameters: minimizeSelectedPaths - If true and a parent and a child is selected, then only the parent is the list. Returns: The nodes selected in the Outline tree
### setSelectionPaths

void setSelectionPaths([TreePath](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/tree/TreePath.html)[] treePath)

Select and scroll the given tree paths.
  Parameters: treePath - The path to select.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
