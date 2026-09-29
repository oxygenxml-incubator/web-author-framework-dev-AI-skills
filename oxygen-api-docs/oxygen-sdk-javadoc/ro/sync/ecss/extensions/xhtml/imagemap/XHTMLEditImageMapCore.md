Package [ro.sync.ecss.extensions.xhtml.imagemap](package-summary.md)

# Class XHTMLEditImageMapCore

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.imagemap.EditImageMapCore](../../commons/imagemap/EditImageMapCore.md)
        * ro.sync.ecss.extensions.xhtml.imagemap.XHTMLEditImageMapCore
   @API(type=INTERNAL, src=PUBLIC) public class XHTMLEditImageMapCore extends [EditImageMapCore](../../commons/imagemap/EditImageMapCore.md)
Edit map core for XHTML.

## Constructor Summary
 Constructors
Constructor

Description
 [XHTMLEditImageMapCore](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorNode](../../api/node/AuthorNode.md)[] [getNodesOfInterest](#getNodesOfInterest(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,boolean))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorNode](../../api/node/AuthorNode.md) interestNode, boolean doSurroundIfMissing)
Gets the nodes to edit.
  [SupportedFrameworks](../../../imagemap/SupportedFrameworks.md) [getSupportedFramework](#getSupportedFramework(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespaceURI)
Detect the supported framework.

### Methods inherited from class ro.sync.ecss.extensions.commons.imagemap.[EditImageMapCore](../../commons/imagemap/EditImageMapCore.md)
 [findNodeOfInterest](../../commons/imagemap/EditImageMapCore.md#findNodeOfInterest(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String%5B%5D)), [getFullySelectedNode](../../commons/imagemap/EditImageMapCore.md#getFullySelectedNode(ro.sync.ecss.extensions.api.AuthorDocumentController,int,int,boolean)), [isNodeOfInterest](../../commons/imagemap/EditImageMapCore.md#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XHTMLEditImageMapCore

public XHTMLEditImageMapCore()

## Method Details

### getNodesOfInterest

public [AuthorNode](../../api/node/AuthorNode.md)[] getNodesOfInterest([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorNode](../../api/node/AuthorNode.md) interestNode, boolean doSurroundIfMissing)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [AuthorOperationException](../../api/AuthorOperationException.md)

Gets the nodes to edit.
  Specified by: [getNodesOfInterest](../../commons/imagemap/EditImageMapCore.md#getNodesOfInterest(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,boolean)) in class [EditImageMapCore](../../commons/imagemap/EditImageMapCore.md) Parameters: authorAccess - The Author access. interestNode - The node of interest if available when calling the method. If nullit will be determined from the AuthorAccess, from the caret position. doSurroundIfMissing - If true the missing part of the image map will be added. Returns: The nodes to edit. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [AuthorOperationException](../../api/AuthorOperationException.md)
### getSupportedFramework

public [SupportedFrameworks](../../../imagemap/SupportedFrameworks.md) getSupportedFramework([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespaceURI)
 Description copied from class: [EditImageMapCore](../../commons/imagemap/EditImageMapCore.md#getSupportedFramework(java.lang.String))
Detect the supported framework.
  Specified by: [getSupportedFramework](../../commons/imagemap/EditImageMapCore.md#getSupportedFramework(java.lang.String)) in class [EditImageMapCore](../../commons/imagemap/EditImageMapCore.md) Parameters: namespaceURI - The namespace uri of the element. Returns: The supported framework. See Also:
        * [EditImageMapCore.getSupportedFramework(java.lang.String)](../../commons/imagemap/EditImageMapCore.md#getSupportedFramework(java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
