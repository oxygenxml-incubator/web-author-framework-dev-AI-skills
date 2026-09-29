Package [ro.sync.exml.workspace.api.util](package-summary.md)

# Interface ImageInverter
    @API(type=INTERNAL, src=PUBLIC) public interface ImageInverter
Inverts certain images based on color theme.
  Since: 16.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [invertImage](#invertImage(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) image)
Attempts to invert an image.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [loadImage](#loadImage(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) imageURL)
Load an image from an URL.
  boolean [shouldInvertImage](#shouldInvertImage(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) image)
Check if an image should be inverted.

## Method Details

### loadImage

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) loadImage([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) imageURL)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Load an image from an URL. Returns either a java.awt.image.BufferedImage for the standalone editor or an org.eclipse.jface.resource.ImageDescriptor for the Oxygen plugin for Eclipse.
  Parameters: imageURL - The image URL Returns: Either a java.awt.image.BufferedImage for the standalone editor or an org.eclipse.jface.resource.ImageDescriptor for the Oxygen plugin for Eclipse. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If it fails to load the image.
### shouldInvertImage

boolean shouldInvertImage([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) image)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Check if an image should be inverted.
  Parameters: image - Either a java.awt.image.BufferedImage for the standalone editor or an org.eclipse.jface.resource.ImageDescriptor for the Oxygen plugin for Eclipse Returns: true if image should be inverted in the current color theme. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the operation fails.
### invertImage

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) invertImage([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) image)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Attempts to invert an image. In the standalone implementation the received image is inverted, in the Eclipse implementation a new ImageDescriptor instance is returned.
  Parameters: image - The image. Either a java.awt.image.BufferedImage for the standalone editor or an org.eclipse.jface.resource.ImageDescriptor for the Oxygen plugin for Eclipse Returns: The inverted image. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the operation fails
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
