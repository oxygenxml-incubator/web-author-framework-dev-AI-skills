Package [ro.sync.ecss.extensions.commons.imagemap.operations](package-summary.md)

# Interface NewShapeDescriptor
    All Known Implementing Classes: [DITAUpdateImageMapOperation.DITANewShapeDescriptor](../../../dita/DITAUpdateImageMapOperation.DITANewShapeDescriptor.md), [XHTMLUpdateImageMapOperation.XHTMLNewShapeDescriptor](../../../xhtml/imagemap/XHTMLUpdateImageMapOperation.XHTMLNewShapeDescriptor.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface NewShapeDescriptor
Descriptor for new shapes that were received from the JavaScript-base image map editor in Web Author.
  Since: 25.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)> [getOriginalLayer](#getOriginalLayer())()

 void [mergeIntoOriginalShape](#mergeIntoOriginalShape(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorDocumentController](../../../api/AuthorDocumentController.md) controller, [AuthorElement](../../../api/node/AuthorElement.md) shapeElement)
Merge this new shape into the exiting one.
  [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [serializeToXml](#serializeToXml())()

## Method Details

### serializeToXml

[Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> serializeToXml()
  Returns: The XML serialization of the new shape in DITA.
### mergeIntoOriginalShape

void mergeIntoOriginalShape([AuthorDocumentController](../../../api/AuthorDocumentController.md) controller, [AuthorElement](../../../api/node/AuthorElement.md) shapeElement)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Merge this new shape into the exiting one.
  Parameters: controller - The document controller. shapeElement - The existing shape element. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### getOriginalLayer

[Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html)> getOriginalLayer()
  Returns: Returns the originalLayer.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
