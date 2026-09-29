Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DITAUpdateImageMapOperation.DITANewShapeDescriptor

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.DITAUpdateImageMapOperation.DITANewShapeDescriptor
   All Implemented Interfaces: [NewShapeDescriptor](../commons/imagemap/operations/NewShapeDescriptor.md)   Enclosing class: [DITAUpdateImageMapOperation](DITAUpdateImageMapOperation.md)   public static class DITAUpdateImageMapOperation.DITANewShapeDescriptor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [NewShapeDescriptor](../commons/imagemap/operations/NewShapeDescriptor.md)
Descriptor of a shape that was added client-side.

## Constructor Summary
 Constructors
Constructor

Description
 [DITANewShapeDescriptor](#%3Cinit%3E(org.w3c.dom.Element))([Element](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/w3c/dom/Element.html) elem)
Descriptor of a shape that was added client-side.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)> [getOriginalLayer](#getOriginalLayer())()

 void [mergeIntoOriginalShape](#mergeIntoOriginalShape(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorDocumentController](../api/AuthorDocumentController.md) controller, [AuthorElement](../api/node/AuthorElement.md) shapeElement)
Merge this new shape into the exiting one.
  [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [serializeToXml](#serializeToXml())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITANewShapeDescriptor

public DITANewShapeDescriptor([Element](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/w3c/dom/Element.html) elem)

Descriptor of a shape that was added client-side.
  Parameters: elem - The DITA XML element.
## Method Details

### serializeToXml

public [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> serializeToXml()
  Specified by: [serializeToXml](../commons/imagemap/operations/NewShapeDescriptor.md#serializeToXml()) in interface [NewShapeDescriptor](../commons/imagemap/operations/NewShapeDescriptor.md) Returns: The XML serialization of the new shape in DITA. See Also:
        * [NewShapeDescriptor.serializeToXml()](../commons/imagemap/operations/NewShapeDescriptor.md#serializeToXml())

### mergeIntoOriginalShape

public void mergeIntoOriginalShape([AuthorDocumentController](../api/AuthorDocumentController.md) controller, [AuthorElement](../api/node/AuthorElement.md) shapeElement)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
 Description copied from interface: [NewShapeDescriptor](../commons/imagemap/operations/NewShapeDescriptor.md#mergeIntoOriginalShape(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorElement))
Merge this new shape into the exiting one.
  Specified by: [mergeIntoOriginalShape](../commons/imagemap/operations/NewShapeDescriptor.md#mergeIntoOriginalShape(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [NewShapeDescriptor](../commons/imagemap/operations/NewShapeDescriptor.md) Parameters: controller - The document controller. shapeElement - The existing shape element. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) See Also:
        * [NewShapeDescriptor.mergeIntoOriginalShape(ro.sync.ecss.extensions.api.AuthorDocumentController, ro.sync.ecss.extensions.api.node.AuthorElement)](../commons/imagemap/operations/NewShapeDescriptor.md#mergeIntoOriginalShape(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorElement))

### getOriginalLayer

public [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)> getOriginalLayer()
  Specified by: [getOriginalLayer](../commons/imagemap/operations/NewShapeDescriptor.md#getOriginalLayer()) in interface [NewShapeDescriptor](../commons/imagemap/operations/NewShapeDescriptor.md) Returns: Returns the originalLayer. See Also:
        * [NewShapeDescriptor.getOriginalLayer()](../commons/imagemap/operations/NewShapeDescriptor.md#getOriginalLayer())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
