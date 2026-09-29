Package [ro.sync.ecss.extensions.commons.imagemap](package-summary.md)

# Class EditImageMapCore

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.imagemap.EditImageMapCore
   Direct Known Subclasses: [EditImageMapWithSurroundCore](EditImageMapWithSurroundCore.md), [XHTMLEditImageMapCore](../../xhtml/imagemap/XHTMLEditImageMapCore.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class EditImageMapCore extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Core methods to be used from the operations and from the image map decorators.

## Constructor Summary
 Constructors
Constructor

Description
 [EditImageMapCore](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected final [AuthorNode](../../api/node/AuthorNode.md) [findNodeOfInterest](#findNodeOfInterest(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String%5B%5D))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorNode](../../api/node/AuthorNode.md) interestNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] properties2Check)
Check the current node and its parents for a specified property value.
  protected [AuthorNode](../../api/node/AuthorNode.md) [getFullySelectedNode](#getFullySelectedNode(ro.sync.ecss.extensions.api.AuthorDocumentController,int,int,boolean))([AuthorDocumentController](../../api/AuthorDocumentController.md) ctrl, int selStart, int selEnd, boolean hasSelection)
Get the fully selected node if any.
  abstract [AuthorNode](../../api/node/AuthorNode.md)[] [getNodesOfInterest](#getNodesOfInterest(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,boolean))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorNode](../../api/node/AuthorNode.md) interestNode, boolean doSurroundIfMissing)
Gets the nodes to edit.
  abstract [SupportedFrameworks](../../../imagemap/SupportedFrameworks.md) [getSupportedFramework](#getSupportedFramework(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespaceURI)
Detect the supported framework.
  protected boolean [isNodeOfInterest](#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([AuthorNode](../../api/node/AuthorNode.md) nodeToEdit, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) property2Check)
Check if the node is of interest.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### EditImageMapCore

public EditImageMapCore()

## Method Details

### getFullySelectedNode

protected [AuthorNode](../../api/node/AuthorNode.md) getFullySelectedNode([AuthorDocumentController](../../api/AuthorDocumentController.md) ctrl, int selStart, int selEnd, boolean hasSelection)

Get the fully selected node if any.
  Parameters: ctrl - Author document controller. selStart - Selection start (inclusive). selEnd - Selection end (exclusive). hasSelection - true if has selection. Returns: The fully selected node, if any.
### findNodeOfInterest

protected final [AuthorNode](../../api/node/AuthorNode.md) findNodeOfInterest([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorNode](../../api/node/AuthorNode.md) interestNode, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] properties2Check)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Check the current node and its parents for a specified property value. It might be the node name, an attribute value, etc.
  Parameters: authorAccess - The author access. interestNode - The node of interest if available when calling the method. If nullit will be determined from the AuthorAccess, from the caret position. properties2Check - The properties to check. Returns: The identified node if any. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### isNodeOfInterest

protected boolean isNodeOfInterest([AuthorNode](../../api/node/AuthorNode.md) nodeToEdit, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) property2Check)

Check if the node is of interest.
  Parameters: nodeToEdit - The node to edit candidate. property2Check - The property value to check. Returns: true if the node is eligible, false otherwise.
### getNodesOfInterest

public abstract [AuthorNode](../../api/node/AuthorNode.md)[] getNodesOfInterest([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorNode](../../api/node/AuthorNode.md) interestNode, boolean doSurroundIfMissing)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [AuthorOperationException](../../api/AuthorOperationException.md)

Gets the nodes to edit.
  Parameters: authorAccess - The Author access. interestNode - The node of interest if available when calling the method. If nullit will be determined from the AuthorAccess, from the caret position. doSurroundIfMissing - If true the missing part of the image map will be added. Returns: The nodes to edit. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [AuthorOperationException](../../api/AuthorOperationException.md)
### getSupportedFramework

public abstract [SupportedFrameworks](../../../imagemap/SupportedFrameworks.md) getSupportedFramework([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespaceURI)

Detect the supported framework.
  Parameters: namespaceURI - The namespace uri of the element. Returns: The supported framework.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
