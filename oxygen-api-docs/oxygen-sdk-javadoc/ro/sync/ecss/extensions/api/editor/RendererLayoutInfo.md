Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Class RendererLayoutInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.editor.RendererLayoutInfo
   @API(type=EXTENDABLE, src=PUBLIC) public class RendererLayoutInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Class which contains rendering information about a renderer, information like the baseline and the size. The baseline and the size of the renderer are computed in a certain context.
  Since: 14.1
## Constructor Summary
 Constructors
Constructor

Description
 [RendererLayoutInfo](#%3Cinit%3E(int,ro.sync.exml.view.graphics.Dimension))(int baseline, [Dimension](../../../../exml/view/graphics/Dimension.md) size)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getBaseline](#getBaseline())()
Gets the baseline.
  [Dimension](../../../../exml/view/graphics/Dimension.md) [getSize](#getSize())()
Get the size of the renderer, in a certain context.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### RendererLayoutInfo

public RendererLayoutInfo(int baseline, [Dimension](../../../../exml/view/graphics/Dimension.md) size)

Constructor.
  Parameters: baseline - The baseline of the rendering component. size - The size of the renderer.
## Method Details

### getBaseline

public int getBaseline()

Gets the baseline. The baseline is measured from the top of the component. This method is primarily meant for the layout manager to align components along their baseline.
  Returns: The baseline.
### getSize

public [Dimension](../../../../exml/view/graphics/Dimension.md) getSize()

Get the size of the renderer, in a certain context.
  Returns: The renderer size.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
