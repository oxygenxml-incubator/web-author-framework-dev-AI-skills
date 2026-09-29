Package [ro.sync.ecss.extensions.commons.imagemap](package-summary.md)

# Class AuthorImageMapDecorator

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorImageDecorator](../../api/AuthorImageDecorator.md)
        * ro.sync.ecss.extensions.commons.imagemap.AuthorImageMapDecorator
   All Implemented Interfaces: [Extension](../../api/Extension.md)   Direct Known Subclasses: [DITAAuthorImageDecorator](../../dita/DITAAuthorImageDecorator.md), [DocbookAuthorImageDecorator](../../docbook/DocbookAuthorImageDecorator.md), [TEIAuthorImageDecorator](../../tei/TEIAuthorImageDecorator.md), [XHTMLAuthorImageDecorator](../../xhtml/XHTMLAuthorImageDecorator.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorImageMapDecorator extends [AuthorImageDecorator](../../api/AuthorImageDecorator.md)
Image map decorator base for Author. It paints the areas of the image map over the image.

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorImageMapDecorator](#%3Cinit%3E(ro.sync.ecss.extensions.commons.imagemap.EditImageMapCore))([EditImageMapCore](EditImageMapCore.md) imageMapCore)
Base functionality for the Author Image Map Decorator.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected abstract boolean [isNodeOfInterest](#isNodeOfInterest(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.imagemap.SupportedFrameworks))([AuthorNode](../../api/node/AuthorNode.md) node, [SupportedFrameworks](../../../imagemap/SupportedFrameworks.md) framework)
Check if the node to be painted is part of an image map.
  void [paint](#paint(ro.sync.exml.view.graphics.Graphics,int,int,int,int,ro.sync.exml.view.graphics.Rectangle,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,boolean))([Graphics](../../../../exml/view/graphics/Graphics.md) g, int x, int y, int imageWidth, int imageHeight, [Rectangle](../../../../exml/view/graphics/Rectangle.md) originalSize, [AuthorNode](../../api/node/AuthorNode.md) element, [AuthorAccess](../../api/AuthorAccess.md) authorAccess, boolean wasAnnotated)
Decorates an image.

### Methods inherited from class ro.sync.ecss.extensions.api.[AuthorImageDecorator](../../api/AuthorImageDecorator.md)
 [getDescription](../../api/AuthorImageDecorator.md#getDescription())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorImageMapDecorator

public AuthorImageMapDecorator([EditImageMapCore](EditImageMapCore.md) imageMapCore)

Base functionality for the Author Image Map Decorator.
  Parameters: imageMapCore - The image map core.
## Method Details

### isNodeOfInterest

protected abstract boolean isNodeOfInterest([AuthorNode](../../api/node/AuthorNode.md) node, [SupportedFrameworks](../../../imagemap/SupportedFrameworks.md) framework)

Check if the node to be painted is part of an image map.
  Parameters: node - The current node. framework - The current framework. Returns: true if the node is part of an image map and we shall paint something over the image.
### paint

public void paint([Graphics](../../../../exml/view/graphics/Graphics.md) g, int x, int y, int imageWidth, int imageHeight, [Rectangle](../../../../exml/view/graphics/Rectangle.md) originalSize, [AuthorNode](../../api/node/AuthorNode.md) element, [AuthorAccess](../../api/AuthorAccess.md) authorAccess, boolean wasAnnotated)
 Description copied from class: [AuthorImageDecorator](../../api/AuthorImageDecorator.md#paint(ro.sync.exml.view.graphics.Graphics,int,int,int,int,ro.sync.exml.view.graphics.Rectangle,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,boolean))
Decorates an image. The image was already painted in the provided [Graphics](../../../../exml/view/graphics/Graphics.md).
  Specified by: [paint](../../api/AuthorImageDecorator.md#paint(ro.sync.exml.view.graphics.Graphics,int,int,int,int,ro.sync.exml.view.graphics.Rectangle,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,boolean)) in class [AuthorImageDecorator](../../api/AuthorImageDecorator.md) Parameters: g - The graphics. x - The X of the area to be painted. It is the top left corner of the image. y - The Y of the area to be painted. It is the top left corner of the image. imageWidth - The image width. imageHeight - The image height. originalSize - The original size of the image. element - The element to be painted. authorAccess - The author access. wasAnnotated - If true the image was annotated with previous dimensions. See Also:
        * [AuthorImageDecorator.paint(ro.sync.exml.view.graphics.Graphics, int, int, int, int, Rectangle, AuthorNode, ro.sync.ecss.extensions.api.AuthorAccess, boolean)](../../api/AuthorImageDecorator.md#paint(ro.sync.exml.view.graphics.Graphics,int,int,int,int,ro.sync.exml.view.graphics.Rectangle,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,boolean))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
