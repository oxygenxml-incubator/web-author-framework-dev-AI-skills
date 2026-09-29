Package [ro.sync.ecss.extensions.docbook](package-summary.md)

# Class DocbookAuthorImageDecorator

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorImageDecorator](../api/AuthorImageDecorator.md)
        * [ro.sync.ecss.extensions.commons.imagemap.AuthorImageMapDecorator](../commons/imagemap/AuthorImageMapDecorator.md)
            * ro.sync.ecss.extensions.docbook.DocbookAuthorImageDecorator
   All Implemented Interfaces: [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DocbookAuthorImageDecorator extends [AuthorImageMapDecorator](../commons/imagemap/AuthorImageMapDecorator.md)
Handles a Docbook vocabulary image map. It renders the areas from the map over the image.

## Constructor Summary
 Constructors
Constructor

Description
 [DocbookAuthorImageDecorator](#%3Cinit%3E())()
Docbook author image map decorator.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [isNodeOfInterest](#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.imagemap.SupportedFrameworks))([AuthorNode](../api/node/AuthorNode.md) node, [SupportedFrameworks](../../imagemap/SupportedFrameworks.md) framework)
Check if the node to be painted is part of an image map.

### Methods inherited from class ro.sync.ecss.extensions.commons.imagemap.[AuthorImageMapDecorator](../commons/imagemap/AuthorImageMapDecorator.md)
 [paint](../commons/imagemap/AuthorImageMapDecorator.md#paint(ro.sync.exml.view.graphics.Graphics,int,int,int,int,ro.sync.exml.view.graphics.Rectangle,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,boolean))
### Methods inherited from class ro.sync.ecss.extensions.api.[AuthorImageDecorator](../api/AuthorImageDecorator.md)
 [getDescription](../api/AuthorImageDecorator.md#getDescription())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DocbookAuthorImageDecorator

public DocbookAuthorImageDecorator()

Docbook author image map decorator.

## Method Details

### isNodeOfInterest

protected boolean isNodeOfInterest([AuthorNode](../api/node/AuthorNode.md) node, [SupportedFrameworks](../../imagemap/SupportedFrameworks.md) framework)
 Description copied from class: [AuthorImageMapDecorator](../commons/imagemap/AuthorImageMapDecorator.md#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.imagemap.SupportedFrameworks))
Check if the node to be painted is part of an image map.
  Specified by: [isNodeOfInterest](../commons/imagemap/AuthorImageMapDecorator.md#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.imagemap.SupportedFrameworks)) in class [AuthorImageMapDecorator](../commons/imagemap/AuthorImageMapDecorator.md) Parameters: node - The current node. framework - The current framework. Returns: true if the node is part of an image map and we shall paint something over the image. See Also:
        * [AuthorImageMapDecorator.isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode, ro.sync.ecss.imagemap.SupportedFrameworks)](../commons/imagemap/AuthorImageMapDecorator.md#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.imagemap.SupportedFrameworks))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
