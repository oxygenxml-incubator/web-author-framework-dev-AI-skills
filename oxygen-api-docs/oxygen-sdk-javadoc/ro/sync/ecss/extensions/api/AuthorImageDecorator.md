Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorImageDecorator

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorImageDecorator
   All Implemented Interfaces: [Extension](Extension.md)   Direct Known Subclasses: [AuthorImageMapDecorator](../commons/imagemap/AuthorImageMapDecorator.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorImageDecorator extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Extension](Extension.md)
Permits decoration of the images that are displayed in the Author view. For instance it can overlay some meta-information over the image.

It receives the graphics device, the size and position of the underlying image.
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorImageDecorator](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 abstract void [paint](#paint(ro.sync.exml.view.graphics.Graphics,int,int,int,int,ro.sync.exml.view.graphics.Rectangle,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess,boolean))([Graphics](../../../exml/view/graphics/Graphics.md) g, int x, int y, int imageWidth, int imageHeight, [Rectangle](../../../exml/view/graphics/Rectangle.md) originalSize, [AuthorNode](node/AuthorNode.md) element, [AuthorAccess](AuthorAccess.md) authorAccess, boolean wasAnnotated)
Decorates an image.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorImageDecorator

public AuthorImageDecorator()

## Method Details

### paint

public abstract void paint([Graphics](../../../exml/view/graphics/Graphics.md) g, int x, int y, int imageWidth, int imageHeight, [Rectangle](../../../exml/view/graphics/Rectangle.md) originalSize, [AuthorNode](node/AuthorNode.md) element, [AuthorAccess](AuthorAccess.md) authorAccess, boolean wasAnnotated)

Decorates an image. The image was already painted in the provided [Graphics](../../../exml/view/graphics/Graphics.md).
  Parameters: g - The graphics. x - The X of the area to be painted. It is the top left corner of the image. y - The Y of the area to be painted. It is the top left corner of the image. imageWidth - The image width. imageHeight - The image height. originalSize - The original size of the image. element - The element to be painted. authorAccess - The author access. wasAnnotated - If true the image was annotated with previous dimensions.
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](Extension.md#getDescription()) in interface [Extension](Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
