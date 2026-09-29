Package [ro.sync.ecss.extensions.commons.imagemap](package-summary.md)

# Class EditImageMapWithSurroundCore

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.imagemap.EditImageMapCore](EditImageMapCore.md)
        * ro.sync.ecss.extensions.commons.imagemap.EditImageMapWithSurroundCore
   Direct Known Subclasses: [DITAEditImageMapCore](../../dita/DITAEditImageMapCore.md), [DocbookEditImageMapCore](../../docbook/DocbookEditImageMapCore.md), [TEIEditImageMapCore](../../tei/TEIEditImageMapCore.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class EditImageMapWithSurroundCore extends [EditImageMapCore](EditImageMapCore.md)
Core for the frameworks that need to surround the "image" in an "image map".

## Constructor Summary
 Constructors
Constructor

Description
 [EditImageMapWithSurroundCore](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 final [AuthorNode](../../api/node/AuthorNode.md)[] [getNodesOfInterest](#getNodesOfInterest(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,boolean))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorNode](../../api/node/AuthorNode.md) interestNode, boolean doSurroundIfMissing)
Gets the nodes to edit.
  protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getNodesOfInterestCriteria](#getNodesOfInterestCriteria(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Get the criteria for nodes of interest, and the start and end of the fragment to surround with.
  protected boolean [needComplexSurround](#needComplexSurround(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) nodeToEdit)
Check if the edited node need more complex surrounding.

### Methods inherited from class ro.sync.ecss.extensions.commons.imagemap.[EditImageMapCore](EditImageMapCore.md)
 [findNodeOfInterest](EditImageMapCore.md#findNodeOfInterest(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String%5B%5D)), [getFullySelectedNode](EditImageMapCore.md#getFullySelectedNode(ro.sync.ecss.extensions.api.AuthorDocumentController,int,int,boolean)), [getSupportedFramework](EditImageMapCore.md#getSupportedFramework(java.lang.String)), [isNodeOfInterest](EditImageMapCore.md#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### EditImageMapWithSurroundCore

public EditImageMapWithSurroundCore()

## Method Details

### getNodesOfInterest

public final [AuthorNode](../../api/node/AuthorNode.md)[] getNodesOfInterest([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorNode](../../api/node/AuthorNode.md) interestNode, boolean doSurroundIfMissing)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [AuthorOperationException](../../api/AuthorOperationException.md)

Gets the nodes to edit.
  Specified by: [getNodesOfInterest](EditImageMapCore.md#getNodesOfInterest(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,boolean)) in class [EditImageMapCore](EditImageMapCore.md) Parameters: authorAccess - The Author access. interestNode - The node of interest if available when calling the method. If nullit will be determined from the AuthorAccess, from the caret position. doSurroundIfMissing - If true the missing part of the image map will be added. Returns: The nodes to edit. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [AuthorOperationException](../../api/AuthorOperationException.md)
### needComplexSurround

protected boolean needComplexSurround([AuthorNode](../../api/node/AuthorNode.md) nodeToEdit)

Check if the edited node need more complex surrounding.
  Parameters: nodeToEdit - The node to edit. Returns: true if complex surrounding need to be performed.
### getNodesOfInterestCriteria

protected abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getNodesOfInterestCriteria([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)

Get the criteria for nodes of interest, and the start and end of the fragment to surround with.
  Parameters: namespace - The namespace of the document. Returns: A 4 items array with the main property, the secondary property, and the start + end of the fragment to surround with.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
