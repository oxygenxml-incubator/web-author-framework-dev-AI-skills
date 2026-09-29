Package [ro.sync.exml.workspace.api.images](package-summary.md)

# Interface ImageUtilitiesSpecificProvider
    All Known Subinterfaces: [ImageUtilities](ImageUtilities.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ImageUtilitiesSpecificProvider
Platform specific image utilities provider.
  Since: 18.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getIconDecoration](#getIconDecoration(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource)
Get an icon decoration which can be used when presenting a small icon for the URL in a resource explorer tree.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [loadIcon](#loadIcon(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource)
Load an icon from a specified URL resource location.

## Method Details

### getIconDecoration

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getIconDecoration([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource)

Get an icon decoration which can be used when presenting a small icon for the URL in a resource explorer tree. For example if the URL ends in ".xml", this utility returns a small XML-symbol image. This is only implemented in the Swing-based application.
  Parameters: resource - The resource URL. Returns: An icon decoration or null.
### loadIcon

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) loadIcon([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resource)

Load an icon from a specified URL resource location. When running on a retina or HiDPI display, the application will try to load a corresponding image for the current display. Also when running in a dark theme the dark icon will be loaded if available. This topic explains how the application tries to load an image based on the initial given image location and on the display type: https://www.oxygenxml.com/doc/versions/18/ug-author/topics/using-retina-hidpi-images.html  For the Swing-based application, the returned icon is an instance of javax.swing.ImageIcon. For the Eclipse-based plugin the returned icon is an instance of org.eclipse.jface.resource.ImageDescriptor. An example of loading an icon from Oxygen's existing set of icons:  PluginWorkspaceProvider.getPluginWorkspace().getImageUtilities() .loadIcon(ro.sync.exml.Oxygen.class.getResource("/images/OptionsShortcut16.png"));
  Parameters: resource - The resource URL Returns: The loaded icon. If an icon cannot be loaded, a fallback icon is returned.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
