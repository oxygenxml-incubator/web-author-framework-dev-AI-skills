Package [ro.sync.ecss.extensions.api.webapp.imagemap](package-summary.md)

# Class NewWebappAreaView

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.imagemap.NewWebappAreaView
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class NewWebappAreaView extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Descriptor for a new area coming from the client-side editor.
  Since: 25.0
## Constructor Summary
 Constructors
Constructor

Description
 [NewWebappAreaView](#%3Cinit%3E(int,ro.sync.exml.view.graphics.Shape))(int originalLayer, [Shape](../../../../../exml/view/graphics/Shape.md) shape)

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getOriginalLayer](#getOriginalLayer())()

 [Shape](../../../../../exml/view/graphics/Shape.md) [getShape](#getShape())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### NewWebappAreaView

public NewWebappAreaView(int originalLayer, [Shape](../../../../../exml/view/graphics/Shape.md) shape)
  Parameters: shape - The shape. originalLayer - The original layer or -1 if the shape was not in the original image map.
## Method Details

### getOriginalLayer

public int getOriginalLayer()
  Returns: Returns the originalLayer.
### getShape

public [Shape](../../../../../exml/view/graphics/Shape.md) getShape()
  Returns: Returns the shape.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
