Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DITAEditImageMapCore

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.imagemap.EditImageMapCore](../commons/imagemap/EditImageMapCore.md)
        * [ro.sync.ecss.extensions.commons.imagemap.EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md)
            * ro.sync.ecss.extensions.dita.DITAEditImageMapCore
   @API(type=INTERNAL, src=PUBLIC) public class DITAEditImageMapCore extends [EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md)
Edit Image Map Core for DITA.

## Constructor Summary
 Constructors
Constructor

Description
 [DITAEditImageMapCore](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getNodesOfInterestCriteria](#getNodesOfInterestCriteria(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Get the criteria for nodes of interest, and the start and end of the fragment to surround with.
  [SupportedFrameworks](../../imagemap/SupportedFrameworks.md) [getSupportedFramework](#getSupportedFramework(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespaceURI)
Detect the supported framework.
  protected boolean [isNodeOfInterest](#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([AuthorNode](../api/node/AuthorNode.md) nodeToEdit, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) property2Check)
Check if the node is of interest.
  protected boolean [needComplexSurround](#needComplexSurround(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) nodeToEdit)
Check if the edited node need more complex surrounding.

### Methods inherited from class ro.sync.ecss.extensions.commons.imagemap.[EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md)
 [getNodesOfInterest](../commons/imagemap/EditImageMapWithSurroundCore.md#getNodesOfInterest(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,boolean))
### Methods inherited from class ro.sync.ecss.extensions.commons.imagemap.[EditImageMapCore](../commons/imagemap/EditImageMapCore.md)
 [findNodeOfInterest](../commons/imagemap/EditImageMapCore.md#findNodeOfInterest(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String%5B%5D)), [getFullySelectedNode](../commons/imagemap/EditImageMapCore.md#getFullySelectedNode(ro.sync.ecss.extensions.api.AuthorDocumentController,int,int,boolean))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAEditImageMapCore

public DITAEditImageMapCore()

## Method Details

### getSupportedFramework

public [SupportedFrameworks](../../imagemap/SupportedFrameworks.md) getSupportedFramework([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespaceURI)
 Description copied from class: [EditImageMapCore](../commons/imagemap/EditImageMapCore.md#getSupportedFramework(java.lang.String))
Detect the supported framework.
  Specified by: [getSupportedFramework](../commons/imagemap/EditImageMapCore.md#getSupportedFramework(java.lang.String)) in class [EditImageMapCore](../commons/imagemap/EditImageMapCore.md) Parameters: namespaceURI - The namespace uri of the element. Returns: The supported framework. See Also:
        * [EditImageMapCore.getSupportedFramework(java.lang.String)](../commons/imagemap/EditImageMapCore.md#getSupportedFramework(java.lang.String))

### getNodesOfInterestCriteria

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getNodesOfInterestCriteria([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
 Description copied from class: [EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md#getNodesOfInterestCriteria(java.lang.String))
Get the criteria for nodes of interest, and the start and end of the fragment to surround with.
  Specified by: [getNodesOfInterestCriteria](../commons/imagemap/EditImageMapWithSurroundCore.md#getNodesOfInterestCriteria(java.lang.String)) in class [EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md) Parameters: namespace - The namespace of the document. Returns: A 4 items array with the main property, the secondary property, and the start + end of the fragment to surround with. See Also:
        * [EditImageMapWithSurroundCore.getNodesOfInterestCriteria(java.lang.String)](../commons/imagemap/EditImageMapWithSurroundCore.md#getNodesOfInterestCriteria(java.lang.String))

### needComplexSurround

protected boolean needComplexSurround([AuthorNode](../api/node/AuthorNode.md) nodeToEdit)
 Description copied from class: [EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md#needComplexSurround(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if the edited node need more complex surrounding.
  Overrides: [needComplexSurround](../commons/imagemap/EditImageMapWithSurroundCore.md#needComplexSurround(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md) Parameters: nodeToEdit - The node to edit. Returns: true if complex surrounding need to be performed. See Also:
        * [EditImageMapWithSurroundCore.needComplexSurround(ro.sync.ecss.extensions.api.node.AuthorNode)](../commons/imagemap/EditImageMapWithSurroundCore.md#needComplexSurround(ro.sync.ecss.extensions.api.node.AuthorNode))

### isNodeOfInterest

protected boolean isNodeOfInterest([AuthorNode](../api/node/AuthorNode.md) nodeToEdit, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) property2Check)
 Description copied from class: [EditImageMapCore](../commons/imagemap/EditImageMapCore.md#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))
Check if the node is of interest.
  Overrides: [isNodeOfInterest](../commons/imagemap/EditImageMapCore.md#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)) in class [EditImageMapCore](../commons/imagemap/EditImageMapCore.md) Parameters: nodeToEdit - The node to edit candidate. property2Check - The property value to check. Returns: true if the node is eligible, false otherwise. See Also:
        * [EditImageMapCore.isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode, java.lang.String)](../commons/imagemap/EditImageMapCore.md#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
