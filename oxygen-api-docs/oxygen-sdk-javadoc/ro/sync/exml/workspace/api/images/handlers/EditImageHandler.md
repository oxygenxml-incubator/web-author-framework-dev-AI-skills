Package [ro.sync.exml.workspace.api.images.handlers](package-summary.md)

# Class EditImageHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.workspace.api.images.handlers.ImageHandler](ImageHandler.md)
        * ro.sync.exml.workspace.api.images.handlers.EditImageHandler
   Direct Known Subclasses: [XMLImageHandler](XMLImageHandler.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class EditImageHandler extends [ImageHandler](ImageHandler.md)
Special handler for editing images which are either embedded or referenced.
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [EditImageHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract boolean [editImage](#editImage(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Edit the URL that represents an embedded image.
  abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [editImage](#editImage(ro.sync.exml.workspace.api.images.handlers.providers.EmbeddedImageContentProvider))([EmbeddedImageContentProvider](providers/EmbeddedImageContentProvider.md) contentProvider)
Edits the document fragment that represents an embedded image.

### Methods inherited from class ro.sync.exml.workspace.api.images.handlers.[ImageHandler](ImageHandler.md)
 [canHandleFileType](ImageHandler.md#canHandleFileType(java.lang.String)), [clearCache](ImageHandler.md#clearCache()), [getImage](ImageHandler.md#getImage(ro.sync.exml.workspace.api.images.handlers.providers.ImageContentProvider,ro.sync.exml.workspace.api.images.handlers.ImageRenderingContext)), [getImageLayoutInformation](ImageHandler.md#getImageLayoutInformation(ro.sync.exml.workspace.api.images.handlers.providers.ImageContentProvider,ro.sync.exml.workspace.api.images.handlers.ImageRenderingContext))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### EditImageHandler

public EditImageHandler()

## Method Details

### editImage

public abstract [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editImage([EmbeddedImageContentProvider](providers/EmbeddedImageContentProvider.md) contentProvider)throws [CannotEditException](CannotEditException.md)

Edits the document fragment that represents an embedded image.
  Parameters: contentProvider - The image content provider. Returns: The fragment representing the result of the edit, or null if the edit was canceled. Throws: [CannotEditException](CannotEditException.md) - If this handler does not support resource editing.
### editImage

public abstract boolean editImage([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)throws [CannotEditException](CannotEditException.md)

Edit the URL that represents an embedded image.
  Parameters: url - The URL to be edited. Returns: true If the URL content was modified. Throws: [CannotEditException](CannotEditException.md) - If this handler does not support resource editing.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
