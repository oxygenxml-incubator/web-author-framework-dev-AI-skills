Package [com.oxygenxml.editor.imagemap](package-summary.md)

# Class ECImageMapAccess

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.imagemap.ImageMapAccess
        * com.oxygenxml.editor.imagemap.ECImageMapAccess
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class ECImageMapAccess extends ro.sync.ecss.imagemap.ImageMapAccess
Eclipse Image Map Access.

## Constructor Summary
 Constructors
Constructor

Description
 [ECImageMapAccess](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [paintImageMapAreas](#paintImageMapAreas(ro.sync.exml.view.graphics.Graphics,int,int,int,int,double,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.imagemap.IImageMapWrapper,ro.sync.ecss.imagemap.SupportedFrameworks,int,boolean))([Graphics](../../../../ro/sync/exml/view/graphics/Graphics.md) g, int x, int y, int imageWidth, int imageHeight, double scaleFactor, [AuthorAccess](../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) authorAccess, [IImageMapWrapper](../../../../ro/sync/ecss/imagemap/IImageMapWrapper.md)<ro.sync.ecss.imagemap.IImageMap> imageMap, [SupportedFrameworks](../../../../ro/sync/ecss/imagemap/SupportedFrameworks.md) framework, int fontOfNodeSize, boolean wasAnnotated)
Paint ImageMap areas.

### Methods inherited from class ro.sync.ecss.imagemap.ImageMapAccess
 editMap, getInstance, setInstance
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ECImageMapAccess

public ECImageMapAccess()

## Method Details

### paintImageMapAreas

public void paintImageMapAreas([Graphics](../../../../ro/sync/exml/view/graphics/Graphics.md) g, int x, int y, int imageWidth, int imageHeight, double scaleFactor, [AuthorAccess](../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) authorAccess, [IImageMapWrapper](../../../../ro/sync/ecss/imagemap/IImageMapWrapper.md)<ro.sync.ecss.imagemap.IImageMap> imageMap, [SupportedFrameworks](../../../../ro/sync/ecss/imagemap/SupportedFrameworks.md) framework, int fontOfNodeSize, boolean wasAnnotated)

Paint ImageMap areas.
  Overrides: paintImageMapAreas in class ro.sync.ecss.imagemap.ImageMapAccess Parameters: g - The graphics to paint on. x - The horizontal displacement of the image. y - The vertical displacement of the image. imageWidth - The image width. imageHeight - The image height. scaleFactor - The scaling factor. authorAccess - The author access. imageMap - The image map wrapper. framework - The framework. fontOfNodeSize - The size for the node's font. wasAnnotated - If true the image was annotated with previous dimensions.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
