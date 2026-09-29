Package [ro.sync.ecss.extensions.api.webapp.imagemap](package-summary.md)

# Interface WebappImageMapSupportFactory
    All Superinterfaces: [Extension](../../Extension.md)   All Known Implementing Classes: [XHTMLWebappImageMapSupportFactory](../../../xhtml/imagemap/XHTMLWebappImageMapSupportFactory.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface WebappImageMapSupportFactoryextends [Extension](../../Extension.md)
Factory class to create image maps for a specific document element. Subclasses can be given as a parameter to the WebappImageMapRenderer form control.
  Since: 25.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [WebappImageMapSupport](WebappImageMapSupport.md) [createImageMapSupport](#createImageMapSupport(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](../../editor/AuthorInplaceContext.md) context)
Create an image map support.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../Extension.md)
 [getDescription](../../Extension.md#getDescription())
## Method Details

### createImageMapSupport

[WebappImageMapSupport](WebappImageMapSupport.md) createImageMapSupport([AuthorInplaceContext](../../editor/AuthorInplaceContext.md) context)throws [ImageMapFormatException](ImageMapFormatException.md)

Create an image map support.
  Parameters: context - The context. Returns: The image map support. Throws: [ImageMapFormatException](ImageMapFormatException.md) - When the image map cannot be parsed from the given context.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
