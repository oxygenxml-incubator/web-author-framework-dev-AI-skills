Package [ro.sync.ecss.extensions.tei](package-summary.md)

# Class TEIEditImageMapCore

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.imagemap.EditImageMapCore](../commons/imagemap/EditImageMapCore.md)
        * [ro.sync.ecss.extensions.commons.imagemap.EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md)
            * ro.sync.ecss.extensions.tei.TEIEditImageMapCore
   @API(type=INTERNAL, src=PUBLIC) public class TEIEditImageMapCore extends [EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md)
Edit Image Map Core for TEI.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TEI_NS](#TEI_NS)
TEI namespace.

## Constructor Summary
 Constructors
Constructor

Description
 [TEIEditImageMapCore](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getNodesOfInterestCriteria](#getNodesOfInterestCriteria(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Get the criteria for nodes of interest, and the start and end of the fragment to surround with.
  [SupportedFrameworks](../../imagemap/SupportedFrameworks.md) [getSupportedFramework](#getSupportedFramework(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespaceURI)
Detect the supported framework.

### Methods inherited from class ro.sync.ecss.extensions.commons.imagemap.[EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md)
 [getNodesOfInterest](../commons/imagemap/EditImageMapWithSurroundCore.md#getNodesOfInterest(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,boolean)), [needComplexSurround](../commons/imagemap/EditImageMapWithSurroundCore.md#needComplexSurround(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class ro.sync.ecss.extensions.commons.imagemap.[EditImageMapCore](../commons/imagemap/EditImageMapCore.md)
 [findNodeOfInterest](../commons/imagemap/EditImageMapCore.md#findNodeOfInterest(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String%5B%5D)), [getFullySelectedNode](../commons/imagemap/EditImageMapCore.md#getFullySelectedNode(ro.sync.ecss.extensions.api.AuthorDocumentController,int,int,boolean)), [isNodeOfInterest](../commons/imagemap/EditImageMapCore.md#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### TEI_NS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TEI_NS

TEI namespace.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.tei.TEIEditImageMapCore.TEI_NS)

## Constructor Details

### TEIEditImageMapCore

public TEIEditImageMapCore()

## Method Details

### getNodesOfInterestCriteria

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getNodesOfInterestCriteria([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
 Description copied from class: [EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md#getNodesOfInterestCriteria(java.lang.String))
Get the criteria for nodes of interest, and the start and end of the fragment to surround with.
  Specified by: [getNodesOfInterestCriteria](../commons/imagemap/EditImageMapWithSurroundCore.md#getNodesOfInterestCriteria(java.lang.String)) in class [EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md) Parameters: namespace - The namespace of the document. Returns: A 4 items array with the main property, the secondary property, and the start + end of the fragment to surround with. See Also:
        * [EditImageMapWithSurroundCore.getNodesOfInterestCriteria(java.lang.String)](../commons/imagemap/EditImageMapWithSurroundCore.md#getNodesOfInterestCriteria(java.lang.String))

### getSupportedFramework

public [SupportedFrameworks](../../imagemap/SupportedFrameworks.md) getSupportedFramework([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespaceURI)
 Description copied from class: [EditImageMapCore](../commons/imagemap/EditImageMapCore.md#getSupportedFramework(java.lang.String))
Detect the supported framework.
  Specified by: [getSupportedFramework](../commons/imagemap/EditImageMapCore.md#getSupportedFramework(java.lang.String)) in class [EditImageMapCore](../commons/imagemap/EditImageMapCore.md) Parameters: namespaceURI - The namespace uri of the element. Returns: The supported framework. See Also:
        * [EditImageMapCore.getSupportedFramework(java.lang.String)](../commons/imagemap/EditImageMapCore.md#getSupportedFramework(java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
