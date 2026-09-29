Package [ro.sync.exml.workspace.api.images](package-summary.md)

# Interface ImageUtilities
    All Superinterfaces: [ImageUtilitiesSpecificProvider](ImageUtilitiesSpecificProvider.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ImageUtilitiesextends [ImageUtilitiesSpecificProvider](ImageUtilitiesSpecificProvider.md)
Utilities related to registering image handlers...
  Since: 18
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addImageHandler](#addImageHandler(ro.sync.exml.workspace.api.images.handlers.ImageHandler))([ImageHandler](handlers/ImageHandler.md) imageHandler)
Add a new image handler.
  void [clearImageCache](#clearImageCache())()
Clear the cache of images used to display images fast in the Author page.
  [ImageHandler](handlers/ImageHandler.md) [getImageHandlerFor](#getImageHandlerFor(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) extension)
Get the XML image handler for a certain content type.
  void [removeImageHandler](#removeImageHandler(ro.sync.exml.workspace.api.images.handlers.ImageHandler))([ImageHandler](handlers/ImageHandler.md) imageHandler)
Remove an image handler.

### Methods inherited from interface ro.sync.exml.workspace.api.images.[ImageUtilitiesSpecificProvider](ImageUtilitiesSpecificProvider.md)
 [getIconDecoration](ImageUtilitiesSpecificProvider.md#getIconDecoration(java.net.URL)), [loadIcon](ImageUtilitiesSpecificProvider.md#loadIcon(java.net.URL))
## Method Details

### clearImageCache

void clearImageCache()

Clear the cache of images used to display images fast in the Author page.

### getImageHandlerFor

[ImageHandler](handlers/ImageHandler.md) getImageHandlerFor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) extension)

Get the XML image handler for a certain content type.
  Parameters: extension - The extension of the image file which should be supported by the handler. Returns: the XML image handler for a certain content type.
### addImageHandler

void addImageHandler([ImageHandler](handlers/ImageHandler.md) imageHandler)

Add a new image handler. It will have more priority than the builtin handlers.
  Parameters: imageHandler - The image handler.
### removeImageHandler

void removeImageHandler([ImageHandler](handlers/ImageHandler.md) imageHandler)

Remove an image handler.
  Parameters: imageHandler - The image handler to remove.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
